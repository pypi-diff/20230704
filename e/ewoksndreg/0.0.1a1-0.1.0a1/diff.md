# Comparing `tmp/ewoksndreg-0.0.1a1.tar.gz` & `tmp/ewoksndreg-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksndreg-0.0.1a1.tar", last modified: Fri Mar 24 17:18:35 2023, max compression
+gzip compressed data, was "dist/ewoksndreg-0.1.0a1.tar", last modified: Tue Jul  4 06:40:13 2023, max compression
```

## Comparing `ewoksndreg-0.0.1a1.tar` & `ewoksndreg-0.1.0a1.tar`

### file list

```diff
@@ -1,110 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      949 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1887 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/detection/
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/detection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/detection/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4712 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/detection/scikitimage_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     1472 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/detection/silx_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/
--rw-rw-rw-   0 root         (0) root         (0)     2443 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/base.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/numpy_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/scikitimage_backend.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/silx_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/base.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/lstsq.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/numpy_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     2793 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/scikitimage_backend.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/scipy_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/matching/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/matching/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/matching/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5595 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/matching/numpy_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/matching/scikitimage_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/matching/silx_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/features/registration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/intensities/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/intensities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/intensities/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3707 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/intensities/numpy_backend.py
--rw-rw-rw-   0 root         (0) root         (0)      750 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/intensities/registration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/io/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6546 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/io/input_stack.py
--rw-rw-rw-   0 root         (0) root         (0)     2553 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/io/output_stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/math/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 17:18:29.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/math/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2708 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/math/center.py
--rw-rw-rw-   0 root         (0) root         (0)    12676 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/math/fft.py
--rw-rw-rw-   0 root         (0) root         (0)     8125 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/math/fit1d.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/math/fit2d.py
--rw-rw-rw-   0 root         (0) root         (0)     2407 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tasks/example2d_stack.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tasks/reg2d_features.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tasks/reg2d_intensities.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tasks/reg2d_transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 17:18:29.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 17:18:29.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2984 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/data/data_for_registration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/math/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 17:18:29.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/math/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10847 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/math/test_fft.py
--rwxrwxrwx   0 root         (0) root         (0)     1889 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/math/test_fit1d.py
--rwxrwxrwx   0 root         (0) root         (0)      463 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/math/test_fit2d.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_feature_registration.py
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_intensity_registration.py
--rw-rw-rw-   0 root         (0) root         (0)     4673 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_mapping_solvers.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_match_numpy.py
--rw-rw-rw-   0 root         (0) root         (0)     2789 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_stack_io.py
--rw-rw-rw-   0 root         (0) root         (0)     4317 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_transformation_apply.py
--rw-rw-rw-   0 root         (0) root         (0)     3306 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_transformation_numpy.py
--rw-rw-rw-   0 root         (0) root         (0)      950 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_transformation_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/apply.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3451 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/homography.py
--rw-rw-rw-   0 root         (0) root         (0)     9095 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/lstsq.py
--rw-rw-rw-   0 root         (0) root         (0)     4924 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/numpy_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/scikitimage_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     1986 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/scipy_backend.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg.egg-info/
--rw-r--r--   0 root         (0) root         (0)      949 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3593 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      267 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      317 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/ewoksndreg.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/orangecontrib/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3814 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/example2d_stack.py
--rw-rw-rw-   0 root         (0) root         (0)     6049 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/reg2d_features.py
--rw-rw-rw-   0 root         (0) root         (0)     5756 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/reg2d_intensities.py
--rw-rw-rw-   0 root         (0) root         (0)     4795 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/reg2d_transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:18:35.000000 ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 17:18:29.000000 ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/tutorials/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3043 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/tutorials/reg2d_features.ows
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-03-24 17:14:53.000000 ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/tutorials/reg2d_intensities.ows
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      983 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/detection/
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/detection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/detection/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4712 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/detection/scikitimage_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1472 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/detection/silx_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/numpy_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/scikitimage_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/silx_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/lstsq.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/numpy_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     2793 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/scikitimage_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/scipy_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/matching/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/matching/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/matching/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5595 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/matching/numpy_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/matching/scikitimage_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/matching/silx_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/features/registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/intensities/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/intensities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/intensities/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3707 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/intensities/numpy_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/intensities/registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/io/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6546 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/io/input_stack.py
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/io/output_stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/math/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:40:07.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/math/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2708 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/math/center.py
+-rw-rw-rw-   0 root         (0) root         (0)    12676 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/math/fft.py
+-rw-rw-rw-   0 root         (0) root         (0)     8125 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/math/fit1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/math/fit2d.py
+-rw-rw-rw-   0 root         (0) root         (0)     2407 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tasks/example2d_stack.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tasks/reg2d_features.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tasks/reg2d_intensities.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tasks/reg2d_transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:40:07.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:40:07.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/data/data_for_registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/math/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:40:07.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/math/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10847 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/math/test_fft.py
+-rwxrwxrwx   0 root         (0) root         (0)     1889 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/math/test_fit1d.py
+-rwxrwxrwx   0 root         (0) root         (0)      463 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/math/test_fit2d.py
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_feature_registration.py
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_intensity_registration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4673 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_mapping_solvers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_match_numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2789 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_stack_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     4317 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_transformation_apply.py
+-rw-rw-rw-   0 root         (0) root         (0)     3306 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_transformation_numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)      950 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_transformation_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:40:07.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/tutorials/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/tutorials/test_reg2d_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/tests/tutorials/test_reg2d_intensities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/apply.py
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3451 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/homography.py
+-rw-rw-rw-   0 root         (0) root         (0)     9095 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/lstsq.py
+-rw-rw-rw-   0 root         (0) root         (0)     4924 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/numpy_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/scikitimage_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1986 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/scipy_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      983 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3747 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      320 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/ewoksndreg.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/orangecontrib/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/orangecontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3814 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/example2d_stack.py
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/reg2d_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     5756 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/reg2d_intensities.py
+-rw-rw-rw-   0 root         (0) root         (0)     4795 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/reg2d_transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:13.000000 ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 06:40:07.000000 ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/tutorials/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/tutorials/reg2d_features.ows
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-07-04 06:38:04.000000 ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/tutorials/reg2d_intensities.ows
```

### Comparing `ewoksndreg-0.0.1a1/LICENSE.md` & `ewoksndreg-0.1.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/PKG-INFO` & `ewoksndreg-0.1.0a1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ewoksndreg
-Version: 0.0.1a1
+Version: 0.1.0a1
 Summary: Workflows for data registration (e.g. curve, image and volume registration).
