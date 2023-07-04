# Comparing `tmp/ocha-anticipy-1.1.1.tar.gz` & `tmp/ocha-anticipy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocha-anticipy-1.1.1.tar", last modified: Tue May 30 14:08:00 2023, max compression
+gzip compressed data, was "ocha-anticipy-1.1.2.tar", last modified: Tue Jul  4 17:00:52 2023, max compression
```

## Comparing `ocha-anticipy-1.1.1.tar` & `ocha-anticipy-1.1.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.874235 ocha-anticipy-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.878235 ocha-anticipy-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/.github/workflows/run-python-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5995 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3235 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.878235 ocha-anticipy-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/config.rst
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.878235 ocha-anticipy-1.1.1/docs/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)     4362 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/chirps.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/codab.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4187 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/fewsnet.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12684 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/glofas.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/iri_seasonal_forecast.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5950 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources/usgs_ndvi.rst
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/datasources.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.878235 ocha-anticipy-1.1.1/docs/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/utilities/raster.rst
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/docs/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)    11353 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.874235 ocha-anticipy-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.882235 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.882235 ocha-anticipy-1.1.1/src/ochanticipy/
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-30 14:08:00.000000 ocha-anticipy-1.1.1/src/ochanticipy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.882235 ocha-anticipy-1.1.1/src/ochanticipy/config/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/afg.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/bdi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/bfa.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/bgd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/caf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/cmr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/cod.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/col.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/eth.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      333 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/hti.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/irq.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/lby.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2933 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mli.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mmr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/moz.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mwi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ner.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/nga.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/npl.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/pse.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/sdn.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/som.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ssd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/syr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/tcd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ukr.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ven.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countries/yem.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8920 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/countryconfig.py
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/config/pathconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/chirps/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/chirps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19875 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/chirps/chirps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/codab/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/codab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7182 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/codab/codab.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/datasource.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/fewsnet/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/fewsnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13942 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/fewsnet/fewsnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9849 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/forecast.py
--rw-r--r--   0 runner    (1001) docker     (122)    19202 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/glofas.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/reanalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/iri/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/iri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10404 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.886235 ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28079 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/ndvi_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10009 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/ndvi_products.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/src/ochanticipy/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      768 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/check_extra_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/check_file_existence.py
--rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     7202 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/geoboundingbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/hdx_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)    25617 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/src/ochanticipy/utils/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/tests/datasources/
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/fake_codab_multi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/fake_config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    14174 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_chirps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_codab.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_datasource.py
--rw-r--r--   0 runner    (1001) docker     (122)     7536 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_fewsnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     4790 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_glofas.py
--rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_glofas_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     9524 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_glofas_process.py
--rw-r--r--   0 runner    (1001) docker     (122)     7158 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_iri.py
--rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/datasources/test_ndvi.py
--rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/test_country_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 14:08:00.890235 ocha-anticipy-1.1.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_check_extra_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_check_file_existence.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2915 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_geoboundingbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_hdx_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7015 2023-05-30 14:07:39.000000 ocha-anticipy-1.1.1/tests/utils/test_raster.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.142177 ocha-anticipy-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.122177 ocha-anticipy-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.126177 ocha-anticipy-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-07-04 17:00:52.142177 ocha-anticipy-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3235 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.126177 ocha-anticipy-1.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.130177 ocha-anticipy-1.1.2/docs/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)     4362 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/datasources/chirps.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/datasources/codab.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4187 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/datasources/fewsnet.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12684 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/datasources/glofas.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/datasources/iri_seasonal_forecast.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5950 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/datasources/usgs_ndvi.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/datasources.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.130177 ocha-anticipy-1.1.2/docs/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/utilities/raster.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/docs/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    11097 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-07-04 17:00:52.142177 ocha-anticipy-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.122177 ocha-anticipy-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.130177 ocha-anticipy-1.1.2/src/ocha_anticipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-07-04 17:00:52.000000 ocha-anticipy-1.1.2/src/ocha_anticipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-07-04 17:00:52.000000 ocha-anticipy-1.1.2/src/ocha_anticipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 17:00:52.000000 ocha-anticipy-1.1.2/src/ocha_anticipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-04 17:00:52.000000 ocha-anticipy-1.1.2/src/ocha_anticipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-04 17:00:52.000000 ocha-anticipy-1.1.2/src/ocha_anticipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.130177 ocha-anticipy-1.1.2/src/ochanticipy/
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-04 17:00:52.000000 ocha-anticipy-1.1.2/src/ochanticipy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.130177 ocha-anticipy-1.1.2/src/ochanticipy/config/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.134177 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/afg.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/bdi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/bfa.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/bgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/caf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/cmr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/cod.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/col.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/eth.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      333 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/hti.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/irq.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/lby.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2933 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/mli.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/mmr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/moz.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/mwi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/ner.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/nga.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/npl.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/pse.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/sdn.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/som.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/ssd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/syr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/tcd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/ukr.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/ven.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countries/yem.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8920 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/countryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/config/pathconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.134177 ocha-anticipy-1.1.2/src/ochanticipy/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.134177 ocha-anticipy-1.1.2/src/ochanticipy/datasources/chirps/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/chirps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19875 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/chirps/chirps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.134177 ocha-anticipy-1.1.2/src/ochanticipy/datasources/codab/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/codab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7182 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/codab/codab.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/datasource.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.134177 ocha-anticipy-1.1.2/src/ochanticipy/datasources/fewsnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/fewsnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13942 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/fewsnet/fewsnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.134177 ocha-anticipy-1.1.2/src/ochanticipy/datasources/glofas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/glofas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9849 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/glofas/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19202 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/glofas/glofas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/glofas/reanalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.134177 ocha-anticipy-1.1.2/src/ochanticipy/datasources/iri/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/iri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10404 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.138177 ocha-anticipy-1.1.2/src/ochanticipy/datasources/usgs/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/usgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28079 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/usgs/ndvi_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10009 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/datasources/usgs/ndvi_products.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.138177 ocha-anticipy-1.1.2/src/ochanticipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      768 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/utils/check_extra_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/utils/check_file_existence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7202 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/utils/geoboundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/utils/hdx_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25617 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/src/ochanticipy/utils/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.138177 ocha-anticipy-1.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.138177 ocha-anticipy-1.1.2/tests/datasources/
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/fake_codab_multi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/fake_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    14174 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/test_chirps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/test_codab.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7536 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/test_fewsnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4790 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/test_glofas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/test_glofas_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9524 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/test_glofas_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7158 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/test_iri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/datasources/test_ndvi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/test_country_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 17:00:52.142177 ocha-anticipy-1.1.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/utils/test_check_extra_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/utils/test_check_file_existence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/utils/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2915 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/utils/test_geoboundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/utils/test_hdx_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7015 2023-07-04 17:00:40.000000 ocha-anticipy-1.1.2/tests/utils/test_raster.py
```

### Comparing `ocha-anticipy-1.1.1/.github/workflows/publish-to-pypi.yaml` & `ocha-anticipy-1.1.2/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/.github/workflows/run-python-tests.yaml` & `ocha-anticipy-1.1.2/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/.gitignore` & `ocha-anticipy-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/.pre-commit-config.yaml` & `ocha-anticipy-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/CHANGELOG.rst` & `ocha-anticipy-1.1.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 All notable changes to OCHA AnticiPy will be documented in this file.
 
 The format is based on `Keep a
 Changelog <https://keepachangelog.com/en/1.0.0/>`__, and this project
 adheres to `Semantic
 Versioning <https://semver.org/spec/v2.0.0.html>`__.
 
