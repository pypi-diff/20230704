# Comparing `tmp/earthkit-data-0.1.3.tar.gz` & `tmp/earthkit-data-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-data-0.1.3.tar", last modified: Fri May 26 11:14:12 2023, max compression
+gzip compressed data, was "earthkit-data-0.2.0.tar", last modified: Tue Jul  4 09:54:37 2023, max compression
```

## Comparing `earthkit-data-0.1.3.tar` & `earthkit-data-0.2.0.tar`

### file list

```diff
@@ -1,270 +1,318 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.899907 earthkit-data-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.871907 earthkit-data-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.875907 earthkit-data-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.github/workflows/label-public-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.github/workflows/notify_new_issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.github/workflows/notify_new_pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-26 11:14:12.899907 earthkit-data-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.875907 earthkit-data-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.875907 earthkit-data-0.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.875907 earthkit-data-0.1.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/development.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.879907 earthkit-data-0.1.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/Untitled.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/bufr.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/cds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    48723 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/fdb.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_file_pattern.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    46046 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_from_stream.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_indexing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    76259 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_missing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_multi.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   100543 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    45612 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_tar.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_to_netcdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/grib_url.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    34189 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/list_of_dict.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/mars.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/missing.grib
--rw-r--r--   0 runner    (1001) docker     (123)    39112 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/netcdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/odb.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/temp_10.bufr
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/test.grib
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/test.nc
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/test.odb
--rw-r--r--   0 runner    (1001) docker     (123)   521712 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/test4.grib
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/test6.grib
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples/tuv_pl.grib
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.879907 earthkit-data-0.1.3/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/caching.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.879907 earthkit-data-0.1.3/docs/guide/data_format/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/bufr.rst
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/csv.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/grib.rst
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/netcdf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/data_format/odb.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.879907 earthkit-data-0.1.3/docs/guide/include/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/include/settings-1-get.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/include/settings-2-set.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/include/settings-3-reset.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/guide/sources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/licence.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.871907 earthkit-data-0.1.3/earthkit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.879907 earthkit-data-0.1.3/earthkit/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/arguments/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/args_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/earthkit_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/input_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/arguments/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/temporary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/core/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.871907 earthkit-data-0.1.3/earthkit/data/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/data/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/data/css/tab.css
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/data/css/table.css
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/indexing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/indexing/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/indexing/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/indexing/database/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/indexing/database/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/indexing/database/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/input_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/mergers/
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/mergers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/mergers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/mergers/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.883907 earthkit-data-0.1.3/earthkit/data/mirrors/
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/mirrors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/mirrors/directory_mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.887907 earthkit-data-0.1.3/earthkit/data/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/bufr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.887907 earthkit-data-0.1.3/earthkit/data/readers/grib/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27074 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/codes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15965 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/fieldlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.887907 earthkit-data-0.1.3/earthkit/data/readers/grib/index/
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/index/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/index/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/index/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/index/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/grib/xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/odb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/unknown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/readers/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/cds.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/dummy.grib
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/dummy_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/ecmwf_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/fdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/file_indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/file_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/list_of_dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/url_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/virtual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sources/virtual_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit/data/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sphinxext/generate_settings_rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sphinxext/module_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/sphinxext/xref.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit/data/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/factorise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/parts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/serialise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/utils/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit/data/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/vocabularies/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/vocabularies/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/vocabularies/grib-paramid.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/vocabularies/grib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit/data/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/wrappers/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit/data/wrappers/string.py
--rw-r--r--   0 runner    (1001) docker     (123)    65385 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/earthkit-data.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.891907 earthkit-data-0.1.3/earthkit_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 11:14:12.000000 earthkit-data-0.1.3/earthkit_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-26 11:14:12.899907 earthkit-data-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/bufr/
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/bufr/test_bufr_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/core/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/core/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/mercator.grib
--rw-r--r--   0 runner    (1001) docker     (123)    47520 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/ml_data.grib
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/rgg_small_subarea_cellarea_ref.grib
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/t_pl.grib
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/t_time_series.grib
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/test_icon.grib
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/test_single.grib
--rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/test_single.nc
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/test_single_with_missing.grib
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/u_pl.grib
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/data/v_pl.grib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/documentation/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/documentation/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/grib/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    21795 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_order_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_sel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/grib/test_grib_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.895907 earthkit-data-0.1.3/tests/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/indexing_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_indexing_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_indexing_isel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_indexing_order_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_indexing_serialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_order_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/indexing/test_selection_kwargs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.899907 earthkit-data-0.1.3/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_grib_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_netcdf_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_odb_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_tar_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_unknown_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/test_zip_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/unknown_file.unknown_ext
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/readers/unknown_text_file.unknown_ext
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:14:12.899907 earthkit-data-0.1.3/tests/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_cds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/sources/test_url_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 11:13:58.000000 earthkit-data-0.1.3/tests/test_00_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.375955 earthkit-data-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.295955 earthkit-data-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.311955 earthkit-data-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/.github/workflows/label-public-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/.github/workflows/notify-new-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/.github/workflows/notify-new-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-04 09:54:37.375955 earthkit-data-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.311955 earthkit-data-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.311955 earthkit-data-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)    65385 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/_static/earthkit-data.png
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.315955 earthkit-data-0.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/development.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.323955 earthkit-data-0.2.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    25120 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/bufr_synop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    79992 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/bufr_temp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/cds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/ecmwf_open_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    55042 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/fdb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27816 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/from_object.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_file_pattern.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_from_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_indexing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    85764 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_missing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_multi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   100549 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45634 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_tar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_to_netcdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/grib_url.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    34189 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/list_of_dict.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/mars.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/missing.grib
+-rw-r--r--   0 runner    (1001) docker     (123)    39052 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/netcdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/odb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   442849 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/projection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/synop_10.bufr
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/temp_10.bufr
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/test.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/test.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/test.odb
+-rw-r--r--   0 runner    (1001) docker     (123)   521712 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/test4.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/test6.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples/tuv_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.323955 earthkit-data-0.2.0/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/caching.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/data.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.327955 earthkit-data-0.2.0/docs/guide/data_format/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/data_format/bufr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/data_format/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/data_format/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/data_format/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/data_format/netcdf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/data_format/odb.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.327955 earthkit-data-0.2.0/docs/guide/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/include/settings-1-get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/include/settings-2-set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/include/settings-3-reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/guide/sources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.327955 earthkit-data-0.2.0/docs/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/release_notes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/release_notes/version_0.2_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/docs/skip_api_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.299955 earthkit-data-0.2.0/earthkit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.331955 earthkit-data-0.2.0/earthkit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.331955 earthkit-data-0.2.0/earthkit/data/arguments/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/arguments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/arguments/args_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/arguments/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/arguments/earthkit_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/arguments/input_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/arguments/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.335955 earthkit-data-0.2.0/earthkit/data/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20864 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/temporary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/core/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.299955 earthkit-data-0.2.0/earthkit/data/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.335955 earthkit-data-0.2.0/earthkit/data/data/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/data/css/tab.css
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/data/css/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/data/css/tree.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.335955 earthkit-data-0.2.0/earthkit/data/indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/indexing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.335955 earthkit-data-0.2.0/earthkit/data/indexing/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/indexing/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/indexing/database/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/indexing/database/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/indexing/database/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/input_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.339955 earthkit-data-0.2.0/earthkit/data/mergers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/mergers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/mergers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/mergers/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.339955 earthkit-data-0.2.0/earthkit/data/mirrors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/mirrors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/mirrors/directory_mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.339955 earthkit-data-0.2.0/earthkit/data/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.343955 earthkit-data-0.2.0/earthkit/data/readers/bufr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/bufr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21838 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/bufr/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/bufr/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.343955 earthkit-data-0.2.0/earthkit/data/readers/grib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19750 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/fieldlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.347955 earthkit-data-0.2.0/earthkit/data/readers/grib/index/
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/index/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/index/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/index/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/index/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/grib/xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/odb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/readers/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.351955 earthkit-data-0.2.0/earthkit/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/dummy.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/dummy_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/ecmwf_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/ecmwf_open_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/fdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/file_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/file_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/list_of_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/virtual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sources/virtual_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.355955 earthkit-data-0.2.0/earthkit/data/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sphinxext/generate_settings_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sphinxext/module_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/sphinxext/xref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.355955 earthkit-data-0.2.0/earthkit/data/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/translators/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/translators/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/translators/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.359955 earthkit-data-0.2.0/earthkit/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/factorise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.359955 earthkit-data-0.2.0/earthkit/data/utils/projections/
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/projections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/projections/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/projections/proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/serialise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/utils/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-04 09:54:37.000000 earthkit-data-0.2.0/earthkit/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.363955 earthkit-data-0.2.0/earthkit/data/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/vocabularies/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/vocabularies/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/vocabularies/grib-paramid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/vocabularies/grib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.363955 earthkit-data-0.2.0/earthkit/data/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/wrappers/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/wrappers/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/wrappers/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/earthkit/data/wrappers/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.363955 earthkit-data-0.2.0/earthkit_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-04 09:54:37.000000 earthkit-data-0.2.0/earthkit_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-04 09:54:37.000000 earthkit-data-0.2.0/earthkit_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:54:37.000000 earthkit-data-0.2.0/earthkit_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-04 09:54:37.000000 earthkit-data-0.2.0/earthkit_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 09:54:37.000000 earthkit-data-0.2.0/earthkit_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-04 09:54:37.379955 earthkit-data-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.367955 earthkit-data-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.367955 earthkit-data-0.2.0/tests/bufr/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/bufr/test_bufr_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/bufr/test_bufr_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/bufr/test_bufr_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/bufr/test_bufr_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/bufr/test_bufr_sel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/bufr/test_bufr_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.367955 earthkit-data-0.2.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/core/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/core/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/core/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.371955 earthkit-data-0.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/mercator.grib
+-rw-r--r--   0 runner    (1001) docker     (123)    47520 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/ml_data.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/rgg_small_subarea_cellarea_ref.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/t_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/t_time_series.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/test_icon.grib
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/test_single.grib
+-rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/test_single.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/test_single_with_missing.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/u_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/data/v_pl.grib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.371955 earthkit-data-0.2.0/tests/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/documentation/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/documentation/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/environment-unit-tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.375955 earthkit-data-0.2.0/tests/grib/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/grib/test_grib_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25758 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/grib/test_grib_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/grib/test_grib_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/grib/test_grib_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/grib/test_grib_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/grib/test_grib_sel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/grib/test_grib_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/grib/test_grib_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.375955 earthkit-data-0.2.0/tests/indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/indexing/indexing_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/indexing/test_indexing_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/indexing/test_indexing_isel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/indexing/test_indexing_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/indexing/test_indexing_serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/indexing/test_order_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/indexing/test_selection_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.375955 earthkit-data-0.2.0/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/readers/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/readers/test_grib_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/readers/test_netcdf_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/readers/test_odb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/readers/test_reader_padding_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/readers/test_tar_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/readers/test_unknown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/readers/test_zip_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/readers/unknown_file.unknown_ext
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/readers/unknown_text_file.unknown_ext
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.375955 earthkit-data-0.2.0/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/sources/test_cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/sources/test_ecmwf_open_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/sources/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/sources/test_mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/sources/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/sources/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/sources/test_url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/test_00_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.375955 earthkit-data-0.2.0/tests/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/translators/test_translators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.375955 earthkit-data-0.2.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/utils/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/utils/test_download_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/utils/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/utils/test_projections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:54:37.375955 earthkit-data-0.2.0/tests/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/wrappers/test_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/wrappers/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-04 09:54:05.000000 earthkit-data-0.2.0/tests/wrappers/test_xarray.py
```

### Comparing `earthkit-data-0.1.3/.github/workflows/ci.yml` & `earthkit-data-0.2.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 name: ci
 
 on:
   push:
     branches:
     - main
+    - develop
     tags:
     - "*"
   pull_request:
     branches:
     - main
+    - develop
   pull_request_target:
     types: [labeled]
   workflow_dispatch:
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
@@ -42,15 +44,15 @@
     steps:
     - uses: actions/checkout@v3
       with:
         ref: ${{ github.event.pull_request.head.sha || github.ref }}
     - name: Install Conda environment with Micromamba
       uses: mamba-org/provision-with-micromamba@v14
       with:
-        environment-file: environment.yml
+        environment-file: tests/environment-unit-tests.yml
         environment-name: DEVELOP
         channels: conda-forge
         cache-env: true
         extra-specs: |
           python=3.10
     - name: Install package
       run: |
@@ -134,15 +136,15 @@
     steps:
     - uses: actions/checkout@v3
       with:
         ref: ${{ github.event.pull_request.head.sha || github.ref }}
     - name: Install Conda environment with Micromamba
       uses: mamba-org/provision-with-micromamba@v12
       with:
-        environment-file: environment${{ matrix.extra }}.yml
+        environment-file: tests/environment-unit-tests${{ matrix.extra }}.yml
         environment-name: DEVELOP${{ matrix.extra }}
         channels: conda-forge
         cache-env: true
         cache-env-key: ubuntu-latest-${{ matrix.python-version }}${{ matrix.extra }}.
         extra-specs: |
           python=${{matrix.python-version }}
     - name: Install package
```

### Comparing `earthkit-data-0.1.3/.gitignore` & `earthkit-data-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/.pre-commit-config.yaml` & `earthkit-data-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/LICENSE` & `earthkit-data-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/Makefile` & `earthkit-data-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/PKG-INFO` & `earthkit-data-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-data
-Version: 0.1.3
+Version: 0.2.0
 Summary: A format-agnostic Python interface for geospatial data
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # earthkit-data
 