-Home-page: https://gitlab.esrf.fr/workflow/ewoksndreg/
+Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksndreg
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
-Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksndreg/
+Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksndreg
 Project-URL: Documentation, https://ewoksndreg.readthedocs.io/
-Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoksndreg/issues/
-Keywords: orange3 add-on
+Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksndreg/issues/
+Keywords: orange3 add-on,ewoks
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: test
```

### Comparing `ewoksndreg-0.0.1a1/setup.cfg` & `ewoksndreg-0.1.0a1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 version = attr: ewoksndreg.__version__
 author = ESRF
 author_email = wout.de_nolf@esrf.fr
 description = Workflows for data registration (e.g. curve, image and volume registration).
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
-url = https://gitlab.esrf.fr/workflow/ewoksndreg/
+url = https://gitlab.esrf.fr/workflow/ewoksapps/ewoksndreg
 project_urls = 
-	Source = https://gitlab.esrf.fr/workflow/ewoksndreg/
+	Source = https://gitlab.esrf.fr/workflow/ewoksapps/ewoksndreg
 	Documentation = https://ewoksndreg.readthedocs.io/
-	Tracker = https://gitlab.esrf.fr/workflow/ewoksndreg/issues/
+	Tracker = https://gitlab.esrf.fr/workflow/ewoksapps/ewoksndreg/issues/
 classifiers = 
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 keywords = 
-	orange3 add-on
+	orange3 add-on,ewoks
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	strenum >= 0.4.9
 	numpy >=1.15
 	silx >=1.1.2
+	pyopencl
 	ewoksdata >=0.1
 	ewoksorange >=0.1.2
 	ewoks[orange] >=0.1
 namespace_packages = 
 	orangecontrib
 
 [options.packages.find]
@@ -59,29 +60,26 @@
 	ewoksndreg=orangecontrib.ewoksndreg
 orange.widgets = 
 	Registration=orangecontrib.ewoksndreg
 orange.widgets.tutorials = 
 	Registration=orangecontrib.ewoksndreg.tutorials
 orange.canvas.help = 
 	html-index=orangecontrib.ewoksndreg:WIDGET_HELP_PATH
+ewoks.tasks.class = 
+	ewoksndreg.tasks.*=ewoksndreg
 
 [options.package_data]
 * = *.ows, *.png, *.svg
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
 
