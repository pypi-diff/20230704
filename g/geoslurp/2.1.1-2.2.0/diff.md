# Comparing `tmp/geoslurp-2.1.1.tar.gz` & `tmp/geoslurp-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoslurp-2.1.1.tar", last modified: Wed Jun  7 11:59:05 2023, max compression
+gzip compressed data, was "geoslurp-2.2.0.tar", last modified: Tue Jul  4 15:29:18 2023, max compression
```

## Comparing `geoslurp-2.1.1.tar` & `geoslurp-2.2.0.tar`

### file list

```diff
@@ -1,153 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.456416 geoslurp-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-07 11:58:54.000000 geoslurp-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-07 11:59:05.456416 geoslurp-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-07 11:58:54.000000 geoslurp-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.436415 geoslurp-2.1.1/clitools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:58:54.000000 geoslurp-2.1.1/clitools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19296 2023-06-07 11:58:54.000000 geoslurp-2.1.1/clitools/geoslurper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.436415 geoslurp-2.1.1/geoslurp/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.436415 geoslurp-2.1.1/geoslurp/config/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13393 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/config/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/config/localsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/config/slurplogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.440415 geoslurp-2.1.1/geoslurp/datapull/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/cds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/geodesyunr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/icgem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/motu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/thredds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/datapull/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.440415 geoslurp-2.1.1/geoslurp/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/CSVBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/OGRBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/RasterBase.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/cdsbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    13672 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/dataSetBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/datasetgeneric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/era5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/motuGridsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/pandasbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/snrei.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dataset/xarraybase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.440415 geoslurp-2.1.1/geoslurp/db/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/connectorbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/geoslurpdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/db/tabletools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.440415 geoslurp-2.1.1/geoslurp/dbfunc/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dbfunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dbfunc/dbfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dbfunc/maskgeom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dbfunc/radsfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/dbfunc/readfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/earthmodels/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/earthmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/earthmodels/getlove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/fesom/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/fesom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/fesom/extractprofiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/fesom/fesomQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/generic/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/generic/getTableData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/generic/regexQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/gravity/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/gravity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/gravity/graceQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/gravity/gravQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/gravity/staticQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/oceanobs/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/argoProfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/argoQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/awipiesQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/coraQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oceanobs/psmsl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.444415 geoslurp-2.1.1/geoslurp/discover/oras/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/discover/oras/orasQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.448416 geoslurp-2.1.1/geoslurp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/Bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/netcdftools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/ogrgeom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/shapelytools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/spatiallite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/tarsafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/tools/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.448416 geoslurp-2.1.1/geoslurp/types/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/columnmapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/xar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/types/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.448416 geoslurp-2.1.1/geoslurp/view/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/view/graceviews.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-07 11:58:54.000000 geoslurp-2.1.1/geoslurp/view/viewBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.456416 geoslurp-2.1.1/geoslurp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-07 11:59:05.000000 geoslurp-2.1.1/geoslurp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-07 11:59:05.000000 geoslurp-2.1.1/geoslurp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:59:05.000000 geoslurp-2.1.1/geoslurp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 11:59:05.000000 geoslurp-2.1.1/geoslurp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 11:59:05.000000 geoslurp-2.1.1/geoslurp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 11:59:05.456416 geoslurp-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-07 11:58:54.000000 geoslurp-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:59:05.456416 geoslurp-2.1.1/userplugins/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/AWIPIES.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/ArcticDEM.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/Argo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/DuacsGriddedDsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/EasyCora.py
--rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/FESOM.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/GRACEDsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/GSHHGDsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/Hydrosheds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/IceSatDrainDiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/ORAS5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/PSMSL.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/RGIDsets.py
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/RadsDsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/TUGRAZDsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/avisoRefOrbits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/deg1n2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/geodesyunr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/geoshapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/gleam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/glofas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/gracefilters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/grdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/icgemDsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/imerg.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/loadlove.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/mss_cnes_cls2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/naturalearth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/orsiFronts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/sebs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/sentinelreforbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/wgms_fog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-07 11:58:54.000000 geoslurp-2.1.1/userplugins/wribasin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.911387 geoslurp-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-04 15:29:09.000000 geoslurp-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-04 15:29:18.911387 geoslurp-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-04 15:29:09.000000 geoslurp-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.895388 geoslurp-2.2.0/clitools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:09.000000 geoslurp-2.2.0/clitools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19468 2023-07-04 15:29:09.000000 geoslurp-2.2.0/clitools/geoslurper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.895388 geoslurp-2.2.0/geoslurp/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.895388 geoslurp-2.2.0/geoslurp/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/config/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/config/localsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/config/slurplogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.895388 geoslurp-2.2.0/geoslurp/datapull/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/geodesyunr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/icgem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/motu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/thredds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/datapull/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.899387 geoslurp-2.2.0/geoslurp/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/CSVBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/OGRBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/RasterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/cdsbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13672 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/dataSetBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/datasetgeneric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/era5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/motuGridsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/pandasbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/snrei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dataset/xarraybase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.899387 geoslurp-2.2.0/geoslurp/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/db/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/db/connectorbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/db/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/db/geoslurpdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/db/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/db/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/db/tabletools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.899387 geoslurp-2.2.0/geoslurp/dbfunc/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dbfunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dbfunc/dbfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dbfunc/maskgeom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dbfunc/radsfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/dbfunc/readfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.899387 geoslurp-2.2.0/geoslurp/discover/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.899387 geoslurp-2.2.0/geoslurp/discover/earthmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/earthmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/earthmodels/getlove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.899387 geoslurp-2.2.0/geoslurp/discover/fesom/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/fesom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/fesom/extractprofiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/fesom/fesomQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.899387 geoslurp-2.2.0/geoslurp/discover/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/generic/getTableData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/generic/regexQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.903387 geoslurp-2.2.0/geoslurp/discover/gravity/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/gravity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/gravity/graceQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/gravity/gravQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/gravity/staticQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.903387 geoslurp-2.2.0/geoslurp/discover/oceanobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/oceanobs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/oceanobs/argoProfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/oceanobs/argoQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/oceanobs/awipiesQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/oceanobs/coraQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/oceanobs/psmsl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.903387 geoslurp-2.2.0/geoslurp/discover/oras/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/oras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/discover/oras/orasQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.903387 geoslurp-2.2.0/geoslurp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/Bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/netcdftools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/ogrgeom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/shapelytools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/spatiallite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/tarsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/tools/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.903387 geoslurp-2.2.0/geoslurp/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/types/columnmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/types/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/types/xar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/types/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.903387 geoslurp-2.2.0/geoslurp/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/view/graceviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp/view/viewBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.911387 geoslurp-2.2.0/geoslurp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-04 15:29:18.000000 geoslurp-2.2.0/geoslurp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-04 15:29:18.000000 geoslurp-2.2.0/geoslurp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:29:18.000000 geoslurp-2.2.0/geoslurp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 15:29:18.000000 geoslurp-2.2.0/geoslurp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 15:29:18.000000 geoslurp-2.2.0/geoslurp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:29:18.907387 geoslurp-2.2.0/geoslurp_userplugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/AWIPIES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/ArcticDEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/Argo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/DuacsGriddedDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/EasyCora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/FESOM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/GRACEDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/GSHHGDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/Hydrosheds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/IceSatDrainDiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/ORAS5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/PSMSL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/RGIDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/RadsDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/TUGRAZDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/avisoRefOrbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/deg1n2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/geodesyunr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/geoshapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/gleam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/glofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/gracefilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/grdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/icgemDsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/imerg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/loadlove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/mss_cnes_cls2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/naturalearth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/orsiFronts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/sebs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/sentinelreforbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/sword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/wgms_fog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-04 15:29:09.000000 geoslurp-2.2.0/geoslurp_userplugins/wribasin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:29:18.911387 geoslurp-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-04 15:29:09.000000 geoslurp-2.2.0/setup.py
```

### Comparing `geoslurp-2.1.1/LICENSE` & `geoslurp-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/PKG-INFO` & `geoslurp-2.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoslurp
-Version: 2.1.1
+Version: 2.2.0
 Summary: Python postgreSQL-PostGIS client for managing earth science datasets
 Home-page: https://github.com/strawpants/geoslurp
 Author: Roelof Rietbroek
 Author-email: roelof@wobbly.earth
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `geoslurp-2.1.1/README.md` & `geoslurp-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/clitools/geoslurper.py` & `geoslurp-2.2.0/clitools/geoslurper.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,17 @@
 def main(argv):
 
     # add various arguments to the program
     parser=addCommandLineArgs()
     args = parser.parse_args(argv[1:])
     args=check_args(args,parser)
 
-
     # We need a point of contact to communicate with the database
     try:
-        DbConn=GeoslurpConnector(args.host,args.user,args.password,cache=args.cache,dataroot=args.dataroot,plugindir=args.plugindir)
+        DbConn=GeoslurpConnector(args.host,args.user,args.password,cache=args.cache,dataroot=args.dataroot)
     except Exception as e:
         print(e)
         print("Cannot connect to postgresql database, quitting")
         sys.exit(1)
 
 
     # # Process common options
@@ -111,18 +110,21 @@
 
     if args.auth_config:
         for alias,dvals in args.auth_config.items():
             if dvals == "delete":
                 conf.delAuth(alias)
             else:
                 conf.updateAuth(Credentials(alias=alias,**dvals))
-
+    
     if args.refresh:
-        geoslurpCatalogue.refresh(conf)
+        if args.refresh != "DEFAULTPATH":
+            #explicitly supply additional user plugin paths
+            geoslurpCatalogue.setUserPlugPaths(args.refresh.split(";"))
 
+        geoslurpCatalogue.refresh(conf)
 
     if args.list:
         # show available schemes and datasets
         print("Available datasets (SCHEME.DATASET):")
         for catentry in geoslurpCatalogue.listDataSets(conf).keys():
             print("\t%s"%(catentry))
         
@@ -304,16 +306,16 @@
                              help="Prints detailed help (may be used in combination with --dset for detailed JSON options)")
         parser.add_argument('-i','--info',action='store_true',
                             help="Show information about selected datasets")
 
         parser.add_argument('-l','--list',action='store_true',
                             help="List all datasets which are available to use")
 
-        parser.add_argument('--refresh',action='store_true',
-                            help="Refresh the cache of the available datasets")
+        parser.add_argument("--refresh",metavar="USERPLUGINPATHS",nargs="?",type=str,const="DEFAULTPATH", help="Refresh the cache of the available datasets, views and functions. Optionally supply a set of USERPLUGINPATHS (seperate multiple paths with a semicolon) where dataset implementations can be found.")
+
         # parser.add_argument('--purge-scheme',action='store_true',
         #                     help="Purge selected scheme (This deletes all related datasets as well!")
 
         parser.add_argument('--purge-cache',type=str, metavar='filter',const='*',nargs='?',
                             help="Purge the cache of the selected dataset. while optionally applying a filter for the files")
 
         parser.add_argument('--purge-data',type=str, metavar='filter',const='*',nargs='?',
@@ -369,16 +371,14 @@
                             help='Select password for the postgresql user')
 
         parser.add_argument("--port",metavar="port",type=int, default=5432,
                             help='Select the port where the database is served')
 
         parser.add_argument("--dataroot",metavar="DATAROOT",nargs="?",type=str, help="Specify the local root of the data directory. Defaults to ${HOME}/geoslurp_data")
 
-        parser.add_argument("--plugindir",metavar="DIREC",nargs="?",type=str, help="Append a directory where dataset implementations can be found.")
-
 
         parser.add_argument("--dbalias",metavar="DBALIAS",nargs="?",type=str, help="Specify the database alias to connect to. Each database alias can have a different host,port,user,password,dataroot,etc (see the localsettings file")
         # parser.add_argument("--usekeyring",action='store_true',
         #                     help='Set and get the system keyring to store the database password (alternatives are '
         #                          'using --password or the environment variable GEOSLURP_PGPASS')
         parser.add_argument("--keyring","--no-keyring",dest="usekeyring",action=NegateAction, nargs=0,
                             help=" Use/don't use the system keyring to store and retrieve the database password (alternatives are "
```