+[1.1.2] - 2023-07-04
+--------------------
+
+Fixed
+~~~~~
+
+- Temporarily restrict Pydantic to below v2
+
+
 [1.1.1] - 2023-05-30
 --------------------
 
 Fixed
 ~~~~~
 
 - Typo in required extras for ReadTheDocs
```

### Comparing `ocha-anticipy-1.1.1/CONTRIBUTING.rst` & `ocha-anticipy-1.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/LICENSE` & `ocha-anticipy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/PKG-INFO` & `ocha-anticipy-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocha-anticipy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Access data for anticipating humanitarian risk
 Home-page: https://github.com/OCHA-DAP/ocha-anticipy
 Author: Data Science Team, UN OCHA Centre for Humanitarian Data
 Author-email: centrehumdata@un.org
 License: GPLv3
 Project-URL: Documentation, https://ocha-anticipy.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/OCHA-DAP/ocha-anticipy/blob/main/CHANGELOG.rst
```

### Comparing `ocha-anticipy-1.1.1/README.md` & `ocha-anticipy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/api.rst` & `ocha-anticipy-1.1.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/conf.py` & `ocha-anticipy-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/config.rst` & `ocha-anticipy-1.1.2/docs/config.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/datasources/chirps.rst` & `ocha-anticipy-1.1.2/docs/datasources/chirps.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/datasources/codab.rst` & `ocha-anticipy-1.1.2/docs/datasources/codab.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/datasources/fewsnet.rst` & `ocha-anticipy-1.1.2/docs/datasources/fewsnet.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/datasources/glofas.rst` & `ocha-anticipy-1.1.2/docs/datasources/glofas.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/datasources/iri_seasonal_forecast.rst` & `ocha-anticipy-1.1.2/docs/datasources/iri_seasonal_forecast.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/datasources/usgs_ndvi.rst` & `ocha-anticipy-1.1.2/docs/datasources/usgs_ndvi.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/index.rst` & `ocha-anticipy-1.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/introduction.rst` & `ocha-anticipy-1.1.2/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/quickstart.rst` & `ocha-anticipy-1.1.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/docs/utilities/raster.rst` & `ocha-anticipy-1.1.2/docs/utilities/raster.rst`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/requirements.txt` & `ocha-anticipy-1.1.2/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,50 +4,47 @@
 #
 #    pip-compile --extra=dev --output-file=requirements.txt --resolver=backtracking setup.cfg
 #
 affine==2.4.0
     # via rasterio
 alabaster==0.7.13
     # via sphinx
-apeye==1.3.0
+apeye==1.4.0
     # via
     #   shippinglabel
     #   sphinx-toolbox
-apeye-core==1.1.2
+apeye-core==1.1.4
     # via apeye
 attrs==23.1.0
     # via
-    #   cattrs
     #   cfgrib
     #   eccodes
     #   fiona
     #   frictionless
     #   jsonlines
     #   jsonschema
     #   rasterio
-    #   requests-cache
 autodocsumm==0.2.11
     # via sphinx-toolbox
 babel==2.12.1
     # via sphinx
 beautifulsoup4==4.12.2
     # via sphinx-toolbox
-bokeh==3.1.1
+bokeh==3.2.0
     # via dask
-cachecontrol[filecache]==0.12.11
+cachecontrol[filecache]==0.13.1
     # via sphinx-toolbox
 cachetools==5.3.1
     # via tox
-cattrs==22.2.0
-    # via requests-cache
 cdsapi==0.6.1
     # via ocha-anticipy (setup.cfg)
 certifi==2023.5.7
     # via
     #   fiona
+    #   netcdf4
     #   pyproj
     #   rasterio
     #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   eccodes
@@ -89,23 +86,23 @@
     # via
     #   dask
     #   distributed
 colorama==0.4.6
     # via
     #   tox
     #   typer
-contourpy==1.0.7
+contourpy==1.1.0
     # via bokeh
-coverage[toml]==7.2.6
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==40.0.2
+cryptography==41.0.1
     # via pyopenssl
-cssutils==2.6.0
+cssutils==2.7.1
     # via dict2css
-dask[array,complete,dataframe,diagnostics,distributed]==2023.5.1
+dask[array,complete,dataframe,diagnostics,distributed]==2023.6.1
     # via
     #   distributed
     #   xarray
 decorator==5.1.1
     # via
     #   jsonpath-ng
     #   validators
@@ -113,15 +110,15 @@
     # via hdx-python-api
 dict2css==0.3.0
     # via sphinx-toolbox
 dist-meta==0.8.0
     # via shippinglabel
 distlib==0.3.6
     # via virtualenv
-distributed==2023.5.1
+distributed==2023.6.1
     # via dask
 dnspython==2.3.0
     # via email-validator
 docopt==0.6.2
     # via
     #   ckanapi
     #   num2words
@@ -149,56 +146,57 @@
     # via cfgrib
 email-validator==2.0.0.post2
     # via hdx-python-api
 et-xmlfile==1.1.0
     # via openpyxl
 extras-require==0.5.0
     # via ocha-anticipy (setup.cfg)
-filelock==3.12.0
+filelock==3.12.2
     # via
+    #   cachecontrol
     #   tox
     #   virtualenv
 findlibs==0.0.5
     # via eccodes
 fiona==1.9.4.post1
     # via geopandas
-frictionless==5.13.1
+frictionless==5.14.5
     # via hdx-python-utilities
-fsspec==2023.5.0
+fsspec==2023.6.0
     # via dask
-geopandas==0.13.0
+geopandas==0.13.2
     # via ocha-anticipy (setup.cfg)
 handy-archives==0.1.4
     # via dist-meta
-hdx-python-api==6.0.0
+hdx-python-api==6.0.4
     # via ocha-anticipy (setup.cfg)
-hdx-python-country==3.4.8
+hdx-python-country==3.5.1
     # via
     #   hdx-python-api
     #   ocha-anticipy (setup.cfg)
-hdx-python-utilities==3.5.8
+hdx-python-utilities==3.6.1
     # via hdx-python-country
 html5lib==1.1
     # via sphinx-toolbox
-humanize==4.6.0
+humanize==4.7.0
     # via frictionless
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   apeye-core
     #   email-validator
     #   requests
-ijson==3.2.0.post0
+ijson==3.2.2
     # via hdx-python-utilities
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.6.0
+importlib-metadata==6.7.0
     # via dask
-inflect==6.0.4
+inflect==7.0.0
     # via quantulum3
 iniconfig==2.0.0
     # via pytest
 isodate==0.6.1
     # via frictionless
 jinja2==3.1.2
     # via
@@ -212,55 +210,53 @@
     # via hdx-python-utilities
 jsonpath-ng==1.5.3
     # via libhxl
 jsonschema==4.17.3
     # via
     #   frictionless
     #   tableschema-to-template
-libhxl==5.0
+libhxl==5.0.1
     # via hdx-python-country
 locket==1.0.0
     # via
     #   distributed
     #   partd
 lockfile==0.12.2
-    # via
-    #   cachecontrol
-    #   sphinx-toolbox
+    # via sphinx-toolbox
 loguru==0.7.0
     # via hdx-python-utilities
 lz4==4.3.2
     # via dask
 makefun==1.15.1
     # via hdx-python-api
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via rich
-marko==1.3.0
+marko==2.0.0
     # via frictionless
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   sphinx-jinja2-compat
 mdurl==0.1.2
     # via markdown-it-py
 msgpack==1.0.5
     # via
     #   cachecontrol
     #   distributed
-natsort==8.3.1
+natsort==8.4.0
     # via domdf-python-tools
 ndg-httpsclient==0.5.1
     # via hdx-python-api
-netcdf4==1.6.3
+netcdf4==1.6.4
     # via ocha-anticipy (setup.cfg)
 nodeenv==1.8.0
     # via pre-commit
 num2words==0.5.12
     # via quantulum3
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   bokeh
     #   cfgrib
     #   cftime
     #   contourpy
     #   dask
     #   eccodes
@@ -286,93 +282,91 @@
     #   pyproject-api
     #   pytest
     #   rioxarray
     #   shippinglabel
     #   sphinx
     #   tox
     #   xarray
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   bokeh
     #   dask
     #   geopandas
     #   xarray
 partd==1.4.0
     # via dask
 pbr==5.11.1
     # via sphinxcontrib-apidoc
 petl==1.7.12
     # via frictionless
-pillow==9.5.0
+pillow==10.0.0
     # via bokeh
-platformdirs==3.5.1
+platformdirs==3.8.0
     # via
     #   apeye
-    #   requests-cache
     #   shippinglabel
     #   tox
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   pytest
     #   tox
 ply==3.11
     # via
     #   jsonpath-ng
     #   libhxl
 pockets==0.9.1
     # via sphinxcontrib-napoleon
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via ocha-anticipy (setup.cfg)
 psutil==5.9.5
     # via distributed
-pyarrow==12.0.0
+pyarrow==12.0.1
     # via dask
 pyasn1==0.5.0
     # via
     #   hdx-python-api
     #   ndg-httpsclient
 pycparser==2.21
     # via cffi
-pydantic==1.10.8
+pydantic==1.10.10
     # via
-    #   frictionless
     #   inflect
     #   ocha-anticipy (setup.cfg)
 pygments==2.15.1
     # via
     #   rich
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyopenssl==23.1.1
+pyopenssl==23.2.0
     # via
     #   hdx-python-api
     #   ndg-httpsclient
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via snuggs
 pyphonetics==0.5.3
     # via hdx-python-country
-pyproj==3.5.0
+pyproj==3.6.0
     # via
     #   geopandas
     #   rioxarray
-pyproject-api==1.5.1
+pyproject-api==1.5.2
     # via tox
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.1
+pytest==7.4.0
     # via
     #   libhxl
     #   ocha-anticipy (setup.cfg)
     #   pytest-cov
     #   pytest-mock
 pytest-cov==4.1.0
     # via ocha-anticipy (setup.cfg)
-pytest-mock==3.10.0
+pytest-mock==3.11.1
     # via ocha-anticipy (setup.cfg)
 python-dateutil==2.8.2
     # via
     #   frictionless
     #   hdx-python-utilities
     #   libhxl
     #   ocha-anticipy (setup.cfg)
@@ -392,43 +386,40 @@
     #   distributed
     #   frictionless
     #   ocha-anticipy (setup.cfg)
     #   pre-commit
     #   tableschema-to-template
 quantulum3==0.9.0
     # via hdx-python-api
-rasterio==1.3.7
+rasterio==1.3.8
     # via
     #   ocha-anticipy (setup.cfg)
     #   rioxarray
 ratelimit==2.2.1
     # via hdx-python-utilities
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   cdsapi
     #   ckanapi
     #   frictionless
     #   libhxl
     #   ocha-anticipy (setup.cfg)
-    #   requests-cache
     #   requests-file
     #   sphinx
-requests-cache==1.0.1
-    # via libhxl
 requests-file==1.5.1
     # via hdx-python-utilities
 rfc3986==2.0.0
     # via frictionless
-rich==13.3.5
+rich==13.4.2
     # via typer
 rioxarray==0.14.1
     # via ocha-anticipy (setup.cfg)
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.32
     # via
     #   hdx-python-utilities
     #   sphinx-toolbox
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 shapely==2.0.1
     # via geopandas
@@ -445,15 +436,14 @@
     #   html5lib
     #   isodate
     #   jsonpath-ng
     #   pockets
     #   python-dateutil
     #   requests-file
     #   sphinxcontrib-napoleon
-    #   url-normalize
 snowballstemmer==2.2.0
     # via sphinx
 snuggs==1.4.7
     # via rasterio
 sortedcontainers==2.4.0
     # via distributed
 soupsieve==2.4.1
@@ -474,15 +464,15 @@
     # via sphinx-toolbox
 sphinx-jinja2-compat==0.2.0
     # via sphinx-toolbox
 sphinx-prompt==1.5.0
     # via
     #   extras-require
     #   sphinx-toolbox
-sphinx-rtd-theme==1.2.1
+sphinx-rtd-theme==1.2.2
     # via ocha-anticipy (setup.cfg)
 sphinx-tabs==3.4.1
     # via sphinx-toolbox
 sphinx-toolbox==3.4.0
     # via extras-require
 sphinxcontrib-apidoc==0.3.0
     # via ocha-anticipy (setup.cfg)
@@ -508,70 +498,68 @@
     # via libhxl
 tableschema-to-template==0.0.13
     # via hdx-python-utilities
 tabulate==0.9.0
     # via
     #   frictionless
     #   sphinx-toolbox
-tblib==1.7.0
+tblib==2.0.0
     # via distributed
 text-unidecode==1.3
     # via python-slugify
 toml==0.10.2
     # via dom-toml
 toolz==0.12.0
     # via
     #   dask
     #   distributed
     #   partd
 tornado==6.3.2
     # via
     #   bokeh
     #   distributed
-tox==4.5.2
+tox==4.6.3
     # via ocha-anticipy (setup.cfg)
 tqdm==4.65.0
     # via cdsapi
 typer[all]==0.9.0
     # via frictionless
-typing-extensions==4.6.2
+typing-extensions==4.7.1
     # via
     #   domdf-python-tools
     #   frictionless
+    #   inflect
     #   pydantic
     #   shippinglabel
     #   sphinx-toolbox
     #   typer
 tzdata==2023.3
     # via pandas
 unidecode==1.3.6
     # via
     #   libhxl
     #   pyphonetics
-url-normalize==1.4.3
-    # via requests-cache
-urllib3==1.26.16
+urllib3==2.0.3
     # via
     #   distributed
     #   libhxl
     #   requests
-    #   requests-cache
 validators==0.20.0
     # via frictionless
-virtualenv==20.23.0
+virtualenv==20.23.1
     # via
     #   pre-commit
     #   tox
 webencodings==0.5.1
     # via html5lib
 wheel==0.40.0
     # via libhxl
 wrapt==1.15.0
     # via ocha-anticipy (setup.cfg)
-xarray[parallel]==2023.5.0
+xarray[parallel]==2023.6.0
     # via
     #   ocha-anticipy (setup.cfg)
     #   rioxarray
 xlrd==2.0.1
     # via hdx-python-utilities
 xlrd3==1.1.0
     # via libhxl
```