-![earthkit-data](https://raw.githubusercontent.com/ecmwf/earthkit-data/develop/earthkit-data.png)
+![earthkit-data](docs/_static/earthkit-data.png)
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
 
 A format-agnostic interface for geospatial data with a focus on meteorology and
 climate science.
 
 **DISCLAIMER**
```

### Comparing `earthkit-data-0.1.3/README.md` & `earthkit-data-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # earthkit-data
 
-![earthkit-data](https://raw.githubusercontent.com/ecmwf/earthkit-data/develop/earthkit-data.png)
+![earthkit-data](docs/_static/earthkit-data.png)
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
 
 A format-agnostic interface for geospatial data with a focus on meteorology and
 climate science.
 
 **DISCLAIMER**
```

### Comparing `earthkit-data-0.1.3/docs/Makefile` & `earthkit-data-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/_static/style.css` & `earthkit-data-0.2.0/docs/_static/style.css`

 * *Files 27% similar despite different names*

```diff
@@ -35,7 +35,14 @@
     overflow: visible;
 } */
 
 /* Hide notebooks warnings */
 .nboutput .stderr {
     display: none;
 }
+
+/*
+Set logo size
+*/
+.wy-side-nav-search .wy-dropdown > a img.logo, .wy-side-nav-search > a img.logo {
+    width: 80px;
+}
```

### Comparing `earthkit-data-0.1.3/docs/development.rst` & `earthkit-data-0.2.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/bufr.ipynb` & `earthkit-data-0.2.0/docs/examples/odb.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9519231798061719%*

 * *Differences: {"'cells'": "{0: {'cell_type': 'markdown', 'id': '4cf9f31e-4b58-43bd-842e-142f0affb4a8', 'source': "*

 * *            "['## Using ODB data'], delete: ['execution_count', 'outputs']}, 1: {'cell_type': "*

 * *            "'code', 'id': '03108956-3f8e-4132-88e4-7455a4cc78dc', 'source': ['import "*

 * *            'earthkit.data\\n\', \'earthkit.data.download_example_file("test.odb")\'], '*

 * *            "'execution_count': 1, 'outputs': []}, 2: {'id': "*

 * *            "'08cd75b9-6685-4a49-99a7-c5d8a7acc80b', 'source': "*

 * *           […]*

```diff
@@ -1,80 +1,58 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "id": "27c5ff09-4f9f-4eb0-947e-5e75b56a65ba",
+            "cell_type": "markdown",
+            "id": "4cf9f31e-4b58-43bd-842e-142f0affb4a8",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "!test -f temp_10.bufr || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/temp_10.bufr"
+                "## Using ODB data"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "102b1cf9-33a5-4310-af4d-bcd17d598d29",
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "03108956-3f8e-4132-88e4-7455a4cc78dc",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Using BUFR data"
+                "import earthkit.data\n",
+                "earthkit.data.download_example_file(\"test.odb\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e11bb141-5f5d-42c2-9083-3cccbf9b7799",
+            "id": "08cd75b9-6685-4a49-99a7-c5d8a7acc80b",
             "metadata": {},
             "source": [
-                "We load a BUFR file with radiosonde observations."
+                "[ODB](https://odc.readthedocs.io/en/latest/content/introduction.html) is a bespoke format developed at ECMWF to store observations. The following code reads some ODB data from a file containing forecast and analysis departures:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "41f29800-f75d-4adf-a7b9-7fb0381dadd5",
+            "id": "d2f705e7-8336-4355-9b60-1fe05d8e23b3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import earthkit.data\n",
-                "\n",
-                "fs = earthkit.data.from_source(\"file\", \"temp_10.bufr\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
-            "id": "07571864-48af-451b-be4a-6a42436d193c",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "10"
-                        ]
-                    },
-                    "execution_count": 3,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "len(fs)"
+                "ds = earthkit.data.from_source(\"file\", \"test.odb\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "06d99f09-8d9d-4677-8aec-275787162a27",
+            "id": "6a0702a9-0b1a-46e6-bac3-71c78050f2e4",
             "metadata": {},
             "source": [
-                "We can call head(), tail() and ls() to see metadata from the header section of the BUFR messages: "
+                "*to_pandas()* converts data into a Pandas dataframe (uses [pyodc](https://github.com/ecmwf/pyodc) under the hood):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "id": "30e7749a-ea8b-43d2-90d2-31907f228513",
+            "execution_count": 3,
+            "id": "2f252c91-3cc9-46ec-b262-3b2f399ce05d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -90,152 +68,142 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>edition</th>\n",
-                            "      <th>type</th>\n",
-                            "      <th>subtype</th>\n",
-                            "      <th>c</th>\n",
-                            "      <th>mv</th>\n",
-                            "      <th>lv</th>\n",
-                            "      <th>subsets</th>\n",
-                            "      <th>compr</th>\n",
-                            "      <th>typicalDate</th>\n",
-                            "      <th>typicalTime</th>\n",
-                            "      <th>ident</th>\n",
                             "      <th>lat</th>\n",
                             "      <th>lon</th>\n",
+                            "      <th>fg_dep</th>\n",
+                            "      <th>an_dep</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>3</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>101</td>\n",
-                            "      <td>98</td>\n",
-                            "      <td>13</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>20081208</td>\n",
-                            "      <td>120000</td>\n",
-                            "      <td>02836</td>\n",
-                            "      <td>67.37</td>\n",
-                            "      <td>26.63</td>\n",
+                            "      <td>38.808998</td>\n",
+                            "      <td>4.292600</td>\n",
+                            "      <td>0.514543</td>\n",
+                            "      <td>0.513129</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>3</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>101</td>\n",
-                            "      <td>98</td>\n",
-                            "      <td>13</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>20081208</td>\n",
-                            "      <td>120000</td>\n",
-                            "      <td>01400</td>\n",
-                            "      <td>56.90</td>\n",
-                            "      <td>3.35</td>\n",
+                            "      <td>73.693100</td>\n",
+                            "      <td>-3.416700</td>\n",
+                            "      <td>-0.098977</td>\n",
+                            "      <td>-0.123831</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>3</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>101</td>\n",
-                            "      <td>98</td>\n",
-                            "      <td>13</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>20081208</td>\n",
-                            "      <td>120000</td>\n",
-                            "      <td>01415</td>\n",
-                            "      <td>58.87</td>\n",
-                            "      <td>5.67</td>\n",
+                            "      <td>31.168501</td>\n",
+                            "      <td>-29.865499</td>\n",
+                            "      <td>0.420131</td>\n",
+                            "      <td>0.389983</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>3</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>101</td>\n",
-                            "      <td>98</td>\n",
-                            "      <td>13</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>20081208</td>\n",
-                            "      <td>120000</td>\n",
-                            "      <td>01001</td>\n",
-                            "      <td>70.93</td>\n",
-                            "      <td>-8.67</td>\n",
+                            "      <td>49.040798</td>\n",
+                            "      <td>-19.877501</td>\n",
+                            "      <td>-0.182703</td>\n",
+                            "      <td>-0.124131</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>3</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>101</td>\n",
-                            "      <td>98</td>\n",
-                            "      <td>13</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>20081208</td>\n",
-                            "      <td>120000</td>\n",
-                            "      <td>01152</td>\n",
-                            "      <td>67.28</td>\n",
-                            "      <td>14.45</td>\n",
+                            "      <td>73.351097</td>\n",
+                            "      <td>40.176102</td>\n",
+                            "      <td>0.087687</td>\n",
+                            "      <td>0.149949</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>...</th>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>712</th>\n",
+                            "      <td>45.798801</td>\n",
+                            "      <td>-0.527100</td>\n",
+                            "      <td>0.103859</td>\n",
+                            "      <td>0.132765</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>713</th>\n",
+                            "      <td>73.788597</td>\n",
+                            "      <td>-8.806200</td>\n",
+                            "      <td>-0.069707</td>\n",
+                            "      <td>-0.080577</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>714</th>\n",
+                            "      <td>60.162998</td>\n",
+                            "      <td>-14.572900</td>\n",
+                            "      <td>0.138816</td>\n",
+                            "      <td>0.011107</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>715</th>\n",
+                            "      <td>53.455299</td>\n",
+                            "      <td>-29.641600</td>\n",
+                            "      <td>0.082582</td>\n",
+                            "      <td>0.184872</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>716</th>\n",
+                            "      <td>40.669201</td>\n",
+                            "      <td>29.702101</td>\n",
+                            "      <td>-0.023861</td>\n",
+                            "      <td>-0.032721</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
+                            "<p>717 rows \u00d7 4 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "   edition  type  subtype   c  mv  lv  subsets  compr typicalDate typicalTime  \\\n",
-                            "0        3     2      101  98  13   1        1      0    20081208      120000   \n",
-                            "1        3     2      101  98  13   1        1      0    20081208      120000   \n",
-                            "2        3     2      101  98  13   1        1      0    20081208      120000   \n",
-                            "3        3     2      101  98  13   1        1      0    20081208      120000   \n",
-                            "4        3     2      101  98  13   1        1      0    20081208      120000   \n",
+                            "           lat        lon    fg_dep    an_dep\n",
+                            "0    38.808998   4.292600  0.514543  0.513129\n",
+                            "1    73.693100  -3.416700 -0.098977 -0.123831\n",
+                            "2    31.168501 -29.865499  0.420131  0.389983\n",
+                            "3    49.040798 -19.877501 -0.182703 -0.124131\n",
+                            "4    73.351097  40.176102  0.087687  0.149949\n",
+                            "..         ...        ...       ...       ...\n",
+                            "712  45.798801  -0.527100  0.103859  0.132765\n",
+                            "713  73.788597  -8.806200 -0.069707 -0.080577\n",
+                            "714  60.162998 -14.572900  0.138816  0.011107\n",
+                            "715  53.455299 -29.641600  0.082582  0.184872\n",
+                            "716  40.669201  29.702101 -0.023861 -0.032721\n",
                             "\n",
-                            "   ident    lat    lon  \n",
-                            "0  02836  67.37  26.63  \n",
-                            "1  01400  56.90   3.35  \n",
-                            "2  01415  58.87   5.67  \n",
-                            "3  01001  70.93  -8.67  \n",
-                            "4  01152  67.28  14.45  "
+                            "[717 rows x 4 columns]"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs.head()"
+                "df = ds.to_pandas()\n",
+                "df"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "id": "07ca0ea4-cad9-4973-ac79-681f9140c116",
+            "id": "83537ee3-30c8-4797-a550-7387a0e72672",
             "metadata": {},
             "source": [
-                "to_pandas() extracts data into a Pandas dataframe (uses [pdbufr](\"https://github.com/ecmwf/pdbufr\") under the hood). The following example shows how the get the temperature profile for a given station:"
+                "We can directly pass arguments to pyodc. E.g. **columns** specify a subset of the ODB columns we want to extract:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "53ac87d6-09b9-46c3-bc54-07fd2a175b05",
+            "execution_count": 4,
+            "id": "fa1f0e84-a66e-426d-9a23-fc4329afd34e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -251,135 +219,122 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>pressure</th>\n",
-                            "      <th>airTemperature</th>\n",
-                            "      <th>data_datetime</th>\n",
-                            "      <th>WMO_station_id</th>\n",
+                            "      <th>lat</th>\n",
+                            "      <th>lon</th>\n",
+                            "      <th>an_dep</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>100300.0</td>\n",
-                            "      <td>279.8</td>\n",
-                            "      <td>2008-12-08 12:00:00</td>\n",
-                            "      <td>1415</td>\n",
+                            "      <td>38.808998</td>\n",
+                            "      <td>4.292600</td>\n",
+                            "      <td>0.513129</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>100000.0</td>\n",
-                            "      <td>280.0</td>\n",
-                            "      <td>2008-12-08 12:00:00</td>\n",
-                            "      <td>1415</td>\n",
+                            "      <td>73.693100</td>\n",
+                            "      <td>-3.416700</td>\n",
+                            "      <td>-0.123831</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>98900.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>2008-12-08 12:00:00</td>\n",
-                            "      <td>1415</td>\n",
+                            "      <td>31.168501</td>\n",
+                            "      <td>-29.865499</td>\n",
+                            "      <td>0.389983</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>97800.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>2008-12-08 12:00:00</td>\n",
-                            "      <td>1415</td>\n",
+                            "      <td>49.040798</td>\n",
+                            "      <td>-19.877501</td>\n",
+                            "      <td>-0.124131</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>92500.0</td>\n",
-                            "      <td>275.2</td>\n",
-                            "      <td>2008-12-08 12:00:00</td>\n",
-                            "      <td>1415</td>\n",
+                            "      <td>73.351097</td>\n",
+                            "      <td>40.176102</td>\n",
+                            "      <td>0.149949</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>...</th>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>58</th>\n",
-                            "      <td>1840.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>2008-12-08 12:00:00</td>\n",
-                            "      <td>1415</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>59</th>\n",
-                            "      <td>1790.0</td>\n",
-                            "      <td>197.5</td>\n",
-                            "      <td>2008-12-08 12:00:00</td>\n",
-                            "      <td>1415</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>60</th>\n",
-                            "      <td>1500.0</td>\n",
-                            "      <td>193.1</td>\n",
-                            "      <td>2008-12-08 12:00:00</td>\n",
-                            "      <td>1415</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>61</th>\n",
-                            "      <td>1380.0</td>\n",
-                            "      <td>NaN</td>\n",
-                            "      <td>2008-12-08 12:00:00</td>\n",
-                            "      <td>1415</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>62</th>\n",
-                            "      <td>1370.0</td>\n",
-                            "      <td>193.1</td>\n",
-                            "      <td>2008-12-08 12:00:00</td>\n",
-                            "      <td>1415</td>\n",
+                            "      <th>712</th>\n",
+                            "      <td>45.798801</td>\n",
+                            "      <td>-0.527100</td>\n",
+                            "      <td>0.132765</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>713</th>\n",
+                            "      <td>73.788597</td>\n",
+                            "      <td>-8.806200</td>\n",
+                            "      <td>-0.080577</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>714</th>\n",
+                            "      <td>60.162998</td>\n",
+                            "      <td>-14.572900</td>\n",
+                            "      <td>0.011107</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>715</th>\n",
+                            "      <td>53.455299</td>\n",
+                            "      <td>-29.641600</td>\n",
+                            "      <td>0.184872</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>716</th>\n",
+                            "      <td>40.669201</td>\n",
+                            "      <td>29.702101</td>\n",
+                            "      <td>-0.032721</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>63 rows \u00d7 4 columns</p>\n",
+                            "<p>717 rows \u00d7 3 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "    pressure  airTemperature       data_datetime  WMO_station_id\n",
-                            "0   100300.0           279.8 2008-12-08 12:00:00            1415\n",
-                            "1   100000.0           280.0 2008-12-08 12:00:00            1415\n",
-                            "2    98900.0             NaN 2008-12-08 12:00:00            1415\n",
-                            "3    97800.0             NaN 2008-12-08 12:00:00            1415\n",
-                            "4    92500.0           275.2 2008-12-08 12:00:00            1415\n",
-                            "..       ...             ...                 ...             ...\n",
-                            "58    1840.0             NaN 2008-12-08 12:00:00            1415\n",
-                            "59    1790.0           197.5 2008-12-08 12:00:00            1415\n",
-                            "60    1500.0           193.1 2008-12-08 12:00:00            1415\n",
-                            "61    1380.0             NaN 2008-12-08 12:00:00            1415\n",
-                            "62    1370.0           193.1 2008-12-08 12:00:00            1415\n",
+                            "           lat        lon    an_dep\n",
+                            "0    38.808998   4.292600  0.513129\n",
+                            "1    73.693100  -3.416700 -0.123831\n",
+                            "2    31.168501 -29.865499  0.389983\n",
+                            "3    49.040798 -19.877501 -0.124131\n",
+                            "4    73.351097  40.176102  0.149949\n",
+                            "..         ...        ...       ...\n",
+                            "712  45.798801  -0.527100  0.132765\n",
+                            "713  73.788597  -8.806200 -0.080577\n",
+                            "714  60.162998 -14.572900  0.011107\n",
+                            "715  53.455299 -29.641600  0.184872\n",
+                            "716  40.669201  29.702101 -0.032721\n",
                             "\n",
-                            "[63 rows x 4 columns]"
+                            "[717 rows x 3 columns]"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df = fs.to_pandas(columns=(\"WMO_station_id\", \"data_datetime\", \"pressure\", \"airTemperature\"),\n",
-                "    filters={\"WMO_station_id\": 1415})\n",
-                "df"
+                "df1 = ds.to_pandas(odc_read_odb_kwargs={\"columns\": (\"lat\", \"lon\", \"an_dep\")})\n",
+                "df1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "06ca403f-0998-473c-a733-f834f4b61fdf",
+            "id": "62568d51-78d6-46f0-852e-3ed1ccef5da5",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `earthkit-data-0.1.3/docs/examples/cds.ipynb` & `earthkit-data-0.2.0/docs/examples/cds.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/fdb.ipynb` & `earthkit-data-0.2.0/docs/examples/fdb.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9689171254579341%*

 * *Differences: {"'cells'": "{0: {delete: ['attachments']}, 2: {delete: ['attachments']}, 4: {'execution_count': "*

 * *            'None, \'source\': {insert: [(4, "    \'date\': \'20230607\',\\n"), (10, "    '*

 * *            '\'param\': [151, 167, 168]\\n")], delete: [10, 4]}}, 7: {delete: [\'attachments\']}, '*

 * *            "9: {'outputs': {0: {'text': ['GribField(msl,None,20230607,0,0,0)\\n', "*

 * *            "'GribField(2t,None,20230607,0,0,0)\\n', 'GribField(2d,None,20230607,0,0,0)\\n', "*

 * *            "'GribField(msl,None,20230607 […]*

```diff
@@ -1,11 +1,10 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "hourly-multimedia",
             "metadata": {},
             "source": [
                 "## Retrieving data from FDB"
             ]
         },
@@ -16,15 +15,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import earthkit.data"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "numerous-france",
             "metadata": {},
             "source": [
                 "FDB (Fields DataBase) is a domain-specific object store developed at ECMWF for storing, indexing and retrieving GRIB data. For more information on FBD please consult the following pages:\n",
                 "\n",
                 "- [FDB](https://fields-database.readthedocs.io/en/latest/)\n",
@@ -39,30 +37,30 @@
             "metadata": {},
             "source": [
                 "The following request was  written to retrieve data from the operational FDB at ECMWF.  Please note that the **date** must be adjusted since FDB at ECMWF only stores the most recent dates."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "id": "drawn-renewal",
             "metadata": {},
             "outputs": [],
             "source": [
                 "request = {\n",
                 "    'class': 'od',\n",
                 "    'expver': '0001',\n",
                 "    'stream': 'oper',\n",
-                "    'date': '20230524',\n",
+                "    'date': '20230607',\n",
                 "    'time': [0, 12],\n",
                 "    'domain': 'g',\n",
                 "    'type': 'an',\n",
                 "    'levtype': 'sfc',\n",
                 "    'step': 0,\n",
-                "    'param': [151, 167]\n",
+                "    'param': [151, 167, 168]\n",
                 "}"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "compound-pastor",
             "metadata": {},
@@ -75,15 +73,14 @@
             "id": "driving-delivery",
             "metadata": {},
             "source": [
                 "We can retrieve data from FDB as a stream."
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "bizarre-threshold",
             "metadata": {},
             "source": [
                 "#### Stream: iteration with one field at a time in memory"
             ]
         },
@@ -101,18 +98,20 @@
             "id": "signal-rocket",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "GribField(msl,None,20230524,0,0,0)\n",
-                        "GribField(2t,None,20230524,0,0,0)\n",
-                        "GribField(msl,None,20230524,1200,0,0)\n",
-                        "GribField(2t,None,20230524,1200,0,0)\n"
+                        "GribField(msl,None,20230607,0,0,0)\n",
+                        "GribField(2t,None,20230607,0,0,0)\n",
+                        "GribField(2d,None,20230607,0,0,0)\n",
+                        "GribField(msl,None,20230607,1200,0,0)\n",
+                        "GribField(2t,None,20230607,1200,0,0)\n",
+                        "GribField(2d,None,20230607,1200,0,0)\n"
                     ]
                 }
             ],
             "source": [
                 "ds = earthkit.data.from_source(\"fdb\", request)\n",
                 "for f in ds:\n",
                 "    print(f)"
@@ -127,18 +126,75 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "blank-affiliate",
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "0"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "sum([1 for _ in ds])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "7e63bb45-b15d-4a89-b882-bf4db27d4f39",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "#### Stream: using group_by"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "c2c8809e-9d53-4c69-af57-e3617e1df8b8",
+            "metadata": {},
+            "source": [
+                "When we use the **group_by** option `from_source()` gives us a stream iterator object. Each iteration step results in a Fieldlist object, which is built by consuming GRIB messages from the stream until the values of the metadata keys specified in *group_by* change. The generated Fieldlist keeps GRIB messages in memory then gets deleted when going out of scope."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "574757de-cc05-4d73-b71c-cd49af36f655",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
+                        " GribField(msl,None,20230607,0,0,0)\n",
+                        " GribField(2t,None,20230607,0,0,0)\n",
+                        " GribField(2d,None,20230607,0,0,0)\n",
+                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
+                        " GribField(msl,None,20230607,1200,0,0)\n",
+                        " GribField(2t,None,20230607,1200,0,0)\n",
+                        " GribField(2d,None,20230607,1200,0,0)\n"
+                    ]
+                }
+            ],
             "source": [
+                "ds = earthkit.data.from_source(\"fdb\", request, group_by=\"time\")\n",
                 "for f in ds:\n",
-                "    print(f)"
+                "    print(type(f))\n",
+                "    for g in f:\n",
+                "        print(f\" {g}\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ethical-canyon",
             "metadata": {},
             "source": [
@@ -146,40 +202,45 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "standard-soviet",
             "metadata": {},
             "source": [
-                "We can read multiple fields into memory from the stream at a time by using **batch_size** in *from_source()*:"
+                "We can read multiple fields into memory from the stream at a time by using **batch_size** in *from_source()*, Please note that *batch_size* cannot be used together with *group_by*."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "id": "precise-guyana",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2\n",
-                        "['msl', '2t']\n",
-                        "2\n",
-                        "['msl', '2t']\n"
+                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
+                        " GribField(msl,None,20230607,0,0,0)\n",
+                        " GribField(2t,None,20230607,0,0,0)\n",
+                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
+                        " GribField(2d,None,20230607,0,0,0)\n",
+                        " GribField(msl,None,20230607,1200,0,0)\n",
+                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
+                        " GribField(2t,None,20230607,1200,0,0)\n",
+                        " GribField(2d,None,20230607,1200,0,0)\n"
                     ]
                 }
             ],
             "source": [
                 "ds = earthkit.data.from_source(\"fdb\", request, batch_size=2)\n",
                 "for f in ds:\n",
-                "    # f is a FieldList containing 2 fields. It gets deleted when going out of scope\n",
-                "    print(len(f))\n",
-                "    print(f.metadata(\"param\"))"
+                "    print(type(f))\n",
+                "    for g in f:\n",
+                "        print(f\" {g}\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "through-seven",
             "metadata": {},
             "source": [
@@ -187,20 +248,20 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "personal-sense",
             "metadata": {},
             "source": [
-                "When we use **batch_size=0** all the fields are loaded into memory and the resulting object iswill behave like a FieldList"
+                "When we use **batch_size=0** all the fields are loaded into memory and the resulting object iswill behave like a FieldList:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "id": "bizarre-basket",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ds = earthkit.data.from_source(\"fdb\", request, batch_size=0)"
             ]
         },
@@ -210,15 +271,15 @@
             "metadata": {},
             "source": [
                 "Nothing is read at this moment:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "id": "defensive-spell",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -236,54 +297,54 @@
             "metadata": {},
             "source": [
                 "If we call any function on the fieldlist it reads the messages into memory"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "id": "exciting-accused",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "4"
+                            "6"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "len(ds)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "id": "efficient-submission",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "stored fields count=4\n"
+                        "stored fields count=6\n"
                     ]
                 }
             ],
             "source": [
                 "print(f\"stored fields count={len(ds._reader._fields)}\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "id": "minus-horizon",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -319,101 +380,124 @@
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>msl</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230524</td>\n",
+                            "      <td>20230607</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230524</td>\n",
+                            "      <td>20230607</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
+                            "      <td>2d</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230607</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>reduced_gg</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>ecmf</td>\n",
                             "      <td>msl</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230524</td>\n",
+                            "      <td>20230607</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>3</th>\n",
+                            "      <th>4</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230524</td>\n",
+                            "      <td>20230607</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>reduced_gg</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>5</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>2d</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230607</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
-                            "0   ecmf       msl     surface      0  20230524         0         0       an   \n",
-                            "1   ecmf        2t     surface      0  20230524         0         0       an   \n",
-                            "2   ecmf       msl     surface      0  20230524      1200         0       an   \n",
-                            "3   ecmf        2t     surface      0  20230524      1200         0       an   \n",
+                            "0   ecmf       msl     surface      0  20230607         0         0       an   \n",
+                            "1   ecmf        2t     surface      0  20230607         0         0       an   \n",
+                            "2   ecmf        2d     surface      0  20230607         0         0       an   \n",
+                            "3   ecmf       msl     surface      0  20230607      1200         0       an   \n",
+                            "4   ecmf        2t     surface      0  20230607      1200         0       an   \n",
+                            "5   ecmf        2d     surface      0  20230607      1200         0       an   \n",
                             "\n",
                             "   number    gridType  \n",
                             "0       0  reduced_gg  \n",
                             "1       0  reduced_gg  \n",
                             "2       0  reduced_gg  \n",
-                            "3       0  reduced_gg  "
+                            "3       0  reduced_gg  \n",
+                            "4       0  reduced_gg  \n",
+                            "5       0  reduced_gg  "
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "id": "tamil-tattoo",
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "remapping={}\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
                             "        vertical-align: middle;\n",
                             "    }\n",
@@ -445,60 +529,60 @@
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230524</td>\n",
+                            "      <td>20230607</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230524</td>\n",
+                            "      <td>20230607</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
-                            "0   ecmf        2t     surface      0  20230524         0         0       an   \n",
-                            "1   ecmf        2t     surface      0  20230524      1200         0       an   \n",
+                            "0   ecmf        2t     surface      0  20230607         0         0       an   \n",
+                            "1   ecmf        2t     surface      0  20230607      1200         0       an   \n",
                             "\n",
                             "   number    gridType  \n",
                             "0       0  reduced_gg  \n",
                             "1       0  reduced_gg  "
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds.sel(param=\"2t\").ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "id": "assumed-month",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -864,60 +948,62 @@
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
                             "Dimensions:     (number: 1, time: 2, step: 1, surface: 1, values: 6599680)\n",
                             "Coordinates:\n",
                             "  * number      (number) int64 0\n",
-                            "  * time        (time) datetime64[ns] 2023-05-24 2023-05-24T12:00:00\n",
+                            "  * time        (time) datetime64[ns] 2023-06-07 2023-06-07T12:00:00\n",
                             "  * step        (step) timedelta64[ns] 00:00:00\n",
                             "  * surface     (surface) int64 0\n",
                             "    latitude    (values) float64 ...\n",
                             "    longitude   (values) float64 ...\n",
                             "    valid_time  (time, step) datetime64[ns] ...\n",
                             "Dimensions without coordinates: values\n",
                             "Data variables:\n",
                             "    msl         (number, time, step, surface, values) float32 ...\n",
                             "    t2m         (number, time, step, surface, values) float32 ...\n",
+                            "    d2m         (number, time, step, surface, values) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-05-26T07:07 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-fa78a10f-d9db-4c7e-bd3e-80361e7356d9' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-fa78a10f-d9db-4c7e-bd3e-80361e7356d9' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 2</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span>values</span>: 6599680</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-4586cc93-b6ba-4c38-8347-116a80f84a86' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4586cc93-b6ba-4c38-8347-116a80f84a86' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-b1c514bb-c70e-4420-83fb-49ee40e7b9a6' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b1c514bb-c70e-4420-83fb-49ee40e7b9a6' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-333ec79b-0849-456b-a125-292e586846c9' class='xr-var-data-in' type='checkbox'><label for='data-333ec79b-0849-456b-a125-292e586846c9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2023-05-24 2023-05-24T12:00:00</div><input id='attrs-b7221341-a7a1-4da6-8680-6946fcb11ef0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b7221341-a7a1-4da6-8680-6946fcb11ef0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-86f69536-4962-4a01-b74e-9c846ad9294b' class='xr-var-data-in' type='checkbox'><label for='data-86f69536-4962-4a01-b74e-9c846ad9294b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2023-05-24T00:00:00.000000000&#x27;, &#x27;2023-05-24T12:00:00.000000000&#x27;],\n",
-                            "      dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-2366611c-92f3-4e80-954b-904efbf7de2b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-2366611c-92f3-4e80-954b-904efbf7de2b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-2facf33b-36eb-4262-8db4-083480031731' class='xr-var-data-in' type='checkbox'><label for='data-2facf33b-36eb-4262-8db4-083480031731' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-a420068a-d7b2-4676-9fca-618cd8a8ae2c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a420068a-d7b2-4676-9fca-618cd8a8ae2c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f8edc595-7f3e-4c6e-a774-6dc73666374f' class='xr-var-data-in' type='checkbox'><label for='data-f8edc595-7f3e-4c6e-a774-6dc73666374f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>latitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-21c15ca7-c6e2-4dec-9919-b1c8e7ae246f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-21c15ca7-c6e2-4dec-9919-b1c8e7ae246f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d082669a-873b-4b72-97e6-8a89385204fc' class='xr-var-data-in' type='checkbox'><label for='data-d082669a-873b-4b72-97e6-8a89385204fc' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>longitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-175be16b-a5e9-43d3-bc9b-b14ce97084f0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-175be16b-a5e9-43d3-bc9b-b14ce97084f0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c2c965ef-055a-45a7-aedc-0c4545cc0280' class='xr-var-data-in' type='checkbox'><label for='data-c2c965ef-055a-45a7-aedc-0c4545cc0280' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-646dd9a0-aecb-463c-80a0-2780f98100ca' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-646dd9a0-aecb-463c-80a0-2780f98100ca' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c07c156f-2019-410c-b5a2-b67eb202664b' class='xr-var-data-in' type='checkbox'><label for='data-c07c156f-2019-410c-b5a2-b67eb202664b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[2 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-54c2e21f-1909-4e94-be1d-26e1d3b82ddc' class='xr-section-summary-in' type='checkbox'  checked><label for='section-54c2e21f-1909-4e94-be1d-26e1d3b82ddc' class='xr-section-summary' >Data variables: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>msl</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-ec5ae1e7-fe00-4070-8148-912b95b6bae6' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ec5ae1e7-fe00-4070-8148-912b95b6bae6' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-829fc772-2027-4df3-8abb-4404cd506bbf' class='xr-var-data-in' type='checkbox'><label for='data-829fc772-2027-4df3-8abb-4404cd506bbf' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>151</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>air_pressure_at_mean_sea_level</dd><dt><span>GRIB_cfVarName :</span></dt><dd>msl</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>msl</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>Pa</dd><dt><span>long_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>units :</span></dt><dd>Pa</dd><dt><span>standard_name :</span></dt><dd>air_pressure_at_mean_sea_level</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-18359663-687c-4ee6-a919-2a739ed1460f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-18359663-687c-4ee6-a919-2a739ed1460f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-59cced59-1037-4e94-9082-18250deac157' class='xr-var-data-in' type='checkbox'><label for='data-59cced59-1037-4e94-9082-18250deac157' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-c7353cab-a0a7-4206-adc0-f5f06d1ede8c' class='xr-section-summary-in' type='checkbox'  ><label for='section-c7353cab-a0a7-4206-adc0-f5f06d1ede8c' class='xr-section-summary' >Indexes: <span>(4)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e5f4101a-e60c-447d-92f0-99c01b927616' class='xr-index-data-in' type='checkbox'/><label for='index-e5f4101a-e60c-447d-92f0-99c01b927616' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-0ffe7750-3f7f-4739-90d6-bada21420101' class='xr-index-data-in' type='checkbox'/><label for='index-0ffe7750-3f7f-4739-90d6-bada21420101' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2023-05-24 00:00:00&#x27;, &#x27;2023-05-24 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-350d14ec-5453-4813-b52b-b48de373bc23' class='xr-index-data-in' type='checkbox'/><label for='index-350d14ec-5453-4813-b52b-b48de373bc23' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-79f62cb5-d16d-48f1-a6dd-8e9b7083bcc0' class='xr-index-data-in' type='checkbox'/><label for='index-79f62cb5-d16d-48f1-a6dd-8e9b7083bcc0' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;surface&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-95e25296-ccc0-4b92-bb44-1885c151bfb1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-95e25296-ccc0-4b92-bb44-1885c151bfb1' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-05-26T07:07 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.30.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "    history:                 2023-06-08T11:49 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-dffa6f53-9be8-4f08-b96d-8904340a6bce' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-dffa6f53-9be8-4f08-b96d-8904340a6bce' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 2</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span>values</span>: 6599680</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-4aa2ffb9-169a-4df0-a8c7-7494a8bfde98' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4aa2ffb9-169a-4df0-a8c7-7494a8bfde98' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-1a9630df-a093-49b8-81fc-998188fc867f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1a9630df-a093-49b8-81fc-998188fc867f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-573b4489-a728-44fb-a034-64e092778b11' class='xr-var-data-in' type='checkbox'><label for='data-573b4489-a728-44fb-a034-64e092778b11' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2023-06-07 2023-06-07T12:00:00</div><input id='attrs-48835aef-88a4-4163-af88-998054832d94' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-48835aef-88a4-4163-af88-998054832d94' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e5ef026a-dde8-4b86-92fb-8c92dc2aa96d' class='xr-var-data-in' type='checkbox'><label for='data-e5ef026a-dde8-4b86-92fb-8c92dc2aa96d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2023-06-07T00:00:00.000000000&#x27;, &#x27;2023-06-07T12:00:00.000000000&#x27;],\n",
+                            "      dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-4c5c85af-316a-41ca-a195-cc7dafe614eb' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-4c5c85af-316a-41ca-a195-cc7dafe614eb' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f5e52f65-860b-4dfb-9461-e6165ec0e935' class='xr-var-data-in' type='checkbox'><label for='data-f5e52f65-860b-4dfb-9461-e6165ec0e935' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-53f01bfd-1aa2-4859-ab67-eb15ded06ae9' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-53f01bfd-1aa2-4859-ab67-eb15ded06ae9' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-93afaf42-acff-498e-ace0-3d2353ba22cc' class='xr-var-data-in' type='checkbox'><label for='data-93afaf42-acff-498e-ace0-3d2353ba22cc' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>latitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-58d3c743-4dbc-4bba-90cb-11de8f473751' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-58d3c743-4dbc-4bba-90cb-11de8f473751' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-64a97a47-7f81-4f8b-ad23-329f98f82e6f' class='xr-var-data-in' type='checkbox'><label for='data-64a97a47-7f81-4f8b-ad23-329f98f82e6f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>longitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-eef38fe3-2175-45d5-a024-198dbbd3c75f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-eef38fe3-2175-45d5-a024-198dbbd3c75f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-8339d5e0-48bf-4a0c-ac02-23c5cd78c511' class='xr-var-data-in' type='checkbox'><label for='data-8339d5e0-48bf-4a0c-ac02-23c5cd78c511' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-390e52c5-14ba-49c9-82d6-a054a9073006' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-390e52c5-14ba-49c9-82d6-a054a9073006' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e7fed87e-5f2b-4966-b395-25ccdc9c148c' class='xr-var-data-in' type='checkbox'><label for='data-e7fed87e-5f2b-4966-b395-25ccdc9c148c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[2 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-eadc2df8-fe5a-4fd8-bcc2-90ca3b6f069b' class='xr-section-summary-in' type='checkbox'  checked><label for='section-eadc2df8-fe5a-4fd8-bcc2-90ca3b6f069b' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>msl</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-2b96ae7d-bcf0-4389-8e0e-8c7692f48f22' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-2b96ae7d-bcf0-4389-8e0e-8c7692f48f22' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1afea29b-c647-49b9-8df4-e63febac087d' class='xr-var-data-in' type='checkbox'><label for='data-1afea29b-c647-49b9-8df4-e63febac087d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>151</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>air_pressure_at_mean_sea_level</dd><dt><span>GRIB_cfVarName :</span></dt><dd>msl</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>msl</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>Pa</dd><dt><span>long_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>units :</span></dt><dd>Pa</dd><dt><span>standard_name :</span></dt><dd>air_pressure_at_mean_sea_level</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-8a90e69d-4b2b-4d07-90b6-8e058b2b054f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-8a90e69d-4b2b-4d07-90b6-8e058b2b054f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c8019ebc-d953-4385-88d0-4da64d674f83' class='xr-var-data-in' type='checkbox'><label for='data-c8019ebc-d953-4385-88d0-4da64d674f83' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>d2m</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-9594c5ef-de0f-4eaf-a673-1e659f0f881e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9594c5ef-de0f-4eaf-a673-1e659f0f881e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e1b705fe-931e-4b6b-8d5c-eefe712dbe9d' class='xr-var-data-in' type='checkbox'><label for='data-e1b705fe-931e-4b6b-8d5c-eefe712dbe9d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>168</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>d2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre dewpoint temperature</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>2d</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre dewpoint temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-38390609-7e8f-4a32-9f4c-05d9e9938f39' class='xr-section-summary-in' type='checkbox'  ><label for='section-38390609-7e8f-4a32-9f4c-05d9e9938f39' class='xr-section-summary' >Indexes: <span>(4)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-43f14fe3-5973-4c20-bdc0-ce88d73bfe0f' class='xr-index-data-in' type='checkbox'/><label for='index-43f14fe3-5973-4c20-bdc0-ce88d73bfe0f' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-332e6b04-16fa-4f1b-97d4-ad30202e90d9' class='xr-index-data-in' type='checkbox'/><label for='index-332e6b04-16fa-4f1b-97d4-ad30202e90d9' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2023-06-07 00:00:00&#x27;, &#x27;2023-06-07 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-3349020b-286d-445c-b847-d235c85e2753' class='xr-index-data-in' type='checkbox'/><label for='index-3349020b-286d-445c-b847-d235c85e2753' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e8cf740b-5f14-46cf-a62d-2f380bc34f3c' class='xr-index-data-in' type='checkbox'/><label for='index-e8cf740b-5f14-46cf-a62d-2f380bc34f3c' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;surface&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-64a95d2a-9d62-4c0a-a2b2-258e446ec68a' class='xr-section-summary-in' type='checkbox'  checked><label for='section-64a95d2a-9d62-4c0a-a2b2-258e446ec68a' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-06-08T11:49 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.30.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:     (number: 1, time: 2, step: 1, surface: 1, values: 6599680)\n",
                             "Coordinates:\n",
                             "  * number      (number) int64 0\n",
-                            "  * time        (time) datetime64[ns] 2023-05-24 2023-05-24T12:00:00\n",
+                            "  * time        (time) datetime64[ns] 2023-06-07 2023-06-07T12:00:00\n",
                             "  * step        (step) timedelta64[ns] 00:00:00\n",
                             "  * surface     (surface) int64 0\n",
                             "    latitude    (values) float64 ...\n",
                             "    longitude   (values) float64 ...\n",
                             "    valid_time  (time, step) datetime64[ns] ...\n",
                             "Dimensions without coordinates: values\n",
                             "Data variables:\n",
                             "    msl         (number, time, step, surface, values) float32 ...\n",
                             "    t2m         (number, time, step, surface, values) float32 ...\n",
+                            "    d2m         (number, time, step, surface, values) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-05-26T07:07 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2023-06-08T11:49 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds.to_xarray()"
             ]
@@ -936,25 +1022,25 @@
             "metadata": {},
             "source": [
                 "We can retrieve data from FDB into a file, which is located in the cache: "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 14,
             "id": "passing-georgia",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ds = earthkit.data.from_source(\"fdb\", request, stream=False)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 15,
             "id": "foster-profile",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -990,79 +1076,109 @@
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>msl</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230524</td>\n",
+                            "      <td>20230607</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230524</td>\n",
+                            "      <td>20230607</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
+                            "      <td>2d</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230607</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>reduced_gg</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>ecmf</td>\n",
                             "      <td>msl</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230524</td>\n",
+                            "      <td>20230607</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>3</th>\n",
+                            "      <th>4</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230524</td>\n",
+                            "      <td>20230607</td>\n",
+                            "      <td>1200</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>an</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>reduced_gg</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>5</th>\n",
+                            "      <td>ecmf</td>\n",
+                            "      <td>2d</td>\n",
+                            "      <td>surface</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>20230607</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
-                            "0   ecmf       msl     surface      0  20230524         0         0       an   \n",
-                            "1   ecmf        2t     surface      0  20230524         0         0       an   \n",
-                            "2   ecmf       msl     surface      0  20230524      1200         0       an   \n",
-                            "3   ecmf        2t     surface      0  20230524      1200         0       an   \n",
+                            "0   ecmf       msl     surface      0  20230607         0         0       an   \n",
+                            "1   ecmf        2t     surface      0  20230607         0         0       an   \n",
+                            "2   ecmf        2d     surface      0  20230607         0         0       an   \n",
+                            "3   ecmf       msl     surface      0  20230607      1200         0       an   \n",
+                            "4   ecmf        2t     surface      0  20230607      1200         0       an   \n",
+                            "5   ecmf        2d     surface      0  20230607      1200         0       an   \n",
                             "\n",
                             "   number    gridType  \n",
                             "0       0  reduced_gg  \n",
                             "1       0  reduced_gg  \n",
                             "2       0  reduced_gg  \n",
-                            "3       0  reduced_gg  "
+                            "3       0  reduced_gg  \n",
+                            "4       0  reduced_gg  \n",
+                            "5       0  reduced_gg  "
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds.ls()"
             ]
@@ -1082,27 +1198,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "pyfdb",
+            "display_name": "mpy38",
             "language": "python",
-            "name": "pyfdb"
+            "name": "mpy38"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.12"
+            "version": "3.8.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_file_pattern.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_file_pattern.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9348524305555556%*

 * *Differences: {"'cells'": "{2: {'execution_count': 1, 'outputs': {0: {'execution_count': 1}}, 'source': {insert: "*

 * *            "[(0, 'import earthkit.data\\n'), (1, '\\n')]}}, insert: [(3, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', "*

 * *            "'e87ac225-94b1-4d7e-8ed9-b71b301d711c'), ('metadata', OrderedDict()), ('outputs', "*

 * *            "[]), ('source', [])]))], delete: [1, 0]}"}*

```diff
@@ -1,33 +1,10 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "id": "96e90730-5bc9-420e-b67a-d6c69044db33",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "!test -f test4.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test4.grib\n",
-                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 2,
-            "id": "bc208232-02b2-4ce2-bfb8-34a480198f33",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import earthkit.data"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "id": "38237d70-0971-44a3-9cac-fd08071c8af9",
             "metadata": {},
             "source": [
                 "### Using file patterns"
             ]
         },
@@ -37,15 +14,15 @@
             "metadata": {},
             "source": [
                 "The \"file\" source can also be specified by using patterns. In the example below when pattern \"id\" is substituted it will match two files: test4.grib and test6.grib:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 1,
             "id": "d52872d1-8ff8-4f52-9ffc-9b72621a9a67",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -235,24 +212,34 @@
                             "5       an       0  regular_ll  \n",
                             "6       an       0  regular_ll  \n",
                             "7       an       0  regular_ll  \n",
                             "8       an       0  regular_ll  \n",
                             "9       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 3,
+                    "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "import earthkit.data\n",
+                "\n",
                 "fs = earthkit.data.from_source(\"file-pattern\", \"./test{id}.grib\",\n",
                 "                        {\"id\": [4, 6]})\n",
                 "fs.ls()"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "e87ac225-94b1-4d7e-8ed9-b71b301d711c",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "mpy38",
             "language": "python",
             "name": "mpy38"
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_from_stream.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_from_stream.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9667709103852591%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1}, 2: {'source': {insert: [(2, 'For simplicity, in this "*

 * *            'notebook we will use a **file stream** to demonstrate the usage of streams. First we '*

 * *            "ensure the example file is available.')], delete: [2]}, 'attachments': "*

 * *            "OrderedDict()}, 7: {'source': ['We load it into earthkit-data by using the default "*

 * *            'settings (batch_size=1). With this when we iterate through *fs* it will consume one '*

 * *            "message from the str […]*

```diff
@@ -1,45 +1,46 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "id": "collectible-accreditation",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "id": "recovered-organizer",
             "metadata": {},
             "source": [
                 "## Reading GRIB from a stream"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "id": "sticky-refrigerator",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import earthkit.data"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "german-simulation",
             "metadata": {},
             "source": [
                 "earthkit-data can load GRIB data from a **stream**, which can be an FDB stream, a standard Python IO stream or any object implementing the necessary stream methods. \n",
                 "\n",
-                "For simplicity, in this notebook we will use a **file stream** to demonstrate the usage of streams."
+                "For simplicity, in this notebook we will use a **file stream** to demonstrate the usage of streams. First we ensure the example file is available."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "939a3b56-a434-457c-966f-f5b8bb6d74dc",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "earthkit.data.download_example_file(\"test6.grib\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "prescribed-giant",
             "metadata": {},
             "source": [
@@ -65,15 +66,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "covered-greensboro",
             "metadata": {},
             "source": [
-                "We load it into earthkit-data by using the **batch_size=1** (default) option. With this when we iterate through *fs* it will consume one message from the stream at a time:"
+                "We load it into earthkit-data by using the default settings (batch_size=1). With this when we iterate through *fs* it will consume one message from the stream at a time:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "durable-helicopter",
             "metadata": {},
@@ -83,15 +84,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "resident-guard",
             "metadata": {},
             "source": [
-                "At this point nothing is read from the stream. As we progressing with the iteration GribField objects are created then get deleted when going out of scope. As a result there is only one GRIB message is kept in memory at a time."
+                "At this point nothing is read from the stream. As we progressing with the iteration GribField objects are created then get deleted when going out of scope. As a result, only one GRIB message is kept in memory at a time."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "animated-prayer",
             "metadata": {},
@@ -116,91 +117,167 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "brilliant-struggle",
             "metadata": {},
             "source": [
-                "Having finished the iteration there is no data available any longer in *fs*.  We can close the stream:"
+                "Having finished the iteration there is no data available in *fs*.  We can close the stream:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "unique-metadata",
             "metadata": {},
             "outputs": [],
             "source": [
                 "stream.close()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "7122a9a4-9ca0-4d75-9194-144074c6dcad",
+            "metadata": {},
+            "source": [
+                "### Using group_by"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "3b7e9e3c-df32-44c6-aa4a-fcd2ff72b3b2",
+            "metadata": {},
+            "source": [
+                "When we use the **group_by** option `from_source()` gives us a stream iterator object. Each iteration step results in a Fieldlist object, which is built by consuming GRIB messages from the stream until the values of the metadata keys specified in *group_by* change. The generated Fieldlist keeps GRIB messages in memory then gets deleted when going out of scope."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "8e1be478-6eb6-4732-bb96-9d6fa942c20d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "stream = open(\"test6.grib\", \"rb\")\n",
+                "fs = earthkit.data.from_source(\"stream\", stream, group_by=\"level\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "810cc3eb-4a3f-4806-b799-23e1bc5523c6",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
+                        " GribField(t,1000,20180801,1200,0,0)\n",
+                        " GribField(u,1000,20180801,1200,0,0)\n",
+                        " GribField(v,1000,20180801,1200,0,0)\n",
+                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
+                        " GribField(t,850,20180801,1200,0,0)\n",
+                        " GribField(u,850,20180801,1200,0,0)\n",
+                        " GribField(v,850,20180801,1200,0,0)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "for f in fs:\n",
+                "    print(type(f))\n",
+                "    for g in f:\n",
+                "        print(f\" {g}\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "89d33d4c-00d2-4f0b-996e-aaf5a5c9e161",
+            "metadata": {},
+            "source": [
+                "Having finished the iteration there is no data available in *fs*.  We can close the stream:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "2ac79f14-cb43-40c0-8a56-9bc16943d7e7",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "stream.close()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "judicial-backing",
             "metadata": {},
             "source": [
                 "### Using batch_size"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "planned-weekly",
             "metadata": {},
             "source": [
-                "This time we create a stream and read 2 fields from it at a time by using **batch_size=2** in *from_source()*:"
+                "The **batch_size** option controls how many fields we read from the stream in one go. Please note that *batch_size* cannot be used together with *group_by*. In this example we create a stream and read 2 fields from it at a time by using **batch_size=2** in *from_source()*:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 10,
             "id": "placed-blues",
             "metadata": {},
             "outputs": [],
             "source": [
                 "stream = open(\"test6.grib\", \"rb\")\n",
                 "fs = earthkit.data.from_source(\"stream\", stream, batch_size=2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 11,
             "id": "outside-tennis",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2\n",
-                        "['t', 'u']\n",
-                        "2\n",
-                        "['v', 't']\n",
-                        "2\n",
-                        "['u', 'v']\n"
+                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
+                        " GribField(t,1000,20180801,1200,0,0)\n",
+                        " GribField(u,1000,20180801,1200,0,0)\n",
+                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
+                        " GribField(v,1000,20180801,1200,0,0)\n",
+                        " GribField(t,850,20180801,1200,0,0)\n",
+                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
+                        " GribField(u,850,20180801,1200,0,0)\n",
+                        " GribField(v,850,20180801,1200,0,0)\n"
                     ]
                 }
             ],
             "source": [
                 "for f in fs:\n",
-                "    # f is a FieldList containing 2 fields. It gets deleted when going out of scope\n",
-                "    print(len(f))\n",
-                "    print(f.metadata(\"param\"))"
+                "    print(type(f))\n",
+                "    for g in f:\n",
+                "        print(f\" {g}\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "unavailable-actress",
             "metadata": {},
             "source": [
-                "Having finished the iteration there is no data available any longer in *fs*.  We can close the stream:"
+                "Having finished the iteration there is no data available in *fs*.  We can close the stream:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 12,
             "id": "jewish-season",
             "metadata": {},
             "outputs": [],
             "source": [
                 "stream.close()"
             ]
         },
@@ -218,15 +295,15 @@
             "metadata": {},
             "source": [
                 "We can also set **batch_size=0** in *from_source()*:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 13,
             "id": "simple-london",
             "metadata": {},
             "outputs": [],
             "source": [
                 "stream = open(\"test6.grib\", \"rb\")\n",
                 "fs = earthkit.data.from_source(\"stream\", stream, batch_size=0)"
             ]
@@ -239,36 +316,36 @@
                 "The resulting earthkit-data object is empty at this point. However, as soon as we call any method on it it will consume the whole stream and load all the GRIB messages into memory. They will be stored in memory as long as *fs* exists.\n",
                 "\n",
                 "We can call all the standard earthkit-data methods on *fs*:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 14,
             "id": "meaning-oxide",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "6"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "len(fs)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 15,
             "id": "copyrighted-walnut",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -398,26 +475,26 @@
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  \n",
                             "3       an       0  regular_ll  \n",
                             "4       an       0  regular_ll  \n",
                             "5       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 16,
             "id": "static-reasoning",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -487,27 +564,27 @@
                             "1   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a = fs.sel(param=\"t\")\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 17,
             "id": "spanish-wagon",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -876,56 +953,56 @@
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
                             "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * number         (number) int64 0\n",
                             "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
                             "  * step           (step) timedelta64[ns] 00:00:00\n",
-                            "  * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0\n",
+                            "  * isobaricInhPa  (isobaricInhPa) int64 1000 850\n",
                             "  * latitude       (latitude) float64 90.0 60.0 30.0 0.0 -30.0 -60.0 -90.0\n",
                             "  * longitude      (longitude) float64 0.0 30.0 60.0 90.0 ... 270.0 300.0 330.0\n",
                             "    valid_time     (time, step) datetime64[ns] ...\n",
                             "Data variables:\n",
                             "    t              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-d1102122-03a0-4c94-a5d5-9aa6331891c6' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-d1102122-03a0-4c94-a5d5-9aa6331891c6' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-1bfad17d-489c-4bdc-a9be-2261201199c1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-1bfad17d-489c-4bdc-a9be-2261201199c1' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-74878baa-8b46-4268-843e-75b535349650' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-74878baa-8b46-4268-843e-75b535349650' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-fd1a2a80-a11b-4fb7-80b1-7df3425546d5' class='xr-var-data-in' type='checkbox'><label for='data-fd1a2a80-a11b-4fb7-80b1-7df3425546d5' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-459d7a98-f21d-43c4-8b7f-d7320623694e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-459d7a98-f21d-43c4-8b7f-d7320623694e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-62fed23c-60e2-42aa-9c50-c4e6c28bfcf9' class='xr-var-data-in' type='checkbox'><label for='data-62fed23c-60e2-42aa-9c50-c4e6c28bfcf9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-e7dfcd39-0370-490d-8f4e-9e0a4c59e4a2' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e7dfcd39-0370-490d-8f4e-9e0a4c59e4a2' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-cbe7237d-c31b-43cc-8622-40affcf8f8d4' class='xr-var-data-in' type='checkbox'><label for='data-cbe7237d-c31b-43cc-8622-40affcf8f8d4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>1e+03 850.0</div><input id='attrs-674d75b1-141e-4018-94ed-9b461b091097' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-674d75b1-141e-4018-94ed-9b461b091097' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-cd99e54d-ce83-46f0-857c-a7871908233c' class='xr-var-data-in' type='checkbox'><label for='data-cd99e54d-ce83-46f0-857c-a7871908233c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000.,  850.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-76de01e4-646f-43fd-baeb-6cf24109b05b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-76de01e4-646f-43fd-baeb-6cf24109b05b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-26a9b8e8-322f-4292-a96a-b55fe11d1eb6' class='xr-var-data-in' type='checkbox'><label for='data-26a9b8e8-322f-4292-a96a-b55fe11d1eb6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-03e49b50-1a37-4301-8f2c-a587605e298c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-03e49b50-1a37-4301-8f2c-a587605e298c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f4f250f5-ab5e-4052-acae-29f207b3c8d2' class='xr-var-data-in' type='checkbox'><label for='data-f4f250f5-ab5e-4052-acae-29f207b3c8d2' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-fff6e7ad-b975-4ed4-b2db-c40deffcec45' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-fff6e7ad-b975-4ed4-b2db-c40deffcec45' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-8b1dd2a2-2317-494d-84eb-af2c90812d77' class='xr-var-data-in' type='checkbox'><label for='data-8b1dd2a2-2317-494d-84eb-af2c90812d77' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-99e0fcc8-e571-4ca9-a56a-47a96b8f5fea' class='xr-section-summary-in' type='checkbox'  checked><label for='section-99e0fcc8-e571-4ca9-a56a-47a96b8f5fea' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-504787b9-5383-4000-8bee-eb57f345fdf0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-504787b9-5383-4000-8bee-eb57f345fdf0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-3a8b3c65-707e-4e21-ba20-21e44f7825eb' class='xr-var-data-in' type='checkbox'><label for='data-3a8b3c65-707e-4e21-ba20-21e44f7825eb' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-7bcee6c5-54d1-47be-ae6b-070a01f7a6b6' class='xr-section-summary-in' type='checkbox'  ><label for='section-7bcee6c5-54d1-47be-ae6b-070a01f7a6b6' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-1e6aff8a-d34f-4523-a4d7-314f63ac9e46' class='xr-index-data-in' type='checkbox'/><label for='index-1e6aff8a-d34f-4523-a4d7-314f63ac9e46' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-bc7283a6-3b42-44aa-a35d-3a856d8858b8' class='xr-index-data-in' type='checkbox'/><label for='index-bc7283a6-3b42-44aa-a35d-3a856d8858b8' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-8a23791c-655d-4519-ac04-91b406350ced' class='xr-index-data-in' type='checkbox'/><label for='index-8a23791c-655d-4519-ac04-91b406350ced' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-07d43a66-10e8-42e6-aff0-ea8158d8ca00' class='xr-index-data-in' type='checkbox'/><label for='index-07d43a66-10e8-42e6-aff0-ea8158d8ca00' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([1000.0, 850.0], dtype=&#x27;float64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-0a7f772a-949e-4f4b-8fbc-ccb737da61f6' class='xr-index-data-in' type='checkbox'/><label for='index-0a7f772a-949e-4f4b-8fbc-ccb737da61f6' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9a50b678-4515-48e3-9f1b-335dca4a5adf' class='xr-index-data-in' type='checkbox'/><label for='index-9a50b678-4515-48e3-9f1b-335dca4a5adf' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
+                            "    history:                 2023-06-08T12:46 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-731477d2-fe41-4adb-baed-a595dcfecd3d' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-731477d2-fe41-4adb-baed-a595dcfecd3d' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-ce4e4447-10d3-4273-b2c5-5f00e4c31055' class='xr-section-summary-in' type='checkbox'  checked><label for='section-ce4e4447-10d3-4273-b2c5-5f00e4c31055' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-08cf44d9-6432-462b-a5a0-c119d7867516' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-08cf44d9-6432-462b-a5a0-c119d7867516' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-504226e8-d5ea-46c0-85c6-48ca7cb8d6ca' class='xr-var-data-in' type='checkbox'><label for='data-504226e8-d5ea-46c0-85c6-48ca7cb8d6ca' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-6afd3ea4-8459-4d4e-b3d8-8db82e558094' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6afd3ea4-8459-4d4e-b3d8-8db82e558094' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-745a938d-73d2-4686-8f44-defe2fdcd06a' class='xr-var-data-in' type='checkbox'><label for='data-745a938d-73d2-4686-8f44-defe2fdcd06a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-3726eb19-6c86-4f64-96a6-79732938e162' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-3726eb19-6c86-4f64-96a6-79732938e162' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f568088e-ee0d-4337-a8a0-1a7ce591cb07' class='xr-var-data-in' type='checkbox'><label for='data-f568088e-ee0d-4337-a8a0-1a7ce591cb07' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-09e30367-a39b-46ef-a5c5-dec5576483af' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-09e30367-a39b-46ef-a5c5-dec5576483af' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-b56b4332-105c-4449-bd4c-34ac16ef187a' class='xr-var-data-in' type='checkbox'><label for='data-b56b4332-105c-4449-bd4c-34ac16ef187a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-54fe7756-c5ab-4527-b89c-8ffbde0b6276' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-54fe7756-c5ab-4527-b89c-8ffbde0b6276' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-a3192ca7-df31-49e6-ae7c-bc6dca7af65e' class='xr-var-data-in' type='checkbox'><label for='data-a3192ca7-df31-49e6-ae7c-bc6dca7af65e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-50142c43-0158-4973-81cd-0beb8201d4a8' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-50142c43-0158-4973-81cd-0beb8201d4a8' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-079d774c-142e-42f5-9cc0-d07f13d3c020' class='xr-var-data-in' type='checkbox'><label for='data-079d774c-142e-42f5-9cc0-d07f13d3c020' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-8a14fb9b-6b9c-4864-a329-a8ed9f8e7b18' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-8a14fb9b-6b9c-4864-a329-a8ed9f8e7b18' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d135f31a-0d81-4bb2-baf4-f7719500273a' class='xr-var-data-in' type='checkbox'><label for='data-d135f31a-0d81-4bb2-baf4-f7719500273a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-1747c5fa-30d4-4f59-8764-8090930efe0e' class='xr-section-summary-in' type='checkbox'  checked><label for='section-1747c5fa-30d4-4f59-8764-8090930efe0e' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-28bce572-0820-4e27-8cb5-f1665add0f40' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-28bce572-0820-4e27-8cb5-f1665add0f40' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-0efb232b-92ed-4780-858f-7d87794678e9' class='xr-var-data-in' type='checkbox'><label for='data-0efb232b-92ed-4780-858f-7d87794678e9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-054d3d08-8d5c-43a1-9f6f-09d2cc8737cb' class='xr-section-summary-in' type='checkbox'  ><label for='section-054d3d08-8d5c-43a1-9f6f-09d2cc8737cb' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-847e3096-77fc-4edc-9a32-eea394fd3b30' class='xr-index-data-in' type='checkbox'/><label for='index-847e3096-77fc-4edc-9a32-eea394fd3b30' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-1d591b5e-3d75-4486-aff1-c450a6fc075a' class='xr-index-data-in' type='checkbox'/><label for='index-1d591b5e-3d75-4486-aff1-c450a6fc075a' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-b3cb05a8-fb5a-4b45-852f-20183f2e48c4' class='xr-index-data-in' type='checkbox'/><label for='index-b3cb05a8-fb5a-4b45-852f-20183f2e48c4' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-7bec313e-f2b5-40d7-a4ec-ede7848f270b' class='xr-index-data-in' type='checkbox'/><label for='index-7bec313e-f2b5-40d7-a4ec-ede7848f270b' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-1380b445-9a3d-4543-852c-22c0ff619e76' class='xr-index-data-in' type='checkbox'/><label for='index-1380b445-9a3d-4543-852c-22c0ff619e76' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-51ec8e35-6359-40fc-8b31-a9aeb950e96e' class='xr-index-data-in' type='checkbox'/><label for='index-51ec8e35-6359-40fc-8b31-a9aeb950e96e' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
                             "              300.0, 330.0],\n",
-                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-a695af4e-6bf4-479c-827a-ec82c26c911b' class='xr-section-summary-in' type='checkbox'  checked><label for='section-a695af4e-6bf4-479c-827a-ec82c26c911b' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.28.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-f6e9d6eb-7d40-420c-9545-3849b69fa27a' class='xr-section-summary-in' type='checkbox'  checked><label for='section-f6e9d6eb-7d40-420c-9545-3849b69fa27a' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-06-08T12:46 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * number         (number) int64 0\n",
                             "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
                             "  * step           (step) timedelta64[ns] 00:00:00\n",
-                            "  * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0\n",
+                            "  * isobaricInhPa  (isobaricInhPa) int64 1000 850\n",
                             "  * latitude       (latitude) float64 90.0 60.0 30.0 0.0 -30.0 -60.0 -90.0\n",
                             "  * longitude      (longitude) float64 0.0 30.0 60.0 90.0 ... 270.0 300.0 330.0\n",
                             "    valid_time     (time, step) datetime64[ns] ...\n",
                             "Data variables:\n",
                             "    t              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-04-05T15:29 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2023-06-08T12:46 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a = a.to_xarray()\n",
                 "a"
@@ -937,15 +1014,15 @@
             "metadata": {},
             "source": [
                 "We close the stream:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 18,
             "id": "through-mistress",
             "metadata": {},
             "outputs": [],
             "source": [
                 "stream.close()"
             ]
         },
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_indexing.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_indexing.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9781925154320987%*

 * *Differences: {"'cells'": "{1: {'source': ['import earthkit.data']}, 2: {'source': ['First we prepare the "*

 * *            'data:\']}, 3: {\'source\': [\'earthkit.data.download_example_file(["test.grib", '*

 * *            '"tuv_pl.grib"])\']}, 7: {\'execution_count\': 4}, 8: {\'execution_count\': 5, '*

 * *            "'outputs': {0: {'execution_count': 5}}}, 10: {'execution_count': 6}, 11: "*

 * *            "{'execution_count': 7, 'outputs': {0: {'execution_count': 7}}}, 14: "*

 * *            "{'execution_count': 8, 'outputs': {0: {'execut […]*

```diff
@@ -1,64 +1,85 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Using GRIB indexing "
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!test -f test.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib\n",
-                "!test -f tuv_pl.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib\n",
-                "!test -d _grib_dir_with_sql || (mkdir -p _grib_dir_with_sql; cp -f test.grib tuv_pl.grib _grib_dir_with_sql/)"
+                "import earthkit.data"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Using GRIB indexing "
+                "First we prepare the data:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import earthkit.data"
+                "earthkit.data.download_example_file([\"test.grib\", \"tuv_pl.grib\"])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "!test -d _grib_dir_with_sql || (mkdir -p _grib_dir_with_sql; cp -f test.grib tuv_pl.grib _grib_dir_with_sql/)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Indexing"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can perform indexing on the input GRIB data by using the **indexing** option in *load_source()*. The indexing is performed on first data access using the MARS ecCodes keys. The index-data is stored in a sqlite database, which is located in the earthkit-data cache. Subsequent loading of the same data is very fast because it will use the cached index-data."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "fs = earthkit.data.from_source(\"file\", \"tuv_pl.grib\", indexing=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "18"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "len(fs)"
             ]
@@ -68,33 +89,33 @@
             "metadata": {},
             "source": [
                 "Indexing works for a list of files or directories (here \"\\_grib_dir_with_sql\") is a directory:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "fs = earthkit.data.from_source(\"file\", \"./_grib_dir_with_sql\", indexing=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "20"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "len(fs)"
             ]
@@ -111,73 +132,66 @@
             "metadata": {},
             "source": [
                 "When calling *sel()*, *isel()* or *order_by()* the metadata is directly read from the index database, so there is no need to load/open any of the GRIB messages."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "3"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a = fs.sel(level=500)\n",
                 "len(a)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "20"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a = fs.order_by(\"param\")\n",
                 "len(a)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "coord_vals=[300, 400, 500, 700, 850, 1000] len=6\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
                             "3"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a = fs.isel(level=2)\n",
                 "len(a)"
@@ -188,15 +202,15 @@
             "metadata": {},
             "source": [
                 "When keys not present in the index db are used the functions above do not work:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    a = fs.sel(gridType=\"regular_ll\")\n",
                 "except KeyError as e:\n",
                 "    print(f\"error: {e}\")   "
@@ -214,15 +228,15 @@
             "metadata": {},
             "source": [
                 "Most of the other methods still need to load/open the GRIB messages to extract the required metadata. Ideally they should all use the index database. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "GribField(u,1000,20180801,1200,0,0)\n"
@@ -231,24 +245,24 @@
             ],
             "source": [
                 "print(fs[1])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['v', 't']"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs[2:4].metadata(\"param\")"
             ]
@@ -265,15 +279,15 @@
             "metadata": {},
             "source": [
                 "Selection and sorting arguments can be directly passed to *from_souce()*:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -357,27 +371,27 @@
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs = earthkit.data.from_source(\"file\", \"./_grib_dir_with_sql\", indexing=True, level=500)\n",
                 "fs.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -506,15 +520,15 @@
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  \n",
                             "3       an       0  regular_ll  \n",
                             "4       an       0  regular_ll  \n",
                             "5       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs = earthkit.data.from_source(\"file\", \"./_grib_dir_with_sql\", indexing=True, level=[500, 850], order_by=\"variable\")\n",
                 "fs.ls()"
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_metadata.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_metadata.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9784355732605343%*

 * *Differences: {"'cells'": "{1: {'source': ['We load a GRIB file containing 6 messages. First we ensure the "*

 * *            "example file is avialable.']}, 3: {'metadata': {replace: OrderedDict()}, 'source': "*

 * *            "{delete: [1, 0]}}, 30: {'outputs': {0: {'data': {'text/html': {insert: [(1, '#T_bf5b3 "*

 * *            "th {\\n'), (4, '#T_bf5b3_row0_col0, #T_bf5b3_row0_col1, #T_bf5b3_row0_col2, "*

 * *            '#T_bf5b3_row0_col3, #T_bf5b3_row0_col4, #T_bf5b3_row0_col5, #T_bf5b3_row0_col6, '*

 * *            '#T_bf5b3_row0_col7, […]*

```diff
@@ -1,44 +1,41 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Inspecting GRIB contents"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We load a GRIB file containing 6 messages:"
+                "We load a GRIB file containing 6 messages. First we ensure the example file is avialable."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import earthkit.data\n",
-                "\n",
+                "earthkit.data.download_example_file(\"test6.grib\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "fs = earthkit.data.from_source(\"file\", \"test6.grib\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1329,35 +1326,35 @@
             "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_c83aa th {\n",
+                            "#T_bf5b3 th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_c83aa_row0_col0, #T_c83aa_row0_col1, #T_c83aa_row0_col2, #T_c83aa_row0_col3, #T_c83aa_row0_col4, #T_c83aa_row0_col5, #T_c83aa_row0_col6, #T_c83aa_row0_col7, #T_c83aa_row0_col8, #T_c83aa_row1_col0, #T_c83aa_row1_col1, #T_c83aa_row1_col2, #T_c83aa_row1_col3, #T_c83aa_row1_col4, #T_c83aa_row1_col5, #T_c83aa_row1_col6, #T_c83aa_row1_col7, #T_c83aa_row1_col8, #T_c83aa_row2_col0, #T_c83aa_row2_col1, #T_c83aa_row2_col2, #T_c83aa_row2_col3, #T_c83aa_row2_col4, #T_c83aa_row2_col5, #T_c83aa_row2_col6, #T_c83aa_row2_col7, #T_c83aa_row2_col8 {\n",
+                            "#T_bf5b3_row0_col0, #T_bf5b3_row0_col1, #T_bf5b3_row0_col2, #T_bf5b3_row0_col3, #T_bf5b3_row0_col4, #T_bf5b3_row0_col5, #T_bf5b3_row0_col6, #T_bf5b3_row0_col7, #T_bf5b3_row0_col8, #T_bf5b3_row1_col0, #T_bf5b3_row1_col1, #T_bf5b3_row1_col2, #T_bf5b3_row1_col3, #T_bf5b3_row1_col4, #T_bf5b3_row1_col5, #T_bf5b3_row1_col6, #T_bf5b3_row1_col7, #T_bf5b3_row1_col8, #T_bf5b3_row2_col0, #T_bf5b3_row2_col1, #T_bf5b3_row2_col2, #T_bf5b3_row2_col3, #T_bf5b3_row2_col4, #T_bf5b3_row2_col5, #T_bf5b3_row2_col6, #T_bf5b3_row2_col7, #T_bf5b3_row2_col8 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_c83aa\">\n",
+                            "<table id=\"T_bf5b3\">\n",
                             "  <thead>\n",
                             "    <tr>\n",
                             "      <th class=\"blank\" >&nbsp;</th>\n",
                             "      <th class=\"blank level0\" >&nbsp;</th>\n",
-                            "      <th id=\"T_c83aa_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
-                            "      <th id=\"T_c83aa_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
-                            "      <th id=\"T_c83aa_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
-                            "      <th id=\"T_c83aa_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
-                            "      <th id=\"T_c83aa_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
-                            "      <th id=\"T_c83aa_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
-                            "      <th id=\"T_c83aa_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
-                            "      <th id=\"T_c83aa_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
-                            "      <th id=\"T_c83aa_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
+                            "      <th id=\"T_bf5b3_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
+                            "      <th id=\"T_bf5b3_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
+                            "      <th id=\"T_bf5b3_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
+                            "      <th id=\"T_bf5b3_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
+                            "      <th id=\"T_bf5b3_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
+                            "      <th id=\"T_bf5b3_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
+                            "      <th id=\"T_bf5b3_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
+                            "      <th id=\"T_bf5b3_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
+                            "      <th id=\"T_bf5b3_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th class=\"index_name level0\" >shortName</th>\n",
                             "      <th class=\"index_name level1\" >typeOfLevel</th>\n",
                             "      <th class=\"blank col0\" >&nbsp;</th>\n",
                             "      <th class=\"blank col1\" >&nbsp;</th>\n",
                             "      <th class=\"blank col2\" >&nbsp;</th>\n",
@@ -1367,57 +1364,57 @@
                             "      <th class=\"blank col6\" >&nbsp;</th>\n",
                             "      <th class=\"blank col7\" >&nbsp;</th>\n",
                             "      <th class=\"blank col8\" >&nbsp;</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_c83aa_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
-                            "      <th id=\"T_c83aa_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_c83aa_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_c83aa_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
-                            "      <td id=\"T_c83aa_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
-                            "      <td id=\"T_c83aa_row0_col3\" class=\"data row0 col3\" >0</td>\n",
-                            "      <td id=\"T_c83aa_row0_col4\" class=\"data row0 col4\" >130</td>\n",
-                            "      <td id=\"T_c83aa_row0_col5\" class=\"data row0 col5\" >od</td>\n",
-                            "      <td id=\"T_c83aa_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
-                            "      <td id=\"T_c83aa_row0_col7\" class=\"data row0 col7\" >an</td>\n",
-                            "      <td id=\"T_c83aa_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_c83aa_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
-                            "      <th id=\"T_c83aa_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_c83aa_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_c83aa_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
-                            "      <td id=\"T_c83aa_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
-                            "      <td id=\"T_c83aa_row1_col3\" class=\"data row1 col3\" >0</td>\n",
-                            "      <td id=\"T_c83aa_row1_col4\" class=\"data row1 col4\" >131</td>\n",
-                            "      <td id=\"T_c83aa_row1_col5\" class=\"data row1 col5\" >od</td>\n",
-                            "      <td id=\"T_c83aa_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
-                            "      <td id=\"T_c83aa_row1_col7\" class=\"data row1 col7\" >an</td>\n",
-                            "      <td id=\"T_c83aa_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_c83aa_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
-                            "      <th id=\"T_c83aa_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_c83aa_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_c83aa_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
-                            "      <td id=\"T_c83aa_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
-                            "      <td id=\"T_c83aa_row2_col3\" class=\"data row2 col3\" >0</td>\n",
-                            "      <td id=\"T_c83aa_row2_col4\" class=\"data row2 col4\" >132</td>\n",
-                            "      <td id=\"T_c83aa_row2_col5\" class=\"data row2 col5\" >od</td>\n",
-                            "      <td id=\"T_c83aa_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
-                            "      <td id=\"T_c83aa_row2_col7\" class=\"data row2 col7\" >an</td>\n",
-                            "      <td id=\"T_c83aa_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
+                            "      <th id=\"T_bf5b3_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
+                            "      <th id=\"T_bf5b3_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_bf5b3_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_bf5b3_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
+                            "      <td id=\"T_bf5b3_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
+                            "      <td id=\"T_bf5b3_row0_col3\" class=\"data row0 col3\" >0</td>\n",
+                            "      <td id=\"T_bf5b3_row0_col4\" class=\"data row0 col4\" >130</td>\n",
+                            "      <td id=\"T_bf5b3_row0_col5\" class=\"data row0 col5\" >od</td>\n",
+                            "      <td id=\"T_bf5b3_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
+                            "      <td id=\"T_bf5b3_row0_col7\" class=\"data row0 col7\" >an</td>\n",
+                            "      <td id=\"T_bf5b3_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_bf5b3_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
+                            "      <th id=\"T_bf5b3_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_bf5b3_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_bf5b3_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
+                            "      <td id=\"T_bf5b3_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
+                            "      <td id=\"T_bf5b3_row1_col3\" class=\"data row1 col3\" >0</td>\n",
+                            "      <td id=\"T_bf5b3_row1_col4\" class=\"data row1 col4\" >131</td>\n",
+                            "      <td id=\"T_bf5b3_row1_col5\" class=\"data row1 col5\" >od</td>\n",
+                            "      <td id=\"T_bf5b3_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
+                            "      <td id=\"T_bf5b3_row1_col7\" class=\"data row1 col7\" >an</td>\n",
+                            "      <td id=\"T_bf5b3_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_bf5b3_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
+                            "      <th id=\"T_bf5b3_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_bf5b3_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_bf5b3_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
+                            "      <td id=\"T_bf5b3_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
+                            "      <td id=\"T_bf5b3_row2_col3\" class=\"data row2 col3\" >0</td>\n",
+                            "      <td id=\"T_bf5b3_row2_col4\" class=\"data row2 col4\" >132</td>\n",
+                            "      <td id=\"T_bf5b3_row2_col5\" class=\"data row2 col5\" >od</td>\n",
+                            "      <td id=\"T_bf5b3_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
+                            "      <td id=\"T_bf5b3_row2_col7\" class=\"data row2 col7\" >an</td>\n",
+                            "      <td id=\"T_bf5b3_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x12d88fdc0>"
+                            "<pandas.io.formats.style.Styler at 0x10417fc10>"
                         ]
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1437,74 +1434,74 @@
             "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_1c6d0 th {\n",
+                            "#T_41753 th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_1c6d0_row0_col0, #T_1c6d0_row1_col0, #T_1c6d0_row2_col0, #T_1c6d0_row3_col0, #T_1c6d0_row4_col0, #T_1c6d0_row5_col0, #T_1c6d0_row6_col0, #T_1c6d0_row7_col0, #T_1c6d0_row8_col0, #T_1c6d0_row9_col0, #T_1c6d0_row10_col0 {\n",
+                            "#T_41753_row0_col0, #T_41753_row1_col0, #T_41753_row2_col0, #T_41753_row3_col0, #T_41753_row4_col0, #T_41753_row5_col0, #T_41753_row6_col0, #T_41753_row7_col0, #T_41753_row8_col0, #T_41753_row9_col0, #T_41753_row10_col0 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_1c6d0\">\n",
+                            "<table id=\"T_41753\">\n",
                             "  <thead>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
-                            "      <td id=\"T_1c6d0_row0_col0\" class=\"data row0 col0\" >t</td>\n",
+                            "      <th id=\"T_41753_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
+                            "      <td id=\"T_41753_row0_col0\" class=\"data row0 col0\" >t</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
-                            "      <td id=\"T_1c6d0_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
+                            "      <th id=\"T_41753_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
+                            "      <td id=\"T_41753_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
-                            "      <td id=\"T_1c6d0_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <th id=\"T_41753_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
+                            "      <td id=\"T_41753_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
-                            "      <td id=\"T_1c6d0_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
+                            "      <th id=\"T_41753_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
+                            "      <td id=\"T_41753_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
-                            "      <td id=\"T_1c6d0_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
+                            "      <th id=\"T_41753_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
+                            "      <td id=\"T_41753_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
-                            "      <td id=\"T_1c6d0_row5_col0\" class=\"data row5 col0\" >0</td>\n",
+                            "      <th id=\"T_41753_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
+                            "      <td id=\"T_41753_row5_col0\" class=\"data row5 col0\" >0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
-                            "      <td id=\"T_1c6d0_row6_col0\" class=\"data row6 col0\" >130</td>\n",
+                            "      <th id=\"T_41753_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
+                            "      <td id=\"T_41753_row6_col0\" class=\"data row6 col0\" >130</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
-                            "      <td id=\"T_1c6d0_row7_col0\" class=\"data row7 col0\" >od</td>\n",
+                            "      <th id=\"T_41753_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
+                            "      <td id=\"T_41753_row7_col0\" class=\"data row7 col0\" >od</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
-                            "      <td id=\"T_1c6d0_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
+                            "      <th id=\"T_41753_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
+                            "      <td id=\"T_41753_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
-                            "      <td id=\"T_1c6d0_row9_col0\" class=\"data row9 col0\" >an</td>\n",
+                            "      <th id=\"T_41753_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
+                            "      <td id=\"T_41753_row9_col0\" class=\"data row9 col0\" >an</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_1c6d0_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
-                            "      <td id=\"T_1c6d0_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
+                            "      <th id=\"T_41753_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
+                            "      <td id=\"T_41753_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x12d8998e0>"
+                            "<pandas.io.formats.style.Styler at 0x1183f7460>"
                         ]
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1517,74 +1514,74 @@
             "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_7aaba th {\n",
+                            "#T_4242a th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_7aaba_row0_col0, #T_7aaba_row1_col0, #T_7aaba_row2_col0, #T_7aaba_row3_col0, #T_7aaba_row4_col0, #T_7aaba_row5_col0, #T_7aaba_row6_col0, #T_7aaba_row7_col0, #T_7aaba_row8_col0, #T_7aaba_row9_col0, #T_7aaba_row10_col0 {\n",
+                            "#T_4242a_row0_col0, #T_4242a_row1_col0, #T_4242a_row2_col0, #T_4242a_row3_col0, #T_4242a_row4_col0, #T_4242a_row5_col0, #T_4242a_row6_col0, #T_4242a_row7_col0, #T_4242a_row8_col0, #T_4242a_row9_col0, #T_4242a_row10_col0 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_7aaba\">\n",
+                            "<table id=\"T_4242a\">\n",
                             "  <thead>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
-                            "      <td id=\"T_7aaba_row0_col0\" class=\"data row0 col0\" >u</td>\n",
+                            "      <th id=\"T_4242a_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
+                            "      <td id=\"T_4242a_row0_col0\" class=\"data row0 col0\" >u</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
-                            "      <td id=\"T_7aaba_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
+                            "      <th id=\"T_4242a_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
+                            "      <td id=\"T_4242a_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
-                            "      <td id=\"T_7aaba_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <th id=\"T_4242a_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
+                            "      <td id=\"T_4242a_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
-                            "      <td id=\"T_7aaba_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
+                            "      <th id=\"T_4242a_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
+                            "      <td id=\"T_4242a_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
-                            "      <td id=\"T_7aaba_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
+                            "      <th id=\"T_4242a_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
+                            "      <td id=\"T_4242a_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
-                            "      <td id=\"T_7aaba_row5_col0\" class=\"data row5 col0\" >0</td>\n",
+                            "      <th id=\"T_4242a_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
+                            "      <td id=\"T_4242a_row5_col0\" class=\"data row5 col0\" >0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
-                            "      <td id=\"T_7aaba_row6_col0\" class=\"data row6 col0\" >131</td>\n",
+                            "      <th id=\"T_4242a_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
+                            "      <td id=\"T_4242a_row6_col0\" class=\"data row6 col0\" >131</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
-                            "      <td id=\"T_7aaba_row7_col0\" class=\"data row7 col0\" >od</td>\n",
+                            "      <th id=\"T_4242a_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
+                            "      <td id=\"T_4242a_row7_col0\" class=\"data row7 col0\" >od</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
-                            "      <td id=\"T_7aaba_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
+                            "      <th id=\"T_4242a_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
+                            "      <td id=\"T_4242a_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
-                            "      <td id=\"T_7aaba_row9_col0\" class=\"data row9 col0\" >an</td>\n",
+                            "      <th id=\"T_4242a_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
+                            "      <td id=\"T_4242a_row9_col0\" class=\"data row9 col0\" >an</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_7aaba_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
-                            "      <td id=\"T_7aaba_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
+                            "      <th id=\"T_4242a_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
+                            "      <td id=\"T_4242a_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x12d909a90>"
+                            "<pandas.io.formats.style.Styler at 0x1183f6bf0>"
                         ]
                     },
                     "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1864,107 +1861,107 @@
                             "</style><div class=\"eh-description\">GribField</div>\n",
                             "<div>\n",
                             "<section class=\"eh-section>\n",
                             "<div class=\"eh-tabs-container\">\n",
                             "<div class=\"eh-tabs-block\">\n",
                             "<div class=\"eh-tabs\">\n",
                             "\n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"74688028-9b3d-4994-ae66-f9af3ffea504\"  />\n",
-                            "<label for=\"74688028-9b3d-4994-ae66-f9af3ffea504\" title=\"Keys in the ecCodes default namespace\">default</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"1237fa78-77bc-4beb-9c57-568b3cc5af30\"  />\n",
+                            "<label for=\"1237fa78-77bc-4beb-9c57-568b3cc5af30\" title=\"Keys in the ecCodes default namespace\">default</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
-                            "<tr><td><b>globalDomain</b></td><td>g</td></tr> <tr><td><b>GRIBEditionNumber</b></td><td>1</td></tr> <tr><td><b>eps</b></td><td>0</td></tr> <tr><td><b>offsetSection0</b></td><td>0</td></tr> <tr><td><b>section0Length</b></td><td>8</td></tr> <tr><td><b>totalLength</b></td><td>150</td></tr> <tr><td><b>editionNumber</b></td><td>1</td></tr> <tr><td><b>WMO</b></td><td>0</td></tr> <tr><td><b>productionStatusOfProcessedData</b></td><td>0</td></tr> <tr><td><b>section1Length</b></td><td>52</td></tr> <tr><td><b>wrongPadding</b></td><td>0</td></tr> <tr><td><b>table2Version</b></td><td>128</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>centreDescription</b></td><td>European Centre for Medium-Range Weather Forecasts</td></tr> <tr><td><b>generatingProcessIdentifier</b></td><td>254</td></tr> <tr><td><b>gridDefinition</b></td><td>255</td></tr> <tr><td><b>indicatorOfParameter</b></td><td>130</td></tr> <tr><td><b>parameterName</b></td><td>Temperature</td></tr> <tr><td><b>parameterUnits</b></td><td>K</td></tr> <tr><td><b>indicatorOfTypeOfLevel</b></td><td>pl</td></tr> <tr><td><b>pressureUnits</b></td><td>hPa</td></tr> <tr><td><b>typeOfLevelECMF</b></td><td>isobaricInhPa</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>yearOfCentury</b></td><td>18</td></tr> <tr><td><b>month</b></td><td>8</td></tr> <tr><td><b>day</b></td><td>1</td></tr> <tr><td><b>hour</b></td><td>12</td></tr> <tr><td><b>minute</b></td><td>0</td></tr> <tr><td><b>second</b></td><td>0</td></tr> <tr><td><b>unitOfTimeRange</b></td><td>1</td></tr> <tr><td><b>P1</b></td><td>0</td></tr> <tr><td><b>P2</b></td><td>0</td></tr> <tr><td><b>timeRangeIndicator</b></td><td>0</td></tr> <tr><td><b>numberIncludedInAverage</b></td><td>0</td></tr> <tr><td><b>mybits</b></td><td>None</td></tr> <tr><td><b>numberMissingFromAveragesOrAccumulations</b></td><td>0</td></tr> <tr><td><b>centuryOfReferenceTimeOfData</b></td><td>21</td></tr> <tr><td><b>subCentre</b></td><td>0</td></tr> <tr><td><b>paramIdECMF</b></td><td>130</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>cfNameECMF</b></td><td>air_temperature</td></tr> <tr><td><b>cfName</b></td><td>air_temperature</td></tr> <tr><td><b>cfVarNameECMF</b></td><td>t</td></tr> <tr><td><b>cfVarName</b></td><td>t</td></tr> <tr><td><b>unitsECMF</b></td><td>K</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>nameECMF</b></td><td>Temperature</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>decimalScaleFactor</b></td><td>0</td></tr> <tr><td><b>setLocalDefinition</b></td><td>0</td></tr> <tr><td><b>optimizeScaleFactor</b></td><td>0</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>year</b></td><td>2018</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>julianDay</b></td><td>2458332.0</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>marsParam</b></td><td>130.128</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr> <tr><td><b>deleteLocalDefinition</b></td><td>0</td></tr> <tr><td><b>localUsePresent</b></td><td>1</td></tr> <tr><td><b>reservedNeedNotBePresent</b></td><td>None</td></tr> <tr><td><b>localDefinitionNumber</b></td><td>1</td></tr> <tr><td><b>GRIBEXSection1Problem</b></td><td>0</td></tr> <tr><td><b>marsClass</b></td><td>od</td></tr> <tr><td><b>marsType</b></td><td>an</td></tr> <tr><td><b>marsStream</b></td><td>oper</td></tr> <tr><td><b>experimentVersionNumber</b></td><td>0001</td></tr> <tr><td><b>perturbationNumber</b></td><td>0</td></tr> <tr><td><b>numberOfForecastsInEnsemble</b></td><td>0</td></tr> <tr><td><b>padding_local1_1</b></td><td>None</td></tr> <tr><td><b>grib2LocalSectionNumber</b></td><td>1</td></tr> <tr><td><b>localExtensionPadding</b></td><td>None</td></tr> <tr><td><b>_x</b></td><td>None</td></tr> <tr><td><b>section1Padding</b></td><td>None</td></tr> <tr><td><b>shortNameECMF</b></td><td>t</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>ifsParam</b></td><td>130</td></tr> <tr><td><b>stepTypeForConversion</b></td><td>unknown</td></tr> <tr><td><b>md5Section1</b></td><td>3ae6b1f6f34f431c6134c40ec42f27fa</td></tr> <tr><td><b>md5Product</b></td><td>54697e1d910c88b76a8759b67e5c7a9c</td></tr> <tr><td><b>gridDescriptionSectionPresent</b></td><td>1</td></tr> <tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>angleSubdivisions</b></td><td>1000</td></tr> <tr><td><b>section2Length</b></td><td>32</td></tr> <tr><td><b>radius</b></td><td>6367470</td></tr> <tr><td><b>numberOfVerticalCoordinateValues</b></td><td>0</td></tr> <tr><td><b>neitherPresent</b></td><td>255</td></tr> <tr><td><b>pvlLocation</b></td><td>255</td></tr> <tr><td><b>dataRepresentationType</b></td><td>0</td></tr> <tr><td><b>gridDefinitionDescription</b></td><td>Latitude/Longitude Grid</td></tr> <tr><td><b>gridDefinitionTemplateNumber</b></td><td>0</td></tr> <tr><td><b>Ni</b></td><td>12</td></tr> <tr><td><b>Nj</b></td><td>7</td></tr> <tr><td><b>latitudeOfFirstGridPoint</b></td><td>90000</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPoint</b></td><td>0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>resolutionAndComponentFlags</b></td><td>128</td></tr> <tr><td><b>ijDirectionIncrementGiven</b></td><td>1</td></tr> <tr><td><b>earthIsOblate</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags3</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags4</b></td><td>0</td></tr> <tr><td><b>uvRelativeToGrid</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags6</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags7</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags8</b></td><td>0</td></tr> <tr><td><b>latitudeOfLastGridPoint</b></td><td>-90000</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPoint</b></td><td>330000</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>jDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>scanningMode</b></td><td>0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>alternativeRowScanning</b></td><td>0</td></tr> <tr><td><b>iScansPositively</b></td><td>1</td></tr> <tr><td><b>scanningMode4</b></td><td>0</td></tr> <tr><td><b>scanningMode5</b></td><td>0</td></tr> <tr><td><b>scanningMode6</b></td><td>0</td></tr> <tr><td><b>scanningMode7</b></td><td>0</td></tr> <tr><td><b>scanningMode8</b></td><td>0</td></tr> <tr><td><b>swapScanningAlternativeRows</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>numberOfDataPoints</b></td><td>84</td></tr> <tr><td><b>numberOfValues</b></td><td>84</td></tr> <tr><td><b>zeros</b></td><td></td></tr> <tr><td><b>PVPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_2</b></td><td>None</td></tr> <tr><td><b>PLPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_1</b></td><td>None</td></tr> <tr><td><b>deletePV</b></td><td>1</td></tr> <tr><td><b>padding_sec2_3</b></td><td>None</td></tr> <tr><td><b>md5Section2</b></td><td>e09e4d6171c0ac85da1d256b2f8acf88</td></tr> <tr><td><b>lengthOfHeaders</b></td><td>85</td></tr> <tr><td><b>md5Headers</b></td><td>9160fb809a9d7b1efc95163bf36e6b51</td></tr> <tr><td><b>missingValue</b></td><td>9999</td></tr> <tr><td><b>tableReference</b></td><td>0</td></tr> <tr><td><b>section4Length</b></td><td>54</td></tr> <tr><td><b>halfByte</b></td><td>8</td></tr> <tr><td><b>dataFlag</b></td><td>8</td></tr> <tr><td><b>binaryScaleFactor</b></td><td>3</td></tr> <tr><td><b>referenceValue</b></td><td>240.56417846679688</td></tr> <tr><td><b>referenceValueError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>sphericalHarmonics</b></td><td>0</td></tr> <tr><td><b>complexPacking</b></td><td>0</td></tr> <tr><td><b>integerPointValues</b></td><td>0</td></tr> <tr><td><b>additionalFlagPresent</b></td><td>0</td></tr> <tr><td><b>orderOfSPD</b></td><td>2</td></tr> <tr><td><b>boustrophedonic</b></td><td>0</td></tr> <tr><td><b>hideThis</b></td><td>0</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>bitsPerValue</b></td><td>4</td></tr> <tr><td><b>constantFieldHalfByte</b></td><td>8</td></tr> <tr><td><b>bitMapIndicator</b></td><td>255</td></tr> <tr><td><b>numberOfCodedValues</b></td><td>84</td></tr> <tr><td><b>packingError</b></td><td>4.000007629394531</td></tr> <tr><td><b>unpackedError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>maximum</b></td><td>320.5641784667969</td></tr> <tr><td><b>minimum</b></td><td>240.56417846679688</td></tr> <tr><td><b>average</b></td><td>279.70703560965404</td></tr> <tr><td><b>numberOfMissing</b></td><td>0</td></tr> <tr><td><b>standardDeviation</b></td><td>19.67421739058438</td></tr> <tr><td><b>skewness</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurtosis</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>isConstant</b></td><td>0.0</td></tr> <tr><td><b>dataLength</b></td><td>5</td></tr> <tr><td><b>changeDecimalPrecision</b></td><td>0</td></tr> <tr><td><b>decimalPrecision</b></td><td>0</td></tr> <tr><td><b>bitsPerValueAndRepack</b></td><td>4</td></tr> <tr><td><b>scaleValuesBy</b></td><td>1.0</td></tr> <tr><td><b>offsetValuesBy</b></td><td>0.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr> <tr><td><b>getNumberOfValues</b></td><td>84</td></tr> <tr><td><b>padding_sec4_1</b></td><td>None</td></tr> <tr><td><b>md5Section4</b></td><td>7ea3331d80a962b5dc99276b76451eac</td></tr> <tr><td><b>section5Length</b></td><td>4</td></tr> <tr><td><b>7777</b></td><td>7777</td></tr>\n",
+                            "<tr><td><b>globalDomain</b></td><td>g</td></tr> <tr><td><b>GRIBEditionNumber</b></td><td>1</td></tr> <tr><td><b>eps</b></td><td>0</td></tr> <tr><td><b>offsetSection0</b></td><td>0</td></tr> <tr><td><b>section0Length</b></td><td>8</td></tr> <tr><td><b>totalLength</b></td><td>150</td></tr> <tr><td><b>editionNumber</b></td><td>1</td></tr> <tr><td><b>WMO</b></td><td>0</td></tr> <tr><td><b>productionStatusOfProcessedData</b></td><td>0</td></tr> <tr><td><b>section1Length</b></td><td>52</td></tr> <tr><td><b>wrongPadding</b></td><td>0</td></tr> <tr><td><b>table2Version</b></td><td>128</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>centreDescription</b></td><td>European Centre for Medium-Range Weather Forecasts</td></tr> <tr><td><b>generatingProcessIdentifier</b></td><td>254</td></tr> <tr><td><b>gridDefinition</b></td><td>255</td></tr> <tr><td><b>indicatorOfParameter</b></td><td>130</td></tr> <tr><td><b>parameterName</b></td><td>Temperature</td></tr> <tr><td><b>parameterUnits</b></td><td>K</td></tr> <tr><td><b>indicatorOfTypeOfLevel</b></td><td>pl</td></tr> <tr><td><b>pressureUnits</b></td><td>hPa</td></tr> <tr><td><b>typeOfLevelECMF</b></td><td>isobaricInhPa</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>yearOfCentury</b></td><td>18</td></tr> <tr><td><b>month</b></td><td>8</td></tr> <tr><td><b>day</b></td><td>1</td></tr> <tr><td><b>hour</b></td><td>12</td></tr> <tr><td><b>minute</b></td><td>0</td></tr> <tr><td><b>second</b></td><td>0</td></tr> <tr><td><b>unitOfTimeRange</b></td><td>1</td></tr> <tr><td><b>P1</b></td><td>0</td></tr> <tr><td><b>P2</b></td><td>0</td></tr> <tr><td><b>timeRangeIndicator</b></td><td>0</td></tr> <tr><td><b>numberIncludedInAverage</b></td><td>0</td></tr> <tr><td><b>numberMissingFromAveragesOrAccumulations</b></td><td>0</td></tr> <tr><td><b>centuryOfReferenceTimeOfData</b></td><td>21</td></tr> <tr><td><b>subCentre</b></td><td>0</td></tr> <tr><td><b>paramIdECMF</b></td><td>130</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>cfNameECMF</b></td><td>air_temperature</td></tr> <tr><td><b>cfName</b></td><td>air_temperature</td></tr> <tr><td><b>cfVarNameECMF</b></td><td>t</td></tr> <tr><td><b>cfVarName</b></td><td>t</td></tr> <tr><td><b>unitsECMF</b></td><td>K</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>nameECMF</b></td><td>Temperature</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>decimalScaleFactor</b></td><td>0</td></tr> <tr><td><b>setLocalDefinition</b></td><td>0</td></tr> <tr><td><b>optimizeScaleFactor</b></td><td>0</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>year</b></td><td>2018</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>julianDay</b></td><td>2458332.0</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>marsParam</b></td><td>130.128</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr> <tr><td><b>deleteLocalDefinition</b></td><td>0</td></tr> <tr><td><b>localUsePresent</b></td><td>1</td></tr> <tr><td><b>reservedNeedNotBePresent</b></td><td>['']</td></tr> <tr><td><b>localDefinitionNumber</b></td><td>1</td></tr> <tr><td><b>GRIBEXSection1Problem</b></td><td>0</td></tr> <tr><td><b>marsClass</b></td><td>od</td></tr> <tr><td><b>marsType</b></td><td>an</td></tr> <tr><td><b>marsStream</b></td><td>oper</td></tr> <tr><td><b>experimentVersionNumber</b></td><td>0001</td></tr> <tr><td><b>perturbationNumber</b></td><td>0</td></tr> <tr><td><b>numberOfForecastsInEnsemble</b></td><td>0</td></tr> <tr><td><b>padding_local1_1</b></td><td>00</td></tr> <tr><td><b>grib2LocalSectionNumber</b></td><td>1</td></tr> <tr><td><b>localExtensionPadding</b></td><td></td></tr> <tr><td><b>_x</b></td><td>None</td></tr> <tr><td><b>section1Padding</b></td><td></td></tr> <tr><td><b>shortNameECMF</b></td><td>t</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>ifsParam</b></td><td>130</td></tr> <tr><td><b>stepTypeForConversion</b></td><td>unknown</td></tr> <tr><td><b>md5Section1</b></td><td>3ae6b1f6f34f431c6134c40ec42f27fa</td></tr> <tr><td><b>md5Product</b></td><td>54697e1d910c88b76a8759b67e5c7a9c</td></tr> <tr><td><b>gridDescriptionSectionPresent</b></td><td>1</td></tr> <tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>angleSubdivisions</b></td><td>1000</td></tr> <tr><td><b>section2Length</b></td><td>32</td></tr> <tr><td><b>radius</b></td><td>6367470</td></tr> <tr><td><b>numberOfVerticalCoordinateValues</b></td><td>0</td></tr> <tr><td><b>neitherPresent</b></td><td>255</td></tr> <tr><td><b>pvlLocation</b></td><td>255</td></tr> <tr><td><b>dataRepresentationType</b></td><td>0</td></tr> <tr><td><b>gridDefinitionDescription</b></td><td>Latitude/Longitude Grid</td></tr> <tr><td><b>gridDefinitionTemplateNumber</b></td><td>0</td></tr> <tr><td><b>Ni</b></td><td>12</td></tr> <tr><td><b>Nj</b></td><td>7</td></tr> <tr><td><b>latitudeOfFirstGridPoint</b></td><td>90000</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPoint</b></td><td>0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>resolutionAndComponentFlags</b></td><td>128</td></tr> <tr><td><b>ijDirectionIncrementGiven</b></td><td>1</td></tr> <tr><td><b>earthIsOblate</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags3</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags4</b></td><td>0</td></tr> <tr><td><b>uvRelativeToGrid</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags6</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags7</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags8</b></td><td>0</td></tr> <tr><td><b>latitudeOfLastGridPoint</b></td><td>-90000</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPoint</b></td><td>330000</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>jDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>scanningMode</b></td><td>0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>alternativeRowScanning</b></td><td>0</td></tr> <tr><td><b>iScansPositively</b></td><td>1</td></tr> <tr><td><b>jScansNegatively</b></td><td>1</td></tr> <tr><td><b>scanningMode4</b></td><td>0</td></tr> <tr><td><b>scanningMode5</b></td><td>0</td></tr> <tr><td><b>scanningMode6</b></td><td>0</td></tr> <tr><td><b>scanningMode7</b></td><td>0</td></tr> <tr><td><b>scanningMode8</b></td><td>0</td></tr> <tr><td><b>swapScanningAlternativeRows</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>numberOfDataPoints</b></td><td>84</td></tr> <tr><td><b>numberOfValues</b></td><td>84</td></tr> <tr><td><b>zeros</b></td><td></td></tr> <tr><td><b>PVPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_2</b></td><td></td></tr> <tr><td><b>PLPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_1</b></td><td></td></tr> <tr><td><b>deletePV</b></td><td>1</td></tr> <tr><td><b>padding_sec2_3</b></td><td></td></tr> <tr><td><b>md5Section2</b></td><td>e09e4d6171c0ac85da1d256b2f8acf88</td></tr> <tr><td><b>lengthOfHeaders</b></td><td>85</td></tr> <tr><td><b>md5Headers</b></td><td>9160fb809a9d7b1efc95163bf36e6b51</td></tr> <tr><td><b>missingValue</b></td><td>9999</td></tr> <tr><td><b>tableReference</b></td><td>0</td></tr> <tr><td><b>section4Length</b></td><td>54</td></tr> <tr><td><b>halfByte</b></td><td>8</td></tr> <tr><td><b>dataFlag</b></td><td>8</td></tr> <tr><td><b>binaryScaleFactor</b></td><td>3</td></tr> <tr><td><b>referenceValue</b></td><td>240.56417846679688</td></tr> <tr><td><b>referenceValueError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>sphericalHarmonics</b></td><td>0</td></tr> <tr><td><b>complexPacking</b></td><td>0</td></tr> <tr><td><b>integerPointValues</b></td><td>0</td></tr> <tr><td><b>additionalFlagPresent</b></td><td>0</td></tr> <tr><td><b>orderOfSPD</b></td><td>2</td></tr> <tr><td><b>boustrophedonic</b></td><td>0</td></tr> <tr><td><b>hideThis</b></td><td>0</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>bitsPerValue</b></td><td>4</td></tr> <tr><td><b>constantFieldHalfByte</b></td><td>8</td></tr> <tr><td><b>bitMapIndicator</b></td><td>255</td></tr> <tr><td><b>numberOfCodedValues</b></td><td>84</td></tr> <tr><td><b>packingError</b></td><td>4.000007629394531</td></tr> <tr><td><b>unpackedError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>maximum</b></td><td>320.5641784667969</td></tr> <tr><td><b>minimum</b></td><td>240.56417846679688</td></tr> <tr><td><b>average</b></td><td>279.70703560965404</td></tr> <tr><td><b>standardDeviation</b></td><td>19.67421739058438</td></tr> <tr><td><b>skewness</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurtosis</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>isConstant</b></td><td>0.0</td></tr> <tr><td><b>numberOfMissing</b></td><td>0</td></tr> <tr><td><b>dataLength</b></td><td>5</td></tr> <tr><td><b>changeDecimalPrecision</b></td><td>0</td></tr> <tr><td><b>decimalPrecision</b></td><td>0</td></tr> <tr><td><b>bitsPerValueAndRepack</b></td><td>4</td></tr> <tr><td><b>scaleValuesBy</b></td><td>1.0</td></tr> <tr><td><b>offsetValuesBy</b></td><td>0.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr> <tr><td><b>getNumberOfValues</b></td><td>84</td></tr> <tr><td><b>padding_sec4_1</b></td><td></td></tr> <tr><td><b>md5Section4</b></td><td>7ea3331d80a962b5dc99276b76451eac</td></tr> <tr><td><b>section5Length</b></td><td>4</td></tr> <tr><td><b>7777</b></td><td>7777</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"339cb5be-05ae-40c9-a395-23c0530e2284\"  />\n",
-                            "<label for=\"339cb5be-05ae-40c9-a395-23c0530e2284\" title=\"Keys in the ecCodes ls namespace\">ls</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"660b2bd9-ba06-4cab-8d6d-de437246ee47\"  />\n",
+                            "<label for=\"660b2bd9-ba06-4cab-8d6d-de437246ee47\" title=\"Keys in the ecCodes ls namespace\">ls</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>edition</b></td><td>1</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>dataType</b></td><td>an</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"e2750566-42bb-4618-af6b-be16d22b6274\"  />\n",
-                            "<label for=\"e2750566-42bb-4618-af6b-be16d22b6274\" title=\"Keys in the ecCodes geography namespace\">geography</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"07810b0f-a4b1-4379-b3fd-54115d7a7327\"  />\n",
+                            "<label for=\"07810b0f-a4b1-4379-b3fd-54115d7a7327\" title=\"Keys in the ecCodes geography namespace\">geography</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"694e962e-4d1f-42ab-a7b8-b34fb25a04c8\"  />\n",
-                            "<label for=\"694e962e-4d1f-42ab-a7b8-b34fb25a04c8\" title=\"Keys in the ecCodes mars namespace\">mars</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"fe651588-7589-48ea-b8c5-1bb902aae4c6\"  />\n",
+                            "<label for=\"fe651588-7589-48ea-b8c5-1bb902aae4c6\" title=\"Keys in the ecCodes mars namespace\">mars</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>domain</b></td><td>g</td></tr> <tr><td><b>levtype</b></td><td>pl</td></tr> <tr><td><b>levelist</b></td><td>1000</td></tr> <tr><td><b>date</b></td><td>20180801</td></tr> <tr><td><b>time</b></td><td>1200</td></tr> <tr><td><b>step</b></td><td>0</td></tr> <tr><td><b>param</b></td><td>t</td></tr> <tr><td><b>class</b></td><td>od</td></tr> <tr><td><b>type</b></td><td>an</td></tr> <tr><td><b>stream</b></td><td>oper</td></tr> <tr><td><b>expver</b></td><td>0001</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"96d0fd35-c0af-4330-8b3d-efe22671f74b\" checked />\n",
-                            "<label for=\"96d0fd35-c0af-4330-8b3d-efe22671f74b\" title=\"Keys in the ecCodes parameter namespace\">parameter</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"984edc29-3daf-42ee-9f2f-dc9874e451d4\" checked />\n",
+                            "<label for=\"984edc29-3daf-42ee-9f2f-dc9874e451d4\" title=\"Keys in the ecCodes parameter namespace\">parameter</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"ebb99973-46d6-41d2-aaec-338624f06c33\"  />\n",
-                            "<label for=\"ebb99973-46d6-41d2-aaec-338624f06c33\" title=\"Keys in the ecCodes statistics namespace\">statistics</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"19377454-1b25-425f-8762-a875206af34f\"  />\n",
+                            "<label for=\"19377454-1b25-425f-8762-a875206af34f\" title=\"Keys in the ecCodes statistics namespace\">statistics</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>max</b></td><td>320.5641784667969</td></tr> <tr><td><b>min</b></td><td>240.56417846679688</td></tr> <tr><td><b>avg</b></td><td>279.70703560965404</td></tr> <tr><td><b>sd</b></td><td>19.67421739058438</td></tr> <tr><td><b>skew</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurt</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>const</b></td><td>0.0</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"6a4e876c-1996-4579-83d3-498dc6fce73d\"  />\n",
-                            "<label for=\"6a4e876c-1996-4579-83d3-498dc6fce73d\" title=\"Keys in the ecCodes time namespace\">time</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"b66af60e-0a9b-485a-b8f2-344f21ec0d3c\"  />\n",
+                            "<label for=\"b66af60e-0a9b-485a-b8f2-344f21ec0d3c\" title=\"Keys in the ecCodes time namespace\">time</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"92b144c0-bde3-474e-bfbf-9b982af5efe0\"  />\n",
-                            "<label for=\"92b144c0-bde3-474e-bfbf-9b982af5efe0\" title=\"Keys in the ecCodes vertical namespace\">vertical</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"fb8fdf33-e801-49f5-a974-b9d53996a226\"  />\n",
+                            "<label for=\"fb8fdf33-e801-49f5-a974-b9d53996a226\" title=\"Keys in the ecCodes vertical namespace\">vertical</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
@@ -1976,42 +1973,288 @@
                             "</div>\n",
                             "</div>\n",
                             "</section>\n",
                             "</div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.core.display.HTML object>"
+                            "{'default': {'globalDomain': 'g',\n",
+                            "  'GRIBEditionNumber': 1,\n",
+                            "  'eps': 0,\n",
+                            "  'offsetSection0': 0,\n",
+                            "  'section0Length': 8,\n",
+                            "  'totalLength': 150,\n",
+                            "  'editionNumber': 1,\n",
+                            "  'WMO': 0,\n",
+                            "  'productionStatusOfProcessedData': 0,\n",
+                            "  'section1Length': 52,\n",
+                            "  'wrongPadding': 0,\n",
+                            "  'table2Version': 128,\n",
+                            "  'centre': 'ecmf',\n",
+                            "  'centreDescription': 'European Centre for Medium-Range Weather Forecasts',\n",
+                            "  'generatingProcessIdentifier': 254,\n",
+                            "  'gridDefinition': 255,\n",
+                            "  'indicatorOfParameter': 130,\n",
+                            "  'parameterName': 'Temperature',\n",
+                            "  'parameterUnits': 'K',\n",
+                            "  'indicatorOfTypeOfLevel': 'pl',\n",
+                            "  'pressureUnits': 'hPa',\n",
+                            "  'typeOfLevelECMF': 'isobaricInhPa',\n",
+                            "  'typeOfLevel': 'isobaricInhPa',\n",
+                            "  'level': 1000,\n",
+                            "  'yearOfCentury': 18,\n",
+                            "  'month': 8,\n",
+                            "  'day': 1,\n",
+                            "  'hour': 12,\n",
+                            "  'minute': 0,\n",
+                            "  'second': 0,\n",
+                            "  'unitOfTimeRange': 1,\n",
+                            "  'P1': 0,\n",
+                            "  'P2': 0,\n",
+                            "  'timeRangeIndicator': 0,\n",
+                            "  'numberIncludedInAverage': 0,\n",
+                            "  'numberMissingFromAveragesOrAccumulations': 0,\n",
+                            "  'centuryOfReferenceTimeOfData': 21,\n",
+                            "  'subCentre': 0,\n",
+                            "  'paramIdECMF': '130',\n",
+                            "  'paramId': 130,\n",
+                            "  'cfNameECMF': 'air_temperature',\n",
+                            "  'cfName': 'air_temperature',\n",
+                            "  'cfVarNameECMF': 't',\n",
+                            "  'cfVarName': 't',\n",
+                            "  'unitsECMF': 'K',\n",
+                            "  'units': 'K',\n",
+                            "  'nameECMF': 'Temperature',\n",
+                            "  'name': 'Temperature',\n",
+                            "  'decimalScaleFactor': 0,\n",
+                            "  'setLocalDefinition': 0,\n",
+                            "  'optimizeScaleFactor': 0,\n",
+                            "  'dataDate': 20180801,\n",
+                            "  'year': 2018,\n",
+                            "  'dataTime': 1200,\n",
+                            "  'julianDay': 2458332.0,\n",
+                            "  'stepUnits': 1,\n",
+                            "  'stepType': 'instant',\n",
+                            "  'stepRange': '0',\n",
+                            "  'startStep': 0,\n",
+                            "  'endStep': 0,\n",
+                            "  'marsParam': '130.128',\n",
+                            "  'validityDate': 20180801,\n",
+                            "  'validityTime': 1200,\n",
+                            "  'deleteLocalDefinition': 0,\n",
+                            "  'localUsePresent': 1,\n",
+                            "  'reservedNeedNotBePresent': [''],\n",
+                            "  'localDefinitionNumber': 1,\n",
+                            "  'GRIBEXSection1Problem': 0,\n",
+                            "  'marsClass': 'od',\n",
+                            "  'marsType': 'an',\n",
+                            "  'marsStream': 'oper',\n",
+                            "  'experimentVersionNumber': '0001',\n",
+                            "  'perturbationNumber': 0,\n",
+                            "  'numberOfForecastsInEnsemble': 0,\n",
+                            "  'padding_local1_1': '00',\n",
+                            "  'grib2LocalSectionNumber': 1,\n",
+                            "  'localExtensionPadding': '',\n",
+                            "  '_x': None,\n",
+                            "  'section1Padding': '',\n",
+                            "  'shortNameECMF': 't',\n",
+                            "  'shortName': 't',\n",
+                            "  'ifsParam': 130,\n",
+                            "  'stepTypeForConversion': 'unknown',\n",
+                            "  'md5Section1': '3ae6b1f6f34f431c6134c40ec42f27fa',\n",
+                            "  'md5Product': '54697e1d910c88b76a8759b67e5c7a9c',\n",
+                            "  'gridDescriptionSectionPresent': 1,\n",
+                            "  'bitmapPresent': 0,\n",
+                            "  'angleSubdivisions': 1000,\n",
+                            "  'section2Length': 32,\n",
+                            "  'radius': 6367470,\n",
+                            "  'numberOfVerticalCoordinateValues': 0,\n",
+                            "  'neitherPresent': 255,\n",
+                            "  'pvlLocation': 255,\n",
+                            "  'dataRepresentationType': 0,\n",
+                            "  'gridDefinitionDescription': 'Latitude/Longitude Grid',\n",
+                            "  'gridDefinitionTemplateNumber': 0,\n",
+                            "  'Ni': 12,\n",
+                            "  'Nj': 7,\n",
+                            "  'latitudeOfFirstGridPoint': 90000,\n",
+                            "  'latitudeOfFirstGridPointInDegrees': 90.0,\n",
+                            "  'longitudeOfFirstGridPoint': 0,\n",
+                            "  'longitudeOfFirstGridPointInDegrees': 0.0,\n",
+                            "  'resolutionAndComponentFlags': 128,\n",
+                            "  'ijDirectionIncrementGiven': 1,\n",
+                            "  'earthIsOblate': 0,\n",
+                            "  'resolutionAndComponentFlags3': 0,\n",
+                            "  'resolutionAndComponentFlags4': 0,\n",
+                            "  'uvRelativeToGrid': 0,\n",
+                            "  'resolutionAndComponentFlags6': 0,\n",
+                            "  'resolutionAndComponentFlags7': 0,\n",
+                            "  'resolutionAndComponentFlags8': 0,\n",
+                            "  'latitudeOfLastGridPoint': -90000,\n",
+                            "  'latitudeOfLastGridPointInDegrees': -90.0,\n",
+                            "  'longitudeOfLastGridPoint': 330000,\n",
+                            "  'longitudeOfLastGridPointInDegrees': 330.0,\n",
+                            "  'iDirectionIncrement': 30000,\n",
+                            "  'jDirectionIncrement': 30000,\n",
+                            "  'scanningMode': 0,\n",
+                            "  'iScansNegatively': 0,\n",
+                            "  'jScansPositively': 0,\n",
+                            "  'jPointsAreConsecutive': 0,\n",
+                            "  'alternativeRowScanning': 0,\n",
+                            "  'iScansPositively': 1,\n",
+                            "  'jScansNegatively': 1,\n",
+                            "  'scanningMode4': 0,\n",
+                            "  'scanningMode5': 0,\n",
+                            "  'scanningMode6': 0,\n",
+                            "  'scanningMode7': 0,\n",
+                            "  'scanningMode8': 0,\n",
+                            "  'swapScanningAlternativeRows': 0,\n",
+                            "  'jDirectionIncrementInDegrees': 30.0,\n",
+                            "  'iDirectionIncrementInDegrees': 30.0,\n",
+                            "  'numberOfDataPoints': 84,\n",
+                            "  'numberOfValues': 84,\n",
+                            "  'zeros': '',\n",
+                            "  'PVPresent': 0,\n",
+                            "  'padding_sec2_2': '',\n",
+                            "  'PLPresent': 0,\n",
+                            "  'padding_sec2_1': '',\n",
+                            "  'deletePV': '1',\n",
+                            "  'padding_sec2_3': '',\n",
+                            "  'md5Section2': 'e09e4d6171c0ac85da1d256b2f8acf88',\n",
+                            "  'lengthOfHeaders': 85,\n",
+                            "  'md5Headers': '9160fb809a9d7b1efc95163bf36e6b51',\n",
+                            "  'missingValue': 9999,\n",
+                            "  'tableReference': 0,\n",
+                            "  'section4Length': 54,\n",
+                            "  'halfByte': 8,\n",
+                            "  'dataFlag': 8,\n",
+                            "  'binaryScaleFactor': 3,\n",
+                            "  'referenceValue': 240.56417846679688,\n",
+                            "  'referenceValueError': 1.52587890625e-05,\n",
+                            "  'sphericalHarmonics': 0,\n",
+                            "  'complexPacking': 0,\n",
+                            "  'integerPointValues': 0,\n",
+                            "  'additionalFlagPresent': 0,\n",
+                            "  'orderOfSPD': 2,\n",
+                            "  'boustrophedonic': 0,\n",
+                            "  'hideThis': 0,\n",
+                            "  'packingType': 'grid_simple',\n",
+                            "  'bitsPerValue': 4,\n",
+                            "  'constantFieldHalfByte': 8,\n",
+                            "  'bitMapIndicator': 255,\n",
+                            "  'numberOfCodedValues': 84,\n",
+                            "  'packingError': 4.000007629394531,\n",
+                            "  'unpackedError': 1.52587890625e-05,\n",
+                            "  'maximum': 320.5641784667969,\n",
+                            "  'minimum': 240.56417846679688,\n",
+                            "  'average': 279.70703560965404,\n",
+                            "  'standardDeviation': 19.67421739058438,\n",
+                            "  'skewness': -0.7312302105044429,\n",
+                            "  'kurtosis': -0.16904561574741717,\n",
+                            "  'isConstant': 0.0,\n",
+                            "  'numberOfMissing': 0,\n",
+                            "  'dataLength': 5,\n",
+                            "  'changeDecimalPrecision': 0,\n",
+                            "  'decimalPrecision': 0,\n",
+                            "  'bitsPerValueAndRepack': 4,\n",
+                            "  'scaleValuesBy': 1.0,\n",
+                            "  'offsetValuesBy': 0.0,\n",
+                            "  'gridType': 'regular_ll',\n",
+                            "  'getNumberOfValues': 84,\n",
+                            "  'padding_sec4_1': '',\n",
+                            "  'md5Section4': '7ea3331d80a962b5dc99276b76451eac',\n",
+                            "  'section5Length': 4,\n",
+                            "  '7777': '7777'},\n",
+                            " 'ls': {'edition': 1,\n",
+                            "  'centre': 'ecmf',\n",
+                            "  'typeOfLevel': 'isobaricInhPa',\n",
+                            "  'level': 1000,\n",
+                            "  'dataDate': 20180801,\n",
+                            "  'stepRange': '0',\n",
+                            "  'dataType': 'an',\n",
+                            "  'shortName': 't',\n",
+                            "  'packingType': 'grid_simple',\n",
+                            "  'gridType': 'regular_ll'},\n",
+                            " 'geography': {'bitmapPresent': 0,\n",
+                            "  'latitudeOfFirstGridPointInDegrees': 90.0,\n",
+                            "  'longitudeOfFirstGridPointInDegrees': 0.0,\n",
+                            "  'latitudeOfLastGridPointInDegrees': -90.0,\n",
+                            "  'longitudeOfLastGridPointInDegrees': 330.0,\n",
+                            "  'iScansNegatively': 0,\n",
+                            "  'jScansPositively': 0,\n",
+                            "  'jPointsAreConsecutive': 0,\n",
+                            "  'jDirectionIncrementInDegrees': 30.0,\n",
+                            "  'iDirectionIncrementInDegrees': 30.0,\n",
+                            "  'gridType': 'regular_ll'},\n",
+                            " 'mars': {'domain': 'g',\n",
+                            "  'levtype': 'pl',\n",
+                            "  'levelist': 1000,\n",
+                            "  'date': 20180801,\n",
+                            "  'time': 1200,\n",
+                            "  'step': 0,\n",
+                            "  'param': 't',\n",
+                            "  'class': 'od',\n",
+                            "  'type': 'an',\n",
+                            "  'stream': 'oper',\n",
+                            "  'expver': '0001'},\n",
+                            " 'parameter': {'centre': 'ecmf',\n",
+                            "  'paramId': 130,\n",
+                            "  'units': 'K',\n",
+                            "  'name': 'Temperature',\n",
+                            "  'shortName': 't'},\n",
+                            " 'statistics': {'max': 320.5641784667969,\n",
+                            "  'min': 240.56417846679688,\n",
+                            "  'avg': 279.70703560965404,\n",
+                            "  'sd': 19.67421739058438,\n",
+                            "  'skew': -0.7312302105044429,\n",
+                            "  'kurt': -0.16904561574741717,\n",
+                            "  'const': 0.0},\n",
+                            " 'time': {'dataDate': 20180801,\n",
+                            "  'dataTime': 1200,\n",
+                            "  'stepUnits': 1,\n",
+                            "  'stepType': 'instant',\n",
+                            "  'stepRange': '0',\n",
+                            "  'startStep': 0,\n",
+                            "  'endStep': 0,\n",
+                            "  'validityDate': 20180801,\n",
+                            "  'validityTime': 1200},\n",
+                            " 'vertical': {'typeOfLevel': 'isobaricInhPa', 'level': 1000}}"
                         ]
                     },
                     "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs[0].dump()"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "mpy10",
             "language": "python",
-            "name": "python3"
+            "name": "mpy10"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.16"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_missing.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_missing.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9721590909090909%*

 * *Differences: {"'cells'": "{1: {'source': ['We read a GRIB file containing 2 messages with missing values. First "*

 * *            "we ensure the example file is available.'], 'attachments': OrderedDict()}, 3: "*

 * *            "{'source': {delete: [2, 1, 0]}}, insert: [(2, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', 1), ('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            "['import numpy as np\\n', 'import earthkit.data\\n', "*

 * *            '\'earthkit.data.download_example_file("missi […]*

```diff
@@ -1,41 +1,41 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "!test -f missing.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/missing.grib"
+                "## GRIB missing values"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## GRIB missing values"
+                "We read a GRIB file containing 2 messages with missing values. First we ensure the example file is available."
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 1,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "We read a GRIB file containing 2 messages with missing values:"
+                "import numpy as np\n",
+                "import earthkit.data\n",
+                "earthkit.data.download_example_file(\"missing.grib\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import numpy as np\n",
-                "import earthkit.data\n",
-                "\n",
                 "fs = earthkit.data.from_source(\"file\", \"missing.grib\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_multi.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_multi.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9829861111111111%*

 * *Differences: {"'cells'": "{1: {'source': ['First we prepare the data.']}, 3: {'source': ['!test -d "*

 * *            '_grib_dir_no_sql || (mkdir -p _grib_dir_no_sql; cp -f test.grib test4.grib '*

 * *            "_grib_dir_no_sql/)']}, insert: [(2, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', 1), ('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            '[\'import earthkit.data\\n\', \'earthkit.data.download_example_file(["test.grib", '*

 * *            '"test4.grib"])\'])])), (4, OrderedDict([( […]*

```diff
@@ -1,41 +1,47 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "!test -f test.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.grib\n",
-                "!test -f test4.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test4.grib\n",
-                "!test -d _grib_dir_no_sql || (mkdir -p _grib_dir_no_sql; cp -f test.grib test4.grib _grib_dir_no_sql/)"
+                "## Handling multiple GRIB files"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Handling multiple GRIB files"
+                "First we prepare the data."
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 1,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Multiple GRIB files can be read in various ways:"
+                "import earthkit.data\n",
+                "earthkit.data.download_example_file([\"test.grib\", \"test4.grib\"])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import earthkit.data"
+                "!test -d _grib_dir_no_sql || (mkdir -p _grib_dir_no_sql; cp -f test.grib test4.grib _grib_dir_no_sql/)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Multiple GRIB files can be read in various ways:"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Option 1: using wildcards"
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_overview.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_overview.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991523836345451%*

 * *Differences: {"'cells'": "{1: {'source': ['We load a GRIB file containing 6 messages from disk. First we ensure "*

 * *            "the example file is available.'], 'attachments': OrderedDict()}, 3: {'source': "*

 * *            "{delete: [1, 0]}}, 11: {'outputs': {0: {'data': {'text/html': {insert: [(1, '#T_57b5e "*

 * *            "th {\\n'), (4, '#T_57b5e_row0_col0, #T_57b5e_row0_col1, #T_57b5e_row0_col2, "*

 * *            '#T_57b5e_row0_col3, #T_57b5e_row0_col4, #T_57b5e_row0_col5, #T_57b5e_row0_col6, '*

 * *            '#T_57b5e_row0_col […]*

```diff
@@ -1,40 +1,40 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test6.grib"
+                "## Using GRIB data overview"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Using GRIB data overview"
+                "We load a GRIB file containing 6 messages from disk. First we ensure the example file is available."
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 1,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "We load a GRIB file containing 6 messages from disk:"
+                "import earthkit.data\n",
+                "earthkit.data.download_example_file(\"test6.grib\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import earthkit.data\n",
-                "\n",
                 "fs = earthkit.data.from_source(\"file\", \"test6.grib\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -258,35 +258,35 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_41673 th {\n",
+                            "#T_57b5e th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_41673_row0_col0, #T_41673_row0_col1, #T_41673_row0_col2, #T_41673_row0_col3, #T_41673_row0_col4, #T_41673_row0_col5, #T_41673_row0_col6, #T_41673_row0_col7, #T_41673_row0_col8, #T_41673_row1_col0, #T_41673_row1_col1, #T_41673_row1_col2, #T_41673_row1_col3, #T_41673_row1_col4, #T_41673_row1_col5, #T_41673_row1_col6, #T_41673_row1_col7, #T_41673_row1_col8, #T_41673_row2_col0, #T_41673_row2_col1, #T_41673_row2_col2, #T_41673_row2_col3, #T_41673_row2_col4, #T_41673_row2_col5, #T_41673_row2_col6, #T_41673_row2_col7, #T_41673_row2_col8 {\n",
+                            "#T_57b5e_row0_col0, #T_57b5e_row0_col1, #T_57b5e_row0_col2, #T_57b5e_row0_col3, #T_57b5e_row0_col4, #T_57b5e_row0_col5, #T_57b5e_row0_col6, #T_57b5e_row0_col7, #T_57b5e_row0_col8, #T_57b5e_row1_col0, #T_57b5e_row1_col1, #T_57b5e_row1_col2, #T_57b5e_row1_col3, #T_57b5e_row1_col4, #T_57b5e_row1_col5, #T_57b5e_row1_col6, #T_57b5e_row1_col7, #T_57b5e_row1_col8, #T_57b5e_row2_col0, #T_57b5e_row2_col1, #T_57b5e_row2_col2, #T_57b5e_row2_col3, #T_57b5e_row2_col4, #T_57b5e_row2_col5, #T_57b5e_row2_col6, #T_57b5e_row2_col7, #T_57b5e_row2_col8 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_41673\">\n",
+                            "<table id=\"T_57b5e\">\n",
                             "  <thead>\n",
                             "    <tr>\n",
                             "      <th class=\"blank\" >&nbsp;</th>\n",
                             "      <th class=\"blank level0\" >&nbsp;</th>\n",
-                            "      <th id=\"T_41673_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
-                            "      <th id=\"T_41673_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
-                            "      <th id=\"T_41673_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
-                            "      <th id=\"T_41673_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
-                            "      <th id=\"T_41673_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
-                            "      <th id=\"T_41673_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
-                            "      <th id=\"T_41673_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
-                            "      <th id=\"T_41673_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
-                            "      <th id=\"T_41673_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
+                            "      <th id=\"T_57b5e_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
+                            "      <th id=\"T_57b5e_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
+                            "      <th id=\"T_57b5e_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
+                            "      <th id=\"T_57b5e_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
+                            "      <th id=\"T_57b5e_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
+                            "      <th id=\"T_57b5e_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
+                            "      <th id=\"T_57b5e_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
+                            "      <th id=\"T_57b5e_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
+                            "      <th id=\"T_57b5e_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th class=\"index_name level0\" >shortName</th>\n",
                             "      <th class=\"index_name level1\" >typeOfLevel</th>\n",
                             "      <th class=\"blank col0\" >&nbsp;</th>\n",
                             "      <th class=\"blank col1\" >&nbsp;</th>\n",
                             "      <th class=\"blank col2\" >&nbsp;</th>\n",
@@ -296,57 +296,57 @@
                             "      <th class=\"blank col6\" >&nbsp;</th>\n",
                             "      <th class=\"blank col7\" >&nbsp;</th>\n",
                             "      <th class=\"blank col8\" >&nbsp;</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_41673_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
-                            "      <th id=\"T_41673_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_41673_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_41673_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
-                            "      <td id=\"T_41673_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
-                            "      <td id=\"T_41673_row0_col3\" class=\"data row0 col3\" >0</td>\n",
-                            "      <td id=\"T_41673_row0_col4\" class=\"data row0 col4\" >130</td>\n",
-                            "      <td id=\"T_41673_row0_col5\" class=\"data row0 col5\" >od</td>\n",
-                            "      <td id=\"T_41673_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
-                            "      <td id=\"T_41673_row0_col7\" class=\"data row0 col7\" >an</td>\n",
-                            "      <td id=\"T_41673_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
+                            "      <th id=\"T_57b5e_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
+                            "      <th id=\"T_57b5e_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_57b5e_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_57b5e_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
+                            "      <td id=\"T_57b5e_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
+                            "      <td id=\"T_57b5e_row0_col3\" class=\"data row0 col3\" >0</td>\n",
+                            "      <td id=\"T_57b5e_row0_col4\" class=\"data row0 col4\" >130</td>\n",
+                            "      <td id=\"T_57b5e_row0_col5\" class=\"data row0 col5\" >od</td>\n",
+                            "      <td id=\"T_57b5e_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
+                            "      <td id=\"T_57b5e_row0_col7\" class=\"data row0 col7\" >an</td>\n",
+                            "      <td id=\"T_57b5e_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_41673_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
-                            "      <th id=\"T_41673_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_41673_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_41673_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
-                            "      <td id=\"T_41673_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
-                            "      <td id=\"T_41673_row1_col3\" class=\"data row1 col3\" >0</td>\n",
-                            "      <td id=\"T_41673_row1_col4\" class=\"data row1 col4\" >131</td>\n",
-                            "      <td id=\"T_41673_row1_col5\" class=\"data row1 col5\" >od</td>\n",
-                            "      <td id=\"T_41673_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
-                            "      <td id=\"T_41673_row1_col7\" class=\"data row1 col7\" >an</td>\n",
-                            "      <td id=\"T_41673_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
+                            "      <th id=\"T_57b5e_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
+                            "      <th id=\"T_57b5e_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_57b5e_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_57b5e_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
+                            "      <td id=\"T_57b5e_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
+                            "      <td id=\"T_57b5e_row1_col3\" class=\"data row1 col3\" >0</td>\n",
+                            "      <td id=\"T_57b5e_row1_col4\" class=\"data row1 col4\" >131</td>\n",
+                            "      <td id=\"T_57b5e_row1_col5\" class=\"data row1 col5\" >od</td>\n",
+                            "      <td id=\"T_57b5e_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
+                            "      <td id=\"T_57b5e_row1_col7\" class=\"data row1 col7\" >an</td>\n",
+                            "      <td id=\"T_57b5e_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_41673_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
-                            "      <th id=\"T_41673_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_41673_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_41673_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
-                            "      <td id=\"T_41673_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
-                            "      <td id=\"T_41673_row2_col3\" class=\"data row2 col3\" >0</td>\n",
-                            "      <td id=\"T_41673_row2_col4\" class=\"data row2 col4\" >132</td>\n",
-                            "      <td id=\"T_41673_row2_col5\" class=\"data row2 col5\" >od</td>\n",
-                            "      <td id=\"T_41673_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
-                            "      <td id=\"T_41673_row2_col7\" class=\"data row2 col7\" >an</td>\n",
-                            "      <td id=\"T_41673_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
+                            "      <th id=\"T_57b5e_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
+                            "      <th id=\"T_57b5e_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_57b5e_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_57b5e_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
+                            "      <td id=\"T_57b5e_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
+                            "      <td id=\"T_57b5e_row2_col3\" class=\"data row2 col3\" >0</td>\n",
+                            "      <td id=\"T_57b5e_row2_col4\" class=\"data row2 col4\" >132</td>\n",
+                            "      <td id=\"T_57b5e_row2_col5\" class=\"data row2 col5\" >od</td>\n",
+                            "      <td id=\"T_57b5e_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
+                            "      <td id=\"T_57b5e_row2_col7\" class=\"data row2 col7\" >an</td>\n",
+                            "      <td id=\"T_57b5e_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x130267b50>"
+                            "<pandas.io.formats.style.Styler at 0x12e4cdd30>"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1387,17 +1387,17 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-1841cade-985f-43dd-8a97-34c5f7f9d70c' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-1841cade-985f-43dd-8a97-34c5f7f9d70c' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-cfe0690a-a41a-4517-a72c-864269dbb782' class='xr-section-summary-in' type='checkbox'  checked><label for='section-cfe0690a-a41a-4517-a72c-864269dbb782' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-ba2b4ce4-83c6-49ac-a83b-165d26807394' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ba2b4ce4-83c6-49ac-a83b-165d26807394' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-399b1d7a-e45a-428f-a7e5-bdaabb4379ef' class='xr-var-data-in' type='checkbox'><label for='data-399b1d7a-e45a-428f-a7e5-bdaabb4379ef' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-afd247a7-4b1f-41dc-a882-f589aef2012a' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-afd247a7-4b1f-41dc-a882-f589aef2012a' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1fdf56ad-c6ad-4b12-a201-f50338684570' class='xr-var-data-in' type='checkbox'><label for='data-1fdf56ad-c6ad-4b12-a201-f50338684570' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-018b7074-b540-4741-83ae-5d691efb8e02' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-018b7074-b540-4741-83ae-5d691efb8e02' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-3b483e70-a6c5-4445-a3a6-a646fb299d13' class='xr-var-data-in' type='checkbox'><label for='data-3b483e70-a6c5-4445-a3a6-a646fb299d13' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-1a866171-d371-47b6-8df7-ccdeaeedf474' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1a866171-d371-47b6-8df7-ccdeaeedf474' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f5d0a1cf-9fce-4ab2-bb81-f331dbf7f36f' class='xr-var-data-in' type='checkbox'><label for='data-f5d0a1cf-9fce-4ab2-bb81-f331dbf7f36f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-54ae76ec-da6d-410d-acff-e5f9a14365f0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-54ae76ec-da6d-410d-acff-e5f9a14365f0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-050c3b54-85df-4872-b060-c7e08224b0b4' class='xr-var-data-in' type='checkbox'><label for='data-050c3b54-85df-4872-b060-c7e08224b0b4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-28f28bd1-cb3b-4631-acc7-10151f301e31' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-28f28bd1-cb3b-4631-acc7-10151f301e31' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d26aa714-604e-4228-8048-9739843a04c0' class='xr-var-data-in' type='checkbox'><label for='data-d26aa714-604e-4228-8048-9739843a04c0' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-cd26a69c-bfa8-426c-b4dc-e9f256df319a' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-cd26a69c-bfa8-426c-b4dc-e9f256df319a' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ebc34426-222a-41f1-b713-e2917c492493' class='xr-var-data-in' type='checkbox'><label for='data-ebc34426-222a-41f1-b713-e2917c492493' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-d9bb2937-7fdf-4343-94ad-ab5c88c3f407' class='xr-section-summary-in' type='checkbox'  checked><label for='section-d9bb2937-7fdf-4343-94ad-ab5c88c3f407' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-d074b3f7-d50c-4582-a481-f61e454eae9b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-d074b3f7-d50c-4582-a481-f61e454eae9b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e2925141-2cff-4610-8919-64c2e0a5444e' class='xr-var-data-in' type='checkbox'><label for='data-e2925141-2cff-4610-8919-64c2e0a5444e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-17b65f4b-4e2d-4e00-81f6-e1ccd38b3b69' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-17b65f4b-4e2d-4e00-81f6-e1ccd38b3b69' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-53ac77b9-e5af-4940-904e-8a52848c41e0' class='xr-var-data-in' type='checkbox'><label for='data-53ac77b9-e5af-4940-904e-8a52848c41e0' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-6742e27d-da1e-4940-97b3-24a079a190d5' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6742e27d-da1e-4940-97b3-24a079a190d5' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ee3b3cb2-a6cf-4304-9d63-e257cfa9c57a' class='xr-var-data-in' type='checkbox'><label for='data-ee3b3cb2-a6cf-4304-9d63-e257cfa9c57a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-5f527475-7d93-4024-b24d-8d2079da693a' class='xr-section-summary-in' type='checkbox'  ><label for='section-5f527475-7d93-4024-b24d-8d2079da693a' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-b4ce9783-836b-4a43-a112-bd3eb1d7da22' class='xr-index-data-in' type='checkbox'/><label for='index-b4ce9783-836b-4a43-a112-bd3eb1d7da22' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9b0c78d8-18f6-426f-856c-179e063f2eda' class='xr-index-data-in' type='checkbox'/><label for='index-9b0c78d8-18f6-426f-856c-179e063f2eda' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-72655b31-4cb6-4864-a315-58a3fdd41b46' class='xr-index-data-in' type='checkbox'/><label for='index-72655b31-4cb6-4864-a315-58a3fdd41b46' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e76203c4-6ed3-4aaa-874c-79b878955b73' class='xr-index-data-in' type='checkbox'/><label for='index-e76203c4-6ed3-4aaa-874c-79b878955b73' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9e80af1f-890c-4106-91bc-3bd5b8fa27b6' class='xr-index-data-in' type='checkbox'/><label for='index-9e80af1f-890c-4106-91bc-3bd5b8fa27b6' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-fca27e0e-aeca-4529-a62a-38214239ca2f' class='xr-index-data-in' type='checkbox'/><label for='index-fca27e0e-aeca-4529-a62a-38214239ca2f' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
+                            "    history:                 2023-06-05T10:06 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-2d345009-cf18-45f6-a7b5-7e3f909741b2' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-2d345009-cf18-45f6-a7b5-7e3f909741b2' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-89983ae2-b29a-4a78-ae41-1a10f2e6dbf6' class='xr-section-summary-in' type='checkbox'  checked><label for='section-89983ae2-b29a-4a78-ae41-1a10f2e6dbf6' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-06343d62-5a64-4914-9f37-7320d6f41a3c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-06343d62-5a64-4914-9f37-7320d6f41a3c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-6c13787f-fe59-47ae-9d98-f2abdf6b6738' class='xr-var-data-in' type='checkbox'><label for='data-6c13787f-fe59-47ae-9d98-f2abdf6b6738' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-f95dd911-0e59-4f72-8bde-cec8970ab5b8' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-f95dd911-0e59-4f72-8bde-cec8970ab5b8' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-225aceab-ab9c-4315-a83b-8b788da7c5f9' class='xr-var-data-in' type='checkbox'><label for='data-225aceab-ab9c-4315-a83b-8b788da7c5f9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-8883c69c-ceed-43cc-9d8a-1f7dc1ac4b27' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-8883c69c-ceed-43cc-9d8a-1f7dc1ac4b27' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-9fadcd92-48b3-40f1-a52f-d52d69815f9c' class='xr-var-data-in' type='checkbox'><label for='data-9fadcd92-48b3-40f1-a52f-d52d69815f9c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-b31dff4d-7732-4b71-81e6-245735577fbc' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b31dff4d-7732-4b71-81e6-245735577fbc' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-4c88c00f-e67b-4d16-8815-fc67b8dce85c' class='xr-var-data-in' type='checkbox'><label for='data-4c88c00f-e67b-4d16-8815-fc67b8dce85c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-e691c84e-b6ff-4842-a520-585a4b58d7fb' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e691c84e-b6ff-4842-a520-585a4b58d7fb' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-0379d9e4-999e-4d8a-8f23-14fef9c40ee2' class='xr-var-data-in' type='checkbox'><label for='data-0379d9e4-999e-4d8a-8f23-14fef9c40ee2' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-1b8be8ee-b972-46fa-ab45-519462926c64' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1b8be8ee-b972-46fa-ab45-519462926c64' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1195440b-2868-4678-a71a-06ef8cac17c9' class='xr-var-data-in' type='checkbox'><label for='data-1195440b-2868-4678-a71a-06ef8cac17c9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-1f6318b8-007f-4f2d-ab5e-4611ded2e703' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1f6318b8-007f-4f2d-ab5e-4611ded2e703' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-a9c34858-1423-4090-9404-3833fab06a75' class='xr-var-data-in' type='checkbox'><label for='data-a9c34858-1423-4090-9404-3833fab06a75' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-4f12d2e6-59f9-457d-a3f0-b34d90a162d0' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4f12d2e6-59f9-457d-a3f0-b34d90a162d0' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-94b7aa67-11ea-4a4d-b710-76412909cedb' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-94b7aa67-11ea-4a4d-b710-76412909cedb' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ae562b86-5615-4e27-9be9-e5c0aabc64e6' class='xr-var-data-in' type='checkbox'><label for='data-ae562b86-5615-4e27-9be9-e5c0aabc64e6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-7db811b1-0482-451b-9968-e80aa8dc70da' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-7db811b1-0482-451b-9968-e80aa8dc70da' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-6c677396-aad4-4649-aa46-b3c75b6a079d' class='xr-var-data-in' type='checkbox'><label for='data-6c677396-aad4-4649-aa46-b3c75b6a079d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-ff26d4bd-84f8-42e8-9c37-db00c45badac' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ff26d4bd-84f8-42e8-9c37-db00c45badac' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-dfada2f2-7fbd-44ce-add9-2ab7878d0fd5' class='xr-var-data-in' type='checkbox'><label for='data-dfada2f2-7fbd-44ce-add9-2ab7878d0fd5' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-2e6c5930-e4b7-4697-ab75-169179f212e0' class='xr-section-summary-in' type='checkbox'  ><label for='section-2e6c5930-e4b7-4697-ab75-169179f212e0' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c7530eab-f26c-43aa-8779-de83676f1684' class='xr-index-data-in' type='checkbox'/><label for='index-c7530eab-f26c-43aa-8779-de83676f1684' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e4111354-6ff5-44dc-adbf-6492299cabe3' class='xr-index-data-in' type='checkbox'/><label for='index-e4111354-6ff5-44dc-adbf-6492299cabe3' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-bb8d51ee-68fb-4a4e-a5b8-b515f959840e' class='xr-index-data-in' type='checkbox'/><label for='index-bb8d51ee-68fb-4a4e-a5b8-b515f959840e' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-0b4a4db4-5fb2-4bdb-a5bb-2df24261a79d' class='xr-index-data-in' type='checkbox'/><label for='index-0b4a4db4-5fb2-4bdb-a5bb-2df24261a79d' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-2f16f3e1-db62-4b73-8dda-ab57d1b12ab0' class='xr-index-data-in' type='checkbox'/><label for='index-2f16f3e1-db62-4b73-8dda-ab57d1b12ab0' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-ed19c54f-ca88-448b-aba8-ba3d414da6ec' class='xr-index-data-in' type='checkbox'/><label for='index-ed19c54f-ca88-448b-aba8-ba3d414da6ec' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
                             "              300.0, 330.0],\n",
-                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-927c801a-a45e-42c2-bde0-154985e63192' class='xr-section-summary-in' type='checkbox'  checked><label for='section-927c801a-a45e-42c2-bde0-154985e63192' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-b87cfd2a-e91b-40fe-aef8-85c3f7d33ac3' class='xr-section-summary-in' type='checkbox'  checked><label for='section-b87cfd2a-e91b-40fe-aef8-85c3f7d33ac3' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-06-05T10:06 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * number         (number) int64 0\n",
@@ -1414,15 +1414,15 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2023-06-05T10:06 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
                     "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1826,17 +1826,17 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-342df797-d354-4636-bbe4-b6970390c297' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-342df797-d354-4636-bbe4-b6970390c297' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-53776147-d34c-4c72-9035-4d3afecf75a1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-53776147-d34c-4c72-9035-4d3afecf75a1' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-99135cb9-9abb-4f75-808e-a67469aaf52c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-99135cb9-9abb-4f75-808e-a67469aaf52c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-5471c338-dca7-4591-8562-00ff93ecd8e1' class='xr-var-data-in' type='checkbox'><label for='data-5471c338-dca7-4591-8562-00ff93ecd8e1' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-b658ad58-1a96-48b1-b6d8-6ea7bf206063' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b658ad58-1a96-48b1-b6d8-6ea7bf206063' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-0d277e90-cc0a-42ce-930b-da3dfdd1df25' class='xr-var-data-in' type='checkbox'><label for='data-0d277e90-cc0a-42ce-930b-da3dfdd1df25' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-5f846d80-0858-45a9-8581-9e4f6da5cab7' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5f846d80-0858-45a9-8581-9e4f6da5cab7' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-00396e82-f5de-4366-83d2-c7fad5844fa1' class='xr-var-data-in' type='checkbox'><label for='data-00396e82-f5de-4366-83d2-c7fad5844fa1' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-74096228-e9e1-49b2-b87a-262484acac9b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-74096228-e9e1-49b2-b87a-262484acac9b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-bdc03411-ab02-4bf1-9040-cf9cfa1c4134' class='xr-var-data-in' type='checkbox'><label for='data-bdc03411-ab02-4bf1-9040-cf9cfa1c4134' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-27ff62a2-0295-4bf7-b7cb-e1f3957adf49' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-27ff62a2-0295-4bf7-b7cb-e1f3957adf49' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-4d29d1c4-8fca-4788-9e2d-3a1fe0bfa67e' class='xr-var-data-in' type='checkbox'><label for='data-4d29d1c4-8fca-4788-9e2d-3a1fe0bfa67e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-a74262ed-3a3a-4e73-88ba-1feba25ac1e5' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a74262ed-3a3a-4e73-88ba-1feba25ac1e5' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-674e840c-4345-4f99-9388-77018d20f746' class='xr-var-data-in' type='checkbox'><label for='data-674e840c-4345-4f99-9388-77018d20f746' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-28f2dc4a-e075-4692-a759-e85dab58084a' class='xr-section-summary-in' type='checkbox'  checked><label for='section-28f2dc4a-e075-4692-a759-e85dab58084a' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-5f814b44-c347-4dd0-981f-252c11b03adf' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5f814b44-c347-4dd0-981f-252c11b03adf' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-dce1ac10-96d8-4706-a3ec-c8e8c1ecd55e' class='xr-var-data-in' type='checkbox'><label for='data-dce1ac10-96d8-4706-a3ec-c8e8c1ecd55e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-5a628772-171c-429e-ba44-b34b43eaad2e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5a628772-171c-429e-ba44-b34b43eaad2e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-7c018c72-4456-4e0c-a5b8-2ae67f445768' class='xr-var-data-in' type='checkbox'><label for='data-7c018c72-4456-4e0c-a5b8-2ae67f445768' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-64df24d5-74a4-405d-9552-b8a412f40ab0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-64df24d5-74a4-405d-9552-b8a412f40ab0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c2f1f3d5-458f-4fb1-9383-9a6f27aca991' class='xr-var-data-in' type='checkbox'><label for='data-c2f1f3d5-458f-4fb1-9383-9a6f27aca991' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-4213f844-5c41-47e1-a95f-8ebfc797a7f5' class='xr-section-summary-in' type='checkbox'  ><label for='section-4213f844-5c41-47e1-a95f-8ebfc797a7f5' class='xr-section-summary' >Indexes: <span>(5)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-f21370f2-2d99-47de-aa94-368321ce64b6' class='xr-index-data-in' type='checkbox'/><label for='index-f21370f2-2d99-47de-aa94-368321ce64b6' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c6502882-1a79-41fd-8007-84de45639ef4' class='xr-index-data-in' type='checkbox'/><label for='index-c6502882-1a79-41fd-8007-84de45639ef4' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-077ae806-6cd7-46f0-842a-24c560289233' class='xr-index-data-in' type='checkbox'/><label for='index-077ae806-6cd7-46f0-842a-24c560289233' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c9510b7a-bddf-4e3f-b124-be6b0dcc2a0e' class='xr-index-data-in' type='checkbox'/><label for='index-c9510b7a-bddf-4e3f-b124-be6b0dcc2a0e' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-7f71d23e-8f3a-4a57-baf1-ece1a13759cb' class='xr-index-data-in' type='checkbox'/><label for='index-7f71d23e-8f3a-4a57-baf1-ece1a13759cb' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
+                            "    history:                 2023-06-05T10:06 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-801257ba-de9d-4291-9ed0-7dc01f34d26f' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-801257ba-de9d-4291-9ed0-7dc01f34d26f' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-3a54b93b-5a88-423a-bf34-c86205862f17' class='xr-section-summary-in' type='checkbox'  checked><label for='section-3a54b93b-5a88-423a-bf34-c86205862f17' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-271f7993-bb6c-42fe-b411-91d9abc71e8d' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-271f7993-bb6c-42fe-b411-91d9abc71e8d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-affab024-4944-4f33-9521-cbd86c9e6031' class='xr-var-data-in' type='checkbox'><label for='data-affab024-4944-4f33-9521-cbd86c9e6031' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-60316c7f-7321-4470-b540-c41ad0782c71' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-60316c7f-7321-4470-b540-c41ad0782c71' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-4922db41-208a-49a9-8b9c-301972df3685' class='xr-var-data-in' type='checkbox'><label for='data-4922db41-208a-49a9-8b9c-301972df3685' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-05f59049-037d-4fec-a68a-dd48b9999e0c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-05f59049-037d-4fec-a68a-dd48b9999e0c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-6e74d44b-ae7c-403e-9a90-c4f74008dc22' class='xr-var-data-in' type='checkbox'><label for='data-6e74d44b-ae7c-403e-9a90-c4f74008dc22' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-ebce8561-f3f2-4536-b413-4266d9fd8402' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ebce8561-f3f2-4536-b413-4266d9fd8402' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1903d51d-d90b-448a-920b-b06c58af2749' class='xr-var-data-in' type='checkbox'><label for='data-1903d51d-d90b-448a-920b-b06c58af2749' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-4f9398a4-5c1f-4f08-8bd3-146197f53e13' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-4f9398a4-5c1f-4f08-8bd3-146197f53e13' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-94ea6c18-a716-40f4-b425-753ad4b768cf' class='xr-var-data-in' type='checkbox'><label for='data-94ea6c18-a716-40f4-b425-753ad4b768cf' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-c107300a-608b-4790-8eff-e821c37c36ea' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-c107300a-608b-4790-8eff-e821c37c36ea' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c4dd51ab-5dea-4215-8775-07b5f23e3edd' class='xr-var-data-in' type='checkbox'><label for='data-c4dd51ab-5dea-4215-8775-07b5f23e3edd' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-a49f5c12-da1e-42ba-9848-711188e60188' class='xr-section-summary-in' type='checkbox'  checked><label for='section-a49f5c12-da1e-42ba-9848-711188e60188' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-08ab6196-42e9-4495-bd0d-0ccacf05349b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-08ab6196-42e9-4495-bd0d-0ccacf05349b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-614793e4-05f5-4fdb-bb34-056a0f91fd8a' class='xr-var-data-in' type='checkbox'><label for='data-614793e4-05f5-4fdb-bb34-056a0f91fd8a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-39f6554b-ae15-44b8-9892-79602a3ed882' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-39f6554b-ae15-44b8-9892-79602a3ed882' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e5d64b8a-fb6a-4124-bc0d-45796c229efa' class='xr-var-data-in' type='checkbox'><label for='data-e5d64b8a-fb6a-4124-bc0d-45796c229efa' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-9fa450ae-e14a-4269-8ce3-70177b066c84' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9fa450ae-e14a-4269-8ce3-70177b066c84' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-06c66980-a6b5-4d4c-96fd-f5bdca28466e' class='xr-var-data-in' type='checkbox'><label for='data-06c66980-a6b5-4d4c-96fd-f5bdca28466e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-bec325d6-be32-4cac-b46d-6d23f5ca47fc' class='xr-section-summary-in' type='checkbox'  ><label for='section-bec325d6-be32-4cac-b46d-6d23f5ca47fc' class='xr-section-summary' >Indexes: <span>(5)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-f1c8c8d4-3086-4e9d-a720-ff4803da38d3' class='xr-index-data-in' type='checkbox'/><label for='index-f1c8c8d4-3086-4e9d-a720-ff4803da38d3' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-b6d3f0a0-7415-4c27-84da-9ba126269e81' class='xr-index-data-in' type='checkbox'/><label for='index-b6d3f0a0-7415-4c27-84da-9ba126269e81' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-ae3022ea-6aff-4401-9c20-5689fedd71f3' class='xr-index-data-in' type='checkbox'/><label for='index-ae3022ea-6aff-4401-9c20-5689fedd71f3' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9e62b8df-4be3-469d-97c8-527bb973aadb' class='xr-index-data-in' type='checkbox'/><label for='index-9e62b8df-4be3-469d-97c8-527bb973aadb' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c4330423-a0e4-404f-bc74-15ba96c2a221' class='xr-index-data-in' type='checkbox'/><label for='index-c4330423-a0e4-404f-bc74-15ba96c2a221' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
                             "              300.0, 330.0],\n",
-                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-0bab1f97-9927-421d-b0ab-92692c0a212f' class='xr-section-summary-in' type='checkbox'  checked><label for='section-0bab1f97-9927-421d-b0ab-92692c0a212f' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-83ee4f8c-6908-4c5e-a22a-00e2b64419d8' class='xr-section-summary-in' type='checkbox'  checked><label for='section-83ee4f8c-6908-4c5e-a22a-00e2b64419d8' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-06-05T10:06 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:        (time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
@@ -1852,15 +1852,15 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-05-17T17:40 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2023-06-05T10:06 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
                     "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1889,13 +1889,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.16"
+            "version": "3.8.17"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_selection.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_selection.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9859245600414079%*

 * *Differences: {"'cells'": "{1: {'source': ['We read a GRIB file containing 18 messages. First we ensure the "*

 * *            "example file is available.'], 'attachments': OrderedDict()}, 3: {'source': {delete: "*

 * *            "[1, 0]}}, insert: [(2, OrderedDict([('cell_type', 'code'), ('execution_count', 1), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', ['import earthkit.data\\n', "*

 * *            '\'earthkit.data.download_example_file("tuv_pl.grib")\'])]))], delete: [0]}',*

 * * "'metadata'": "{'kernelspec' […]*

```diff
@@ -1,42 +1,42 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "!test -f tuv_pl.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "## GRIB selection using metadata"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We read a GRIB file containing 18 messages:"
+                "We read a GRIB file containing 18 messages. First we ensure the example file is available."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import earthkit.data\n",
-                "\n",
+                "earthkit.data.download_example_file(\"tuv_pl.grib\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "ds = earthkit.data.from_source(\"file\", \"tuv_pl.grib\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
@@ -1634,27 +1634,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "dev",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.8.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_tar.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_tar.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9652083333333333%*

 * *Differences: {"'cells'": "{1: {'source': ['We read a tar file containing 2 GRIB files. First we ensure the "*

 * *            "example file is available.'], 'attachments': OrderedDict()}, 3: {'outputs': "*

 * *            "[OrderedDict([('data', OrderedDict([('application/vnd.jupyter.widget-view+json', "*

 * *            "OrderedDict([('model_id', ''), ('version_major', 2), ('version_minor', 0)])), "*

 * *            "('text/plain', ['  0%|          | 0/2 [00:00<?, ?it/s]'])])), ('metadata', "*

 * *            "OrderedDict()), ('output_type', ' […]*

```diff
@@ -1,40 +1,55 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "!test -f test_gribs.tar || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test_gribs.tar"
+                "## Reading GRIB in tar or zip archive"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Reading GRIB in tar or zip archive"
+                "We read a tar file containing 2 GRIB files. First we ensure the example file is available."
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 1,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "We read a tar file containing 2 GRIB files:"
+                "import earthkit.data\n",
+                "earthkit.data.download_example_file(\"test_gribs.tar\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "  0%|          | 0/2 [00:00<?, ?it/s]"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
             "source": [
-                "import earthkit.data\n",
-                "\n",
                 "fs = earthkit.data.from_source(\"file\", \"test_gribs.tar\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -43,25 +58,29 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        " MultiFieldList\n",
-                        "    GRIBReader(/var/folders/ng/g0zkhc2s42xbslpsywwp_26m0000gn/T/earthkit-data-cgr/file-461599e4bea1fe52b7dfd30afff92448fce511fe6e8c41fba0893c7822ab2f30.d/test.grib)\n",
-                        "    GRIBReader(/var/folders/ng/g0zkhc2s42xbslpsywwp_26m0000gn/T/earthkit-data-cgr/file-461599e4bea1fe52b7dfd30afff92448fce511fe6e8c41fba0893c7822ab2f30.d/test4.grib)\n"
-                    ]
+                    "data": {
+                        "text/html": [
+                            "MultiFieldList(GRIBReader(/var/folders/ng/g0zkhc2s42xbslpsywwp_26m0000gn/T/earthkit-data-cgr/file-461599e4bea1fe52b7dfd30afff92448fce511fe6e8c41fba0893c7822ab2f30.d/test.grib),GRIBReader(/var/folders/ng/g0zkhc2s42xbslpsywwp_26m0000gn/T/earthkit-data-cgr/file-461599e4bea1fe52b7dfd30afff92448fce511fe6e8c41fba0893c7822ab2f30.d/test4.grib))"
+                        ],
+                        "text/plain": [
+                            "MultiFieldList(GRIBReader(/var/folders/ng/g0zkhc2s42xbslpsywwp_26m0000gn/T/earthkit-data-cgr/file-461599e4bea1fe52b7dfd30afff92448fce511fe6e8c41fba0893c7822ab2f30.d/test.grib),GRIBReader(/var/folders/ng/g0zkhc2s42xbslpsywwp_26m0000gn/T/earthkit-data-cgr/file-461599e4bea1fe52b7dfd30afff92448fce511fe6e8c41fba0893c7822ab2f30.d/test4.grib))"
+                        ]
+                    },
+                    "execution_count": 3,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs.graph()"
+                "fs"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The resulting object behaves like any standard GRIB object:"
@@ -217,22 +236,14 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "args=() kwargs={'levelist': 500}\n",
-                        "args=() kwargs={'levelist': 500}\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
                             "        vertical-align: middle;\n",
                             "    }\n",
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_to_netcdf.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_to_netcdf.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9747023809523809%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1, 'source': ['import earthkit.data\\n', "*

 * *            '\'earthkit.data.download_example_file("tuv_pl.grib")\']}, 2: {\'execution_count\': '*

 * *            "2}, 3: {'execution_count': 3}, 4: {'execution_count': 4}, delete: [0]}"}*

```diff
@@ -1,60 +1,51 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "id": "bea7a770-c42d-488f-a533-d8fe9202a38f",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "!test -f tuv_pl.grib || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/tuv_pl.grib"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "id": "9c53d7c8-7f38-4a5f-93d0-e05919408b6e",
             "metadata": {},
             "source": [
                 "## Converting GRIB to NetCDF"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "id": "950b9aa8-6b76-47f8-b470-17476f99a733",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import earthkit.data"
+                "import earthkit.data\n",
+                "earthkit.data.download_example_file(\"tuv_pl.grib\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "id": "96b640fd-0039-4061-8cb4-70cfc751cb9c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "fs = earthkit.data.from_source(\"file\", \"tuv_pl.grib\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "id": "0efd9676-6c4f-4e07-a14a-a5337de50461",
             "metadata": {},
             "outputs": [],
             "source": [
                 "fs.to_xarray().to_netcdf(\"_tuv_pl.nc\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "id": "a45aa289-8c85-42bd-a637-8999d8720fcf",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
```

### Comparing `earthkit-data-0.1.3/docs/examples/grib_url.ipynb` & `earthkit-data-0.2.0/docs/examples/grib_url.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/list_of_dict.ipynb` & `earthkit-data-0.2.0/docs/examples/list_of_dict.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/mars.ipynb` & `earthkit-data-0.2.0/docs/examples/mars.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/missing.grib` & `earthkit-data-0.2.0/docs/examples/missing.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/netcdf.ipynb` & `earthkit-data-0.2.0/docs/examples/netcdf.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9712952669814083%*

 * *Differences: {"'cells'": "{2: {'source': {delete: [1, 0]}}, 6: {'outputs': {0: {'data': {'text/html': {insert: "*

 * *            '[(383, "    history:                 GRIB to CDM+CF via cfgrib-0.9.5/ecCodes-2.17.0 '*

 * *            "w...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div "*

 * *            "class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li "*

 * *            "class='xr-section-item'><input id='section-22d3cf59-3fa4-4b46-aba5-9f1764c1367d' "*

 * *            "class='xr-section-su […]*

```diff
@@ -1,33 +1,32 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "!test -f test.nc || wget https://get.ecmwf.int/repository/test-data/earthkit-data/examples/test.nc"
+                "## Using NetCDF data"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 1,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Using NetCDF data"
+                "import earthkit.data\n",
+                "earthkit.data.download_example_file(\"test.nc\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import earthkit.data\n",
-                "\n",
                 "fs = earthkit.data.from_source(\"file\", \"test.nc\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
@@ -473,16 +472,16 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 GRIB to CDM+CF via cfgrib-0.9.5/ecCodes-2.17.0 w...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-2a772f4b-b210-49bf-ac2d-9d4f5f42b21b' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-2a772f4b-b210-49bf-ac2d-9d4f5f42b21b' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>longitude</span>: 19</li><li><span class='xr-has-index'>latitude</span>: 11</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-b4ab701f-922a-4482-a22f-13963a3c2fde' class='xr-section-summary-in' type='checkbox'  checked><label for='section-b4ab701f-922a-4482-a22f-13963a3c2fde' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-27.0 -23.0 -19.0 ... 41.0 45.0</div><input id='attrs-ff895363-cb2e-4e87-8a56-b9f3ab09afb7' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ff895363-cb2e-4e87-8a56-b9f3ab09afb7' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-79f04d13-5458-4f80-848c-76c6d104bfec' class='xr-var-data-in' type='checkbox'><label for='data-79f04d13-5458-4f80-848c-76c6d104bfec' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-27., -23., -19., -15., -11.,  -7.,  -3.,   1.,   5.,   9.,  13.,  17.,\n",
-                            "        21.,  25.,  29.,  33.,  37.,  41.,  45.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>73.0 69.0 65.0 ... 41.0 37.0 33.0</div><input id='attrs-54165375-f1c6-4496-986c-8d7d258493ff' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-54165375-f1c6-4496-986c-8d7d258493ff' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ece3040c-134a-4ea1-9ba3-9b9660dcfb15' class='xr-var-data-in' type='checkbox'><label for='data-ece3040c-134a-4ea1-9ba3-9b9660dcfb15' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([73., 69., 65., 61., 57., 53., 49., 45., 41., 37., 33.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>number</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>int32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-db01c5d9-f96e-47fe-a54d-dfaf675f38f4' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-db01c5d9-f96e-47fe-a54d-dfaf675f38f4' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-93352b59-26e3-45b2-a5e7-d382e29d53d7' class='xr-var-data-in' type='checkbox'><label for='data-93352b59-26e3-45b2-a5e7-d382e29d53d7' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=int32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>time</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-9fe86115-bcd5-4a84-96ac-999e281ef543' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9fe86115-bcd5-4a84-96ac-999e281ef543' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-2d2f0684-3c43-46c1-8c31-112d30ecb979' class='xr-var-data-in' type='checkbox'><label for='data-2d2f0684-3c43-46c1-8c31-112d30ecb979' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>step</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-4545af6d-7e0e-424d-9346-4986a3f8854d' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-4545af6d-7e0e-424d-9346-4986a3f8854d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-39b83b0d-0fb3-4c6d-bb3e-afdd4f2201e3' class='xr-var-data-in' type='checkbox'><label for='data-39b83b0d-0fb3-4c6d-bb3e-afdd4f2201e3' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=timedelta64[ns]]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>surface</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>int32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-9400b0f7-8729-4c60-b6c0-eca8389d4190' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9400b0f7-8729-4c60-b6c0-eca8389d4190' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-11224e3f-2e43-4aa1-bdd6-79096cae26e6' class='xr-var-data-in' type='checkbox'><label for='data-11224e3f-2e43-4aa1-bdd6-79096cae26e6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=int32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-31b60037-d694-4284-8ec0-d79917d800e1' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-31b60037-d694-4284-8ec0-d79917d800e1' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-350ec79c-66ff-450e-8a79-d00f45794a9a' class='xr-var-data-in' type='checkbox'><label for='data-350ec79c-66ff-450e-8a79-d00f45794a9a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-4a9fd08f-e310-4b4a-8cc4-f532d813292c' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4a9fd08f-e310-4b4a-8cc4-f532d813292c' class='xr-section-summary' >Data variables: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>dask.array&lt;chunksize=(11, 19), meta=np.ndarray&gt;</div><input id='attrs-6a3779e4-2fd7-4e19-b6e9-7518ed9ad7f7' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6a3779e4-2fd7-4e19-b6e9-7518ed9ad7f7' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d1313cc1-a105-4902-8d18-96cc2d5edc47' class='xr-var-data-in' type='checkbox'><label for='data-d1313cc1-a105-4902-8d18-96cc2d5edc47' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>209</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_Nx :</span></dt><dd>19</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>4.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-27.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>45.0</dd><dt><span>GRIB_Ny :</span></dt><dd>11</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>4.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>73.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>33.0</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd></dl></div><div class='xr-var-data'><table>\n",
+                            "    history:                 GRIB to CDM+CF via cfgrib-0.9.5/ecCodes-2.17.0 w...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-22d3cf59-3fa4-4b46-aba5-9f1764c1367d' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-22d3cf59-3fa4-4b46-aba5-9f1764c1367d' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>longitude</span>: 19</li><li><span class='xr-has-index'>latitude</span>: 11</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-a38797d5-0eb3-4a59-929d-7a76b949c3d5' class='xr-section-summary-in' type='checkbox'  checked><label for='section-a38797d5-0eb3-4a59-929d-7a76b949c3d5' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-27.0 -23.0 -19.0 ... 41.0 45.0</div><input id='attrs-7b060483-3b2b-4cf2-8d6e-935dd6ab75a8' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-7b060483-3b2b-4cf2-8d6e-935dd6ab75a8' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-02cc9302-7c65-4f4f-9e68-fc28d0d77e9b' class='xr-var-data-in' type='checkbox'><label for='data-02cc9302-7c65-4f4f-9e68-fc28d0d77e9b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-27., -23., -19., -15., -11.,  -7.,  -3.,   1.,   5.,   9.,  13.,  17.,\n",
+                            "        21.,  25.,  29.,  33.,  37.,  41.,  45.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>73.0 69.0 65.0 ... 41.0 37.0 33.0</div><input id='attrs-57d56744-3339-4129-be5e-283302ac0e2a' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-57d56744-3339-4129-be5e-283302ac0e2a' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-6f3ba92f-6b0e-4df9-ab91-8ea9576fe08d' class='xr-var-data-in' type='checkbox'><label for='data-6f3ba92f-6b0e-4df9-ab91-8ea9576fe08d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([73., 69., 65., 61., 57., 53., 49., 45., 41., 37., 33.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>number</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>int32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-5b6c721f-9dc3-4798-b895-0379553c0975' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5b6c721f-9dc3-4798-b895-0379553c0975' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c035ce3e-ae2b-4592-88cd-21c82a4e76af' class='xr-var-data-in' type='checkbox'><label for='data-c035ce3e-ae2b-4592-88cd-21c82a4e76af' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=int32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>time</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-a7d65f8a-7a1f-4e6f-b219-cec2d24864fb' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a7d65f8a-7a1f-4e6f-b219-cec2d24864fb' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-bec9d853-eaab-4911-9e26-ba64bad21ef7' class='xr-var-data-in' type='checkbox'><label for='data-bec9d853-eaab-4911-9e26-ba64bad21ef7' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>step</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-9a10ceda-e8b0-4aca-8105-58927723a04c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9a10ceda-e8b0-4aca-8105-58927723a04c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e0b40303-a140-482a-9dd4-f9881786b9c1' class='xr-var-data-in' type='checkbox'><label for='data-e0b40303-a140-482a-9dd4-f9881786b9c1' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=timedelta64[ns]]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>surface</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>int32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-0405ffaf-4572-4b4e-9e35-588468142e50' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0405ffaf-4572-4b4e-9e35-588468142e50' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-2aec7333-4511-4148-8d6a-5c9f8228e0ce' class='xr-var-data-in' type='checkbox'><label for='data-2aec7333-4511-4148-8d6a-5c9f8228e0ce' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=int32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>()</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-33e520b6-8f1b-489e-870e-ee9b71dc3ff8' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-33e520b6-8f1b-489e-870e-ee9b71dc3ff8' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-944a419c-8089-460e-b185-ae863ed98525' class='xr-var-data-in' type='checkbox'><label for='data-944a419c-8089-460e-b185-ae863ed98525' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-b6ade1ec-5bcf-489a-b707-9100f26c2599' class='xr-section-summary-in' type='checkbox'  checked><label for='section-b6ade1ec-5bcf-489a-b707-9100f26c2599' class='xr-section-summary' >Data variables: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>dask.array&lt;chunksize=(11, 19), meta=np.ndarray&gt;</div><input id='attrs-f148dabe-d639-42a2-b6cb-c428dcba554a' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-f148dabe-d639-42a2-b6cb-c428dcba554a' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d0580f2f-f88b-42d3-9025-5b11a93a5fc2' class='xr-var-data-in' type='checkbox'><label for='data-d0580f2f-f88b-42d3-9025-5b11a93a5fc2' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>209</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_Nx :</span></dt><dd>19</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>4.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-27.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>45.0</dd><dt><span>GRIB_Ny :</span></dt><dd>11</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>4.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>73.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>33.0</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd></dl></div><div class='xr-var-data'><table>\n",
                             "    <tr>\n",
                             "        <td>\n",
                             "            <table style=\"border-collapse: collapse;\">\n",
                             "                <thead>\n",
                             "                    <tr>\n",
                             "                        <td> </td>\n",
                             "                        <th> Array </th>\n",
@@ -529,15 +528,15 @@
                             "\n",
                             "  <!-- Text -->\n",
                             "  <text x=\"60.000000\" y=\"89.473684\" font-size=\"1.0rem\" font-weight=\"100\" text-anchor=\"middle\" >19</text>\n",
                             "  <text x=\"140.000000\" y=\"34.736842\" font-size=\"1.0rem\" font-weight=\"100\" text-anchor=\"middle\" transform=\"rotate(0,140.000000,34.736842)\">11</text>\n",
                             "</svg>\n",
                             "        </td>\n",
                             "    </tr>\n",
-                            "</table></div></li><li class='xr-var-item'><div class='xr-var-name'><span>msl</span></div><div class='xr-var-dims'>(latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>dask.array&lt;chunksize=(11, 19), meta=np.ndarray&gt;</div><input id='attrs-3af12df5-daca-4673-abbe-9f071f227771' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-3af12df5-daca-4673-abbe-9f071f227771' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-02cfd3b6-5582-411b-852d-c23504126c72' class='xr-var-data-in' type='checkbox'><label for='data-02cfd3b6-5582-411b-852d-c23504126c72' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>151</dd><dt><span>GRIB_shortName :</span></dt><dd>msl</dd><dt><span>GRIB_units :</span></dt><dd>Pa</dd><dt><span>GRIB_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>GRIB_cfName :</span></dt><dd>air_pressure_at_mean_sea_level</dd><dt><span>GRIB_cfVarName :</span></dt><dd>msl</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>209</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_Nx :</span></dt><dd>19</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>4.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-27.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>45.0</dd><dt><span>GRIB_Ny :</span></dt><dd>11</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>4.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>73.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>33.0</dd><dt><span>long_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>units :</span></dt><dd>Pa</dd><dt><span>standard_name :</span></dt><dd>air_pressure_at_mean_sea_level</dd></dl></div><div class='xr-var-data'><table>\n",
+                            "</table></div></li><li class='xr-var-item'><div class='xr-var-name'><span>msl</span></div><div class='xr-var-dims'>(latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>dask.array&lt;chunksize=(11, 19), meta=np.ndarray&gt;</div><input id='attrs-ce81f7ca-df8d-4f87-9dbe-a5336007cf85' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ce81f7ca-df8d-4f87-9dbe-a5336007cf85' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-bb2f9d28-0897-43c0-a51f-7a09fad02af9' class='xr-var-data-in' type='checkbox'><label for='data-bb2f9d28-0897-43c0-a51f-7a09fad02af9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>151</dd><dt><span>GRIB_shortName :</span></dt><dd>msl</dd><dt><span>GRIB_units :</span></dt><dd>Pa</dd><dt><span>GRIB_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>GRIB_cfName :</span></dt><dd>air_pressure_at_mean_sea_level</dd><dt><span>GRIB_cfVarName :</span></dt><dd>msl</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>209</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_Nx :</span></dt><dd>19</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>4.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-27.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>45.0</dd><dt><span>GRIB_Ny :</span></dt><dd>11</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>4.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>73.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>33.0</dd><dt><span>long_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>units :</span></dt><dd>Pa</dd><dt><span>standard_name :</span></dt><dd>air_pressure_at_mean_sea_level</dd></dl></div><div class='xr-var-data'><table>\n",
                             "    <tr>\n",
                             "        <td>\n",
                             "            <table style=\"border-collapse: collapse;\">\n",
                             "                <thead>\n",
                             "                    <tr>\n",
                             "                        <td> </td>\n",
                             "                        <th> Array </th>\n",
@@ -584,20 +583,20 @@
                             "\n",
                             "  <!-- Text -->\n",
                             "  <text x=\"60.000000\" y=\"89.473684\" font-size=\"1.0rem\" font-weight=\"100\" text-anchor=\"middle\" >19</text>\n",
                             "  <text x=\"140.000000\" y=\"34.736842\" font-size=\"1.0rem\" font-weight=\"100\" text-anchor=\"middle\" transform=\"rotate(0,140.000000,34.736842)\">11</text>\n",
                             "</svg>\n",
                             "        </td>\n",
                             "    </tr>\n",
-                            "</table></div></li></ul></div></li><li class='xr-section-item'><input id='section-461c6afd-940b-4516-abde-54d02c9be1d4' class='xr-section-summary-in' type='checkbox'  ><label for='section-461c6afd-940b-4516-abde-54d02c9be1d4' class='xr-section-summary' >Indexes: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-ca95febf-7e3f-437b-bb65-a7901f138bff' class='xr-index-data-in' type='checkbox'/><label for='index-ca95febf-7e3f-437b-bb65-a7901f138bff' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([-27.0, -23.0, -19.0, -15.0, -11.0,  -7.0,  -3.0,   1.0,   5.0,\n",
+                            "</table></div></li></ul></div></li><li class='xr-section-item'><input id='section-19d71873-4a56-4ee5-8667-2cac51274ba7' class='xr-section-summary-in' type='checkbox'  ><label for='section-19d71873-4a56-4ee5-8667-2cac51274ba7' class='xr-section-summary' >Indexes: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-da54813b-56f7-4db5-b45c-8add6796c241' class='xr-index-data-in' type='checkbox'/><label for='index-da54813b-56f7-4db5-b45c-8add6796c241' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([-27.0, -23.0, -19.0, -15.0, -11.0,  -7.0,  -3.0,   1.0,   5.0,\n",
                             "                9.0,  13.0,  17.0,  21.0,  25.0,  29.0,  33.0,  37.0,  41.0,\n",
                             "               45.0],\n",
-                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c759af26-6828-48d7-98bf-c8ec9fdf5890' class='xr-index-data-in' type='checkbox'/><label for='index-c759af26-6828-48d7-98bf-c8ec9fdf5890' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([73.0, 69.0, 65.0, 61.0, 57.0, 53.0, 49.0, 45.0, 41.0, 37.0,\n",
+                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-f48513d9-286e-41d6-b16a-36fa22a79f42' class='xr-index-data-in' type='checkbox'/><label for='index-f48513d9-286e-41d6-b16a-36fa22a79f42' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([73.0, 69.0, 65.0, 61.0, 57.0, 53.0, 49.0, 45.0, 41.0, 37.0,\n",
                             "              33.0],\n",
-                            "             dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-cd5d76ae-0947-46d2-9c6e-1ccfe3174747' class='xr-section-summary-in' type='checkbox'  checked><label for='section-cd5d76ae-0947-46d2-9c6e-1ccfe3174747' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>GRIB to CDM+CF via cfgrib-0.9.5/ecCodes-2.17.0 with source=&#x27;/Users/baudouin/git/climet/test.grib&#x27;, filter_by_keys={}, encode_cf=(&#x27;parameter&#x27;, &#x27;time&#x27;, &#x27;geography&#x27;, &#x27;vertical&#x27;)</dd></dl></div></li></ul></div></div>"
+                            "             dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-a9fb882d-446b-46ad-b0f3-0d8a9d2892b7' class='xr-section-summary-in' type='checkbox'  checked><label for='section-a9fb882d-446b-46ad-b0f3-0d8a9d2892b7' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>GRIB to CDM+CF via cfgrib-0.9.5/ecCodes-2.17.0 with source=&#x27;/Users/baudouin/git/climet/test.grib&#x27;, filter_by_keys={}, encode_cf=(&#x27;parameter&#x27;, &#x27;time&#x27;, &#x27;geography&#x27;, &#x27;vertical&#x27;)</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:     (longitude: 19, latitude: 11)\n",
                             "Coordinates:\n",
                             "  * longitude   (longitude) float64 -27.0 -23.0 -19.0 -15.0 ... 37.0 41.0 45.0\n",
                             "  * latitude    (latitude) float64 73.0 69.0 65.0 61.0 ... 45.0 41.0 37.0 33.0\n",
```

### Comparing `earthkit-data-0.1.3/docs/examples/temp_10.bufr` & `earthkit-data-0.2.0/docs/examples/temp_10.bufr`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/test.grib` & `earthkit-data-0.2.0/docs/examples/test.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/test.nc` & `earthkit-data-0.2.0/docs/examples/test.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/test.odb` & `earthkit-data-0.2.0/docs/examples/test.odb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/test4.grib` & `earthkit-data-0.2.0/docs/examples/test4.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/test6.grib` & `earthkit-data-0.2.0/docs/examples/test6.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples/tuv_pl.grib` & `earthkit-data-0.2.0/docs/examples/tuv_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/examples.rst` & `earthkit-data-0.2.0/docs/examples.rst`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 .. toctree::
     :maxdepth: 1
     :caption: Retrieve
 
     examples/mars.ipynb
     examples/cds.ipynb
+    examples/ecmwf_open_data.ipynb
     examples/fdb.ipynb
 
 
 .. toctree::
     :maxdepth: 1
     :caption: GRIB
 
@@ -50,11 +51,19 @@
     :caption: ODB
     :glob:
 
     examples/odb*
 
 .. toctree::
     :maxdepth: 1
-    :caption: List of dicts
+    :caption: Other inputs
     :glob:
 
+    examples/from_object.ipynb
     examples/list_of_dict*
+
+.. toctree::
+    :maxdepth: 1
+    :caption: Miscellaneous
+    :glob:
+
+    examples/projection.ipynb
```

### Comparing `earthkit-data-0.1.3/docs/guide/caching.rst` & `earthkit-data-0.2.0/docs/guide/caching.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/guide/data.rst` & `earthkit-data-0.2.0/docs/guide/data.rst`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     8
 
 .. _iter:
 
 Iteration
 ~~~~~~~~~
 
-When an earthkit-data data `source` or dataset provides a list of fields, it can be iterated over to access each field (in a given order see :ref:`below <order_by>`).
+When an earthkit-data data `source` or dataset provides a list of fields or messages, we can iterated through it to access each element (in a given order see :ref:`below <order_by>`).
 
 In the the following example we read a GRIB file from disk. In the iteration each element is a field (representing a GRIB message):
 
 .. code-block:: python
 
     >>> import earthkit.data
     >>> ds = earthkit.data.from_source("file", "docs/examples/test6.grib")
@@ -78,15 +78,15 @@
     GribField(v,850,20180801,1200,0,0)
 
 .. _slice:
 
 Selection with ``[...]``
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
-When an earthkit-data data `source` or dataset provides a list of fields, a subset of the list can be created using the standard python list interface relying on brackets and slices. A subsetting also works by providing a list or ndarray of indices.
+When an earthkit-data data `source` or dataset provides a list of fields or messages, a subset of it can be created using the standard python list interface relying on brackets and slices. Slicing also works by providing a list or ndarray of indices.
 
 .. code-block:: python
 
     >>> import earthkit.data
     >>> ds = earthkit.data.from_source("file", "docs/examples/test6.grib")
 
     >>> len(ds)
@@ -128,15 +128,15 @@
 
 
 .. _sel:
 
 Selection with ``.sel()``
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-When an earthkit-data data `source` or dataset provides a list of fields, the method ``.sel()`` allows filtering this list and we can **select a subset** of the list of fields. ``.sel()`` returns a view to original data, so no data is copied. The selection offers the same functionality as the original data object, so methods like ``.to_numpy()``, ``.to_xarray()``, etc. are all available.
+When an earthkit-data data `source` or dataset provides a list of fields or messages, the method ``.sel()`` allows filtering this list and we can **select a subset** of the list. ``.sel()`` returns a view to original data, so no data is copied. The selection offers the same functionality as the original data object, so methods like ``.to_numpy()``, ``.to_xarray()``, etc. are all available.
 
 For more details see: :meth:`FieldList.sel() <data.readers.grib.index.FieldList.sel>`
 
 The following example demonstrates the usage of ``.sel()``. The input data contains temperature and wind fields on various pressure levels.
 
 .. code-block:: python
 
@@ -175,15 +175,15 @@
     GribField(v,400,20180801,1200,0,0)
 
 .. _isel:
 
 Selection with ``.isel()``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-When an earthkit-data data `source` or dataset provides a list of fields, the method ``.isel()`` allows filtering this list and we can **select a subset** of the list of fields. ``.isel()`` returns a view to the original data, so no data is copied. The selection offers the same functionality as the original data object, so methods like ``.to_numpy()``, ``.to_xarray()`` , etc. are all available.
+When an earthkit-data data `source` or dataset provides a list of fields, the method ``.isel()`` allows filtering this list and we can **select a subset** of the list. ``.isel()`` returns a view to the original data, so no data is copied. The selection offers the same functionality as the original data object, so methods like ``.to_numpy()``, ``.to_xarray()`` , etc. are all available.
 
 ``.isel()`` works similarly to :ref:`sel <sel>` but conditions are specified by indices of metadata keys. A metadata index stores the unique, **sorted** values of the corresponding metadata key from all the fields in the input data.
 
 For more details see: :meth:`FieldList.isel() <data.readers.grib.index.FieldList.isel>`
 
 The following example demonstrates the usage of ``.isel()``. The input data contains temperature and wind fields on various pressure levels.
 
@@ -225,15 +225,15 @@
 
 
 .. _order_by:
 
 Ordering with ``.order_by()``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-When an earthkit-data data `source` or dataset provides a list of fields, the method ``.order_by()`` allows sorting this list.
+When an earthkit-data data `source` or dataset provides a list of fields or messages, the method ``.order_by()`` allows sorting this list.
 
 ``.order_by()`` returns a "view" so no new data is generated on disk or in memory. The resulting object offers the same functionality as the original data object, so methods like ``.to_numpy()``, ``.to_xarray()``, etc. are all available.
 
 For more details see: :meth:`FieldList.sel() <data.readers.grib.index.FieldList.order_by>`
 
 .. code-block:: python
 
@@ -324,15 +324,15 @@
 .. _metadata:
 
 Accessing metadata
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 We can extract metadata from data objects using the ``.metadata()`` method.
 
-When an earthkit-data :ref:`source <data-sources>` provides a list of fields, this method can be called both on the whole object and on the individual fields, too.
+When an earthkit-data :ref:`source <data-sources>` provides a list of fields or messages, this method can be called both on the whole object and on the individual fields, too.
 
 For more details see: :meth:`FieldList.metadata() <data.readers.grib.index.FieldList.metadata>` and
 :meth:`GribField._metadata() <data.readers.grib.codes.GribField.metadata>`
 
 .. _inspection:
 
 Inspecting contents
```

### Comparing `earthkit-data-0.1.3/docs/guide/settings.rst` & `earthkit-data-0.2.0/docs/guide/settings.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _settings:
+
 Settings
 ========
 
 *earthkit-data* is maintaining a set of global settings which control
 its behaviour.
 
 The settings are saved in ``~/.earthkit-data/settings.yaml``. They can
```

### Comparing `earthkit-data-0.1.3/docs/guide/sources.rst` & `earthkit-data-0.2.0/docs/guide/sources.rst`

 * *Files 18% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 Getting data from a source
 ----------------------------
 
 We can get data from a given source by using :func:`from_source`:
 
 .. py:function:: from_source(name, *args, **kwargs)
 
-  Returns a :ref:`data object <data-object>` from the source specified by ``name``.
+  Returns a :ref:`data object <data-object>` from the source specified by ``name`` .
 
   :param str name: the source (see below)
   :param tuple *args: specifies the data location and additional parameters to access the data
   :param dict **kwargs: provides **additional functionalities** including caching, filtering, sorting and indexing
 
   **earthkit-data** has the following built-in sources:
 
   .. list-table:: Data sources
-    :widths: 20 80
+    :widths: 30 70
     :header-rows: 1
 
     * - Name
       - Description
     * - :ref:`data-sources-file`
       - read data from a file/files
     * - :ref:`data-sources-file-pattern`
@@ -36,14 +36,16 @@
       - read data from a stream
     * - :ref:`data-sources-memory`
       - read data from a memory buffer
     * - :ref:`data-sources-mars`
       - retrieve data from the ECMWF `MARS archive <https://confluence.ecmwf.int/display/UDOC/MARS+user+documentation>`_
     * - :ref:`data-sources-cds`
       - retrieve data from the `Copernicus Climate Data Store <https://cds.climate.copernicus.eu/>`_ (CDS)
+    * - :ref:`data-sources-eod`
+      - retrieve `ECMWF open data <https://www.ecmwf.int/en/forecasts/datasets/open-data>`_
     * - :ref:`data-sources-fdb`
       - retrieve data from the `Fields DataBase <https://fields-database.readthedocs.io/en/latest/>`_ (FDB)
 
 
 ----------------------------------
 
 .. _data-sources-file:
@@ -85,15 +87,15 @@
       ds = earthkit.data.from_source("file", "path/to/dir")
 
 
   Further examples:
 
     - :ref:`/examples/grib_overview.ipynb`
     - :ref:`/examples/grib_multi.ipynb`
-    - :ref:`/examples/bufr.ipynb`
+    - :ref:`/examples/bufr_temp.ipynb`
     - :ref:`/examples/netcdf.ipynb`
     - :ref:`/examples/odb.ipynb`
 
 .. _data-sources-file-pattern:
 
 file-pattern
 --------------
@@ -300,15 +302,14 @@
   :param tuple *args: positional arguments specifying the request as a dict
   :param dict **kwargs: other keyword arguments specifying the request
 
   The following example retrieves analysis GRIB data for a subarea for 2 surface parameters:
 
   .. code-block:: python
 
-      import io
       import earthkit.data
 
       ds = earthkit.data.from_source(
           "mars",
           {
               "param": ["2t", "msl"],
               "levtype": "sfc",
@@ -354,80 +355,142 @@
           grid=[2, 2],
           date="2012-05-10",
       )
 
 
   Data downloaded from the CDS is stored in the the :ref:`cache <caching>`.
 
-  To access data from the CDS, you will need to register and retrieve an access token. The process is described here_. For more information, see the CDS `knowledge base`_.
+  To access data from the CDS, you will need to register and retrieve an access token. The process is described `here <https://cds.climate.copernicus.eu/api-how-to>`__. For more information, see the CDS `knowledge base`_.
 
   Further examples:
 
       - :ref:`/examples/cds.ipynb`
 
+
+.. _data-sources-eod:
+
+ecmwf-open-data
+-------------------
+
+.. py:function:: from_source("ecmwf-open-data", *args, **kwargs)
+  :noindex:
+
+  The ``ecmwf-open-data`` source provides access to the `ECMWF open data`_, which is a subset of ECMWF real-time forecast data made available to the public free of charge.  It uses the `ecmwf-opendata <https://github.com/ecmwf/ecmwf-opendata>`_ package.
+
+  :param tuple *args: specifies the request as a dict
+  :param dict **kwargs: other keyword arguments specifying the request
+
+  Details about the request format can be found `here <https://github.com/ecmwf/ecmwf-opendata>`__.
+
+  The following example retrieves forecast for 2 surface parameters from the latest forecast:
+
+  .. code-block:: python
+
+      import earthkit.data
+
+      ds = earthkit.data.from_source(
+          "ecmwf-open-data", param=["2t", "msl"], levtype="sfc", step=[0, 6, 12]
+      )
+
+
+  The resulting GRIB data files are stored in the :ref:`cache <caching>`.
+
+  Further examples:
+
+      - :ref:`/examples/ecmwf_open_data.ipynb`
+
+
 .. _data-sources-fdb:
 
 fdb
 ---
 
-.. py:function:: from_source("fdb", *args, stream=True, batch_size=1, **kwargs)
+.. py:function:: from_source("fdb", *args, stream=True, group_by=None, batch_size=1, **kwargs)
   :noindex:
 
   The ``fdb`` source accesses the `FDB (Fields DataBase) <https://fields-database.readthedocs.io/en/latest/>`_, which is a domain-specific object store developed at ECMWF for storing, indexing and retrieving GRIB data. earthkit-data uses the `pyfdb <https://pyfdb.readthedocs.io/en/latest>`_ package to retrieve data from FDB.
 
-  :param str dataset: the name of the CDS dataset
   :param tuple *args: positional arguments specifying the request as a dict
   :param bool stream: when it is ``True`` the data is read as a stream. Otherwise the data is retrieved into a file and stored in the :ref:`cache <caching>`.
-  :param bool batch_size: used when ``stream=True`` and defines how many GRIB messages are consumed from the stream and kept in memory at a time. ``batch_size=0`` means all the messages will be loaded and stored in memory.  When ``batch_size`` is not zero ``from_source`` gives us a stream iterator object. During the iteration temporary objects are created for each message then get deleted when going out of scope.
+  :param group_by: used when ``stream=True`` and can specify one or more metadata keys to control how GRIB messages are read from the stream. When it is set ``from_source`` gives us a stream iterator object. Each iteration step results in a Fieldlist object, which is built by consuming GRIB messages from the stream until the values of the ``group_by`` metadata keys change. The generated Fieldlist keeps GRIB messages in memory then gets deleted when going out of scope. When ``group_by`` is set ``batch_size`` cannot be used.
+  :type group_by: str, list of str
+  :param bool batch_size: used when ``stream=True`` and ``group_by`` is unset. It defines how many GRIB messages are consumed from the stream and kept in memory at a time. ``batch_size=0`` means all the messages will be loaded and stored in memory.  When ``batch_size`` is not zero ``from_source`` gives us a stream iterator object. During the iteration temporary objects are created for each message then get deleted when going out of scope.
   :param dict **kwargs: other keyword arguments specifying the request
 
-  The following example retrieves analysis :ref:`grib` data for 2 surface parameters as stream.
-  By default (``batch_size=1``) we will consume one message at a time and ``ds`` in the code can only be used as an iterator:
+  The following example retrieves analysis :ref:`grib` data for 3 surface parameters as stream.
+  By default we will consume one message at a time and ``ds`` can only be used as an iterator:
 
   .. code-block:: python
 
       >>> import earthkit.data
       >>> request = {
       ...     "class": "od",
       ...     "expver": "0001",
       ...     "stream": "oper",
-      ...     "date": "20230524",
+      ...     "date": "20230607",
       ...     "time": [0, 12],
       ...     "domain": "g",
       ...     "type": "an",
       ...     "levtype": "sfc",
       ...     "step": 0,
-      ...     "param": [151, 167],
+      ...     "param": [151, 167, 168],
       ... }
       >>>
       >>> ds = earthkit.data.from_source("fdb", request)
       >>> for f in ds:
       ...     print(f)
       ...
-      GribField(msl,None,20230524,0,0,0)
-      GribField(2t,None,20230524,0,0,0)
-      GribField(msl,None,20230524,1200,0,0)
-      GribField(2t,None,20230524,1200,0,0)
+      GribField(msl,None,20230607,0,0,0)
+      GribField(2t,None,20230607,0,0,0)
+      GribField(msl,None,20230607,1200,0,0)
+      GribField(2t,None,20230607,1200,0,0)
+
+  We can use ``group_by`` to read fields with a matching time. ``ds`` is still just an iterator, but ``f`` is now a :obj:`FieldList <data.readers.grib.index.FieldList>`:
+
+      >>> ds = earthkit.data.from_source("fdb", request, group_by="time")
+      >>> for f in ds:
+      ...     print(f)
+      ...     for g in f:
+      ...         print(f" {g}")
+      ...
+      <class 'earthkit.data.readers.grib.memory.FieldListInMemory'>
+       GribField(msl,None,20230607,0,0,0)
+       GribField(2t,None,20230607,0,0,0)
+       GribField(2d,None,20230607,0,0,0)
+      <class 'earthkit.data.readers.grib.memory.FieldListInMemory'>
+       GribField(msl,None,20230607,1200,0,0)
+       GribField(2t,None,20230607,1200,0,0)
+       GribField(2d,None,20230607,1200,0,0)
 
   We can use ``batch_size=2`` to read 2 fields at a time. ``ds`` is still just an iterator, but ``f`` is now a :obj:`FieldList <data.readers.grib.index.FieldList>` containing 2 fields:
 
       >>> ds = earthkit.data.from_source("fdb", request, batch_size=2)
       >>> for f in ds:
-      ...     print(len(f))
+      ...     print(f)
+      ...     for g in f:
+      ...         print(f" {g}")
       ...
-      2
-      2
+      <class 'earthkit.data.readers.grib.memory.FieldListInMemory'>
+        GribField(msl,None,20230607,0,0,0)
+        GribField(2t,None,20230607,0,0,0)
+      <class 'earthkit.data.readers.grib.memory.FieldListInMemory'>
+        GribField(2d,None,20230607,0,0,0)
+        GribField(msl,None,20230607,1200,0,0)
+      <class 'earthkit.data.readers.grib.memory.FieldListInMemory'>
+        GribField(2t,None,20230607,1200,0,0)
+        GribField(2d,None,20230607,1200,0,0)
 
 
   Further examples:
 
       - :ref:`/examples/fdb.ipynb`
 
 
 .. _MARS catalog: https://apps.ecmwf.int/archive-catalogue/
 .. _MARS user documentation: https://confluence.ecmwf.int/display/UDOC/MARS+user+documentation
 .. _web API: https://www.ecmwf.int/en/forecasts/access-forecasts/ecmwf-web-api
 
 .. _Copernicus Climate Data Store: https://cds.climate.copernicus.eu/
-.. _here: https://cds.climate.copernicus.eu/api-how-to
 .. _cdsapi: https://pypi.org/project/cdsapi/
 .. _knowledge base: https://confluence.ecmwf.int/display/CKB/Copernicus+Knowledge+Base
+
+.. _ECMWF open data: https://www.ecmwf.int/en/forecasts/datasets/open-data
```

### Comparing `earthkit-data-0.1.3/docs/index.rst` & `earthkit-data-0.2.0/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
    api
 
 .. toctree::
    :maxdepth: 1
    :caption: Installation
 
    install
+   release_notes/index
    development
    licence
 
 
 Indices and tables
 ==================
```

### Comparing `earthkit-data-0.1.3/docs/install.rst` & `earthkit-data-0.2.0/docs/install.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 Installation
 ============
 
 Installing earthkit-data
 ----------------------------
 
-Install **earthkit-data** with python3 (>= 3.8) and **pip** as follows:
+Install **earthkit-data** with python3 (>= 3.8) and ``pip`` as follows:
 
 .. code-block:: bash
 
     python3 -m pip install earthkit-data
 
+Alternatively, install via ``conda`` with:
+
+.. code-block:: bash
+
+    conda install earthkit-data -c conda-forge
+
+This will bring in some necessary binary dependencies for you.
 
 Installing the binary dependencies
 --------------------------------------
 
-eccCodes
+ecCodes
 +++++++++++
 
-**earthkit-data** depends on the ECMWF *ecCodes* library
-that must be installed on the system and accessible as a shared library. The easiest way to install it is to use Conda:
+**earthkit-data** depends on the ECMWF :xref:`eccodes` library
+that must be installed on the system and accessible as a shared library.
 
-.. code-block:: bash
+When earthkit-data is installed from ``conda`` ecCodes will **also be installed** for you. Otherwise, you need to install it using one of the following methods:
 
-    conda install eccodes -c conda-forge
+    - The easiest way to install it is to use ``conda``:
 
+        .. code-block:: bash
 
-On a MacOS it is also available from HomeBrew:
+            conda install eccodes -c conda-forge
 
-.. code-block:: bash
+    - On a MacOS it is also available from ``HomeBrew``:
+
+        .. code-block:: bash
 
-    brew install eccodes
+            brew install eccodes
 
-As an alternative you may install the official source distribution
-by following the instructions at
-https://software.ecmwf.int/wiki/display/ECC/ecCodes+installation
+    - As an alternative you may install the official source distribution by following the instructions `here <https://software.ecmwf.int/wiki/display/ECC/ecCodes+installation>`_.
 
 FDB
 +++++
 
-For FDB (Fields DataBase) access FDB5 must be installed in the system. See the `FDB documentation <https://fields-database.readthedocs.io/en/latest/>`_ for details.
+For FDB (Fields DataBase) access FDB5 must be installed on the system. See the `FDB documentation <https://fields-database.readthedocs.io/en/latest/>`_ for details.
```

### Comparing `earthkit-data-0.1.3/docs/licence.rst` & `earthkit-data-0.2.0/docs/licence.rst`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/docs/make.bat` & `earthkit-data-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/__init__.py` & `earthkit-data-0.2.0/earthkit/data/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,22 +11,30 @@
     # NOTE: the `version.py` file must not be present in the git repository
     #   as it is generated by setuptools at install time
     from .version import __version__
 except ImportError:  # pragma: no cover
     # Local copy or not installed with setuptools
     __version__ = "999"
 
+from earthkit.data.translators import transform
+from earthkit.data.wrappers import get_wrapper as from_object
+
 from .arguments.transformers import ALL
 from .core.caching import CACHE as cache
 from .core.settings import SETTINGS as settings
 from .readers.grib.output import new_grib_output
 from .sources import from_source, from_source_lazily
+from .utils.examples import download_example_file, remote_example_file
 
 __all__ = [
     "ALL",
     "cache",
+    "download_example_file",
     "from_source",
     "from_source_lazily",
+    "from_object",
+    "transform",
     "new_grib_output",
+    "remote_example_file",
     "settings",
     "__version__",
 ]
```

### Comparing `earthkit-data-0.1.3/earthkit/data/arguments/__init__.py` & `earthkit-data-0.2.0/earthkit/data/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/arguments/args_kwargs.py` & `earthkit-data-0.2.0/earthkit/data/arguments/args_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/arguments/argument.py` & `earthkit-data-0.2.0/earthkit/data/arguments/argument.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/arguments/earthkit_types.py` & `earthkit-data-0.2.0/earthkit/data/arguments/earthkit_types.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/arguments/input_manager.py` & `earthkit-data-0.2.0/earthkit/data/arguments/input_manager.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/arguments/transformers.py` & `earthkit-data-0.2.0/earthkit/data/arguments/transformers.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/core/__init__.py` & `earthkit-data-0.2.0/earthkit/data/core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,22 @@
         self._not_implemented()
 
     @abstractmethod
     def order_by(self, *args, **kwargs):
         """Reorder the elements of the object."""
         self._not_implemented()
 
+    @abstractmethod
+    def to_points(self, *args, **kwargs):
+        self._not_implemented()
+
+    @abstractmethod
+    def to_latlon(self, *args, **kwargs):
+        self._not_implemented()
+
     def __add__(self, other):
         self._not_implemented()
 
     #
     def _not_implemented(self):
         import inspect
```

### Comparing `earthkit-data-0.1.3/earthkit/data/core/caching.py` & `earthkit-data-0.2.0/earthkit/data/core/caching.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/core/index.py` & `earthkit-data-0.2.0/earthkit/data/core/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     def new_mask_index(self, *args, **kwargs):
         return MaskIndex(*args, **kwargs)
 
     @abstractmethod
     def __len__(self):
         self._not_implemented()
 
-    def _normalize_kwargs_names(**kwargs):
+    def _normalize_kwargs_names(self, **kwargs):
         return kwargs
 
     def sel(self, *args, remapping=None, **kwargs):
         """Uses metadata values to select a subset of the elements from a fieldlist-like object.
 
         Parameters
         ----------
@@ -416,15 +416,15 @@
         Returns
         -------
         object
             Returns a new object with reordered elements. It contains a view to the data in the
             original object, so no data is copied.
 
 
-        Ordering by a single metadata key ("param"). The default ordering directio
+        Ordering by a single metadata key ("param"). The default ordering direction
         is ``ascending``:
 
         >>> import earthkit.data
         >>> ds = earthkit.data.from_source("file", "docs/examples/test6.grib")
         >>> for f in ds.order_by("param"):
         ...     print(f)
         ...
```

### Comparing `earthkit-data-0.1.3/earthkit/data/core/ipython.py` & `earthkit-data-0.2.0/earthkit/data/core/ipython.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/core/order.py` & `earthkit-data-0.2.0/earthkit/data/core/order.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/core/plugins.py` & `earthkit-data-0.2.0/earthkit/data/core/plugins.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/core/select.py` & `earthkit-data-0.2.0/earthkit/data/core/select.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/core/settings.py` & `earthkit-data-0.2.0/earthkit/data/core/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,37 +15,64 @@
 from contextlib import contextmanager
 from typing import Callable
 
 import yaml
 
 from earthkit.data import __version__ as VERSION
 from earthkit.data.utils.html import css
-from earthkit.data.utils.humanize import as_bytes, as_percent, as_seconds
+from earthkit.data.utils.humanize import (
+    as_bytes,
+    as_percent,
+    as_seconds,
+    interval_to_human,
+)
+from earthkit.data.utils.interval import Interval
 
 LOG = logging.getLogger(__name__)
 
 DOT_EARTHKIT_DATA = os.path.expanduser("~/.earthkit_data")
 
 
+class Validator:
+    def check(self, value):
+        raise NotImplementedError()
+
+    def explain(self):
+        return str()
+
+
+class IntervalValidator(Validator):
+    def __init__(self, interval):
+        self.interval = interval
+
+    def check(self, value):
+        return value in self.interval
+
+    def explain(self):
+        return f"Valid when {interval_to_human(self.interval)}."
+
+
 class Setting:
     def __init__(
         self,
         default,
         description,
         getter=None,
         none_ok=False,
         kind=None,
         docs_default=None,
+        validator=None,
     ):
         self.default = default
         self.description = description
         self.getter = getter
         self.none_ok = none_ok
         self.kind = kind if kind is not None else type(default)
         self.docs_default = docs_default if docs_default is not None else self.default
+        self.validator = validator
 
     def kind(self):
         return type(self.default)
 
     def save(self, name, value, f):
         for n in self.description.split("\n"):
             print(f"# {n.strip()}", file=f)
@@ -54,14 +81,23 @@
         for n in comment.split("\n"):
             if n:
                 print(f"# {n}", file=f)
         if value != self.default:
             print(file=f)
             yaml.dump({name: value}, f, default_flow_style=False)
 
+    @property
+    def docs_description(self):
+        d = self.description
+        if self.validator:
+            t = self.validator.explain()
+            if t:
+                return d + " " + t
+        return d
+
 
 _ = Setting
 
 
 SETTINGS_AND_HELP = {
     "cache-directory": _(
         os.path.join(tempfile.gettempdir(), "earthkit-data-%s" % (getpass.getuser(),)),
@@ -114,14 +150,19 @@
         False,
         "Re-download URLs when the remote version of a cached file as been changed",
     ),
     "use-standalone-mars-client-when-available": _(
         True,
         "Use the standalone mars client when available instead of using the web API.",
     ),
+    "reader-type-check-bytes": _(
+        64,
+        "Number of bytes read from the beginning of a source to identify its type.",
+        validator=IntervalValidator(Interval(8, 4096)),
+    ),
 }
 
 
 NONE = object()
 DEFAULTS = {}
 for k, v in SETTINGS_AND_HELP.items():
     DEFAULTS[k] = v.default
@@ -254,14 +295,21 @@
             value = args[0]
             # Check if value is properly formatted for getter
             getattr(self, getter)(name, value, none_ok)
         else:
             if not isinstance(value, klass):
                 raise TypeError("Setting '%s' must be of type '%s'" % (name, klass))
 
+        validator = SETTINGS_AND_HELP[name].validator
+        if validator is not None:
+            if not validator.check(value):
+                raise ValueError(
+                    f"Settings {name} cannot be set to {value}. {validator.explain()}"
+                )
+
         self._settings[name] = value
         self._changed()
 
     @forward
     def reset(self, name: str = None):
         """Reset setting(s) to default values.
```

### Comparing `earthkit-data-0.1.3/earthkit/data/core/statistics.py` & `earthkit-data-0.2.0/earthkit/data/core/statistics.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/core/temporary.py` & `earthkit-data-0.2.0/earthkit/data/core/temporary.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/core/thread.py` & `earthkit-data-0.2.0/earthkit/data/core/thread.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/data/css/tab.css` & `earthkit-data-0.2.0/earthkit/data/data/css/tab.css`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/decorators.py` & `earthkit-data-0.2.0/earthkit/data/decorators.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/indexing/__init__.py` & `earthkit-data-0.2.0/earthkit/data/indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/indexing/database/__init__.py` & `earthkit-data-0.2.0/earthkit/data/indexing/database/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/indexing/database/json.py` & `earthkit-data-0.2.0/earthkit/data/indexing/database/json.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/indexing/database/sql.py` & `earthkit-data-0.2.0/earthkit/data/indexing/database/sql.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/indexing/database/stdout.py` & `earthkit-data-0.2.0/earthkit/data/indexing/database/stdout.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/input_manager.py` & `earthkit-data-0.2.0/earthkit/data/input_manager.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/mergers/__init__.py` & `earthkit-data-0.2.0/earthkit/data/mergers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/mergers/pandas.py` & `earthkit-data-0.2.0/earthkit/data/mergers/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/mergers/xarray.py` & `earthkit-data-0.2.0/earthkit/data/mergers/xarray.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/mirrors/__init__.py` & `earthkit-data-0.2.0/earthkit/data/mirrors/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/mirrors/directory_mirror.py` & `earthkit-data-0.2.0/earthkit/data/mirrors/directory_mirror.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/__init__.py` & `earthkit-data-0.2.0/earthkit/data/readers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import logging
 import os
 import weakref
 from importlib import import_module
 
 from earthkit.data.core import Base
+from earthkit.data.core.settings import SETTINGS
 from earthkit.data.decorators import locked
 
 LOG = logging.getLogger(__name__)
 
 
 class ReaderMeta(type(Base), type(os.PathLike)):
     pass
@@ -150,34 +151,37 @@
 
     if os.path.isdir(path):
         from .directory import DirectoryReader
 
         return DirectoryReader(source, path).mutate()
     LOG.debug("Reader for %s", path)
 
+    n_bytes = SETTINGS.get("reader-type-check-bytes")
     with open(path, "rb") as f:
-        magic = f.read(8)
+        magic = f.read(n_bytes)
 
     LOG.debug("Looking for a reader for %s (%s)", path, magic)
 
     return _find_reader("reader", source, path, magic)
 
 
 def memory_reader(source, buf):
     """Create a reader for data held in a memory buffer"""
     assert isinstance(buf, (bytes, bytearray)), source
-    magic = buf[:8] if len(buf) > 8 else None
+    n_bytes = SETTINGS.get("reader-type-check-bytes")
+    magic = buf[: min(n_bytes, len(buf) - 1)]
     return _find_reader("memory_reader", source, buf, magic)
 
 
 def stream_reader(source, stream):
     """Create a reader for a stream"""
     magic = None
     if hasattr(stream, "peek") and callable(stream.peek):
         try:
-            magic = stream.peek(8)
-            if len(magic) > 8:
-                magic = magic[:8]
+            n_bytes = SETTINGS.get("reader-type-check-bytes")
+            magic = stream.peek(n_bytes)
+            if len(magic) > n_bytes:
+                magic = magic[:n_bytes]
         except Exception:
             pass
 
     return _find_reader("stream_reader", source, stream, magic)
```

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/archive.py` & `earthkit-data-0.2.0/earthkit/data/readers/archive.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/csv.py` & `earthkit-data-0.2.0/earthkit/data/readers/csv.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/directory.py` & `earthkit-data-0.2.0/earthkit/data/readers/directory.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/__init__.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,33 +7,39 @@
 # nor does it submit to any jurisdiction.
 #
 import logging
 
 LOG = logging.getLogger(__name__)
 
 
-def _match_magic(magic):
-    return magic is None or (len(magic) >= 4 and magic[:4] == b"GRIB")
+def _match_magic(magic, deeper_check):
+    if magic is not None:
+        type_id = b"GRIB"
+        if not deeper_check:
+            return len(magic) >= 4 and magic[:4] == type_id
+        else:
+            return type_id in magic
+    return False
 
 
 def reader(source, path, magic=None, deeper_check=False):
-    if _match_magic(magic):
+    if _match_magic(magic, deeper_check):
         from .reader import GRIBReader
 
         return GRIBReader(source, path)
 
 
 def memory_reader(source, buf, magic=None, deeper_check=False):
-    if _match_magic(magic):
+    if _match_magic(magic, deeper_check):
         from .memory import FieldListInMemory, GribMessageMemoryReader
 
         return FieldListInMemory(source, GribMessageMemoryReader(buf))
 
 
 def stream_reader(source, stream, magic=None, deeper_check=False):
-    if _match_magic(magic):
+    if _match_magic(magic, deeper_check):
         from .memory import FieldListInMemory, GribStreamReader
 
         r = GribStreamReader(stream)
         if source.batch_size == 0:
             r = FieldListInMemory(source, r)
         return r
```

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/codes.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/codes.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,140 +6,114 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import datetime
 import logging
 import os
-import threading
-import time
 
 import eccodes
 import numpy as np
 
 from earthkit.data.core import Base
 from earthkit.data.utils.bbox import BoundingBox
+from earthkit.data.utils.message import (
+    CodesHandle,
+    CodesMessagePositionIndex,
+    CodesReader,
+)
+from earthkit.data.utils.metadata import metadata_argument
+from earthkit.data.utils.projections import Projection
 
 LOG = logging.getLogger(__name__)
 
 _GRIB_NAMESPACES = {"default": None}
 
 for k in ("ls", "geography", "mars", "parameter", "statistics", "time", "vertical"):
     _GRIB_NAMESPACES[k] = k
 
 
 def missing_is_none(x):
     return None if x == 2147483647 else x
 
 
-# This does not belong here, should be in the C library
-def get_messages_positions(path):
-    fd = os.open(path, os.O_RDONLY)
-    try:
-
-        def get(count):
-            buf = os.read(fd, count)
-            assert len(buf) == count
-            return int.from_bytes(
-                buf,
-                byteorder="big",
-                signed=False,
-            )
-
-        offset = 0
-        while True:
-            code = os.read(fd, 4)
-            if len(code) < 4:
-                break
-
-            if code != b"GRIB":
-                offset = os.lseek(fd, offset + 1, os.SEEK_SET)
-                continue
-
-            length = get(3)
-            edition = get(1)
-
-            if edition == 1:
-                if length & 0x800000:
-                    sec1len = get(3)
-                    os.lseek(fd, 4, os.SEEK_CUR)
-                    flags = get(1)
-                    os.lseek(fd, sec1len - 8, os.SEEK_CUR)
-
-                    if flags & (1 << 7):
-                        sec2len = get(3)
-                        os.lseek(fd, sec2len - 3, os.SEEK_CUR)
-
-                    if flags & (1 << 6):
-                        sec3len = get(3)
-                        os.lseek(fd, sec3len - 3, os.SEEK_CUR)
-
-                    sec4len = get(3)
-
-                    if sec4len < 120:
-                        length &= 0x7FFFFF
-                        length *= 120
-                        length -= sec4len
-                        length += 4
-
-            if edition == 2:
-                length = get(8)
-
-            yield offset, length
-            offset = os.lseek(fd, offset + length, os.SEEK_SET)
-
-    finally:
-        os.close(fd)
-
-
-# For some reason, cffi can ge stuck in the GC if that function
-# needs to be called defined for the first time in a GC thread.
-try:
-    _h = eccodes.codes_new_from_samples(
-        "regular_ll_pl_grib1", eccodes.CODES_PRODUCT_GRIB
-    )
-    eccodes.codes_release(_h)
-except Exception:
-    pass
-
-
-class CodesHandle(eccodes.Message):
-    MISSING_VALUE = np.finfo(np.float32).max
-    KEY_TYPES = {"s": str, "l": int, "d": float}
+class GribCodesMessagePositionIndex(CodesMessagePositionIndex):
+    # This does not belong here, should be in the C library
+    def _get_message_positions(self, path):
+        fd = os.open(path, os.O_RDONLY)
+        try:
 
-    def __init__(self, handle, path, offset):
-        super().__init__(handle)
-        self.path = path
-        self.offset = offset
+            def get(count):
+                buf = os.read(fd, count)
+                assert len(buf) == count
+                return int.from_bytes(
+                    buf,
+                    byteorder="big",
+                    signed=False,
+                )
+
+            offset = 0
+            while True:
+                code = os.read(fd, 4)
+                if len(code) < 4:
+                    break
+
+                if code != b"GRIB":
+                    offset = os.lseek(fd, offset + 1, os.SEEK_SET)
+                    continue
+
+                length = get(3)
+                edition = get(1)
+
+                if edition == 1:
+                    if length & 0x800000:
+                        sec1len = get(3)
+                        os.lseek(fd, 4, os.SEEK_CUR)
+                        flags = get(1)
+                        os.lseek(fd, sec1len - 8, os.SEEK_CUR)
+
+                        if flags & (1 << 7):
+                            sec2len = get(3)
+                            os.lseek(fd, sec2len - 3, os.SEEK_CUR)
+
+                        if flags & (1 << 6):
+                            sec3len = get(3)
+                            os.lseek(fd, sec3len - 3, os.SEEK_CUR)
+
+                        sec4len = get(3)
+
+                        if sec4len < 120:
+                            length &= 0x7FFFFF
+                            length *= 120
+                            length -= sec4len
+                            length += 4
+
+                if edition == 2:
+                    length = get(8)
+
+                yield offset, length
+                offset = os.lseek(fd, offset + length, os.SEEK_SET)
 
-    @classmethod
-    def from_sample(cls, name):
-        return cls(
-            eccodes.codes_new_from_samples(name, eccodes.CODES_PRODUCT_GRIB), None, None
-        )
+        finally:
+            os.close(fd)
+
+
+class GribCodesHandle(CodesHandle):
+    PRODUCT_ID = eccodes.CODES_PRODUCT_GRIB
 
     # TODO: just a wrapper around the base class implementation to handle the
     # s,l,d qualifiers. Once these are implemented in the base class this method can
     # be removed. md5GridSection is also handled!
     def get(self, name, ktype=None, **kwargs):
         if name == "values":
             return self.get_values()
         elif name == "md5GridSection":
             return self.get_md5GridSection()
 
-        if ktype is None:
-            name, _, key_type_str = name.partition(":")
-            if key_type_str in CodesHandle.KEY_TYPES:
-                ktype = CodesHandle.KEY_TYPES[key_type_str]
-
-        if "default" in kwargs:
-            return super().get(name, ktype=ktype, **kwargs)
-        else:
-            # this will throw if name is not available
-            return super()._get(name, ktype=ktype)
+        return super().get(name, ktype, **kwargs)
 
     def get_md5GridSection(self):
         # Special case because:
         #
         # 1) eccodes is returning size > 1 for 'md5GridSection'
         # (size = 16 : it is the number of bytes of the value)
         # This is already fixed in eccodes 2.27.1
@@ -160,20 +134,14 @@
 
         save = eccodes.codes_get_long(self._handle, "shapeOfTheEarth")
         eccodes.codes_set_long(self._handle, "shapeOfTheEarth", 255)
         result = eccodes.codes_get_string(self._handle, "md5GridSection")
         eccodes.codes_set_long(self._handle, "shapeOfTheEarth", save)
         return result
 
-    def get_string(self, name):
-        return self.get(name, ktype=str)
-
-    def get_long(self, name):
-        return self.get(name, ktype=int)
-
     def as_namespace(self, namespace, param="shortName"):
         r = {}
         ignore = {
             "distinctLatitudes",
             "distinctLongitudes",
             "distinctLatitudes",
             "latLonValues",
@@ -200,139 +168,31 @@
 
     def get_longitudes(self):
         return self.get("longitudes")
 
     def get_data_points(self):
         return eccodes.codes_grib_get_data(self._handle)
 
-    def clone(self):
-        return CodesHandle(eccodes.codes_clone(self._handle), None, None)
+    # def clone(self):
+    #     return CodesHandle(eccodes.codes_clone(self._handle), None, None)
 
     def set_values(self, values):
         assert self.path is None, "Only cloned handles can have values changed"
         eccodes.codes_set_values(self._handle, values.flatten())
         # This is writing on the GRIB that something has been modified (255=unknown)
         eccodes.codes_set_long(self._handle, "generatingProcessIdentifier", 255)
 
     def set_multiple(self, values):
         assert self.path is None, "Only cloned handles can have values changed"
         eccodes.codes_set_key_vals(self._handle, values)
 
-    def set_long(self, name, value):
-        try:
-            assert self.path is None, "Only cloned handles can have values changed"
-            eccodes.codes_set_long(self._handle, name, value)
-        except Exception as e:
-            LOG.error("Error setting %s=%s", name, value)
-            LOG.exception(e)
-
-    def set_double(self, name, value):
-        try:
-            assert self.path is None, "Only cloned handles can have values changed"
-            eccodes.codes_set_double(self._handle, name, value)
-        except Exception as e:
-            LOG.error("Error setting %s=%s", name, value)
-            LOG.exception(e)
-
-    def set_string(self, name, value):
-        try:
-            assert self.path is None, "Only cloned handles can have values changed"
-            eccodes.codes_set_string(self._handle, name, value)
-        except Exception as e:
-            LOG.error("Error setting %s=%s", name, value)
-            LOG.exception(e)
-
-    def set(self, name, value):
-        try:
-            assert self.path is None, "Only cloned handles can have values changed"
-
-            if isinstance(value, list):
-                return eccodes.codes_set_array(self._handle, name, value)
 
-            return eccodes.codes_set(self._handle, name, value)
-        except Exception as e:
-            LOG.error("Error setting %s=%s", name, value)
-            LOG.exception(e)
-
-    def write(self, f):
-        eccodes.codes_write(self._handle, f)
-
-    def save(self, path):
-        with open(path, "wb") as f:
-            self.write_to(f)
-            self.path = path
-            self.offset = 0
-
-    def read_bytes(self, offset, length):
-        if self.path is not None:
-            with open(self.path, "rb") as f:
-                f.seek(offset)
-                return f.read(length)
-
-
-class ReaderLRUCache(dict):
-    def __init__(self, size):
-        self.readers = dict()
-        self.lock = threading.Lock()
-        self.size = size
-
-    def __getitem__(self, path):
-        key = (
-            path,
-            os.getpid(),
-        )
-        with self.lock:
-            try:
-                return super().__getitem__(key)
-            except KeyError:
-                pass
-
-            c = self[key] = CodesReader(path)
-            while len(self) >= self.size:
-                _, oldest = min((v.last, k) for k, v in self.items())
-                del self[oldest]
-
-            return c
-
-
-cache = ReaderLRUCache(32)  # TODO: Add to config
-
-
-class CodesReader:
-    def __init__(self, path):
-        self.path = path
-        self.lock = threading.Lock()
-        # print("OPEN", self.path)
-        self.file = open(self.path, "rb")
-        self.last = time.time()
-
-    def __del__(self):
-        try:
-            # print("CLOSE", self.path)
-            self.file.close()
-        except Exception:
-            pass
-
-    @classmethod
-    def from_cache(cls, path):
-        return cache[path]
-
-    def at_offset(self, offset):
-        with self.lock:
-            self.last = time.time()
-            self.file.seek(offset, 0)
-            handle = eccodes.codes_new_from_file(
-                self.file,
-                eccodes.CODES_PRODUCT_GRIB,
-            )
-            assert handle is not None
-            return CodesHandle(handle, self.path, offset)
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}({self.path}"
+class GribCodesReader(CodesReader):
+    PRODUCT_ID = eccodes.CODES_PRODUCT_GRIB
+    HANDLE_TYPE = GribCodesHandle
 
 
 class GribField(Base):
     r"""Represents a GRIB message in a GRIB file.
 
     Parameters
     ----------
@@ -351,15 +211,15 @@
         self._handle = None
 
     @property
     def handle(self):
         r""":class:`CodesHandle`: Gets an object providing access to the low level GRIB message structure."""
         if self._handle is None:
             assert self._offset is not None
-            self._handle = CodesReader.from_cache(self.path).at_offset(self._offset)
+            self._handle = GribCodesReader.from_cache(self.path).at_offset(self._offset)
         return self._handle
 
     @property
     def values(self):
         r"""ndarray: Gets the values stored in the GRIB field as a 1D ndarray."""
         return self.handle.get_values()
 
@@ -452,14 +312,43 @@
         if not flatten:
             values = self.values.reshape(self.shape)
         if dtype is not None:
             values = values.astype(dtype)
         return values
 
     def to_points(self, flatten=False):
+        r"""Returns the geographical coordinates in the data's original
+        Coordinate Reference System (CRS).
+
+        Parameters
+        ----------
+        flatten: bool
+            When it is True 1D ndarrays are returned. Otherwise ndarrays with the field's
+            :obj:`shape` are returned.
+
+        Returns
+        -------
+        dict
+            Dictionary with items "x" and "y", containing the ndarrays of the x and
+            y coordinates, respectively.
+
+        Raises
+        ------
+        ValueError
+            When the coordinates in the data's original CRS are not available.
+
+        """
+        grid_type = self.metadata("gridType", default=None)
+        if grid_type in ["regular_ll", "reduced_gg", "regular_gg"]:
+            lon, lat = self.data(("lon", "lat"), flatten=flatten)
+            return dict(x=lon, y=lat)
+        else:
+            raise ValueError("grid_type={grid_type} is not supported in to_points()")
+
+    def to_latlon(self, flatten=False):
         r"""Returns the latitudes/longitudes of all the gridpoints in the field.
 
         Parameters
         ----------
         flatten: bool
             When it is True 1D ndarrays are returned. Otherwise ndarrays with the field's
             :obj:`shape` are returned.
@@ -468,15 +357,15 @@
         -------
         dict
             Dictionary with items "lat" and "lon", containing the ndarrays of the latitudes and
             longitudes, respectively.
 
         """
         lon, lat = self.data(("lon", "lat"), flatten=flatten)
-        return dict(lon=lon, lat=lat)
+        return dict(lat=lat, lon=lon)
 
     def __repr__(self):
         return "GribField(%s,%s,%s,%s,%s,%s)" % (
             self.handle.get("shortName", default=None),
             self.handle.get("levelist", default=None),
             self.handle.get("date", default=None),
             self.handle.get("time", default=None),
@@ -516,29 +405,53 @@
             time % 100,
         )
 
     def _valid_datetime(self):
         step = self.handle.get("endStep", default=None)
         return self._base_datetime() + datetime.timedelta(hours=step)
 
-    def proj_string(self):
-        return self.proj_target_string()
+    def projection(self):
+        r"""Returns information about the projection.
 
-    def proj_source_string(self):
-        return self.handle.get("projSourceString", default=None)
+        Returns
+        -------
+        :obj:`Projection`
 
-    def proj_target_string(self):
-        return self.handle.get("projTargetString", default=None)
+        Examples
+        --------
+        >>> import earthkit.data
+        >>> ds = earthkit.data.from_source("file", "docs/examples/test.grib")
+        >>> ds.projection()
+        <Projected CRS: +proj=eqc +ellps=WGS84 +a=6378137.0 +lon_0=0.0 +to ...>
+        Name: unknown
+        Axis Info [cartesian]:
+        - E[east]: Easting (unknown)
+        - N[north]: Northing (unknown)
+        - h[up]: Ellipsoidal height (metre)
+        Area of Use:
+        - undefined
+        Coordinate Operation:
+        - name: unknown
+        - method: Equidistant Cylindrical
+        Datum: Unknown based on WGS 84 ellipsoid
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+        >>> ds.projection().to_proj_string()
+        '+proj=eqc +ellps=WGS84 +a=6378137.0 +lon_0=0.0 +to_meter=111319.4907932736 +no_defs +type=crs'
+        """
+        return Projection.from_proj_string(
+            self.handle.get("projTargetString", default=None)
+        )
 
     def bounding_box(self):
         r"""Returns the bounding box of the field.
 
         Returns
         -------
-        :class:`BoundingBox`
+        :obj:`BoundingBox <data.utils.bbox.BoundingBox>`
         """
         return BoundingBox(
             north=self.handle.get("latitudeOfFirstGridPointInDegrees", default=None),
             south=self.handle.get("latitudeOfLastGridPointInDegrees", default=None),
             west=self.handle.get("longitudeOfFirstGridPointInDegrees", default=None),
             east=self.handle.get("longitudeOfLastGridPointInDegrees", default=None),
         )
@@ -553,60 +466,14 @@
         """Private, for testing only"""
         # paramId is renamed as param to get rid of the
         # additional '.128' (in earthkit/data/scripts/grib.py)
         if name == "param":
             name = "paramId"
         return self.handle.get(name)
 
-    # TODO: move it into core or util
-    @staticmethod
-    def _parse_metadata_args(*args, namespace=None, astype=None):
-        key = []
-        key_arg_type = None
-        if len(args) == 1 and isinstance(args[0], str):
-            key_arg_type = str
-        elif len(args) >= 1:
-            key_arg_type = tuple
-            for k in args:
-                if isinstance(k, list):
-                    key_arg_type = list
-
-        for k in args:
-            if isinstance(k, str):
-                key.append(k)
-            elif isinstance(k, (list, tuple)):
-                key.extend(k)
-            else:
-                raise ValueError(f"metadata: invalid key argument={k}")
-
-        if key:
-            if namespace is not None:
-                if not isinstance(namespace, str):
-                    raise ValueError(
-                        f"metadata: namespace={namespace} must be a str when key specified"
-                    )
-
-            if isinstance(astype, (list, tuple)):
-                if len(astype) != len(key):
-                    if len(astype) == 1:
-                        astype = [astype[0]] * len(key)
-                    else:
-                        raise ValueError(
-                            "metadata: astype must have the same number of items as key"
-                        )
-            else:
-                astype = [astype] * len(key)
-
-        if namespace is None:
-            namespace = []
-        elif isinstance(namespace, str):
-            namespace = [namespace]
-
-        return (key, namespace, astype, key_arg_type)
-
     def metadata(self, *keys, namespace=None, astype=None, **kwargs):
         r"""Returns metadata values from the GRIB message.
 
         Parameters
         ----------
         *keys: tuple
             Positional arguments specifying metadata keys. Only ecCodes GRIB keys can be used
@@ -632,15 +499,15 @@
                 :obj:`metadata` will raise KeyError.
 
         Returns
         -------
         single value, :obj:`list`, :obj:`tuple` or :obj:`dict`
             - when ``keys`` is not empty:
                 - single value when ``keys`` is a str
-                - otherwise the same type as that of ``keys`` (:obj:`lits` or :obj:`tuple`)
+                - otherwise the same type as that of ``keys`` (:obj:`list` or :obj:`tuple`)
             - when ``keys`` is empty:
                 - when ``namespace`` is :obj:`str` returns a :obj:`dict` with the keys and values
                   in that namespace
                 - otherwise returns a :obj:`dict` with one item per namespace (dict of dict)
 
         Raises
         ------
@@ -695,15 +562,15 @@
         def _key_name(key):
             if key == "param":
                 key = "shortName"
             elif key == "_param_id":
                 key = "paramId"
             return key
 
-        key, namespace, astype, key_arg_type = self._parse_metadata_args(
+        key, namespace, astype, key_arg_type = metadata_argument(
             *keys, namespace=namespace, astype=astype
         )
 
         assert isinstance(key, list)
         assert isinstance(namespace, (list, tuple))
 
         if key:
@@ -736,59 +603,51 @@
                 return r
 
     def __getitem__(self, key):
         """Returns the value of the metadata ``key``."""
         return self.metadata(key)
 
     def dump(self, namespace=None, **kwargs):
-        r"""Generates dump with all the metadata keys belonging to ``namespace``.
+        r"""Generates dump with all the metadata keys belonging to ``namespace``
+        offering a tabbed interface in a Jupyter notebook.
 
         Parameters
         ----------
         namespace: :obj:`str`, :obj:`list` or :obj:`tuple`
             The namespace to dump. Any :xref:`eccodes_namespace` can be used here.
             :obj:`dump` also defines the "default" namespace, which contains all the GRIB keys
             that ecCodes can access without specifying a namespace.
             When ``namespace`` is None all the available namespaces will be used.
         **kwargs: dict, optional
-            Other keyword arguments:
-
-            print: bool, optional
-                Enables printing the dump to the standard output when not in a Jupyter notebook.
-                Default: False
-            html: bool, optional
-                Enables generating HTML based content in a Jupyter notebook. Default: True
-
+            Other keyword arguments used for testing only
 
         Returns
         -------
-        html or dict
-            - When in Jupyter notebook returns HTML code providing a tabbed interface to browse the
-              dump content. When ``html`` is False a dict is returned.
-            - dict otherwise. When ``print`` is True also prints the dict to stdout.
-
+        NamespaceDump
+            Dict-like object with one item per namespace. In a Jupyter notebook represented
+            as a tabbed interface to browse the dump contents.
 
         Examples
         --------
         :ref:`/examples/grib_metadata.ipynb`
 
         """
-        from earthkit.data.utils.summary import format_info
+        from earthkit.data.utils.summary import format_namespace_dump
 
         namespace = _GRIB_NAMESPACES.keys() if namespace is None else [namespace]
         r = [
             {
                 "title": ns,
                 "data": self.handle.as_namespace(_GRIB_NAMESPACES.get(ns)),
                 "tooltip": f"Keys in the ecCodes {ns} namespace",
             }
             for ns in namespace
         ]
 
-        return format_info(
+        return format_namespace_dump(
             r, selected="parameter", details=self.__class__.__name__, **kwargs
         )
 
     def write(self, f):
         r"""Writes the message to a file object.
 
         Parameters
```

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/fieldlist.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/fieldlist.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import json
 import logging
 from collections import defaultdict
 
 from earthkit.data.core.caching import auxiliary_cache_file
 from earthkit.data.core.index import ScaledIndex
-from earthkit.data.utils.bbox import BoundingBox
+from earthkit.data.decorators import cached_method
 
 from .pandas import PandasMixIn
 from .xarray import XarrayMixIn
 
 LOG = logging.getLogger(__name__)
 
 GRIB_LS_KEYS = [
@@ -256,15 +256,15 @@
 
         """
         result = []
         for s in self:
             result.append(s.metadata(*args, **kwargs))
         return result
 
-    def ls(self, n=None, keys=None, extra_keys=None, namespace=None, **kwargs):
+    def ls(self, n=None, keys=None, extra_keys=None, namespace=None):
         r"""Generates a list like summary of fieldlist using a set of metadata keys.
 
         Parameters
         ----------
         n: int, None
             The number of :obj:`GribField <data.readers.grib.codes.GribField>`\ s to be
             listed. None means all the messages, ``n > 0`` means fields from the front, while
@@ -275,27 +275,19 @@
             "number", "gridType". To specify a column title for each key in the output use a dict.
         extra_keys: list of str, dict, None
             List of additional keys to ``keys``. To specify a column title for each key in the output
             use a dict.
         namespace: str, None
             The :xref:`eccodes_namespace` to choose the ``keys`` from. When it is set ``keys`` and
             ``extra_keys`` are omitted.
-        **kwargs: dict, optional
-            Other keyword arguments:
-
-            print: bool, optional
-                Enables printing the DataFrame to the standard output when not in a Jupyter notebook.
-                Default: False
 
         Returns
         -------
         Pandas DataFrame
             DataFrame with one row per :obj:`GribField <data.readers.grib.codes.GribField>`.
-            If not in a Jupyter notebook and ``print`` is True the DataFrame is printed to
-            the standard output
 
         """
         from earthkit.data.utils.summary import ls
 
         def _proc(keys, n):
             num = len(self)
             pos = slice(0, num)
@@ -312,15 +304,15 @@
                         v.update(f._attributes(keys))
                     yield (v)
             else:
                 for i in pos_range:
                     yield (self[i]._attributes(keys))
 
         _keys = GRIB_LS_KEYS if namespace is None else dict(namespace=namespace)
-        return ls(_proc, _keys, n=n, keys=keys, extra_keys=extra_keys, **kwargs)
+        return ls(_proc, _keys, n=n, keys=keys, extra_keys=extra_keys)
 
     def head(self, n=5, **kwargs):
         r"""Generates a list like summary of the first ``n``
         :obj:`GribField <data.readers.grib.codes.GribField>`\ s using a set of metadata keys.
         Same as calling :obj:`ls` with ``n``.
 
         Parameters
@@ -419,24 +411,153 @@
         valid = set()
         for s in self:
             d = s.datetime()
             base.add(d["base_time"])
             valid.add(d["valid_time"])
         return {"base_time": sorted(base), "valid_time": sorted(valid)}
 
+    @cached_method
+    def _is_shared_grid(self):
+        if len(self) > 0:
+            for i, f in enumerate(self):
+                if i == 0:
+                    grid = f.metadata("md5GridSection")
+                elif f.metadata("md5GridSection") != grid:
+                    return False
+            return True
+        return False
+
+    def to_points(self, **kwargs):
+        r"""Returns the geographical coordinates shared by all the fields in
+        the data's original Coordinate Reference System (CRS).
+
+        Parameters
+        ----------
+        **kwargs: dict, optional
+            Keyword arguments passed to
+            :obj:`GribField.to_points() <data.readers.grib.codes.GribField.to_points>`
+
+        Returns
+        -------
+        dict
+            Dictionary with items "x" and "y", containing the ndarrays of the x and
+            y coordinates, respectively.
+
+        Raises
+        ------
+        ValueError
+            When not all the fields have the same grid geometry.
+        """
+        if self._is_shared_grid():
+            return self[0].to_points(**kwargs)
+        elif len(self) == 0:
+            return dict(x=None, y=None)
+        else:
+            raise ValueError("Fields do not have the same grid geometry")
+
+    def to_latlon(self, **kwargs):
+        r"""Returns the latitudes/longitudes shared by all the fields.
+
+        Parameters
+        ----------
+        **kwargs: dict, optional
+            Keyword arguments passed to
+            :obj:`GribField.to_latlon() <data.readers.grib.codes.GribField.to_latlon>`
+
+        Returns
+        -------
+        dict
+            Dictionary with items "lat" and "lon", containing the ndarrays of the latitudes and
+            longitudes, respectively.
+
+        Raises
+        ------
+        ValueError
+            When not all the fields have the same grid geometry
+
+        Examples
+        --------
+        >>> import earthkit.data
+        >>> ds = earthkit.data.from_source("file", "docs/examples/test.grib")
+        >>> for f in ds:
+        ...     print(f.shape)
+        ...
+        (11, 19)
+        (11, 19)
+        >>> r = ds.to_latlon()
+        >>> for k, v in r.items():
+        ...     print(f"{k}: shape={v.shape}")
+        ...
+        lat: shape=(11, 19)
+        lon: shape=(11, 19)
+        >>> r["lon"][:2]
+        array([[-27., -23., -19., -15., -11.,  -7.,  -3.,   1.,   5.,   9.,  13.,
+         17.,  21.,  25.,  29.,  33.,  37.,  41.,  45.],
+        [-27., -23., -19., -15., -11.,  -7.,  -3.,   1.,   5.,   9.,  13.,
+         17.,  21.,  25.,  29.,  33.,  37.,  41.,  45.]])
+
+        """
+        if self._is_shared_grid():
+            return self[0].to_latlon(**kwargs)
+        elif len(self) == 0:
+            return dict(lat=None, lon=None)
+        else:
+            raise ValueError("Fields do not have the same grid geometry")
+
+    def projection(self):
+        r"""Returns the projection information shared by all the fields.
+
+        Returns
+        -------
+        :obj:`Projection`
+
+        Raises
+        ------
+        ValueError
+            When not all the fields have the same grid geometry
+
+        Examples
+        --------
+        >>> import earthkit.data
+        >>> ds = earthkit.data.from_source("file", "docs/examples/test.grib")
+        >>> ds.projection()
+        <Projected CRS: +proj=eqc +ellps=WGS84 +a=6378137.0 +lon_0=0.0 +to ...>
+        Name: unknown
+        Axis Info [cartesian]:
+        - E[east]: Easting (unknown)
+        - N[north]: Northing (unknown)
+        - h[up]: Ellipsoidal height (metre)
+        Area of Use:
+        - undefined
+        Coordinate Operation:
+        - name: unknown
+        - method: Equidistant Cylindrical
+        Datum: Unknown based on WGS 84 ellipsoid
+        - Ellipsoid: WGS 84
+        - Prime Meridian: Greenwich
+        >>> ds.projection().to_proj_string()
+        '+proj=eqc +ellps=WGS84 +a=6378137.0 +lon_0=0.0 +to_meter=111319.4907932736 +no_defs +type=crs'
+        """
+        if self._is_shared_grid():
+            return self[0].projection()
+        elif len(self) == 0:
+            return None
+        else:
+            raise ValueError("Fields do not have the same grid geometry")
+
     def bounding_box(self):
         r"""Returns the bounding box for each field.
 
         Returns
         -------
         list
-            List with one :obj:`BoundingBox` per
+            List with one :obj:`BoundingBox <data.utils.bbox.BoundingBox>` per
             :obj:`GribField <data.readers.grib.codes.GribField>`
         """
-        return BoundingBox.multi_merge([s.bounding_box() for s in self])
+        return [s.bounding_box() for s in self]
 
     def statistics(self):
         import numpy as np
 
         if self._statistics is not None:
             return self._statistics
```

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/index/__init__.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/index/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/index/db.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/index/db.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/index/json.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/index/json.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/index/sql.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/index/sql.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/memory.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/memory.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,57 +3,100 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-
 import logging
 
 import eccodes
 
 from earthkit.data.readers import Reader
-from earthkit.data.readers.grib.codes import CodesHandle, GribField
+from earthkit.data.readers.grib.codes import GribCodesHandle, GribField
 from earthkit.data.readers.grib.index import FieldList
 
 LOG = logging.getLogger(__name__)
 
 
 class GribMemoryReader(Reader):
+    def __init__(self):
+        self._peeked = None
+
     def __iter__(self):
         return self
 
     def __next__(self):
+        if self._peeked is not None:
+            msg = self._peeked
+            self._peeked = None
+            return msg
         handle = self._next_handle()
+        msg = self._message_from_handle(handle)
         if handle is not None:
-            return GribFieldInMemory(CodesHandle(handle, None, None))
+            return msg
         raise StopIteration
 
     def _next_handle(self):
         raise NotImplementedError
 
+    def _message_from_handle(self, handle):
+        if handle is not None:
+            return GribFieldInMemory(GribCodesHandle(handle, None, None))
+
+    def peek(self):
+        """Returns the next available message without consuming it"""
+        if self._peeked is None:
+            handle = self._next_handle()
+            self._peeked = self._message_from_handle(handle)
+        return self._peeked
+
     def read_batch(self, n):
         fields = [self.__next__() for _ in range(n)]
         return FieldListInMemory.from_fields(fields)
 
+    def read_group(self, group):
+        assert isinstance(group, list)
+
+        fields = []
+        current_group = {}
+        while True:
+            f = self.peek()
+            if f is not None:
+                group_md = f._attributes(group)
+                if not current_group:
+                    current_group = group_md
+                if current_group == group_md:
+                    fields.append(f)
+                    self.__next__()
+                else:
+                    break
+            elif fields:
+                break
+            else:
+                raise StopIteration
+
+        return FieldListInMemory.from_fields(fields)
+
 
 class GribFileMemoryReader(GribMemoryReader):
     def __init__(self, path):
+        super().__init__()
         self.fp = open(path, "rb")
 
     def __del__(self):
         self.fp.close()
 
     def _next_handle(self):
         return eccodes.codes_new_from_file(self.fp, eccodes.CODES_PRODUCT_GRIB)
 
 
 class GribMessageMemoryReader(GribMemoryReader):
     def __init__(self, buf):
+        super().__init__()
         self.buf = buf
 
     def __del__(self):
         self.buf = None
 
     def _next_handle(self):
         if self.buf is None:
@@ -67,14 +110,15 @@
     """Wrapper around eccodes.Streamreader. The problem is that when iterating via
     the StreamReader it returns an eccodes.GRIBMessage that releases the handle when deleted.
     However, the handle has to be managed by earthkit-data so we access it directly
     using _next_handle
     """
 
     def __init__(self, stream):
+        super().__init__()
         self._stream = eccodes.StreamReader(stream)
 
     def _next_handle(self):
         return self._stream._next_handle()
 
     def mutate(self):
         return self
```

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/output.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             param = metadata.pop("param")
             try:
                 metadata["paramId"] = int(param)
             except ValueError:
                 metadata["shortName"] = param
 
     def handle_from_metadata(self, values, metadata, compulsory):
-        from .codes import CodesHandle  # Lazy loading of eccodes
+        from .codes import GribCodesHandle  # Lazy loading of eccodes
 
         if len(values.shape) == 1:
             sample = self._gg_field(values, metadata)
         elif len(values.shape) == 2:
             sample = self._ll_field(values, metadata)
         else:
             raise ValueError(
@@ -223,16 +223,16 @@
             if not isinstance(check, tuple):
                 check = [check]
 
             if not any(c in metadata for c in check):
                 choices = list_to_human([f"'{c}'" for c in check], "or")
                 raise ValueError(f"Please provide a value for {choices}.")
 
-        LOG.debug("CodesHandle.from_sample(%s)", sample)
-        return CodesHandle.from_sample(sample)
+        LOG.debug("GribCodesHandle.from_sample(%s)", sample)
+        return GribCodesHandle.from_sample(sample)
 
     def _ll_field(self, values, metadata):
         Nj, Ni = values.shape
         metadata["Nj"] = Nj
         metadata["Ni"] = Ni
 
         # We assume the scanning mode north->south, west->east
```

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/pandas.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/parsing.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     path,
     with_statistics=False,
     with_valid_date=True,
     with_parameter_level=True,
 ):
     import eccodes
 
-    from earthkit.data.readers.grib.codes import CodesHandle
+    from earthkit.data.readers.grib.codes import GribCodesHandle
 
     post_process_mars = []
     if with_valid_date:
         post_process_mars.append(post_process_valid_date)
     if with_parameter_level:
         post_process_mars.append(post_process_parameter_level)
     if with_statistics:
@@ -108,15 +108,15 @@
     )
 
     with open(path, "rb") as f:
         old_position = f.tell()
         h = eccodes.codes_grib_new_from_file(f)
 
         while h:
-            yield parse_field(CodesHandle(h, path, offset=old_position))
+            yield parse_field(GribCodesHandle(h, path, offset=old_position))
 
             position = f.tell()
             pbar.update(position - old_position)
             old_position = position
             h = eccodes.codes_grib_new_from_file(f)
 
     pbar.close()
```

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/reader.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/grib/xarray.py` & `earthkit-data-0.2.0/earthkit/data/readers/grib/xarray.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/netcdf.py` & `earthkit-data-0.2.0/earthkit/data/readers/netcdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import numpy as np
 import xarray as xr
 
 from earthkit.data.core import Base
 from earthkit.data.utils.bbox import BoundingBox
 from earthkit.data.utils.dates import to_datetime
+from earthkit.data.utils.projections import Projection
 
 from . import Reader
 
 GEOGRAPHIC_COORDS = {
     "x": ["x", "projection_x_coordinate", "lon", "longitude"],
     "y": ["y", "projection_y_coordinate", "lat", "latitude"],
 }
@@ -207,14 +208,26 @@
             )
 
         # Simply assume a WGS 84 target projection for CF-compliant netCDF
         proj_target = "+proj=eqc +datum=WGS84 +units=m +no_defs"
 
         return proj_source, proj_target
 
+    def _grid_mapping(self):
+        if "grid_mapping" in self._da.attrs:
+            grid_mapping = self._ds[self._da.attrs["grid_mapping"]]
+        else:
+            raise AttributeError(
+                "no CF-compliant 'grid_mapping' detected in netCDF attributes"
+            )
+        return grid_mapping
+
+    def projection(self):
+        return Projection.from_cf_grid_mapping(**self._grid_mapping().attrs)
+
     def to_points(self, flatten=False):
         points = dict()
         for axis in ("x", "y"):
             for coord in self._da.coords:
                 if self._da.coords[coord].attrs.get("axis", "").lower() == axis:
                     break
             else:
@@ -380,13 +393,20 @@
         )
 
     def datetime(self):
         r = sorted({to_datetime(s.time) for s in self.get_fields()})
         return {"base_time": r, "valid_time": r}
 
     def bounding_box(self):
-        return BoundingBox.multi_merge([s.bounding_box() for s in self.get_fields()])
+        return [s.bounding_box() for s in self.get_fields()]
+
+
+def _match_magic(magic, deeper_check):
+    if magic is not None:
+        type_id = (b"\x89HDF", b"CDF\x01", b"CDF\x02")
+        return len(magic) >= 4 and magic[:4] in type_id
+    return False
 
 
 def reader(source, path, magic=None, deeper_check=False):
-    if magic is None or magic[:4] in (b"\x89HDF", b"CDF\x01", b"CDF\x02"):
+    if _match_magic(magic, deeper_check):
         return NetCDFReader(source, path)
```

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/numpy.py` & `earthkit-data-0.2.0/earthkit/data/readers/numpy.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/odb.py` & `earthkit-data-0.2.0/earthkit/data/readers/odb.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,10 +23,20 @@
 
             LOG.debug("Using pure Python odc decoder.")
 
         odc_read_odb_kwargs = kwargs.get("odc_read_odb_kwargs", {})
         return odc.read_odb(self.path, single=True, **odc_read_odb_kwargs)
 
 
+def _match_magic(magic, deeper_check):
+    if magic is not None:
+        type_id = b"\xff\xffODA"
+        if not deeper_check:
+            return len(magic) >= 5 and magic[:5] == type_id
+        else:
+            return type_id in magic
+    return False
+
+
 def reader(source, path, magic=None, deeper_check=False):
-    if magic is None or magic[:5] == b"\xff\xffODA":
+    if _match_magic(magic, deeper_check):
         return ODBReader(source, path)
```

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/tar.py` & `earthkit-data-0.2.0/earthkit/data/readers/tar.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/text.py` & `earthkit-data-0.2.0/earthkit/data/readers/text.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/unknown.py` & `earthkit-data-0.2.0/earthkit/data/readers/unknown.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/readers/zip.py` & `earthkit-data-0.2.0/earthkit/data/readers/zip.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/__init__.py` & `earthkit-data-0.2.0/earthkit/data/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/cds.py` & `earthkit-data-0.2.0/earthkit/data/sources/cds.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/dummy_source.py` & `earthkit-data-0.2.0/earthkit/data/sources/dummy_source.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/ecmwf_api.py` & `earthkit-data-0.2.0/earthkit/data/sources/ecmwf_api.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/empty.py` & `earthkit-data-0.2.0/earthkit/data/sources/empty.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/fdb.py` & `earthkit-data-0.2.0/earthkit/data/sources/fdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 LOG = logging.getLogger(__name__)
 
 
 class FDBSource(Source):
     def __init__(self, *args, stream=True, **kwargs):
         super().__init__()
 
-        self._stream_kwargs = kwargs.pop("batch_size", 1)
+        self._stream_kwargs = dict()
+        for k in ["group_by", "batch_size"]:
+            if k in kwargs:
+                self._stream_kwargs[k] = kwargs.pop(k)
+
         self.stream = stream
 
         self.request = {}
         for a in args:
             self.request.update(a)
         self.request.update(kwargs)
 
@@ -39,15 +43,15 @@
                 """No FDB_HOME environment variable was set! Please define it to make the FDB access work. See:
                 https://fields-database.readthedocs.io for details about FDB."""
             )
 
     def mutate(self):
         if self.stream:
             stream = pyfdb.retrieve(self.request)
-            return StreamSource(stream, self._stream_kwargs)
+            return StreamSource(stream, **self._stream_kwargs)
         else:
             return FDBFileSource(self.request)
 
 
 class FDBFileSource(FileSource):
     def __init__(self, request):
         super().__init__()
```

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/file.py` & `earthkit-data-0.2.0/earthkit/data/sources/file.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/file_indexed.py` & `earthkit-data-0.2.0/earthkit/data/sources/file_indexed.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/file_pattern.py` & `earthkit-data-0.2.0/earthkit/data/sources/file_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/indexed.py` & `earthkit-data-0.2.0/earthkit/data/sources/indexed.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/list_of_dicts.py` & `earthkit-data-0.2.0/earthkit/data/sources/list_of_dicts.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/mars.py` & `earthkit-data-0.2.0/earthkit/data/sources/mars.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/memory.py` & `earthkit-data-0.2.0/earthkit/data/sources/memory.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/multi.py` & `earthkit-data-0.2.0/earthkit/data/sources/multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,11 +134,11 @@
     def datetime(self, **kwargs):
         result = dict()
         for s in self.sources:
             result.update(s.datetime(**kwargs))
         return {k: sorted(v) for k, v in result.items()}
 
     def bounding_box(self):
-        return BoundingBox.multi_merge([s.bounding_box() for s in self.sources])
+        return BoundingBox.union([s.bounding_box() for s in self.sources])
 
 
 source = MultiSource
```

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/multi_url.py` & `earthkit-data-0.2.0/earthkit/data/sources/multi_url.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/prompt.py` & `earthkit-data-0.2.0/earthkit/data/sources/prompt.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/stream.py` & `earthkit-data-0.2.0/earthkit/data/utils/lazy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-# (C) Copyright 2020 ECMWF.
+# (C) Copyright 2021 ECMWF.
 #
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
-
 import logging
 
-from earthkit.data.readers import stream_reader
-from earthkit.data.sources.memory import MemoryBaseSource
-
-from . import Source
+from earthkit.data import from_source
 
 LOG = logging.getLogger(__name__)
 
 
-class StreamMemorySource(MemoryBaseSource):
-    def __init__(self, reader, **kwargs):
-        super().__init__(**kwargs)
-        self._reader = reader
-
-    def __iter__(self):
-        return iter(self._reader)
+class LazySourceError(Exception):
+    pass
 
 
-class StreamSource(Source):
-    def __init__(self, stream, batch_size=1, **kwargs):
-        super().__init__(**kwargs)
-        self._stream = stream
-        self._reader_ = None
-        self._batch_size = batch_size
+class LazySource:
+    def __init__(self, name, *args, **kwargs):
+        self.name = name
+        self.args = args
+        self.kwargs = kwargs
+        self._source = None
+        self._exception = None
 
     @property
-    def batch_size(self):
-        return self._batch_size
+    def source(self):
+        if self._source is None:
+            try:
+                self._source = from_source(
+                    self.name,
+                    lazily=False,
+                    *self.args,
+                    **self.kwargs,
+                )
+            # except AttributeError as e:
+            #     self._exception = e
+            #     raise LazySource(e)
+            except Exception as e:
+                self._exception = e
+                raise
 
-    def mutate(self):
-        if self.batch_size == 0:
-            source = StreamMemorySource(self._reader)
-            return source
-        else:
-            return self
+        return self._source
 
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        assert self.batch_size > 0
-        if self.batch_size == 1:
-            return self._reader.__next__()
-        else:
-            return self._reader.read_batch(self.batch_size)
+    def __getitem__(self, name):
+        return self.source[name]
 
-    @property
-    def _reader(self):
-        if self._reader_ is None:
-            self._reader_ = stream_reader(self, self._stream)
-            self._stream = None
-        return self._reader_
+    def __iter__(self):
+        return iter(self.source)
 
+    def __len__(self):
+        return len(self.source)
 
-source = StreamSource
+    def __getattr__(self, name):
+        if self._exception is not None:
+            raise self._exception(name)
+        assert name != "source"
+        return getattr(self.source, name)
+
+    def __call__(self, **kwargs):
+        assert self._source is None
+        self.kwargs.update(kwargs)
+        return self.source
```

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/url.py` & `earthkit-data-0.2.0/earthkit/data/sources/url.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/url_pattern.py` & `earthkit-data-0.2.0/earthkit/data/sources/url_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/virtual.py` & `earthkit-data-0.2.0/earthkit/data/sources/virtual.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sources/virtual_directory.py` & `earthkit-data-0.2.0/earthkit/data/sources/virtual_directory.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sphinxext/generate_settings_rst.py` & `earthkit-data-0.2.0/earthkit/data/sphinxext/generate_settings_rst.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,13 +51,13 @@
     print()
     for k, v in sorted(SETTINGS_AND_HELP.items()):
         if len(args) and not any(re.match(arg, k) for arg in args):
             continue
 
         print("   * - ", k.replace("-", "\u2011"))  # Non-breaking hyphen
         print("     - ", repr(tidy(v.docs_default)).replace("-", "\u2011"))
-        print("     - ", v.description)
+        print("     - ", v.docs_description)
     print()
 
 
 if __name__ == "__main__":
     execute()
```

### Comparing `earthkit-data-0.1.3/earthkit/data/sphinxext/module_output.py` & `earthkit-data-0.2.0/earthkit/data/sphinxext/module_output.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/sphinxext/xref.py` & `earthkit-data-0.2.0/earthkit/data/sphinxext/xref.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/testing.py` & `earthkit-data-0.2.0/earthkit/data/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,20 @@
             return False
     return True
 
 
 NO_MARS = not os.path.exists(os.path.expanduser("~/.ecmwfapirc"))
 NO_CDS = not os.path.exists(os.path.expanduser("~/.cdsapirc"))
 IN_GITHUB = os.environ.get("GITHUB_WORKFLOW") is not None
-NO_EOD = not os.path.exists(os.path.expanduser("~/.ecmwf-open-data"))
+try:
+    import ecmwf.opendata  # noqa
+
+    NO_EOD = False
+except Exception:
+    NO_EOD = True
 
 
 def MISSING(*modules):
     return not modules_installed(*modules)
 
 
 UNSAFE_SAMPLES_URL = "https://github.com/jwilk/traversal-archives/releases/download/0"
```

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/__init__.py` & `earthkit-data-0.2.0/earthkit/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/availability.py` & `earthkit-data-0.2.0/earthkit/data/utils/availability.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/bbox.py` & `earthkit-data-0.2.0/earthkit/data/utils/bbox.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,14 +17,28 @@
     while lon >= minimum + 360:
         lon -= 360
 
     return lon
 
 
 class BoundingBox:
+    r"""Represents a geographic bounding box.
+
+    Parameters
+    ----------
+    north: number
+        Northern latitude (degrees)
+    west: number
+        Western longitude (degrees)
+    south: number
+        Southern latitude (degrees)
+    east: number
+        Eastern longitude (degrees)
+    """
+
     def __init__(self, *, north, west, south, east):
         # Convert to float as these values may come from Numpy
         self.north = min(float(north), 90.0)
         self.south = max(float(south), -90.0)
 
         self.is_periodic_west_east = (east - west) == 360
         self.west = _normalize(float(west), -180)  # Or 0?
@@ -61,22 +75,41 @@
         if self.__class__ is not other.__class__:
             return False
 
         return self.as_tuple() == other.as_tuple()
 
     @property
     def width(self):
+        """number: Returns the East-West size (degrees)"""
         return self.east - self.west
 
     @property
     def height(self):
+        """number: Returns the North-South size (degrees)"""
         return self.north - self.south
 
     @classmethod
-    def multi_merge(cls, bboxes):
+    def union(cls, bboxes):
+        """Generates the union of a list of :obj:`BoundingBox` objects.
+
+        Parameters
+        ----------
+        bboxes: list
+            Input  :obj:`BoundingBox` objects.
+
+        Returns
+        -------
+        :obj:`BoundingBox`
+            Union of input objects.
+
+        See Also
+        --------
+        :obj:`union_with`
+
+        """
         north = max(z.north for z in bboxes)
         south = min(z.south for z in bboxes)
 
         first = bboxes[0]
 
         origin = first.east % 360
         full = BoundingBox(
@@ -137,18 +170,48 @@
         return BoundingBox(
             north=north,
             west=origin + west,
             south=south,
             east=origin + east,
         )
 
-    def merge(self, other):
-        return self.multi_merge([self, other])
+    def union_with(self, other):
+        """Generates the union of the current object and ``other``.
+
+        Parameters
+        ----------
+        other: :obj:`BoundingBox`
+            The object to make the union with.
+
+        Returns
+        -------
+        :obj:`BoundingBox`
+            New object containing the union.
+
+        See Also
+        --------
+        :obj:`union`
+
+        """
+        return self.union([self, other])
 
     def add_margins(self, margins):
+        """Generates a new :obj:`BoundingBox` object with adjusted ``margins``.
+
+        Parameters
+        ----------
+        margins: str or number
+            The margin to be added to each side. When it is a ``str`` must specify a percentage
+            in terms of the current size like "50%", while a ``number`` must specify degrees.
+
+        Returns
+        -------
+        :obj:`BoundingBox`
+            New object with adjusted ``margins``.
+        """
         if isinstance(margins, str) and margins[-1] == "%":
             margins = int(margins[:-1]) / 100.0
             margins = max(
                 (self.north - self.south) * margins, (self.east - self.west) * margins
             )
 
         # TODO:check east/west
```

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/conventions.py` & `earthkit-data-0.2.0/earthkit/data/utils/conventions.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/dates.py` & `earthkit-data-0.2.0/earthkit/data/utils/dates.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/factorise.py` & `earthkit-data-0.2.0/earthkit/data/utils/factorise.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/html.py` & `earthkit-data-0.2.0/earthkit/data/utils/html.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/humanize.py` & `earthkit-data-0.2.0/earthkit/data/utils/humanize.py`

 * *Files 4% similar despite different names*

```diff
@@ -341,7 +341,23 @@
 
 
 def rounded_datetime(d):
     if float(d.microsecond) / 1000.0 / 1000.0 >= 0.5:
         d = d + datetime.timedelta(seconds=1)
     d = d.replace(microsecond=0)
     return d
+
+
+def interval_to_human(v, value="x"):
+    if v.bounded:
+        if not v.bounded_left:
+            right_oper = "<=" if v.closed_right else "<"
+            return f"{value} {right_oper} {v.right}"
+        elif not v.bounded_right:
+            left_oper = ">=" if v.closed_left else ">"
+            return f"{value} {left_oper} {v.left}"
+        else:
+            left_oper = "<=" if v.closed_left else "<"
+            right_oper = "<=" if v.closed_right else "<"
+            return f"{v.left} {left_oper} {value} {right_oper} {v.right}"
+    else:
+        return ""
```

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/kwargs.py` & `earthkit-data-0.2.0/earthkit/data/utils/kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/parts.py` & `earthkit-data-0.2.0/earthkit/data/utils/parts.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/patterns.py` & `earthkit-data-0.2.0/earthkit/data/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/utils/serialise.py` & `earthkit-data-0.2.0/earthkit/data/utils/serialise.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/vocabularies/__init__.py` & `earthkit-data-0.2.0/earthkit/data/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/vocabularies/aliases.py` & `earthkit-data-0.2.0/earthkit/data/vocabularies/aliases.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/vocabularies/cf.py` & `earthkit-data-0.2.0/earthkit/data/vocabularies/cf.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/vocabularies/grib-paramid.csv` & `earthkit-data-0.2.0/earthkit/data/vocabularies/grib-paramid.csv`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/vocabularies/grib.py` & `earthkit-data-0.2.0/earthkit/data/vocabularies/grib.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/wrappers/integer.py` & `earthkit-data-0.2.0/earthkit/data/wrappers/integer.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit/data/wrappers/string.py` & `earthkit-data-0.2.0/earthkit/data/wrappers/string.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,18 +33,18 @@
     return parse(dt)
 
 
 class StrWrapper(Wrapper):
     def __init__(self, data):
         self.data = data
 
-    def bounding_box(self):
-        from earthkit.data.utils.domains import domain_to_area
-
-        return domain_to_area(self.data)
+    # DEPENDANCIES NOT YET INSTALLED
+    # def bounding_box(self):
+    #     from earthkit.data.utils.domains import domain_to_area
+    #     return domain_to_area(self.data)
 
     def datetime(self):
         return parse_date(self.data)
 
     def to_datetime_list(self):
         from earthkit.data.utils.dates import mars_like_date_list
 
@@ -56,12 +56,15 @@
         if len(bits) == 5 and bits[1].lower() == "to" and bits[3].lower() == "by":
             return mars_like_date_list(
                 parse_date(bits[0]), parse_date(bits[2]), int(bits[4])
             )
 
         return [parse_date(d) for d in bits]
 
+    def to_string(self):
+        return self.data
+
 
 def wrapper(data, *args, **kwargs):
     if isinstance(data, str):
         return StrWrapper(data)
     return None
```

### Comparing `earthkit-data-0.1.3/earthkit-data.png` & `earthkit-data-0.2.0/docs/_static/earthkit-data.png`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/earthkit_data.egg-info/PKG-INFO` & `earthkit-data-0.2.0/earthkit_data.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-data
-Version: 0.1.3
+Version: 0.2.0
 Summary: A format-agnostic Python interface for geospatial data
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # earthkit-data
 
-![earthkit-data](https://raw.githubusercontent.com/ecmwf/earthkit-data/develop/earthkit-data.png)
+![earthkit-data](docs/_static/earthkit-data.png)
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
 
 A format-agnostic interface for geospatial data with a focus on meteorology and
 climate science.
 
 **DISCLAIMER**
```

### Comparing `earthkit-data-0.1.3/earthkit_data.egg-info/SOURCES.txt` & `earthkit-data-0.2.0/earthkit_data.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 Makefile
 README.md
-earthkit-data.png
 environment.yml
 pyproject.toml
 pytest.ini
 setup.cfg
 .github/workflows/ci.yml
 .github/workflows/label-public-pr.yml
-.github/workflows/notify_new_issue.yml
-.github/workflows/notify_new_pr.yml
+.github/workflows/notify-new-issue.yml
+.github/workflows/notify-new-pr.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/development.rst
 docs/examples.rst
 docs/index.rst
 docs/install.rst
 docs/licence.rst
 docs/make.bat
 docs/requirements.txt
+docs/skip_api_rules.py
 docs/_static/.gitkeep
+docs/_static/earthkit-data.png
 docs/_static/style.css
 docs/_templates/.gitkeep
-docs/examples/Untitled.ipynb
-docs/examples/bufr.ipynb
+docs/examples/bufr_synop.ipynb
+docs/examples/bufr_temp.ipynb
 docs/examples/cds.ipynb
+docs/examples/ecmwf_open_data.ipynb
 docs/examples/fdb.ipynb
+docs/examples/from_object.ipynb
 docs/examples/grib_file_pattern.ipynb
 docs/examples/grib_from_stream.ipynb
 docs/examples/grib_indexing.ipynb
 docs/examples/grib_metadata.ipynb
 docs/examples/grib_missing.ipynb
 docs/examples/grib_multi.ipynb
 docs/examples/grib_overview.ipynb
@@ -42,14 +45,16 @@
 docs/examples/grib_to_netcdf.ipynb
 docs/examples/grib_url.ipynb
 docs/examples/list_of_dict.ipynb
 docs/examples/mars.ipynb
 docs/examples/missing.grib
 docs/examples/netcdf.ipynb
 docs/examples/odb.ipynb
+docs/examples/projection.ipynb
+docs/examples/synop_10.bufr
 docs/examples/temp_10.bufr
 docs/examples/test.grib
 docs/examples/test.nc
 docs/examples/test.odb
 docs/examples/test4.grib
 docs/examples/test6.grib
 docs/examples/tuv_pl.grib
@@ -63,14 +68,16 @@
 docs/guide/data_format/grib.rst
 docs/guide/data_format/index.rst
 docs/guide/data_format/netcdf.rst
 docs/guide/data_format/odb.rst
 docs/guide/include/settings-1-get.py
 docs/guide/include/settings-2-set.py
 docs/guide/include/settings-3-reset.py
+docs/release_notes/index.rst
+docs/release_notes/version_0.2_updates.rst
 earthkit/data/__init__.py
 earthkit/data/decorators.py
 earthkit/data/input_manager.py
 earthkit/data/testing.py
 earthkit/data/version.py
 earthkit/data/arguments/__init__.py
 earthkit/data/arguments/args_kwargs.py
@@ -88,36 +95,39 @@
 earthkit/data/core/select.py
 earthkit/data/core/settings.py
 earthkit/data/core/statistics.py
 earthkit/data/core/temporary.py
 earthkit/data/core/thread.py
 earthkit/data/data/css/tab.css
 earthkit/data/data/css/table.css
+earthkit/data/data/css/tree.css
 earthkit/data/indexing/__init__.py
 earthkit/data/indexing/database/__init__.py
 earthkit/data/indexing/database/json.py
 earthkit/data/indexing/database/sql.py
 earthkit/data/indexing/database/stdout.py
 earthkit/data/mergers/__init__.py
 earthkit/data/mergers/pandas.py
 earthkit/data/mergers/xarray.py
 earthkit/data/mirrors/__init__.py
 earthkit/data/mirrors/directory_mirror.py
 earthkit/data/readers/__init__.py
 earthkit/data/readers/archive.py
-earthkit/data/readers/bufr.py
 earthkit/data/readers/csv.py
 earthkit/data/readers/directory.py
 earthkit/data/readers/netcdf.py
 earthkit/data/readers/numpy.py
 earthkit/data/readers/odb.py
 earthkit/data/readers/tar.py
 earthkit/data/readers/text.py
 earthkit/data/readers/unknown.py
 earthkit/data/readers/zip.py
+earthkit/data/readers/bufr/__init__.py
+earthkit/data/readers/bufr/bufr.py
+earthkit/data/readers/bufr/pandas.py
 earthkit/data/readers/grib/__init__.py
 earthkit/data/readers/grib/codes.py
 earthkit/data/readers/grib/fieldlist.py
 earthkit/data/readers/grib/memory.py
 earthkit/data/readers/grib/output.py
 earthkit/data/readers/grib/pandas.py
 earthkit/data/readers/grib/parsing.py
@@ -129,14 +139,15 @@
 earthkit/data/readers/grib/index/json.py
 earthkit/data/readers/grib/index/sql.py
 earthkit/data/sources/__init__.py
 earthkit/data/sources/cds.py
 earthkit/data/sources/dummy.grib
 earthkit/data/sources/dummy_source.py
 earthkit/data/sources/ecmwf_api.py
+earthkit/data/sources/ecmwf_open_data.py
 earthkit/data/sources/empty.py
 earthkit/data/sources/fdb.py
 earthkit/data/sources/file.py
 earthkit/data/sources/file_indexed.py
 earthkit/data/sources/file_pattern.py
 earthkit/data/sources/indexed.py
 earthkit/data/sources/list_of_dicts.py
@@ -150,45 +161,65 @@
 earthkit/data/sources/url_pattern.py
 earthkit/data/sources/virtual.py
 earthkit/data/sources/virtual_directory.py
 earthkit/data/sphinxext/__init__.py
 earthkit/data/sphinxext/generate_settings_rst.py
 earthkit/data/sphinxext/module_output.py
 earthkit/data/sphinxext/xref.py
+earthkit/data/translators/__init__.py
+earthkit/data/translators/ndarray.py
+earthkit/data/translators/string.py
+earthkit/data/translators/xarray.py
 earthkit/data/utils/__init__.py
 earthkit/data/utils/availability.py
 earthkit/data/utils/bbox.py
 earthkit/data/utils/conventions.py
 earthkit/data/utils/dates.py
+earthkit/data/utils/examples.py
 earthkit/data/utils/factorise.py
 earthkit/data/utils/html.py
 earthkit/data/utils/humanize.py
+earthkit/data/utils/interval.py
 earthkit/data/utils/kwargs.py
 earthkit/data/utils/lazy.py
+earthkit/data/utils/message.py
+earthkit/data/utils/metadata.py
 earthkit/data/utils/parts.py
 earthkit/data/utils/patterns.py
 earthkit/data/utils/serialise.py
 earthkit/data/utils/summary.py
+earthkit/data/utils/projections/__init__.py
+earthkit/data/utils/projections/cf.py
+earthkit/data/utils/projections/proj.py
 earthkit/data/vocabularies/__init__.py
 earthkit/data/vocabularies/aliases.py
 earthkit/data/vocabularies/cf.py
 earthkit/data/vocabularies/grib-paramid.csv
 earthkit/data/vocabularies/grib.py
 earthkit/data/wrappers/__init__.py
 earthkit/data/wrappers/integer.py
+earthkit/data/wrappers/ndarray.py
 earthkit/data/wrappers/string.py
+earthkit/data/wrappers/xarray.py
 earthkit_data.egg-info/PKG-INFO
 earthkit_data.egg-info/SOURCES.txt
 earthkit_data.egg-info/dependency_links.txt
 earthkit_data.egg-info/requires.txt
 earthkit_data.egg-info/top_level.txt
 tests/conftest.py
+tests/environment-unit-tests.yml
 tests/test_00_version.py
+tests/bufr/test_bufr_concat.py
+tests/bufr/test_bufr_contents.py
+tests/bufr/test_bufr_convert.py
+tests/bufr/test_bufr_order_by.py
+tests/bufr/test_bufr_sel.py
 tests/bufr/test_bufr_summary.py
 tests/core/test_cache.py
+tests/core/test_settings.py
 tests/core/test_version.py
 tests/data/mercator.grib
 tests/data/ml_data.grib
 tests/data/rgg_small_subarea_cellarea_ref.grib
 tests/data/t_pl.grib
 tests/data/t_time_series.grib
 tests/data/test_icon.grib
@@ -214,18 +245,28 @@
 tests/indexing/test_indexing_serialisation.py
 tests/indexing/test_order_kwargs.py
 tests/indexing/test_selection_kwargs.py
 tests/readers/test_csv_reader.py
 tests/readers/test_grib_reader.py
 tests/readers/test_netcdf_reader.py
 tests/readers/test_odb_reader.py
+tests/readers/test_reader_padding_bytes.py
 tests/readers/test_tar_reader.py
 tests/readers/test_unknown_reader.py
 tests/readers/test_zip_reader.py
 tests/readers/unknown_file.unknown_ext
 tests/readers/unknown_text_file.unknown_ext
 tests/sources/test_cds.py
+tests/sources/test_ecmwf_open_data.py
 tests/sources/test_file.py
 tests/sources/test_mars.py
 tests/sources/test_multi.py
 tests/sources/test_url.py
-tests/sources/test_url_pattern.py
+tests/sources/test_url_pattern.py
+tests/translators/test_translators.py
+tests/utils/test_bbox.py
+tests/utils/test_download_examples.py
+tests/utils/test_interval.py
+tests/utils/test_projections.py
+tests/wrappers/test_ndarray.py
+tests/wrappers/test_string.py
+tests/wrappers/test_xarray.py
```

### Comparing `earthkit-data-0.1.3/environment.yml` & `earthkit-data-0.2.0/tests/environment-unit-tests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 dependencies:
 - eccodes=>2.19.0
 - python-eccodes
 - pip
 - numpy
 - pandas
 - xarray>=0.19.0
+- cartopy
 - dask
 - netcdf4
 - cfgrib>=0.9.10.1
-- pdbufr
+- pdbufr>=0.11.0
 - pyodc
 - filelock
 - pyyaml
 - entrypoints
 - jupyterlab
 - ecmwf-api-client>=1.6.1
 - cdsapi
 - pip:
   - git+https://github.com/ecmwf/multiurl
   - git+https://github.com/ecmwf/pyfdb
+  - ecmwf-opendata>=0.1.2
 - tqdm
 - markdown
 - make
 - mypy
 - myst-parser
 - pre-commit
 - pydata-sphinx-theme
```

### Comparing `earthkit-data-0.1.3/setup.cfg` & `earthkit-data-0.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 long_description_content_type = text/markdown
 long_description = file: README.md
 test_suite = tests
 
 [options]
 packages = find_namespace:
 install_requires = 
+	cdsapi
 	cfgrib>=0.9.10.1
+	eccodes>=1.5.0
+	ecmwf-api-client>=1.6.1
+	ecmwf-opendata>=0.1.2
 	dask
 	entrypoints
 	filelock
 	jinja2
 	multiurl
 	netcdf4
-	pdbufr
+	pdbufr>=0.11.0
 	pyfdb
 	pyodc
 	pyyaml
 	tqdm
 	xarray>=0.19.0
 
 [options.packages.find]
```

### Comparing `earthkit-data-0.1.3/tests/conftest.py` & `earthkit-data-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/core/test_cache.py` & `earthkit-data-0.2.0/tests/core/test_cache.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/core/test_version.py` & `earthkit-data-0.2.0/tests/core/test_version.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/data/mercator.grib` & `earthkit-data-0.2.0/tests/data/mercator.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/data/ml_data.grib` & `earthkit-data-0.2.0/tests/data/ml_data.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/data/rgg_small_subarea_cellarea_ref.grib` & `earthkit-data-0.2.0/tests/data/rgg_small_subarea_cellarea_ref.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/data/t_pl.grib` & `earthkit-data-0.2.0/tests/data/t_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/data/t_time_series.grib` & `earthkit-data-0.2.0/tests/data/t_time_series.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/data/test_icon.grib` & `earthkit-data-0.2.0/tests/data/test_icon.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/data/test_single.nc` & `earthkit-data-0.2.0/tests/data/test_single.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/data/u_pl.grib` & `earthkit-data-0.2.0/tests/data/u_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/data/v_pl.grib` & `earthkit-data-0.2.0/tests/data/v_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/documentation/test_examples.py` & `earthkit-data-0.2.0/tests/documentation/test_examples.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/documentation/test_notebooks.py` & `earthkit-data-0.2.0/tests/documentation/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/grib/test_grib_concat.py` & `earthkit-data-0.2.0/tests/grib/test_grib_concat.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/grib/test_grib_contents.py` & `earthkit-data-0.2.0/tests/grib/test_grib_contents.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import numpy as np
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.core.temporary import temp_file
 from earthkit.data.testing import earthkit_examples_file, earthkit_test_data_file
+from earthkit.data.utils import projections
 
 
 def check_array(v, shape=None, first=None, last=None, meanv=None, eps=1e-3):
     assert v.shape == shape
     assert np.isclose(v[0], first, eps)
     assert np.isclose(v[-1], last, eps)
     assert np.isclose(v.mean(), meanv, eps)
@@ -598,19 +599,21 @@
     assert np.isclose(v[11], 260.4356, eps)
     assert np.isclose(v[-1], 227.1856, eps)
     m = v[mask]
     assert len(m) == 38
     assert np.count_nonzero(np.isnan(m)) == 38
 
 
-def test_grib_to_points_1():
+@pytest.mark.parametrize("index", [0, None])
+def test_grib_to_latlon_single(index):
     f = from_source("file", earthkit_test_data_file("test_single.grib"))
 
     eps = 1e-5
-    v = f[0].to_points(flatten=True)
+    g = f[index] if index is not None else f
+    v = g.to_latlon(flatten=True)
     assert isinstance(v, dict)
     assert isinstance(v["lon"], np.ndarray)
     assert isinstance(v["lat"], np.ndarray)
     check_array(
         v["lon"],
         (84,),
         first=0.0,
@@ -624,18 +627,20 @@
         first=90,
         last=-90,
         meanv=0,
         eps=eps,
     )
 
 
-def test_grib_to_points_1_shape():
+@pytest.mark.parametrize("index", [0, None])
+def test_grib_to_latlon_single_shape(index):
     f = from_source("file", earthkit_test_data_file("test_single.grib"))
 
-    v = f[0].to_points()
+    g = f[index] if index is not None else f
+    v = g.to_latlon()
     assert isinstance(v, dict)
     assert isinstance(v["lon"], np.ndarray)
     assert isinstance(v["lat"], np.ndarray)
 
     # x
     assert v["lon"].shape == (7, 12)
     for x in v["lon"]:
@@ -643,14 +648,92 @@
 
     # y
     assert v["lat"].shape == (7, 12)
     for i, y in enumerate(v["lat"]):
         assert np.allclose(y, np.ones(12) * (90 - i * 30))
 
 
+def test_grib_to_latlon_multi():
+    f = from_source("file", earthkit_examples_file("test.grib"))
+
+    v_ref = f[0].to_latlon(flatten=True)
+    v = f.to_latlon(flatten=True)
+    assert isinstance(v, dict)
+    assert v.keys() == v_ref.keys()
+
+    assert isinstance(v, dict)
+    assert np.allclose(v["lat"], v_ref["lat"])
+    assert np.allclose(v["lon"], v_ref["lon"])
+
+
+def test_grib_to_latlon_multi_non_shared_grid():
+    f1 = from_source("file", earthkit_examples_file("test.grib"))
+    f2 = from_source("file", earthkit_examples_file("test4.grib"))
+    f = f1 + f2
+
+    with pytest.raises(ValueError):
+        f.to_latlon()
+
+
+@pytest.mark.parametrize("index", [0, None])
+def test_grib_to_points_single(index):
+    f = from_source("file", earthkit_test_data_file("test_single.grib"))
+
+    eps = 1e-5
+    g = f[index] if index is not None else f
+    v = g.to_points(flatten=True)
+    assert isinstance(v, dict)
+    assert isinstance(v["x"], np.ndarray)
+    assert isinstance(v["y"], np.ndarray)
+    check_array(
+        v["x"],
+        (84,),
+        first=0.0,
+        last=330.0,
+        meanv=165.0,
+        eps=eps,
+    )
+    check_array(
+        v["y"],
+        (84,),
+        first=90,
+        last=-90,
+        meanv=0,
+        eps=eps,
+    )
+
+
+def test_grib_to_points_unsupported_grid():
+    f = from_source("file", earthkit_test_data_file("mercator.grib"))
+    with pytest.raises(ValueError):
+        f[0].to_points()
+
+
+def test_grib_to_points_multi():
+    f = from_source("file", earthkit_examples_file("test.grib"))
+
+    v_ref = f[0].to_points(flatten=True)
+    v = f.to_points(flatten=True)
+    assert isinstance(v, dict)
+    assert v.keys() == v_ref.keys()
+
+    assert isinstance(v, dict)
+    assert np.allclose(v["x"], v_ref["x"])
+    assert np.allclose(v["y"], v_ref["y"])
+
+
+def test_grib_to_points_multi_non_shared_grid():
+    f1 = from_source("file", earthkit_examples_file("test.grib"))
+    f2 = from_source("file", earthkit_examples_file("test4.grib"))
+    f = f1 + f2
+
+    with pytest.raises(ValueError):
+        f.to_points()
+
+
 def test_grib_datetime():
     s = from_source("file", earthkit_examples_file("test.grib"))
 
     ref = {
         "base_time": [datetime.datetime(2020, 5, 13, 12)],
         "valid_time": [datetime.datetime(2020, 5, 13, 12)],
     }
@@ -673,39 +756,44 @@
             datetime.datetime(1990, 1, 2, 12, 0),
         ],
     }
     assert s.datetime() == ref
 
 
 def test_bbox():
-    s = from_source("file", earthkit_examples_file("test.grib"))
-    assert s.bounding_box().as_tuple() == (73, -27, 33, 45), s.bounding_box()
+    ds = from_source("file", earthkit_examples_file("test.grib"))
+    bb = ds.bounding_box()
+    assert len(bb) == 2
+    for b in bb:
+        assert b.as_tuple() == (73, -27, 33, 45)
 
 
-def test_grib_proj_string_ll():
+@pytest.mark.parametrize("index", [0, None])
+def test_grib_projection_ll(index):
     f = from_source("file", earthkit_examples_file("test.grib"))
-    r = f[0].proj_string()
-    assert r is None
-    r = f[0].proj_source_string()
-    assert r is None
-    r = f[0].proj_target_string()
-    assert r is None
 
+    if index is not None:
+        g = f[index]
+    else:
+        g = f
+    assert isinstance(g.projection(), projections.EquidistantCylindrical)
 
-def test_grib_proj_string_mercator():
+
+def test_grib_projection_mercator():
     f = from_source("file", earthkit_test_data_file("mercator.grib"))
-    ref_str = (
-        "+proj=merc +lat_ts=20.000000 +lat_0=0 +lon_0=0 +x_0=0 +y_0=0 +R=6371200.000000"
-    )
-    r = f[0].proj_string()
-    assert r == ref_str
-    r = f[0].proj_source_string()
-    assert r == "EPSG:4326"
-    r = f[0].proj_target_string()
-    assert r == ref_str
+    projection = f[0].projection()
+    assert isinstance(projection, projections.Mercator)
+    assert projection.parameters == {
+        "true_scale_latitude": 20,
+        "central_latitude": 0,
+        "central_longitude": 0,
+        "false_easting": 0,
+        "false_northing": 0,
+    }
+    assert projection.globe == dict()
 
 
 def test_message():
     f = from_source("file", earthkit_examples_file("test.grib"))
     v = f[0].message()
     assert len(v) == 526
     assert v[:4] == b"GRIB"
@@ -719,15 +807,58 @@
         data = f.read()
         fs = from_source("memory", data)
         assert len(fs) == 1
         sn = fs.metadata("param")
         assert sn == ["2t"]
 
 
-def test_grib_from_stream_single_group():
+def test_grib_from_stream_invalid_args():
+    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
+        with pytest.raises(TypeError):
+            from_source("stream", stream, order_by="level")
+
+    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
+        with pytest.raises(TypeError):
+            from_source("stream", stream, group_by=1)
+
+    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
+        with pytest.raises(TypeError):
+            from_source("stream", stream, group_by=["level", 1])
+
+    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
+        with pytest.raises(TypeError):
+            from_source("stream", stream, group_by="level", batch_size=1)
+
+    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
+        with pytest.raises(ValueError):
+            from_source("stream", stream, batch_size=-1)
+
+
+@pytest.mark.parametrize("group_by", ["level", ["level", "gridType"]])
+def test_grib_from_stream_group_by(group_by):
+    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
+        fs = from_source("stream", stream, group_by=group_by)
+
+        # no methods are available
+        with pytest.raises(TypeError):
+            len(fs)
+
+        ref = [
+            [("t", 1000), ("u", 1000), ("v", 1000)],
+            [("t", 850), ("u", 850), ("v", 850)],
+        ]
+        for i, f in enumerate(fs):
+            assert len(f) == 3
+            assert f.metadata(("param", "level")) == ref[i]
+
+        # stream consumed, no data is available
+        assert sum([1 for _ in fs]) == 0
+
+
+def test_grib_from_stream_single_batch():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
         fs = from_source("stream", stream)
 
         # no methods are available
         with pytest.raises(TypeError):
             len(fs)
 
@@ -735,39 +866,33 @@
         val = []
         for f in fs:
             v = f.metadata("param")
             val.append(v)
 
         assert val == ref
 
-        # no data is available
-        i = 0
-        for f in fs:
-            i += 1
-        assert i == 0
+        # stream consumed, no data is available
+        assert sum([1 for _ in fs]) == 0
 
 
-def test_grib_from_stream_multi_group():
+def test_grib_from_stream_multi_batch():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
         fs = from_source("stream", stream, batch_size=2)
 
         # no methods are available
         with pytest.raises(TypeError):
             len(fs)
 
         ref = [["t", "u"], ["v", "t"], ["u", "v"]]
         for i, f in enumerate(fs):
             assert len(f) == 2
             f.metadata("param") == ref[i]
 
-        # no data is available
-        i = 0
-        for f in fs:
-            i += 1
-        assert i == 0
+        # stream consumed, no data is available
+        assert sum([1 for _ in fs]) == 0
 
 
 def test_grib_from_stream_in_memory():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
         fs = from_source("stream", stream, batch_size=0)
 
         assert len(fs) == 6
```

### Comparing `earthkit-data-0.1.3/tests/grib/test_grib_convert.py` & `earthkit-data-0.2.0/tests/grib/test_grib_convert.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/grib/test_grib_order_by.py` & `earthkit-data-0.2.0/tests/grib/test_grib_order_by.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/grib/test_grib_output.py` & `earthkit-data-0.2.0/tests/grib/test_grib_output.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/grib/test_grib_sel.py` & `earthkit-data-0.2.0/tests/grib/test_grib_sel.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/grib/test_grib_slice.py` & `earthkit-data-0.2.0/tests/grib/test_grib_slice.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/grib/test_grib_summary.py` & `earthkit-data-0.2.0/tests/grib/test_grib_summary.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from earthkit.data.testing import earthkit_examples_file
 
 
 def test_grib_describe():
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
 
     # full contents
-    df = f.describe(print=False)
+    df = f.describe()
     df = df.data
 
     ref = {
         "level": {
             ("t", "isobaricInhPa"): "1000,300,...",
             ("u", "isobaricInhPa"): "1000,300,...",
             ("v", "isobaricInhPa"): "1000,300,...",
@@ -73,15 +73,15 @@
 
     # repeated use
     df = f.describe()
     df = df.data
     assert ref == df.to_dict()
 
     # single param by shortName
-    df = f.describe("t", print=False)
+    df = f.describe("t")
     df = df.data
 
     ref = {
         0: {
             "shortName": "t",
             "typeOfLevel": "isobaricInhPa",
             "level": "1000,300,400,850,500,700",
@@ -95,28 +95,28 @@
             "experimentVersionNumber": "0001",
         }
     }
 
     assert ref[0] == df[0].to_dict()
 
     # repeated use
-    df = f.describe(param="t", print=False)
+    df = f.describe(param="t")
     df = df.data
     assert ref[0] == df[0].to_dict()
 
     df = f.describe("t")
     df = df.data
     assert ref[0] == df[0].to_dict()
 
     df = f.describe(param="t")
     df = df.data
     assert ref[0] == df[0].to_dict()
 
     # single param by paramId
-    df = f.describe(130, print=False)
+    df = f.describe(130)
     df = df.data
 
     ref = {
         0: {
             "shortName": "t",
             "typeOfLevel": "isobaricInhPa",
             "level": "1000,300,400,850,500,700",
@@ -129,33 +129,25 @@
             "type": "an",
             "experimentVersionNumber": "0001",
         }
     }
 
     assert ref[0] == df[0].to_dict()
 
-    df = f.describe(param=130, print=False)
-    df = df.data
-    assert ref[0] == df[0].to_dict()
-
-    df = f.describe(130)
-    df = df.data
-    assert ref[0] == df[0].to_dict()
-
     df = f.describe(param=130)
     df = df.data
     assert ref[0] == df[0].to_dict()
 
 
 def test_grib_ls():
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
 
     # default keys
     f1 = f.sel(count=[1, 2, 3, 4])
-    df = f1.ls(print=False)
+    df = f1.ls()
 
     ref = {
         "centre": {0: "ecmf", 1: "ecmf", 2: "ecmf", 3: "ecmf"},
         "shortName": {0: "t", 1: "u", 2: "v", 3: "t"},
         "typeOfLevel": {
             0: "isobaricInhPa",
             1: "isobaricInhPa",
@@ -176,15 +168,15 @@
         },
     }
 
     assert ref == df.to_dict()
 
     # extra keys
     f1 = f.sel(count=[1, 2])
-    df = f1.ls(extra_keys=["paramId"], print=False)
+    df = f1.ls(extra_keys=["paramId"])
 
     ref = {
         "centre": {0: "ecmf", 1: "ecmf"},
         "shortName": {0: "t", 1: "u"},
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
         "level": {0: 1000, 1: 1000},
         "dataDate": {0: 20180801, 1: 20180801},
@@ -200,76 +192,76 @@
 
 
 def test_grib_ls_keys():
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
 
     # default keys
     # positive num (=head)
-    df = f.ls(n=2, keys=["shortName", "bitsPerValue", "gridType"], print=False)
+    df = f.ls(n=2, keys=["shortName", "bitsPerValue", "gridType"])
     ref = {
         "shortName": {0: "t", 1: "u"},
         "bitsPerValue": {0: 4, 1: 4},
         "gridType": {0: "regular_ll", 1: "regular_ll"},
     }
 
     assert ref == df.to_dict()
 
     # negative num (=tail)
-    df = f.ls(n=-2, keys=["shortName", "bitsPerValue", "gridType"], print=False)
+    df = f.ls(n=-2, keys=["shortName", "bitsPerValue", "gridType"])
     ref = {
         "shortName": {0: "u", 1: "v"},
         "bitsPerValue": {0: 4, 1: 4},
         "gridType": {0: "regular_ll", 1: "regular_ll"},
     }
 
     assert ref == df.to_dict()
 
 
 def test_grib_ls_namespace():
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
 
-    df = f.ls(n=2, namespace="vertical", print=False)
+    df = f.ls(n=2, namespace="vertical")
     ref = {
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
         "level": {0: 1000, 1: 1000},
     }
     assert ref == df.to_dict()
 
-    df = f.ls(n=2, namespace="vertical", extra_keys="shortName", print=False)
-    print(df.to_dict())
+    df = f.ls(n=2, namespace="vertical", extra_keys="shortName")
+
     ref = {
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
         "level": {0: 1000, 1: 1000},
         "shortName": {0: "t", 1: "u"},
     }
     assert ref == df.to_dict()
 
 
 def test_grib_ls_invalid_num():
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
     with pytest.raises(ValueError):
-        f.ls(n=0, print=False)
+        f.ls(n=0)
 
     with pytest.raises(ValueError):
-        f.ls(0, print=False)
+        f.ls(0)
 
 
 def test_grib_ls_invalid_arg():
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
-    with pytest.raises(ValueError):
-        f.ls(invalid=1, print=False)
+    with pytest.raises(TypeError):
+        f.ls(invalid=1)
 
 
 def test_grib_ls_num():
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
 
     # default keys
 
     # positive num (=head)
-    df = f.ls(n=2, print=False)
+    df = f.ls(n=2)
     ref = {
         "centre": {0: "ecmf", 1: "ecmf"},
         "shortName": {0: "t", 1: "u"},
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
         "level": {0: 1000, 1: 1000},
         "dataDate": {0: 20180801, 1: 20180801},
         "dataTime": {0: 1200, 1: 1200},
@@ -277,19 +269,19 @@
         "dataType": {0: "an", 1: "an"},
         "number": {0: 0, 1: 0},
         "gridType": {0: "regular_ll", 1: "regular_ll"},
     }
 
     assert ref == df.to_dict()
 
-    df = f.ls(2, print=False)
+    df = f.ls(2)
     assert ref == df.to_dict()
 
     # negative num (=tail)
-    df = f.ls(n=-2, print=False)
+    df = f.ls(n=-2)
     ref = {
         "centre": {0: "ecmf", 1: "ecmf"},
         "shortName": {0: "u", 1: "v"},
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
         "level": {0: 300, 1: 300},
         "dataDate": {0: 20180801, 1: 20180801},
         "dataTime": {0: 1200, 1: 1200},
@@ -297,23 +289,23 @@
         "dataType": {0: "an", 1: "an"},
         "number": {0: 0, 1: 0},
         "gridType": {0: "regular_ll", 1: "regular_ll"},
     }
 
     assert ref == df.to_dict()
 
-    df = f.ls(-2, print=False)
+    df = f.ls(-2)
     assert ref == df.to_dict()
 
 
 def test_grib_head_num():
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
 
     # default keys
-    df = f.head(n=2, print=False)
+    df = f.head(n=2)
     ref = {
         "centre": {0: "ecmf", 1: "ecmf"},
         "shortName": {0: "t", 1: "u"},
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
         "level": {0: 1000, 1: 1000},
         "dataDate": {0: 20180801, 1: 20180801},
         "dataTime": {0: 1200, 1: 1200},
@@ -321,23 +313,23 @@
         "dataType": {0: "an", 1: "an"},
         "number": {0: 0, 1: 0},
         "gridType": {0: "regular_ll", 1: "regular_ll"},
     }
 
     assert ref == df.to_dict()
 
-    df = f.head(2, print=False)
+    df = f.head(2)
     assert ref == df.to_dict()
 
 
 def test_grib_tail_num():
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
 
     # default keys
-    df = f.tail(n=2, print=False)
+    df = f.tail(n=2)
     ref = {
         "centre": {0: "ecmf", 1: "ecmf"},
         "shortName": {0: "u", 1: "v"},
         "typeOfLevel": {0: "isobaricInhPa", 1: "isobaricInhPa"},
         "level": {0: 300, 1: 300},
         "dataDate": {0: 20180801, 1: 20180801},
         "dataTime": {0: 1200, 1: 1200},
@@ -345,15 +337,15 @@
         "dataType": {0: "an", 1: "an"},
         "number": {0: 0, 1: 0},
         "gridType": {0: "regular_ll", 1: "regular_ll"},
     }
 
     assert ref == df.to_dict()
 
-    df = f.tail(2, print=False)
+    df = f.tail(2)
     assert ref == df.to_dict()
 
 
 def test_grib_dump():
     f = from_source("file", earthkit_examples_file("test6.grib"))
 
     namespaces = (
@@ -364,15 +356,15 @@
         "parameter",
         "statistics",
         "time",
         "vertical",
     )
 
     # default
-    r = f[0].dump(print=False, _as_raw=True)
+    r = f[0].dump(_as_raw=True)
     ref = [
         {
             "title": "ls",
             "data": {
                 "edition": 1,
                 "centre": "ecmf",
                 "typeOfLevel": "isobaricInhPa",
@@ -458,15 +450,15 @@
     for d in r:
         ns = d["title"]
         assert ns in namespaces
         if ns not in ("default", "statistics"):
             assert d == [x for x in ref if x["title"] == ns][0], ns
 
     # a namespace
-    r = f[0].dump(namespace="mars", print=False, _as_raw=True)
+    r = f[0].dump(namespace="mars", _as_raw=True)
     ref = [
         {
             "title": "mars",
             "data": {
                 "domain": "g",
                 "levtype": "pl",
                 "levelist": 1000,
@@ -481,15 +473,15 @@
             },
             "tooltip": "Keys in the ecCodes mars namespace",
         }
     ]
     assert r == ref
 
     # namespace reformatted
-    r = f[0].dump(namespace="mars", print=False, _as_raw=False)
+    r = f[0].dump(namespace="mars", _as_raw=False)
     ref = {
         "mars": {
             "domain": "g",
             "levtype": "pl",
             "levelist": 1000,
             "date": 20180801,
             "time": 1200,
```

### Comparing `earthkit-data-0.1.3/tests/indexing/indexing_fixtures.py` & `earthkit-data-0.2.0/tests/indexing/indexing_fixtures.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/indexing/test_indexing_db.py` & `earthkit-data-0.2.0/tests/indexing/test_indexing_db.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/indexing/test_indexing_isel.py` & `earthkit-data-0.2.0/tests/indexing/test_indexing_isel.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/indexing/test_indexing_order_by.py` & `earthkit-data-0.2.0/tests/indexing/test_indexing_order_by.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/indexing/test_indexing_serialisation.py` & `earthkit-data-0.2.0/tests/indexing/test_indexing_serialisation.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/indexing/test_order_kwargs.py` & `earthkit-data-0.2.0/tests/indexing/test_order_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/indexing/test_selection_kwargs.py` & `earthkit-data-0.2.0/tests/indexing/test_selection_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/readers/test_csv_reader.py` & `earthkit-data-0.2.0/tests/readers/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/readers/test_grib_reader.py` & `earthkit-data-0.2.0/tests/readers/test_grib_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 from earthkit.data import from_source
-from earthkit.data.testing import earthkit_file
 
 
 def test_grib_len():
     f = from_source("file", "tests/data/test_single.grib")
     assert len(f) == 1
 
     f = from_source("file", "docs/examples/tuv_pl.grib")
@@ -37,16 +36,11 @@
         paramId=[129, 130],
         date=[19900101, 19900102],
         level=[1000, 500],
     )
     assert len(s) == 8
 
 
-def test_bbox():
-    s = from_source("file", earthkit_file("docs/examples/test.grib"))
-    assert s.bounding_box().as_tuple() == (73, -27, 33, 45), s.bounding_box()
-
-
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main()
```

### Comparing `earthkit-data-0.1.3/tests/readers/test_netcdf_reader.py` & `earthkit-data-0.2.0/tests/readers/test_netcdf_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from earthkit.data.readers.netcdf import NetCDFField
 from earthkit.data.testing import (
     earthkit_examples_file,
     earthkit_file,
     earthkit_remote_test_data_file,
     earthkit_test_data_file,
 )
+from earthkit.data.utils import projections
 
 
 def check_array(v, shape=None, first=None, last=None, meanv=None, eps=1e-3):
     assert v.shape == shape
     assert np.isclose(v[0], first, eps)
     assert np.isclose(v[-1], last, eps)
     assert np.isclose(v.mean(), meanv, eps)
@@ -191,16 +192,19 @@
         last=-90,
         meanv=0,
         eps=eps,
     )
 
 
 def test_bbox():
-    s = from_source("file", earthkit_file("docs/examples/test.nc"))
-    assert s.bounding_box().as_tuple() == (73, -27, 33, 45), s.bounding_box()
+    ds = from_source("file", earthkit_file("docs/examples/test.nc"))
+    bb = ds.bounding_box()
+    assert len(bb) == 2
+    for b in bb:
+        assert b.as_tuple() == (73, -27, 33, 45)
 
 
 def test_netcdf_proj_string_non_cf():
     f = from_source("file", earthkit_examples_file("test.nc"))
     with pytest.raises(AttributeError):
         f[0].to_proj()
 
@@ -212,14 +216,29 @@
     assert (
         r[0]
         == "+proj=laea +lat_0=52 +lon_0=10 +x_0=4321000 +y_0=3210000 +ellps=GRS80 +units=m +no_defs"
     )
     assert r[1] == "+proj=eqc +datum=WGS84 +units=m +no_defs"
 
 
+def test_netcdf_projection_laea():
+    f = from_source("url", earthkit_remote_test_data_file("examples", "efas.nc"))
+    projection = f[0].projection()
+    assert isinstance(projection, projections.LambertAzimuthalEqualArea)
+    assert projection.parameters == {
+        "central_latitude": 52.0,
+        "central_longitude": 10.0,
+        "false_northing": 3210000.0,
+        "false_easting": 4321000.0,
+    }
+    assert projection.globe == {
+        "ellipse": "GRS80",
+    }
+
+
 def test_get_fields_missing_standard_name_attr_in_coord_array():
     """test _get_fields() can handle a missing 'standard_name' attr in coordinate data arrays"""
 
     # example dataset
     fs = from_source("file", earthkit_examples_file("test.nc"))
     ds = fs.to_xarray()
```

### Comparing `earthkit-data-0.1.3/tests/readers/test_odb_reader.py` & `earthkit-data-0.2.0/tests/readers/test_odb_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/readers/test_tar_reader.py` & `earthkit-data-0.2.0/tests/readers/test_tar_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/readers/test_unknown_reader.py` & `earthkit-data-0.2.0/tests/readers/test_unknown_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/readers/test_zip_reader.py` & `earthkit-data-0.2.0/tests/readers/test_zip_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/sources/test_cds.py` & `earthkit-data-0.2.0/tests/sources/test_cds.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/sources/test_file.py` & `earthkit-data-0.2.0/tests/sources/test_file.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/sources/test_mars.py` & `earthkit-data-0.2.0/tests/sources/test_mars.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/sources/test_multi.py` & `earthkit-data-0.2.0/tests/sources/test_multi.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/sources/test_url.py` & `earthkit-data-0.2.0/tests/sources/test_url.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.3/tests/sources/test_url_pattern.py` & `earthkit-data-0.2.0/tests/sources/test_url_pattern.py`

 * *Files identical despite different names*