### Comparing `geoslurp-2.1.1/geoslurp/config/catalogue.py` & `geoslurp-2.2.0/geoslurp/config/catalogue.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,28 +33,28 @@
     __dviews__=[]
     # holds factory methods for dyanamically building datasets
     __dsetfac__=[]
     __catalogue__=None
     __dscache__={}
     __dfcache__={}
     __dvcache__={}
+    __pluginpaths__=None
     def __init__(self):
-        pass
+        #Set default plugin path (may have entries appended)
+        self.__pluginpaths__=[os.path.abspath(os.path.dirname(__file__)+"../../../geoslurp_userplugins")] 
     
     @staticmethod 
     def getCacheFile(conf):
         return os.path.join(conf.getCacheDir("Dset"),"Dset_Catalogue.yaml")
     
-    @staticmethod 
-    def addUserPlugPaths(conf,loadmod=False):
-        for upath in conf.db.plugindir.split(";"):
-            if sys.path.count(upath) == 0:
-                sys.path.append(upath)
-                if loadmod:
-                    mod=__import__(os.path.basename(upath))
+    def setUserPlugPaths(self,plugindirs,append=True):
+        if append:
+            self.__pluginpaths__.append(plugindirs)
+        else:
+            self.__pluginpaths__=plugindirs
 
     def addDataset(self, datasetcls):
         self.__dsets__.append(datasetcls)
     
     def addDatasetFactory(self, datasetclsfac):
         self.__dsetfac__.append(datasetclsfac)
     