### Comparing `ocha-anticipy-1.1.1/setup.cfg` & `ocha-anticipy-1.1.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 install_requires = 
 	cftime
 	geopandas
 	hdx-python-api>=5.6.4
 	hdx-python-country
 	netCDF4
 	numpy
-	pydantic
+	pydantic<2.0
 	python-dateutil
 	pyyaml
 	rasterio
 	requests
 	rioxarray
 	wrapt
 	xarray[parallel]
```

### Comparing `ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/PKG-INFO` & `ocha-anticipy-1.1.2/src/ocha_anticipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocha-anticipy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Access data for anticipating humanitarian risk
 Home-page: https://github.com/OCHA-DAP/ocha-anticipy
 Author: Data Science Team, UN OCHA Centre for Humanitarian Data
 Author-email: centrehumdata@un.org
 License: GPLv3
 Project-URL: Documentation, https://ocha-anticipy.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/OCHA-DAP/ocha-anticipy/blob/main/CHANGELOG.rst
```

### Comparing `ocha-anticipy-1.1.1/src/ocha_anticipy.egg-info/SOURCES.txt` & `ocha-anticipy-1.1.2/src/ocha_anticipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/__init__.py` & `ocha-anticipy-1.1.2/src/ochanticipy/__init__.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/bfa.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/bfa.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/bgd.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/bgd.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/caf.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/caf.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/cmr.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/cmr.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/cod.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/cod.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/col.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/col.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/eth.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/eth.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mli.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/mli.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mmr.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/mmr.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/moz.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/moz.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/mwi.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/mwi.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ner.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/ner.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/nga.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/nga.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/npl.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/npl.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/sdn.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/sdn.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/som.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/som.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/tcd.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/tcd.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countries/ven.yaml` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countries/ven.yaml`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/config/countryconfig.py` & `ocha-anticipy-1.1.2/src/ochanticipy/config/countryconfig.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/datasources/chirps/chirps.py` & `ocha-anticipy-1.1.2/src/ochanticipy/datasources/chirps/chirps.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/datasources/codab/codab.py` & `ocha-anticipy-1.1.2/src/ochanticipy/datasources/codab/codab.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/datasources/datasource.py` & `ocha-anticipy-1.1.2/src/ochanticipy/datasources/datasource.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/datasources/fewsnet/fewsnet.py` & `ocha-anticipy-1.1.2/src/ochanticipy/datasources/fewsnet/fewsnet.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/forecast.py` & `ocha-anticipy-1.1.2/src/ochanticipy/datasources/glofas/forecast.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/glofas.py` & `ocha-anticipy-1.1.2/src/ochanticipy/datasources/glofas/glofas.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/datasources/glofas/reanalysis.py` & `ocha-anticipy-1.1.2/src/ochanticipy/datasources/glofas/reanalysis.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py` & `ocha-anticipy-1.1.2/src/ochanticipy/datasources/iri/iri_seasonal_forecast.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/ndvi_base.py` & `ocha-anticipy-1.1.2/src/ochanticipy/datasources/usgs/ndvi_base.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/datasources/usgs/ndvi_products.py` & `ocha-anticipy-1.1.2/src/ochanticipy/datasources/usgs/ndvi_products.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/utils/check_extra_imports.py` & `ocha-anticipy-1.1.2/src/ochanticipy/utils/check_extra_imports.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/utils/check_file_existence.py` & `ocha-anticipy-1.1.2/src/ochanticipy/utils/check_file_existence.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/utils/dates.py` & `ocha-anticipy-1.1.2/src/ochanticipy/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/utils/geoboundingbox.py` & `ocha-anticipy-1.1.2/src/ochanticipy/utils/geoboundingbox.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/utils/hdx_api.py` & `ocha-anticipy-1.1.2/src/ochanticipy/utils/hdx_api.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/utils/io.py` & `ocha-anticipy-1.1.2/src/ochanticipy/utils/io.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/src/ochanticipy/utils/raster.py` & `ocha-anticipy-1.1.2/src/ochanticipy/utils/raster.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/datasources/conftest.py` & `ocha-anticipy-1.1.2/tests/datasources/conftest.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/datasources/test_chirps.py` & `ocha-anticipy-1.1.2/tests/datasources/test_chirps.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/datasources/test_codab.py` & `ocha-anticipy-1.1.2/tests/datasources/test_codab.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/datasources/test_datasource.py` & `ocha-anticipy-1.1.2/tests/datasources/test_datasource.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/datasources/test_fewsnet.py` & `ocha-anticipy-1.1.2/tests/datasources/test_fewsnet.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/datasources/test_glofas.py` & `ocha-anticipy-1.1.2/tests/datasources/test_glofas.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/datasources/test_glofas_download.py` & `ocha-anticipy-1.1.2/tests/datasources/test_glofas_download.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/datasources/test_glofas_process.py` & `ocha-anticipy-1.1.2/tests/datasources/test_glofas_process.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/datasources/test_iri.py` & `ocha-anticipy-1.1.2/tests/datasources/test_iri.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/datasources/test_ndvi.py` & `ocha-anticipy-1.1.2/tests/datasources/test_ndvi.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/test_country_config.py` & `ocha-anticipy-1.1.2/tests/test_country_config.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/utils/test_check_file_existence.py` & `ocha-anticipy-1.1.2/tests/utils/test_check_file_existence.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/utils/test_dates.py` & `ocha-anticipy-1.1.2/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/utils/test_geoboundingbox.py` & `ocha-anticipy-1.1.2/tests/utils/test_geoboundingbox.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/utils/test_hdx_api.py` & `ocha-anticipy-1.1.2/tests/utils/test_hdx_api.py`

 * *Files identical despite different names*

### Comparing `ocha-anticipy-1.1.1/tests/utils/test_raster.py` & `ocha-anticipy-1.1.2/tests/utils/test_raster.py`

 * *Files identical despite different names*