-[build_sphinx]
-project = ewoksndreg
-version = attr: ewoksndreg.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	*/tests/*
 
 [mypy-setuptools.*]
 ignore_missing_imports = True
```

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/detection/scikitimage_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/detection/scikitimage_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/detection/silx_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/detection/silx_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/__init__.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/base.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/base.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/numpy_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/scikitimage_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/scikitimage_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/features/silx_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/features/silx_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/lstsq.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/lstsq.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/numpy_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/scikitimage_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/scikitimage_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/mapping/scipy_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/mapping/scipy_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/matching/numpy_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/matching/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/matching/scikitimage_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/matching/scikitimage_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/matching/silx_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/matching/silx_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/features/registration.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/features/registration.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/intensities/numpy_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/intensities/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/intensities/registration.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/intensities/registration.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/io/input_stack.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/io/input_stack.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/io/output_stack.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/io/output_stack.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/math/center.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/math/center.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/math/fft.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/math/fft.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/math/fit1d.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/math/fit1d.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/math/fit2d.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/math/fit2d.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/registry.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/registry.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tasks/example2d_stack.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tasks/example2d_stack.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tasks/reg2d_features.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tasks/reg2d_features.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tasks/reg2d_intensities.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tasks/reg2d_intensities.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tasks/reg2d_transform.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tasks/reg2d_transform.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/data/data_for_registration.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/data/data_for_registration.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/math/test_fft.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/math/test_fft.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/math/test_fit1d.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/math/test_fit1d.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_feature_registration.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_feature_registration.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_intensity_registration.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_intensity_registration.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_mapping_solvers.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_mapping_solvers.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_match_numpy.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_match_numpy.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_stack_io.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_stack_io.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_tasks.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_transformation_apply.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_transformation_apply.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_transformation_numpy.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_transformation_numpy.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/tests/test_transformation_types.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/tests/test_transformation_types.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/apply.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/apply.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/base.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/base.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/homography.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/homography.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/lstsq.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/lstsq.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/numpy_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/scikitimage_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/scikitimage_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg/transformation/scipy_backend.py` & `ewoksndreg-0.1.0a1/src/ewoksndreg/transformation/scipy_backend.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg.egg-info/PKG-INFO` & `ewoksndreg-0.1.0a1/src/ewoksndreg.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ewoksndreg
-Version: 0.0.1a1
+Version: 0.1.0a1
 Summary: Workflows for data registration (e.g. curve, image and volume registration).
-Home-page: https://gitlab.esrf.fr/workflow/ewoksndreg/
+Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksndreg
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
-Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksndreg/
+Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksndreg
 Project-URL: Documentation, https://ewoksndreg.readthedocs.io/
-Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoksndreg/issues/
-Keywords: orange3 add-on
+Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksndreg/issues/
+Keywords: orange3 add-on,ewoks
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: test
```

### Comparing `ewoksndreg-0.0.1a1/src/ewoksndreg.egg-info/SOURCES.txt` & `ewoksndreg-0.1.0a1/src/ewoksndreg.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 src/ewoksndreg/tests/test_transformation_types.py
 src/ewoksndreg/tests/data/__init__.py
 src/ewoksndreg/tests/data/data_for_registration.py
 src/ewoksndreg/tests/math/__init__.py
 src/ewoksndreg/tests/math/test_fft.py
 src/ewoksndreg/tests/math/test_fit1d.py
 src/ewoksndreg/tests/math/test_fit2d.py
+src/ewoksndreg/tests/tutorials/__init__.py
+src/ewoksndreg/tests/tutorials/test_reg2d_features.py
+src/ewoksndreg/tests/tutorials/test_reg2d_intensities.py
 src/ewoksndreg/transformation/__init__.py
 src/ewoksndreg/transformation/apply.py
 src/ewoksndreg/transformation/base.py
 src/ewoksndreg/transformation/homography.py
 src/ewoksndreg/transformation/lstsq.py
 src/ewoksndreg/transformation/numpy_backend.py
 src/ewoksndreg/transformation/scikitimage_backend.py
```

### Comparing `ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/example2d_stack.py` & `ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/example2d_stack.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/reg2d_features.py` & `ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/reg2d_features.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/reg2d_intensities.py` & `ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/reg2d_intensities.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/reg2d_transform.py` & `ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/reg2d_transform.py`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/tutorials/reg2d_features.ows` & `ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/tutorials/reg2d_features.ows`

 * *Files identical despite different names*

### Comparing `ewoksndreg-0.0.1a1/src/orangecontrib/ewoksndreg/tutorials/reg2d_intensities.ows` & `ewoksndreg-0.1.0a1/src/orangecontrib/ewoksndreg/tutorials/reg2d_intensities.ows`

 * *Files identical despite different names*