@@ -62,14 +62,15 @@
         self.__dbfuncs__.append(dfclass)
 
     def addView(self,dvclass):
         self.__dviews__.append(dvclass)
 
     def refresh(self,conf):
         """Refresh the dataset catalogue"""
+
         self.registerAllDataSets(conf)
         
         #load inventory of existing datasets (for the templated)
         Inv=Inventory(conf.db)
 
         self.__catalogue__={"datasets":{},"factories":{},"functions":{},"views":{}}
         #loop over dataset in the factories
@@ -115,49 +116,57 @@
 
 
         for dv in self.__dviews__:
             name=".".join([dv.scheme,dv.__name__])
             self.__catalogue__["views"][name]={"module":dv.__module__}
             self.__dvcache__[name]=dv
 
+        # add plugin paths before saving
         #save to yaml
+        
         self.__catalogue__["lastupdate"]=datetime.now()
+        self.__catalogue__["pluginpaths"]=self.__pluginpaths__
+         
+
         cachefile=self.getCacheFile(conf)
         slurplog.info("saving available Datasets, functions and views to catalogue %s"%cachefile)
         with open(cachefile,'wt') as fid:
             yaml.dump(self.__catalogue__, fid, default_flow_style=False)
     
     def loadCatalogue(self,conf):
         if self.__catalogue__:
             return
-
-        self.addUserPlugPaths(conf)
+        
         cachefile=self.getCacheFile(conf)
         if not os.path.exists(cachefile):
             self.refresh(conf)
         with open(cachefile,'rt') as fid:
             self.__catalogue__=yaml.safe_load(fid)
+            #extract user plugin paths
+            self.__pluginpaths__=self.__catalogue__["pluginpaths"]
 
     def registerAllDataSets(self,conf):
         """load all dataset classes (but don't construct them)"""
         if self.__dsets__:
             #already loaded (quick return)
             return
         
         #dynamically import all relevant datasets and class factories (including userplugin datasets)
-        # modgeo=__import__("geoslurp.dataset")
        
         #dynamically load functions
         modgeof=__import__("geoslurp.dbfunc")
 
         #dynamically load views
         modgeov=__import__("geoslurp.view")
 
-        #also load userplugins
-        self.addUserPlugPaths(conf,True)
+        #also load datasets from userplugin directories
+        for upath in self.__pluginpaths__:
+            if sys.path.count(upath) == 0:
+                sys.path.append(upath)
+                mod=__import__(os.path.basename(upath))
 
 
     def listDataSets(self,conf):
         self.loadCatalogue(conf)
         return self.__catalogue__["datasets"]
 
     def listFunctions(self,conf):
```

### Comparing `geoslurp-2.1.1/geoslurp/config/localsettings.py` & `geoslurp-2.2.0/geoslurp/config/localsettings.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,15 @@
 
     local_settings=None
     """(str): Alternative local settings file (instead of ${HOME}/.geoslurp_lastused.yaml)"""
 
     cache=None
     write_local_settings=False
     dbalias=None
-    plugindir=None
-    def __init__(self,host=None,user=None,usekeyring=False,password=None,port=None,dataroot=None,cache=None,dbalias=None,plugindir=None):
+    def __init__(self,host=None,user=None,usekeyring=False,password=None,port=None,dataroot=None,cache=None,dbalias=None):
         if host:
             self.host=host
 
         if user:
             self.user=user
 
         if usekeyring:
@@ -65,20 +64,18 @@
             self.dataroot=dataroot
         if cache:
             self.cache=cache
 
         if dbalias:
             self.dbalias=dbalias
         
-        if plugindir:
-            self.plugindir=plugindir
 
 defaultdbdict={"host":None,"user":"geoslurp","port":5432,"readonlyUser":"slurpy",
-        "cache":"/tmp/geoslurp_cache","dataroot":os.path.join(os.path.expanduser('~'),'geoslurp_data'),
-        "plugindir":os.path.abspath(os.path.dirname(__file__)+"../../../userplugins")}
+        "cache":"/tmp/geoslurp_cache","dataroot":os.path.join(os.path.expanduser('~'),'geoslurp_data')}
+        
 
 
 def readLocalSettings(args=settingsArgs(),readonlyuser=True,dbalias=None):
     """Retrieves/updates last used settings from the local settings file .geoslurp_lastused.yaml"""
 
     #We need a deepcopy to properly separate input from output, and funny behavior
     argsout=copy.deepcopy(args)
@@ -221,21 +218,14 @@
         lastOpts[dbalias]["cache"]=argsout.cache
     else:
         if "cache"  in lastOpts[dbalias]:
             argsout.cache=lastOpts[dbalias]["cache"]
         else:
             argsout.cache="/tmp/geoslurp_cache"
     
-    if argsout.plugindir:
-        lastOpts[dbalias]["plugindir"]=argsout.plugindir
-    else:
-        if "plugindir" in lastOpts[dbalias]:
-            argsout.plugindir=lastOpts[dbalias]["plugindir"]
-        else:
-            argsout.plugindir=defaultdbdict["plugindir"]
 
     #write out  options to file to store these settings
     if isUpdated and argsout.write_local_settings:
         lastOpts["lastupdate"]=datetime.now()
         with open(settingsFile,'w') as fid:
             yaml.dump(lastOpts, fid, default_flow_style=False)
```

### Comparing `geoslurp-2.1.1/geoslurp/config/slurplogger.py` & `geoslurp-2.2.0/geoslurp/config/slurplogger.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/cds.py` & `geoslurp-2.2.0/geoslurp/datapull/cds.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/crawler.py` & `geoslurp-2.2.0/geoslurp/datapull/crawler.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/ftp.py` & `geoslurp-2.2.0/geoslurp/datapull/ftp.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/geodesyunr.py` & `geoslurp-2.2.0/geoslurp/datapull/geodesyunr.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/github.py` & `geoslurp-2.2.0/geoslurp/datapull/github.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/http.py` & `geoslurp-2.2.0/geoslurp/datapull/http.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/icgem.py` & `geoslurp-2.2.0/geoslurp/datapull/icgem.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/motu.py` & `geoslurp-2.2.0/geoslurp/datapull/motu.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/rsync.py` & `geoslurp-2.2.0/geoslurp/datapull/rsync.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/sftp.py` & `geoslurp-2.2.0/geoslurp/datapull/sftp.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/thredds.py` & `geoslurp-2.2.0/geoslurp/datapull/thredds.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/uri.py` & `geoslurp-2.2.0/geoslurp/datapull/uri.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/datapull/webdav.py` & `geoslurp-2.2.0/geoslurp/datapull/webdav.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/CSVBase.py` & `geoslurp-2.2.0/geoslurp/dataset/CSVBase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/OGRBase.py` & `geoslurp-2.2.0/geoslurp/dataset/OGRBase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/RasterBase.py` & `geoslurp-2.2.0/geoslurp/dataset/RasterBase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/cdsbase.py` & `geoslurp-2.2.0/geoslurp/dataset/cdsbase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/dataSetBase.py` & `geoslurp-2.2.0/geoslurp/dataset/dataSetBase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/datasetgeneric.py` & `geoslurp-2.2.0/geoslurp/dataset/datasetgeneric.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/era5.py` & `geoslurp-2.2.0/geoslurp/dataset/era5.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/motuGridsBase.py` & `geoslurp-2.2.0/geoslurp/dataset/motuGridsBase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/pandasbase.py` & `geoslurp-2.2.0/geoslurp/dataset/pandasbase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/snrei.py` & `geoslurp-2.2.0/geoslurp/dataset/snrei.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dataset/xarraybase.py` & `geoslurp-2.2.0/geoslurp/dataset/xarraybase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/db/connector.py` & `geoslurp-2.2.0/geoslurp/db/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT
 from geoslurp.config.slurplogger import  slurplogger, debugging
 import getpass
 from geoslurp.db.connectorbase import GeoslurpConnectorBase
 
 class GeoslurpConnector(GeoslurpConnectorBase):
     """Holds a connector to a geoslurp database"""
-    def __init__(self, host, user, passwd=None, port=5432,dataroot=None,cache=None,plugindir=None):
+    def __init__(self, host, user, passwd=None, port=5432,dataroot=None,cache=None):
         """
         establishes a database engine whoch provides the base
         for creating sessions (ORM) or connections (SQL expressions)
         :param dburl: url of the database e.g.: postgresql+psycopg2://geoslurp:password@host/geoslurp
         """
-        super().__init__(dataroot=dataroot,cache=cache,plugindir=plugindir)
+        super().__init__(dataroot=dataroot,cache=cache)
 
 
         self.user=user
         if passwd:
             self.passw=passwd
         else:
             self.passw=getpass.getpass(prompt='Please enter password for %s: '%(user))
```

### Comparing `geoslurp-2.1.1/geoslurp/db/connectorbase.py` & `geoslurp-2.2.0/geoslurp/db/connectorbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,32 +21,28 @@
     fname=inspect.stack()[1].function
     raise NotImplementedError(f"Sorry {fname} is not (yet) implemented for this database type")
 
 class GeoslurpConnectorBase():
     """Holds the base class for a connector to a geoslurp database"""
     cache=None
     localdataroot=None
-    plugindir=None
-    def __init__(self,cache=None,dataroot=None,plugindir=None):
+    def __init__(self,cache=None,dataroot=None):
         """
         Sets the variables which all connectors have in common"""
 
         if dataroot:
             self.localdataroot=dataroot
         else:
             self.localdataroot=os.path.join(os.path.expanduser('~'),'geoslurp_data')
         
         if cache:
             self.cache=cache
         else:
             #default when not specified
             self.cache="/tmp/geoslurp_cache"
-        
-        if plugindir:
-            self.plugindir=plugindir
 
 
     def transsession(self):
         raiseNotImpl()
     
     def vacuumAnalyze(self, tableName, schema):
         """vacuum and analyze a certain table"""
```

### Comparing `geoslurp-2.1.1/geoslurp/db/exporter.py` & `geoslurp-2.2.0/geoslurp/db/exporter.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/db/geoslurpdb.py` & `geoslurp-2.2.0/geoslurp/db/geoslurpdb.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/db/inventory.py` & `geoslurp-2.2.0/geoslurp/db/inventory.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/db/settings.py` & `geoslurp-2.2.0/geoslurp/db/settings.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/db/tabletools.py` & `geoslurp-2.2.0/geoslurp/db/tabletools.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dbfunc/dbfunc.py` & `geoslurp-2.2.0/geoslurp/dbfunc/dbfunc.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dbfunc/maskgeom.py` & `geoslurp-2.2.0/geoslurp/dbfunc/maskgeom.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dbfunc/radsfuncs.py` & `geoslurp-2.2.0/geoslurp/dbfunc/radsfuncs.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/dbfunc/readfile.py` & `geoslurp-2.2.0/geoslurp/dbfunc/readfile.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/__init__.py` & `geoslurp-2.2.0/geoslurp/discover/__init__.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/earthmodels/getlove.py` & `geoslurp-2.2.0/geoslurp/discover/earthmodels/getlove.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/fesom/__init__.py` & `geoslurp-2.2.0/geoslurp/discover/fesom/__init__.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/fesom/extractprofiles.py` & `geoslurp-2.2.0/geoslurp/discover/fesom/extractprofiles.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/fesom/fesomQuery.py` & `geoslurp-2.2.0/geoslurp/discover/fesom/fesomQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/generic/getTableData.py` & `geoslurp-2.2.0/geoslurp/discover/generic/getTableData.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/generic/regexQuery.py` & `geoslurp-2.2.0/geoslurp/discover/generic/regexQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/gravity/__init__.py` & `geoslurp-2.2.0/geoslurp/discover/gravity/__init__.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/gravity/graceQuery.py` & `geoslurp-2.2.0/geoslurp/discover/gravity/graceQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/gravity/gravQuery.py` & `geoslurp-2.2.0/geoslurp/discover/gravity/gravQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/gravity/staticQuery.py` & `geoslurp-2.2.0/geoslurp/discover/gravity/staticQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/oceanobs/__init__.py` & `geoslurp-2.2.0/geoslurp/discover/oceanobs/__init__.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/oceanobs/argoQuery.py` & `geoslurp-2.2.0/geoslurp/discover/oceanobs/argoQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/oceanobs/awipiesQuery.py` & `geoslurp-2.2.0/geoslurp/discover/oceanobs/awipiesQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/oceanobs/coraQuery.py` & `geoslurp-2.2.0/geoslurp/discover/oceanobs/coraQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/oceanobs/psmsl.py` & `geoslurp-2.2.0/geoslurp/discover/oceanobs/psmsl.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/oras/__init__.py` & `geoslurp-2.2.0/geoslurp/discover/oras/__init__.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/discover/oras/orasQuery.py` & `geoslurp-2.2.0/geoslurp/discover/oras/orasQuery.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/Bounds.py` & `geoslurp-2.2.0/geoslurp/tools/Bounds.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/cf.py` & `geoslurp-2.2.0/geoslurp/tools/cf.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/csv.py` & `geoslurp-2.2.0/geoslurp/tools/csv.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/gravity.py` & `geoslurp-2.2.0/geoslurp/tools/gravity.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/netcdftools.py` & `geoslurp-2.2.0/geoslurp/tools/netcdftools.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/ogrgeom.py` & `geoslurp-2.2.0/geoslurp/tools/ogrgeom.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/pandas.py` & `geoslurp-2.2.0/geoslurp/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/shapelytools.py` & `geoslurp-2.2.0/geoslurp/tools/shapelytools.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/spatiallite.py` & `geoslurp-2.2.0/geoslurp/tools/spatiallite.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/tarsafe.py` & `geoslurp-2.2.0/geoslurp/tools/tarsafe.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/time.py` & `geoslurp-2.2.0/geoslurp/tools/time.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/tools/xarray.py` & `geoslurp-2.2.0/geoslurp/tools/xarray.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/types/columnmapper.py` & `geoslurp-2.2.0/geoslurp/types/columnmapper.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/types/json.py` & `geoslurp-2.2.0/geoslurp/types/json.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/types/numpy.py` & `geoslurp-2.2.0/geoslurp/types/numpy.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/types/xar.py` & `geoslurp-2.2.0/geoslurp/types/xar.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/types/zarr.py` & `geoslurp-2.2.0/geoslurp/types/zarr.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/view/graceviews.py` & `geoslurp-2.2.0/geoslurp/view/graceviews.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp/view/viewBase.py` & `geoslurp-2.2.0/geoslurp/view/viewBase.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/geoslurp.egg-info/PKG-INFO` & `geoslurp-2.2.0/geoslurp.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoslurp
-Version: 2.1.1
+Version: 2.2.0
 Summary: Python postgreSQL-PostGIS client for managing earth science datasets
 Home-page: https://github.com/strawpants/geoslurp
 Author: Roelof Rietbroek
 Author-email: roelof@wobbly.earth
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `geoslurp-2.1.1/setup.py` & `geoslurp-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_description = fh.read()
 
 
 setuptools.setup(
     name="geoslurp",
     author="Roelof Rietbroek",
     author_email="roelof@wobbly.earth",
-    version="2.1.1",
+    version="2.2.0",
     description="Python postgreSQL-PostGIS client for managing earth science datasets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/strawpants/geoslurp",
     packages=find_packages("."),
     package_dir={"":"."},
     scripts=['clitools/geoslurper.py'],
```

### Comparing `geoslurp-2.1.1/userplugins/AWIPIES.py` & `geoslurp-2.2.0/geoslurp_userplugins/AWIPIES.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/ArcticDEM.py` & `geoslurp-2.2.0/geoslurp_userplugins/ArcticDEM.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/Argo.py` & `geoslurp-2.2.0/geoslurp_userplugins/Argo.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/DuacsGriddedDsets.py` & `geoslurp-2.2.0/geoslurp_userplugins/DuacsGriddedDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/EasyCora.py` & `geoslurp-2.2.0/geoslurp_userplugins/EasyCora.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/FESOM.py` & `geoslurp-2.2.0/geoslurp_userplugins/FESOM.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/GRACEDsets.py` & `geoslurp-2.2.0/geoslurp_userplugins/GRACEDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/GSHHGDsets.py` & `geoslurp-2.2.0/geoslurp_userplugins/GSHHGDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/Hydrosheds.py` & `geoslurp-2.2.0/geoslurp_userplugins/Hydrosheds.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/IceSatDrainDiv.py` & `geoslurp-2.2.0/geoslurp_userplugins/IceSatDrainDiv.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/ORAS5.py` & `geoslurp-2.2.0/geoslurp_userplugins/ORAS5.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/PSMSL.py` & `geoslurp-2.2.0/geoslurp_userplugins/PSMSL.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/RGIDsets.py` & `geoslurp-2.2.0/geoslurp_userplugins/RGIDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/RadsDsets.py` & `geoslurp-2.2.0/geoslurp_userplugins/RadsDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/TUGRAZDsets.py` & `geoslurp-2.2.0/geoslurp_userplugins/TUGRAZDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/__init__.py` & `geoslurp-2.2.0/geoslurp_userplugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,7 +27,8 @@
 from .FESOM import *
 from .grdc import *
 from .AWIPIES import *
 from .ORAS5 import *
 from .sebs import *
 from .gleam import *
 from .imerg import *
+from .sword import *
```

### Comparing `geoslurp-2.1.1/userplugins/avisoRefOrbits.py` & `geoslurp-2.2.0/geoslurp_userplugins/avisoRefOrbits.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/deg1n2.py` & `geoslurp-2.2.0/geoslurp_userplugins/deg1n2.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/geodesyunr.py` & `geoslurp-2.2.0/geoslurp_userplugins/geodesyunr.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/geoshapes.py` & `geoslurp-2.2.0/geoslurp_userplugins/geoshapes.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/gleam.py` & `geoslurp-2.2.0/geoslurp_userplugins/gleam.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/glofas.py` & `geoslurp-2.2.0/geoslurp_userplugins/glofas.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/gracefilters.py` & `geoslurp-2.2.0/geoslurp_userplugins/gracefilters.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/grdc.py` & `geoslurp-2.2.0/geoslurp_userplugins/grdc.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/icgemDsets.py` & `geoslurp-2.2.0/geoslurp_userplugins/icgemDsets.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/imerg.py` & `geoslurp-2.2.0/geoslurp_userplugins/imerg.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/loadlove.py` & `geoslurp-2.2.0/geoslurp_userplugins/loadlove.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/mss_cnes_cls2015.py` & `geoslurp-2.2.0/geoslurp_userplugins/mss_cnes_cls2015.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/naturalearth.py` & `geoslurp-2.2.0/geoslurp_userplugins/naturalearth.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/orsiFronts.py` & `geoslurp-2.2.0/geoslurp_userplugins/orsiFronts.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/sebs.py` & `geoslurp-2.2.0/geoslurp_userplugins/sebs.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/sentinelreforbits.py` & `geoslurp-2.2.0/geoslurp_userplugins/sentinelreforbits.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/wgms_fog.py` & `geoslurp-2.2.0/geoslurp_userplugins/wgms_fog.py`

 * *Files identical despite different names*

### Comparing `geoslurp-2.1.1/userplugins/wribasin.py` & `geoslurp-2.2.0/geoslurp_userplugins/wribasin.py`

 * *Files identical despite different names*

