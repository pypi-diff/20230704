# Comparing `tmp/Finance-Seleya-1.1.2.tar.gz` & `tmp/Finance-Seleya-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Seleya-1.1.2.tar", last modified: Tue Mar 14 07:39:33 2023, max compression
+gzip compressed data, was "dist/Finance-Seleya-1.1.3.tar", last modified: Tue Jul  4 06:39:59 2023, max compression
```

## Comparing `Finance-Seleya-1.1.2.tar` & `Finance-Seleya-1.1.3.tar`

### file list

```diff
@@ -1,111 +1,116 @@
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/Finance_Seleya.egg-info/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        1 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/Finance_Seleya.egg-info/dependency_links.txt
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      213 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/Finance_Seleya.egg-info/requires.txt
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     2941 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/Finance_Seleya.egg-info/SOURCES.txt
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      222 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/Finance_Seleya.egg-info/PKG-INFO
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        7 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/Finance_Seleya.egg-info/top_level.txt
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     2074 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      132 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/seleya.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/core/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2023-01-05 01:44:08.000000 Finance-Seleya-1.1.2/seleya/core/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     1921 2023-01-05 01:44:08.000000 Finance-Seleya-1.1.2/seleya/core/parallel.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     7809 2023-01-05 01:44:08.000000 Finance-Seleya-1.1.2/seleya/core/helper.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     3121 2023-01-05 01:44:08.000000 Finance-Seleya-1.1.2/seleya/core/env.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     9714 2023-01-05 01:44:08.000000 Finance-Seleya-1.1.2/seleya/core/fixes.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/config/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/config/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      489 2023-01-05 01:44:08.000000 Finance-Seleya-1.1.2/seleya/config/default_config.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/Toolset/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     7223 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/Toolset/file_util.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      107 2023-01-05 01:44:08.000000 Finance-Seleya-1.1.2/seleya/Toolset/__init__.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/Toolset/tests/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)       24 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/Toolset/tests/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      632 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/Toolset/tests/runner.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      244 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/Toolset/tests/suite.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     3486 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/Toolset/blob_service.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/Toolset/portfolio/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/Toolset/portfolio/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     6676 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/Toolset/portfolio/esg_metrics.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     4827 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/Toolset/calendar.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/Toolset/audit/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/Toolset/audit/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     2112 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/Toolset/audit/esg_metrics.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     5733 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/Toolset/translator.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/data/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/__init__.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      383 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     1265 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     1168 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      866 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      877 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     2042 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/engine.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      633 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/basic.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)       23 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/__init__.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      592 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      836 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/feature_importance.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      527 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      700 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      537 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/company.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      525 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      611 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     1476 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/industry.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     1577 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/engine.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      836 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/sector.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      626 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      497 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/gd_overview.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      937 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/basic.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     2278 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/metrics.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/mongo/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)       62 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/mongo/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      348 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/mongo/fetch_engine.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     2408 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/mongo/mongodb.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)       94 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/__init__.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/http/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     2288 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/http/USER.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     4296 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/http/SEARCH.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      382 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/http/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      599 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/http/utils.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     3211 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/http/GD.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     3533 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/http/ESG.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/sqlatom/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      117 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/sqlatom/__init__.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/sqlatom/sly/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/sqlatom/sly/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)    55563 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/sqlatom/sly/sly_engine.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)    36127 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/sqlatom/db_factory.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     5777 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/sqlatom/fetch_engine.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)       21 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/data/DataAPI/version.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/mfc/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/mfc/__init__.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/mfc/alchemy/
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/mfc/alchemy/tsi/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/mfc/alchemy/tsi/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)    11460 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/mfc/alchemy/tsi/s2f.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     7957 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/mfc/alchemy/tsi/aerosol.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      218 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/mfc/alchemy/__init__.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/mfc/alchemy/qrank/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/mfc/alchemy/qrank/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)   497381 2023-03-14 07:39:32.000000 Finance-Seleya-1.1.2/seleya/mfc/alchemy/qrank/glassdoor.c
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     7745 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/mfc/alchemy/qrank/glassdoor.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)       21 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/version.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/seleya/utilities/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/utilities/__init__.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      399 2023-01-05 01:44:08.000000 Finance-Seleya-1.1.2/seleya/utilities/warning.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     3293 2023-01-05 01:44:08.000000 Finance-Seleya-1.1.2/seleya/utilities/api_base.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      418 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/utilities/exceptions.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     5108 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/seleya/utilities/kd_logger.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      490 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/seleya/utilities/singleton.py
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      114 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/MANIFEST.in
--rw-rw-r--   0 kerry     (1000) kerry     (1000)     3338 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/setup.py
-drwxrwxr-x   0 kerry     (1000) kerry     (1000)        0 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/requirements/
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      212 2023-03-14 07:38:51.000000 Finance-Seleya-1.1.2/requirements/py3.txt
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        0 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/requirements/py2.txt
--rw-rw-r--   0 kerry     (1000) kerry     (1000)       38 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/setup.cfg
--rw-rw-r--   0 kerry     (1000) kerry     (1000)        9 2022-06-28 13:50:38.000000 Finance-Seleya-1.1.2/README.md
--rw-rw-r--   0 kerry     (1000) kerry     (1000)      222 2023-03-14 07:39:33.000000 Finance-Seleya-1.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3083 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/Finance_Seleya.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      190 2023-06-24 10:22:53.000000 Finance-Seleya-1.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        9 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/requirements/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/requirements/py2.txt
+-rw-r--r--   0 root         (0) root         (0)      212 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.3/requirements/py3.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/Toolset/
+-rw-r--r--   0 root         (0) root         (0)      107 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/Toolset/audit/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/audit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/Toolset/audit/esg_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3486 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/Toolset/blob_service.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/calendar.py
+-rw-r--r--   0 root         (0) root         (0)     7223 2023-02-23 08:27:43.000000 Finance-Seleya-1.1.3/seleya/Toolset/file_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/Toolset/portfolio/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/portfolio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/Toolset/portfolio/esg_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/Toolset/tests/
+-rw-r--r--   0 root         (0) root         (0)       24 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      632 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/tests/runner.py
+-rw-r--r--   0 root         (0) root         (0)      244 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/tests/suite.py
+-rw-r--r--   0 root         (0) root         (0)     5733 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/Toolset/translator.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/config/default_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.3/seleya/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.3/seleya/core/env.py
+-rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.3/seleya/core/fixes.py
+-rw-r--r--   0 root         (0) root         (0)     7809 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.3/seleya/core/helper.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.3/seleya/core/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/ESG.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/GD.py
+-rw-r--r--   0 root         (0) root         (0)     4296 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/SEARCH.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/USER.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      599 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/http/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/mongo/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/mongo/fetch_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/mongo/mongodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36127 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/db_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7397 2023-04-17 00:03:09.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/sly/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/sly/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55584 2023-07-04 06:39:24.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/sly/sly_engine.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/DataAPI/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-02-28 12:53:15.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-03-03 01:31:51.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/engine.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-02-28 10:24:23.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py
+-rw-r--r--   0 root         (0) root         (0)      877 2023-02-28 12:26:53.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-03-28 11:57:26.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-03-02 23:18:44.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/basic.py
+-rw-r--r--   0 root         (0) root         (0)      626 2023-03-01 14:55:21.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-03-02 23:18:57.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/company.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-03-02 01:54:52.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py
+-rw-r--r--   0 root         (0) root         (0)      525 2023-03-02 02:20:33.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-03-30 06:02:56.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/engine.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/feature_importance.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/gd_overview.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-03-28 12:22:57.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-03-28 12:11:51.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/industry.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2023-03-16 08:51:54.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/sector.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/mfc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/
+-rw-r--r--   0 root         (0) root         (0)      284 2023-03-16 07:14:16.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/qrank/
+-rwxr-xr-x   0 root         (0) root         (0)   145856 2023-06-24 10:17:00.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/qrank/glassdoo.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0 root         (0) root         (0)   504608 2023-06-24 10:13:04.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/qrank/glassdoor.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/sbti/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 14:22:17.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/sbti/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22737 2023-04-02 13:21:46.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/sbti/emission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7878 2023-03-17 00:13:38.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/aerosol.py
+-rw-r--r--   0 root         (0) root         (0)    11460 2023-03-10 06:20:30.000000 Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/s2f.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/mfc/micro/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 13:27:54.000000 Finance-Seleya-1.1.3/seleya/mfc/micro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      132 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/seleya.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/seleya/utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/utilities/api_base.py
+-rw-r--r--   0 root         (0) root         (0)      418 2023-03-03 01:22:19.000000 Finance-Seleya-1.1.3/seleya/utilities/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.3/seleya/utilities/kd_logger.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/utilities/singleton.py
+-rw-r--r--   0 root         (0) root         (0)      399 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.3/seleya/utilities/warning.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 06:28:45.000000 Finance-Seleya-1.1.3/seleya/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 06:39:59.000000 Finance-Seleya-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3338 2023-06-24 15:02:35.000000 Finance-Seleya-1.1.3/setup.py
```

### Comparing `Finance-Seleya-1.1.2/Finance_Seleya.egg-info/SOURCES.txt` & `Finance-Seleya-1.1.3/Finance_Seleya.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,25 +62,28 @@
 seleya/data/SurfaceAPI/sqlatom/company.py
 seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py
 seleya/data/SurfaceAPI/sqlatom/emission_score_average.py
 seleya/data/SurfaceAPI/sqlatom/engine.py
 seleya/data/SurfaceAPI/sqlatom/feature_importance.py
 seleya/data/SurfaceAPI/sqlatom/gd_overview.py
 seleya/data/SurfaceAPI/sqlatom/gd_reviews.py
+seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py
 seleya/data/SurfaceAPI/sqlatom/industry.py
 seleya/data/SurfaceAPI/sqlatom/metrics.py
 seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
 seleya/data/SurfaceAPI/sqlatom/sector.py
 seleya/mfc/__init__.py
 seleya/mfc/alchemy/__init__.py
-seleya/mfc/alchemy/qrank/__init__.py
+seleya/mfc/alchemy/qrank/glassdoo.cpython-37m-x86_64-linux-gnu.so
 seleya/mfc/alchemy/qrank/glassdoor.c
-seleya/mfc/alchemy/qrank/glassdoor.py
+seleya/mfc/alchemy/sbti/__init__.py
+seleya/mfc/alchemy/sbti/emission.py
 seleya/mfc/alchemy/tsi/__init__.py
 seleya/mfc/alchemy/tsi/aerosol.py
 seleya/mfc/alchemy/tsi/s2f.py
+seleya/mfc/micro/__init__.py
 seleya/utilities/__init__.py
 seleya/utilities/api_base.py
 seleya/utilities/exceptions.py
 seleya/utilities/kd_logger.py
 seleya/utilities/singleton.py
 seleya/utilities/warning.py
```

### Comparing `Finance-Seleya-1.1.2/seleya/__init__.py` & `Finance-Seleya-1.1.3/seleya/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/core/parallel.py` & `Finance-Seleya-1.1.3/seleya/core/parallel.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/core/helper.py` & `Finance-Seleya-1.1.3/seleya/core/helper.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/core/env.py` & `Finance-Seleya-1.1.3/seleya/core/env.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/core/fixes.py` & `Finance-Seleya-1.1.3/seleya/core/fixes.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/Toolset/file_util.py` & `Finance-Seleya-1.1.3/seleya/Toolset/file_util.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/Toolset/tests/runner.py` & `Finance-Seleya-1.1.3/seleya/Toolset/tests/runner.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/Toolset/blob_service.py` & `Finance-Seleya-1.1.3/seleya/Toolset/blob_service.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/Toolset/portfolio/esg_metrics.py` & `Finance-Seleya-1.1.3/seleya/Toolset/portfolio/esg_metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/Toolset/calendar.py` & `Finance-Seleya-1.1.3/seleya/Toolset/calendar.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/Toolset/audit/esg_metrics.py` & `Finance-Seleya-1.1.3/seleya/Toolset/audit/esg_metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/Toolset/translator.py` & `Finance-Seleya-1.1.3/seleya/Toolset/translator.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/engine.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/mongo/basic.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/mongo/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/feature_importance.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/feature_importance.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/company.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/company.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/industry.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/industry.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,35 @@
         clause_list = [
             self._table_model.sector_id.in_(sector_code),
             self._table_model.industry.in_(industry),
             self._table_model.is_primary.in_(is_primary),
         ]
         return self.customize(clause_list=clause_list, columns=columns)
 
+    def unique_industry(self, industry='SICS', is_primary=1):
+        industry = self._transform_list(industry)
+        is_primary = self._transform_list(is_primary)
+        clause_list = [
+            self._table_model.is_primary.in_(is_primary),
+            self._table_model.industry.in_(industry)
+        ]
+        return self.customize(clause_list=clause_list,
+                              columns=['industry_id1'])
+
+    def extract(self, codes, industry='SICS', is_primary=1, columns=None):
+        codes = self._transform_list(codes)
+        industry = self._transform_list(industry)
+        is_primary = self._transform_list(is_primary)
+        clause_list = [
+            self._table_model.code.in_(codes),
+            self._table_model.industry.in_(industry),
+            self._table_model.is_primary.in_(is_primary),
+        ]
+        return self.customize(clause_list=clause_list, columns=columns)
+
     def fetch(self,
               industry_code,
               industry='SICS',
               is_primary=1,
               columns=None):
         industry_code = self._transform_list(industry_code)
         industry = self._transform_list(industry)
```

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/engine.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,26 +16,30 @@
 
     def client(self):
         return self._engine.sql_engine()
 
     def table_model(self, name):
         return self._base.classes[name]
 
+    def table_models(self):
+        return self._base.classes
+
     def show_indexs(self, name):
         indexs = [ins['column_names'] for ins in self._insp.get_indexes(name)]
         return list(set(itertools.chain.from_iterable(indexs)))
 
     def customize(self, table, clause_list, columns=None):
         new_list = and_(table.__dict__['flag'] == 1,
                         table.__dict__['flag'].isnot(None))
         indices = self.show_indexs(table.__name__)
         for clause in clause_list:
             if clause.left.name in indices:
                 new_list.append(clause)
             else:
-                raise SQLException("{0} not indices".format(clause.left.name))
+                raise SQLException("table:{0} {1} not indices".format(
+                    table.__name__, clause.left.name))
         if len(new_list) <= 2:
             kd_logger.error("unconditional query is not allowed")
             return pd.DataFrame()
         return super(FetchKDEngine, self).customize(table=table,
                                                     clause_list=new_list,
                                                     columns=columns)
```

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/sector.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/sector.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/basic.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/SurfaceAPI/sqlatom/metrics.py` & `Finance-Seleya-1.1.3/seleya/data/SurfaceAPI/sqlatom/metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # -*- coding: utf-8 -*-
+import pdb
 import pandas as pd
 import numpy as np
 from sqlalchemy import select, and_, outerjoin
+from seleya.data.SurfaceAPI.sqlatom.basic import Basic
+from seleya.data.SurfaceAPI.sqlatom.engine import FetchKDEngine
 
 
-class Metrics(object):
+class Metrics(Basic):
 
     def __init__(self):
+        self._engine = FetchKDEngine()
         self._metrcis_table = [
-            self._engine.table_model[k]
-            for k in self._engine.table_model.keys() if 'esg_metrics' in k
+            self._engine.table_models()[k]
+            for k in self._engine.table_models().keys() if 'esg_metrics' in k
         ]
 
     def _map_metrics(self,
                      metrics,
                      used_metric_tables,
                      diff_columns={'date', 'code'}):
         metrics_cols = {}
-        factors = set(factors).difference({'date', 'code'})
-        to_keep = factors.copy()
-        for f in factors:
+        metrics = set(metrics).difference({'date', 'code'})
+        to_keep = metrics.copy()
+        for f in metrics:
             for t in used_metric_tables:
                 if f in t.__table__.columns:
                     metrics_cols[t.__table__.columns[f]] = t
                     to_keep.remove(f)
                     break
 
         if to_keep:
-            raise ValueError("factors in <{0}> can't be find".format(to_keep))
+            raise ValueError("metrics in <{0}> can't be find".format(to_keep))
 
         return metrics_cols
 
     def fetch(self, codes, begin_date, end_date, columns):
         metrics_cols = self._map_metrics(columns, self._metrcis_table)
         joined_tables = set()
         metrics_tables = list(set(metrics_cols.values()))
@@ -52,10 +56,10 @@
         clause_list = and_(
             metrics_tables[0].flag == 1, metrics_tables[0].code.in_(codes),
             metrics_tables[0].date.between(begin_date, end_date))
 
         query = select([metrics_tables[0].date, metrics_tables[0].code] +
                        list(metrics_cols.keys())).select_from(big_table).where(
                            clause_list)
-        return self.custom(query).drop_duplicates(
+        return pd.read_sql(query, self._engine.client()).drop_duplicates(
             subset=['date', 'code']).replace(
                 [-np.inf, np.inf], np.nan).sort_values(by=['date', 'code'])
```

### Comparing `Finance-Seleya-1.1.2/seleya/data/DataAPI/mongo/mongodb.py` & `Finance-Seleya-1.1.3/seleya/data/DataAPI/mongo/mongodb.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/DataAPI/http/USER.py` & `Finance-Seleya-1.1.3/seleya/data/DataAPI/http/USER.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/DataAPI/http/SEARCH.py` & `Finance-Seleya-1.1.3/seleya/data/DataAPI/http/SEARCH.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/DataAPI/http/utils.py` & `Finance-Seleya-1.1.3/seleya/data/DataAPI/http/utils.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/DataAPI/http/GD.py` & `Finance-Seleya-1.1.3/seleya/data/DataAPI/http/GD.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/DataAPI/http/ESG.py` & `Finance-Seleya-1.1.3/seleya/data/DataAPI/http/ESG.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/data/DataAPI/sqlatom/sly/sly_engine.py` & `Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/sly/sly_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1150,15 +1150,15 @@
                     and_(basetable.code == t.code, basetable.date == t.date,
                          t.flag == 1))
         else:
             basetable = list(set(factor_cols.values()))[0]
             bigtable = None
 
         calause = and_(basetable.code.in_(codes), basetable.date >= begin_date,
-                       basetable.date <= end_date)
+                       basetable.date <= end_date, basetable.flag == 1)
 
         if bigtable is None:
             query = select(
                 [basetable.date, basetable.code, basetable.quarter] +
                 list(factor_cols.keys())).where(calause)
         else:
             query = select(
```

### Comparing `Finance-Seleya-1.1.2/seleya/data/DataAPI/sqlatom/db_factory.py` & `Finance-Seleya-1.1.3/seleya/data/DataAPI/sqlatom/db_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/mfc/alchemy/tsi/s2f.py` & `Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/s2f.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/mfc/alchemy/tsi/aerosol.py` & `Finance-Seleya-1.1.3/seleya/mfc/alchemy/tsi/aerosol.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,22 +157,22 @@
             factor_columns = industry_weighted.column_name.unique().tolist()
             clean_dt = clean_data[clean_data['industry_id1'] == industry]
             industry_weighted = industry_weighted.set_index(
                 ['date', 'column_name'])['importance'].unstack()
             industry_data = clean_dt[['date', 'code'] + factor_columns].merge(
                 industry_weighted, on=['date'], suffixes=('', '_w'))
             w_list = [f + '_w' for f in factor_columns]
-            industry_data['score'] = (
-                (2 * industry_data[factor_columns].fillna(0).values - 1) *
-                industry_data[w_list].fillna(0).values * 5).sum(axis=1)
-
             industry_data[factor_columns] = (
                 (2 * industry_data[factor_columns].values - 1) *
                 industry_data[w_list].values * 5)
+
+            industry_data['score'] = industry_data[factor_columns].fillna(
+                0).sum(axis=1)
             industry_data['industry'] = industry
+
             res[industry] = industry_data.drop(w_list, axis=1)
         return res
 
     def run(self, begin_date, end_date, threshold=0.5):
         total_data, feature_data = self.prepare_data(begin_date=begin_date,
                                                      end_date=end_date)
```

### Comparing `Finance-Seleya-1.1.2/seleya/mfc/alchemy/qrank/glassdoor.c` & `Finance-Seleya-1.1.3/seleya/mfc/alchemy/qrank/glassdoor.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.5 */
+/* Generated by Cython 0.29.21 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "seleya.mfc.alchemy.qrank.glassdoo",
         "sources": [
             "seleya/mfc/alchemy/qrank/glassdoor.py"
@@ -15,16 +15,16 @@
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_5"
-#define CYTHON_HEX_VERSION 0x001D05F0
+#define CYTHON_ABI "0_29_21"
+#define CYTHON_HEX_VERSION 0x001D15F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -318,16 +318,21 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
+#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
+  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+#else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+#endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
@@ -438,15 +443,19 @@
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #else
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -487,26 +496,35 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
+#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
+#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -538,15 +556,15 @@
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -579,19 +597,18 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-
+#define __PYX_MARK_ERR_POS(f_index, lineno) \
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-{ \
-  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
-}
+    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -608,15 +625,16 @@
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
 
 typedef struct {PyObject **p; const char *s; const Py_ssize_t n; const char* encoding;
                 const char is_unicode; const char is_str; const char intern; } __Pyx_StringTabEntry;
 
 #define __PYX_DEFAULT_STRING_ENCODING_IS_ASCII 0
-#define __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT 0
+#define __PYX_DEFAULT_STRING_ENCODING_IS_UTF8 0
+#define __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT (PY_MAJOR_VERSION >= 3 && __PYX_DEFAULT_STRING_ENCODING_IS_UTF8)
 #define __PYX_DEFAULT_STRING_ENCODING ""
 #define __Pyx_PyObject_FromString __Pyx_PyBytes_FromString
 #define __Pyx_PyObject_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
 #define __Pyx_uchar_cast(c) ((unsigned char)c)
 #define __Pyx_long_cast(x) ((long)x)
 #define __Pyx_fits_Py_ssize_t(v, type, is_signed)  (\
     (sizeof(type) < sizeof(Py_ssize_t))  ||\
@@ -811,42 +829,42 @@
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews;
 struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute;
 struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result;
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":41
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
 struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews {
   PyObject_HEAD
   PyObject *__pyx_v_self;
 };
 
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":117
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
 struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute {
   PyObject_HEAD
   PyObject *__pyx_v_res;
   PyObject *__pyx_v_self;
 };
 
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":151
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
 struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result {
@@ -949,15 +967,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
 #else
 #define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
 #define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
 #endif
 
 /* PyDictVersioning.proto */
-#if CYTHON_USE_DICT_VERSIONS
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP) {\
     static PY_UINT64_T __pyx_dict_version = 0;\
@@ -1007,15 +1025,15 @@
 #endif
 
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
 #if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs);
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
 #else
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
@@ -1085,15 +1103,15 @@
 
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
-/* CythonFunction.proto */
+/* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
 #define __Pyx_CYFUNCTION_CCLASS        0x04
 #define __Pyx_CyFunction_GetClosure(f)\
     (((__pyx_CyFunctionObject *) (f))->func_closure)
 #define __Pyx_CyFunction_GetClassObj(f)\
@@ -1113,25 +1131,24 @@
     PyObject *func_doc;
     PyObject *func_globals;
     PyObject *func_code;
     PyObject *func_closure;
     PyObject *func_classobj;
     void *defaults;
     int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
 } __pyx_CyFunctionObject;
 static PyTypeObject *__pyx_CyFunctionType = 0;
 #define __Pyx_CyFunction_Check(obj)  (__Pyx_TypeCheck(obj, __pyx_CyFunctionType))
-#define __Pyx_CyFunction_NewEx(ml, flags, qualname, self, module, globals, code)\
-    __Pyx_CyFunction_New(__pyx_CyFunctionType, ml, flags, qualname, self, module, globals, code)
-static PyObject *__Pyx_CyFunction_New(PyTypeObject *, PyMethodDef *ml,
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *self,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
                                                          size_t size,
                                                          int pyobjects);
@@ -1139,14 +1156,21 @@
                                                             PyObject *tuple);
 static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
                                                              PyObject *dict);
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
                                                               PyObject *dict);
 static int __pyx_CyFunction_init(void);
 
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
@@ -1158,15 +1182,15 @@
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        Py_SIZE(list) = len+1;
+        __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
@@ -1186,15 +1210,15 @@
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        Py_SIZE(list) = len+1;
+        __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
@@ -1363,14 +1387,15 @@
 static const char __pyx_k__14[] = "_";
 static const char __pyx_k_cid[] = "cid";
 static const char __pyx_k_col[] = "col";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_how[] = "how";
 static const char __pyx_k_idx[] = "idx";
 static const char __pyx_k_nan[] = "nan";
+static const char __pyx_k_pdb[] = "pdb";
 static const char __pyx_k_ppf[] = "ppf";
 static const char __pyx_k_res[] = "res";
 static const char __pyx_k_run[] = "run";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_axis[] = "axis";
 static const char __pyx_k_cids[] = "cids";
 static const char __pyx_k_code[] = "code";
@@ -1438,15 +1463,14 @@
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_rankdata[] = "rankdata";
 static const char __pyx_k_raw_data[] = "raw_data";
 static const char __pyx_k_reviewId[] = "reviewId";
 static const char __pyx_k_strftime[] = "strftime";
 static const char __pyx_k_DataFrame[] = "DataFrame";
 static const char __pyx_k_GDOveriew[] = "GDOveriew";
-static const char __pyx_k_GDReviews[] = "GDReviews";
 static const char __pyx_k_Glassdoor[] = "Glassdoor";
 static const char __pyx_k_col_score[] = "col_score";
 static const char __pyx_k_dist_data[] = "dist_data";
 static const char __pyx_k_droplevel[] = "droplevel";
 static const char __pyx_k_kd_logger[] = "kd_logger";
 static const char __pyx_k_mean_cols[] = "_mean_cols";
 static const char __pyx_k_mean_data[] = "mean_data";
@@ -1469,14 +1493,15 @@
 static const char __pyx_k_sort_values[] = "sort_values";
 static const char __pyx_k_to_datetime[] = "to_datetime";
 static const char __pyx_k_SurfaceDBAPI[] = "SurfaceDBAPI";
 static const char __pyx_k_factors_sets[] = "_factors_sets";
 static const char __pyx_k_industry_id1[] = "industry_id1";
 static const char __pyx_k_mapping_dict[] = "_mapping_dict";
 static const char __pyx_k_prepare_data[] = "prepare_data";
+static const char __pyx_k_GDReviewsBase[] = "GDReviewsBase";
 static const char __pyx_k_Glassdoor_run[] = "Glassdoor.run";
 static const char __pyx_k_count_nonzero[] = "count_nonzero";
 static const char __pyx_k_fetch_reviews[] = "_fetch_reviews";
 static const char __pyx_k_industry_code[] = "industry_code";
 static const char __pyx_k_industry_data[] = "industry_data";
 static const char __pyx_k_ratingOverall[] = "ratingOverall";
 static const char __pyx_k_transform_raw[] = "_transform_raw";
@@ -1491,14 +1516,15 @@
 static const char __pyx_k_Glassdoor___init[] = "Glassdoor.__init__";
 static const char __pyx_k_calculate_result[] = "calculate_result";
 static const char __pyx_k_gd_overview_data[] = "gd_overview_data";
 static const char __pyx_k_probability_cols[] = "_probability_cols";
 static const char __pyx_k_raw_data_is_empty[] = "raw data is empty";
 static const char __pyx_k_ultron_sentry_api[] = "ultron.sentry.api";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_calculating_success[] = "calculating success...";
 static const char __pyx_k_calculate_distribute[] = "_calculate_distribute";
 static const char __pyx_k_Glassdoor__blom_score[] = "Glassdoor._blom_score";
 static const char __pyx_k_Glassdoor__distribute[] = "Glassdoor._distribute";
 static const char __pyx_k_Glassdoor__percentile[] = "Glassdoor._percentile";
 static const char __pyx_k_ratingBusinessOutlook[] = "ratingBusinessOutlook";
 static const char __pyx_k_ratingWorkLifeBalance[] = "ratingWorkLifeBalance";
 static const char __pyx_k_Fetching_industry_data[] = "Fetching industry data...";
@@ -1536,15 +1562,15 @@
 static PyObject *__pyx_n_s_CSQuantiles;
 static PyObject *__pyx_n_s_DISAPPROVE;
 static PyObject *__pyx_n_s_DataFrame;
 static PyObject *__pyx_kp_s_Fetching_glassdoor_overview_data;
 static PyObject *__pyx_kp_s_Fetching_glassdoor_reviews_data;
 static PyObject *__pyx_kp_s_Fetching_industry_data;
 static PyObject *__pyx_n_s_GDOveriew;
-static PyObject *__pyx_n_s_GDReviews;
+static PyObject *__pyx_n_s_GDReviewsBase;
 static PyObject *__pyx_n_s_Glassdoor;
 static PyObject *__pyx_n_s_Glassdoor___init;
 static PyObject *__pyx_n_s_Glassdoor__blom_score;
 static PyObject *__pyx_n_s_Glassdoor__calculate_distribute;
 static PyObject *__pyx_n_s_Glassdoor__distribute;
 static PyObject *__pyx_n_s_Glassdoor__distribute_locals_lam;
 static PyObject *__pyx_n_s_Glassdoor__fetch_overview;
@@ -1577,14 +1603,15 @@
 static PyObject *__pyx_n_s_begin_date;
 static PyObject *__pyx_n_s_blom_score;
 static PyObject *__pyx_n_s_by;
 static PyObject *__pyx_n_s_calculate_distribute;
 static PyObject *__pyx_n_s_calculate_result;
 static PyObject *__pyx_kp_s_calculating_blom_score;
 static PyObject *__pyx_kp_s_calculating_distribute;
+static PyObject *__pyx_kp_s_calculating_success;
 static PyObject *__pyx_n_s_category_field;
 static PyObject *__pyx_n_s_cid;
 static PyObject *__pyx_n_s_cids;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_code;
 static PyObject *__pyx_n_s_codes;
 static PyObject *__pyx_n_s_col;
@@ -1653,14 +1680,15 @@
 static PyObject *__pyx_n_s_norm;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_n_s_object;
 static PyObject *__pyx_n_s_on;
 static PyObject *__pyx_n_s_pandas;
 static PyObject *__pyx_n_s_pd;
+static PyObject *__pyx_n_s_pdb;
 static PyObject *__pyx_n_s_percentile;
 static PyObject *__pyx_n_s_ppf;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_prepare_data;
 static PyObject *__pyx_n_s_probability_cols;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_range;
@@ -1763,29 +1791,32 @@
 static PyObject *__pyx_codeobj__21;
 static PyObject *__pyx_codeobj__23;
 static PyObject *__pyx_codeobj__25;
 static PyObject *__pyx_codeobj__27;
 static PyObject *__pyx_codeobj__30;
 /* Late includes */
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":12
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":13
  * class Glassdoor(object):
  * 
  *     def __init__(self, industry_code):             # <<<<<<<<<<<<<<
  *         self._industry_code = industry_code
  *         self._mapping_dict = {
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor___init__[] = "Glassdoor.__init__(self, industry_code)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor___init__};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_industry_code = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_industry_code,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -1804,32 +1835,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_industry_code)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 12, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 13, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 12, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 13, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_industry_code = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 12, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 13, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor___init__(__pyx_self, __pyx_v_self, __pyx_v_industry_code);
 
@@ -1840,80 +1871,83 @@
 
 static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_industry_code) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":13
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":14
  * 
  *     def __init__(self, industry_code):
  *         self._industry_code = industry_code             # <<<<<<<<<<<<<<
  *         self._mapping_dict = {
  *             'NO_OPINION': 0,
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2, __pyx_v_industry_code) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2, __pyx_v_industry_code) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":15
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":16
  *         self._industry_code = industry_code
  *         self._mapping_dict = {
  *             'NO_OPINION': 0,             # <<<<<<<<<<<<<<
  *             'NEGATIVE': -1,
  *             'POSITIVE': 1,
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_NO_OPINION, __pyx_int_0) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_NEGATIVE, __pyx_int_neg_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_POSITIVE, __pyx_int_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_NEUTRAL, __pyx_int_0) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_APPROVE, __pyx_int_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_DISAPPROVE, __pyx_int_neg_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_NO_OPINION, __pyx_int_0) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_NEGATIVE, __pyx_int_neg_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_POSITIVE, __pyx_int_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_NEUTRAL, __pyx_int_0) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_APPROVE, __pyx_int_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_DISAPPROVE, __pyx_int_neg_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":14
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":15
  *     def __init__(self, industry_code):
  *         self._industry_code = industry_code
  *         self._mapping_dict = {             # <<<<<<<<<<<<<<
  *             'NO_OPINION': 0,
  *             'NEGATIVE': -1,
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_mapping_dict, __pyx_t_1) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_mapping_dict, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":22
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":23
  *             'DISAPPROVE': -1
  *         }
  *         self._probability_cols = [             # <<<<<<<<<<<<<<
  *             'ratingBusinessOutlook', 'ratingRecommendToFriend', 'ratingCeo'
  *         ]
  */
-  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_ratingBusinessOutlook);
   __Pyx_GIVEREF(__pyx_n_s_ratingBusinessOutlook);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_ratingBusinessOutlook);
   __Pyx_INCREF(__pyx_n_s_ratingRecommendToFriend);
   __Pyx_GIVEREF(__pyx_n_s_ratingRecommendToFriend);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_ratingRecommendToFriend);
   __Pyx_INCREF(__pyx_n_s_ratingCeo);
   __Pyx_GIVEREF(__pyx_n_s_ratingCeo);
   PyList_SET_ITEM(__pyx_t_1, 2, __pyx_n_s_ratingCeo);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_probability_cols, __pyx_t_1) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_probability_cols, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":25
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":26
  *             'ratingBusinessOutlook', 'ratingRecommendToFriend', 'ratingCeo'
  *         ]
  *         self._mean_cols = [             # <<<<<<<<<<<<<<
  *             'ratingWorkLifeBalance', 'ratingCultureAndValues',
  *             'ratingSeniorLeadership', 'ratingCareerOpportunities',
  */
-  __pyx_t_1 = PyList_New(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_ratingWorkLifeBalance);
   __Pyx_GIVEREF(__pyx_n_s_ratingWorkLifeBalance);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_ratingWorkLifeBalance);
   __Pyx_INCREF(__pyx_n_s_ratingCultureAndValues);
   __Pyx_GIVEREF(__pyx_n_s_ratingCultureAndValues);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_ratingCultureAndValues);
@@ -1928,36 +1962,36 @@
   PyList_SET_ITEM(__pyx_t_1, 4, __pyx_n_s_ratingOverall);
   __Pyx_INCREF(__pyx_n_s_ratingCompensationAndBenefits);
   __Pyx_GIVEREF(__pyx_n_s_ratingCompensationAndBenefits);
   PyList_SET_ITEM(__pyx_t_1, 5, __pyx_n_s_ratingCompensationAndBenefits);
   __Pyx_INCREF(__pyx_n_s_ratingDiversityAndInclusion);
   __Pyx_GIVEREF(__pyx_n_s_ratingDiversityAndInclusion);
   PyList_SET_ITEM(__pyx_t_1, 6, __pyx_n_s_ratingDiversityAndInclusion);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_mean_cols, __pyx_t_1) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_mean_cols, __pyx_t_1) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":31
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":32
  *             'ratingDiversityAndInclusion'
  *         ]
  *         self._factors_sets = self._probability_cols + self._mean_cols             # <<<<<<<<<<<<<<
  * 
  *     def _fetch_overview(self, codes):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_probability_cols); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_probability_cols); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_mean_cols); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_mean_cols); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_factors_sets, __pyx_t_3) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_factors_sets, __pyx_t_3) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":12
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":13
  * class Glassdoor(object):
  * 
  *     def __init__(self, industry_code):             # <<<<<<<<<<<<<<
  *         self._industry_code = industry_code
  *         self._mapping_dict = {
  */
 
@@ -1972,29 +2006,32 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":33
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":34
  *         self._factors_sets = self._probability_cols + self._mean_cols
  * 
  *     def _fetch_overview(self, codes):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_2_fetch_overview[] = "Glassdoor._fetch_overview(self, codes)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview = {"_fetch_overview", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_2_fetch_overview};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_codes = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_fetch_overview (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_codes,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -2013,32 +2050,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_codes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_fetch_overview", 1, 2, 2, 1); __PYX_ERR(0, 33, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_fetch_overview", 1, 2, 2, 1); __PYX_ERR(0, 34, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_fetch_overview") < 0)) __PYX_ERR(0, 33, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_fetch_overview") < 0)) __PYX_ERR(0, 34, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_codes = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_fetch_overview", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 33, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_fetch_overview", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 34, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._fetch_overview", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_2_fetch_overview(__pyx_self, __pyx_v_self, __pyx_v_codes);
 
@@ -2050,169 +2087,172 @@
 static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_2_fetch_overview(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_codes) {
   PyObject *__pyx_v_gd_overview_data = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_fetch_overview", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":34
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":35
  * 
  *     def _fetch_overview(self, codes):
  *         kd_logger.info('Fetching glassdoor overview data...')             # <<<<<<<<<<<<<<
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  *             codes=codes, columns=['code', 'cid'])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_Fetching_glassdoor_overview_data) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_Fetching_glassdoor_overview_data);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":35
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":36
  *     def _fetch_overview(self, codes):
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(             # <<<<<<<<<<<<<<
  *             codes=codes, columns=['code', 'cid'])
  *         gd_overview_data = gd_overview_data[['cid', 'code'
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SurfaceDBAPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SurfaceDBAPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_GDOveriew); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_GDOveriew); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_fetch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_fetch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":36
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":37
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  *             codes=codes, columns=['code', 'cid'])             # <<<<<<<<<<<<<<
  *         gd_overview_data = gd_overview_data[['cid', 'code'
  *                                              ]].drop_duplicates(subset=['cid'])
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_codes, __pyx_v_codes) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
-  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_codes, __pyx_v_codes) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_code);
   __Pyx_GIVEREF(__pyx_n_s_code);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_code);
   __Pyx_INCREF(__pyx_n_s_cid);
   __Pyx_GIVEREF(__pyx_n_s_cid);
   PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_cid);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_columns, __pyx_t_3) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_columns, __pyx_t_3) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":35
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":36
  *     def _fetch_overview(self, codes):
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(             # <<<<<<<<<<<<<<
  *             codes=codes, columns=['code', 'cid'])
  *         gd_overview_data = gd_overview_data[['cid', 'code'
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_gd_overview_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":37
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":38
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  *             codes=codes, columns=['code', 'cid'])
  *         gd_overview_data = gd_overview_data[['cid', 'code'             # <<<<<<<<<<<<<<
  *                                              ]].drop_duplicates(subset=['cid'])
  *         return gd_overview_data
  */
-  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_cid);
   __Pyx_GIVEREF(__pyx_n_s_cid);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_cid);
   __Pyx_INCREF(__pyx_n_s_code);
   __Pyx_GIVEREF(__pyx_n_s_code);
   PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_code);
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_gd_overview_data, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_gd_overview_data, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":38
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":39
  *             codes=codes, columns=['code', 'cid'])
  *         gd_overview_data = gd_overview_data[['cid', 'code'
  *                                              ]].drop_duplicates(subset=['cid'])             # <<<<<<<<<<<<<<
  *         return gd_overview_data
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_drop_duplicates); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_drop_duplicates); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_cid);
   __Pyx_GIVEREF(__pyx_n_s_cid);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_cid);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_subset, __pyx_t_2) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_subset, __pyx_t_2) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_gd_overview_data, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":39
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":40
  *         gd_overview_data = gd_overview_data[['cid', 'code'
  *                                              ]].drop_duplicates(subset=['cid'])
  *         return gd_overview_data             # <<<<<<<<<<<<<<
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_gd_overview_data);
   __pyx_r = __pyx_v_gd_overview_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":33
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":34
  *         self._factors_sets = self._probability_cols + self._mean_cols
  * 
  *     def _fetch_overview(self, codes):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  */
 
@@ -2226,15 +2266,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_gd_overview_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":41
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
 
@@ -2243,14 +2283,17 @@
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_4_fetch_reviews[] = "Glassdoor._fetch_reviews(self, begin_date, end_date, cids)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_5_fetch_reviews = {"_fetch_reviews", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_5_fetch_reviews, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_4_fetch_reviews};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_5_fetch_reviews(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_begin_date = 0;
   PyObject *__pyx_v_end_date = 0;
   PyObject *__pyx_v_cids = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_fetch_reviews (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_begin_date,&__pyx_n_s_end_date,&__pyx_n_s_cids,0};
     PyObject* values[4] = {0,0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -2273,31 +2316,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_begin_date)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_fetch_reviews", 1, 4, 4, 1); __PYX_ERR(0, 41, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_fetch_reviews", 1, 4, 4, 1); __PYX_ERR(0, 42, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end_date)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_fetch_reviews", 1, 4, 4, 2); __PYX_ERR(0, 41, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_fetch_reviews", 1, 4, 4, 2); __PYX_ERR(0, 42, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cids)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_fetch_reviews", 1, 4, 4, 3); __PYX_ERR(0, 41, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_fetch_reviews", 1, 4, 4, 3); __PYX_ERR(0, 42, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_fetch_reviews") < 0)) __PYX_ERR(0, 41, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_fetch_reviews") < 0)) __PYX_ERR(0, 42, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -2306,28 +2349,28 @@
     __pyx_v_self = values[0];
     __pyx_v_begin_date = values[1];
     __pyx_v_end_date = values[2];
     __pyx_v_cids = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_fetch_reviews", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 41, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_fetch_reviews", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 42, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._fetch_reviews", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_4_fetch_reviews(__pyx_self, __pyx_v_self, __pyx_v_begin_date, __pyx_v_end_date, __pyx_v_cids);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":54
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":56
  *         for col in self._probability_cols:
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])             # <<<<<<<<<<<<<<
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime'])
  */
 
@@ -2350,32 +2393,35 @@
   struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *__pyx_outer_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 0);
   __pyx_outer_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = (__pyx_v_x == Py_None);
   if ((__pyx_t_2 != 0)) {
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_nan); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_nan); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_1 = __pyx_t_4;
     __pyx_t_4 = 0;
   } else {
-    if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 54, __pyx_L1_error) }
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_mapping_dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
+    if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 56, __pyx_L1_error) }
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_mapping_dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
@@ -2390,15 +2436,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":41
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
 
@@ -2413,445 +2459,456 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   PyObject *(*__pyx_t_6)(PyObject *);
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_fetch_reviews", 0);
   __pyx_cur_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *)__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews(__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 41, __pyx_L1_error)
+    __PYX_ERR(0, 42, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":42
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":43
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):
  *         kd_logger.info('Fetching glassdoor reviews data...')             # <<<<<<<<<<<<<<
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  *                    ] + self._factors_sets
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_Fetching_glassdoor_reviews_data) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_Fetching_glassdoor_reviews_data);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":43
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":44
  *     def _fetch_reviews(self, begin_date, end_date, cids):
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'             # <<<<<<<<<<<<<<
  *                    ] + self._factors_sets
- *         gd_reviews_data = SurfaceDBAPI.GDReviews().fetch(begin_date=begin_date,
+ *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(
  */
-  __pyx_t_1 = PyList_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_id);
   __Pyx_GIVEREF(__pyx_n_s_id);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_id);
   __Pyx_INCREF(__pyx_n_s_cid);
   __Pyx_GIVEREF(__pyx_n_s_cid);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_cid);
   __Pyx_INCREF(__pyx_n_s_reviewId);
   __Pyx_GIVEREF(__pyx_n_s_reviewId);
   PyList_SET_ITEM(__pyx_t_1, 2, __pyx_n_s_reviewId);
   __Pyx_INCREF(__pyx_n_s_reviewDateTime);
   __Pyx_GIVEREF(__pyx_n_s_reviewDateTime);
   PyList_SET_ITEM(__pyx_t_1, 3, __pyx_n_s_reviewDateTime);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":44
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":45
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  *                    ] + self._factors_sets             # <<<<<<<<<<<<<<
- *         gd_reviews_data = SurfaceDBAPI.GDReviews().fetch(begin_date=begin_date,
- *                                                          end_date=end_date,
+ *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(
+ *             begin_date=begin_date,
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_factors_sets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_factors_sets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_columns = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":45
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":46
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  *                    ] + self._factors_sets
- *         gd_reviews_data = SurfaceDBAPI.GDReviews().fetch(begin_date=begin_date,             # <<<<<<<<<<<<<<
- *                                                          end_date=end_date,
- *                                                          cids=cids,
+ *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(             # <<<<<<<<<<<<<<
+ *             begin_date=begin_date,
+ *             end_date=end_date,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SurfaceDBAPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SurfaceDBAPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_GDReviews); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_GDReviewsBase); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_fetch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_fetch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_begin_date, __pyx_v_begin_date) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":46
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":47
  *                    ] + self._factors_sets
- *         gd_reviews_data = SurfaceDBAPI.GDReviews().fetch(begin_date=begin_date,
- *                                                          end_date=end_date,             # <<<<<<<<<<<<<<
- *                                                          cids=cids,
- *                                                          columns=columns)
+ *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(
+ *             begin_date=begin_date,             # <<<<<<<<<<<<<<
+ *             end_date=end_date,
+ *             cids=cids,
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_end_date, __pyx_v_end_date) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_begin_date, __pyx_v_begin_date) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":47
- *         gd_reviews_data = SurfaceDBAPI.GDReviews().fetch(begin_date=begin_date,
- *                                                          end_date=end_date,
- *                                                          cids=cids,             # <<<<<<<<<<<<<<
- *                                                          columns=columns)
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":48
+ *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(
+ *             begin_date=begin_date,
+ *             end_date=end_date,             # <<<<<<<<<<<<<<
+ *             cids=cids,
+ *             columns=columns)
+ */
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_end_date, __pyx_v_end_date) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":49
+ *             begin_date=begin_date,
+ *             end_date=end_date,
+ *             cids=cids,             # <<<<<<<<<<<<<<
+ *             columns=columns)
  *         if gd_reviews_data.empty:
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_cids, __pyx_v_cids) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_cids, __pyx_v_cids) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":48
- *                                                          end_date=end_date,
- *                                                          cids=cids,
- *                                                          columns=columns)             # <<<<<<<<<<<<<<
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":50
+ *             end_date=end_date,
+ *             cids=cids,
+ *             columns=columns)             # <<<<<<<<<<<<<<
  *         if gd_reviews_data.empty:
  *             return None
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_columns, __pyx_v_columns) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_columns, __pyx_v_columns) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":45
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":46
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  *                    ] + self._factors_sets
- *         gd_reviews_data = SurfaceDBAPI.GDReviews().fetch(begin_date=begin_date,             # <<<<<<<<<<<<<<
- *                                                          end_date=end_date,
- *                                                          cids=cids,
+ *         gd_reviews_data = SurfaceDBAPI.GDReviewsBase().fetch(             # <<<<<<<<<<<<<<
+ *             begin_date=begin_date,
+ *             end_date=end_date,
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_gd_reviews_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":49
- *                                                          cids=cids,
- *                                                          columns=columns)
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":51
+ *             cids=cids,
+ *             columns=columns)
  *         if gd_reviews_data.empty:             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_reviews_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_reviews_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":50
- *                                                          columns=columns)
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":52
+ *             columns=columns)
  *         if gd_reviews_data.empty:
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         for col in self._probability_cols:
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":49
- *                                                          cids=cids,
- *                                                          columns=columns)
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":51
+ *             cids=cids,
+ *             columns=columns)
  *         if gd_reviews_data.empty:             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":52
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":54
  *             return None
  * 
  *         for col in self._probability_cols:             # <<<<<<<<<<<<<<
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_probability_cols); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_probability_cols); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
     __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 52, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 54, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 52, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 54, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_6(__pyx_t_2);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 52, __pyx_L1_error)
+          else __PYX_ERR(0, 54, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_col, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":53
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":55
  * 
  *         for col in self._probability_cols:
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(             # <<<<<<<<<<<<<<
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  */
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_gd_reviews_data, __pyx_v_col); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_gd_reviews_data, __pyx_v_col); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_apply); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_apply); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":54
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":56
  *         for col in self._probability_cols:
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])             # <<<<<<<<<<<<<<
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime'])
  */
-    __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_fetch_reviews_lambda, 0, __pyx_n_s_Glassdoor__fetch_reviews_locals, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_fetch_reviews_lambda, 0, __pyx_n_s_Glassdoor__fetch_reviews_locals, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_1);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":53
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":55
  * 
  *         for col in self._probability_cols:
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(             # <<<<<<<<<<<<<<
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  */
-    if (unlikely(PyObject_SetItem(__pyx_v_gd_reviews_data, __pyx_v_col, __pyx_t_3) < 0)) __PYX_ERR(0, 53, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_gd_reviews_data, __pyx_v_col, __pyx_t_3) < 0)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":52
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":54
  *             return None
  * 
  *         for col in self._probability_cols:             # <<<<<<<<<<<<<<
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":55
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":57
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             gd_reviews_data['reviewDateTime'])
  *         gd_reviews_data['date'] = pd.to_datetime(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":56
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":58
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime'])             # <<<<<<<<<<<<<<
  *         gd_reviews_data['date'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime']).dt.strftime('%Y-12-31')
  */
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gd_reviews_data, __pyx_n_s_reviewDateTime); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gd_reviews_data, __pyx_n_s_reviewDateTime); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":55
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":57
  *             gd_reviews_data[col] = gd_reviews_data[col].apply(
  *                 lambda x: np.nan if x is None else self._mapping_dict[x])
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             gd_reviews_data['reviewDateTime'])
  *         gd_reviews_data['date'] = pd.to_datetime(
  */
-  if (unlikely(PyObject_SetItem(__pyx_v_gd_reviews_data, __pyx_n_s_reviewDateTime, __pyx_t_2) < 0)) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_gd_reviews_data, __pyx_n_s_reviewDateTime, __pyx_t_2) < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":57
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":59
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime'])
  *         gd_reviews_data['date'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             gd_reviews_data['reviewDateTime']).dt.strftime('%Y-12-31')
  *         return gd_reviews_data
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":58
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":60
  *             gd_reviews_data['reviewDateTime'])
  *         gd_reviews_data['date'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime']).dt.strftime('%Y-12-31')             # <<<<<<<<<<<<<<
  *         return gd_reviews_data
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gd_reviews_data, __pyx_n_s_reviewDateTime); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gd_reviews_data, __pyx_n_s_reviewDateTime); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_7 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_8, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_dt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_dt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_strftime); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_strftime); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_1, __pyx_kp_s_Y_12_31) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_s_Y_12_31);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":57
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":59
  *         gd_reviews_data['reviewDateTime'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime'])
  *         gd_reviews_data['date'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             gd_reviews_data['reviewDateTime']).dt.strftime('%Y-12-31')
  *         return gd_reviews_data
  */
-  if (unlikely(PyObject_SetItem(__pyx_v_gd_reviews_data, __pyx_n_s_date, __pyx_t_2) < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_gd_reviews_data, __pyx_n_s_date, __pyx_t_2) < 0)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":59
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":61
  *         gd_reviews_data['date'] = pd.to_datetime(
  *             gd_reviews_data['reviewDateTime']).dt.strftime('%Y-12-31')
  *         return gd_reviews_data             # <<<<<<<<<<<<<<
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_gd_reviews_data);
   __pyx_r = __pyx_v_gd_reviews_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":41
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
 
@@ -2870,15 +2927,15 @@
   __Pyx_XDECREF(__pyx_v_col);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":61
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":63
  *         return gd_reviews_data
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  */
 
@@ -2886,14 +2943,17 @@
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_6prepare_data[] = "Glassdoor.prepare_data(self, begin_date=None, end_date=None)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data = {"prepare_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_6prepare_data};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_begin_date = 0;
   PyObject *__pyx_v_end_date = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("prepare_data (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_begin_date,&__pyx_n_s_end_date,0};
     PyObject* values[3] = {0,0,0};
     values[1] = ((PyObject *)((PyObject *)Py_None));
@@ -2926,15 +2986,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end_date);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "prepare_data") < 0)) __PYX_ERR(0, 61, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "prepare_data") < 0)) __PYX_ERR(0, 63, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -2945,15 +3005,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_begin_date = values[1];
     __pyx_v_end_date = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("prepare_data", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 61, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("prepare_data", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 63, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.prepare_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_6prepare_data(__pyx_self, __pyx_v_self, __pyx_v_begin_date, __pyx_v_end_date);
 
@@ -2972,566 +3032,569 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("prepare_data", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":62
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":64
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):
  *         kd_logger.info('Fetching industry data...')             # <<<<<<<<<<<<<<
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  *             industry_code=self._industry_code,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_Fetching_industry_data) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_Fetching_industry_data);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":63
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":65
  *     def prepare_data(self, begin_date=None, end_date=None):
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(             # <<<<<<<<<<<<<<
  *             industry_code=self._industry_code,
  *             columns=['code', 'industry_id1'])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SurfaceDBAPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SurfaceDBAPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Industry); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Industry); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_fetch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_fetch); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":64
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":66
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  *             industry_code=self._industry_code,             # <<<<<<<<<<<<<<
  *             columns=['code', 'industry_id1'])
  *         if industry_data.empty:
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_industry_code, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_industry_code, __pyx_t_3) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":65
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":67
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  *             industry_code=self._industry_code,
  *             columns=['code', 'industry_id1'])             # <<<<<<<<<<<<<<
  *         if industry_data.empty:
  *             kd_logger.error('Industry data is empty')
  */
-  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_code);
   __Pyx_GIVEREF(__pyx_n_s_code);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_code);
   __Pyx_INCREF(__pyx_n_s_industry_id1);
   __Pyx_GIVEREF(__pyx_n_s_industry_id1);
   PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_industry_id1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_columns, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_columns, __pyx_t_3) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":63
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":65
  *     def prepare_data(self, begin_date=None, end_date=None):
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(             # <<<<<<<<<<<<<<
  *             industry_code=self._industry_code,
  *             columns=['code', 'industry_id1'])
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_industry_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":66
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":68
  *             industry_code=self._industry_code,
  *             columns=['code', 'industry_id1'])
  *         if industry_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Industry data is empty')
  *             return None
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_industry_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_industry_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":67
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":69
  *             columns=['code', 'industry_id1'])
  *         if industry_data.empty:
  *             kd_logger.error('Industry data is empty')             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_error); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_error); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_kp_s_Industry_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_s_Industry_data_is_empty);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":68
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":70
  *         if industry_data.empty:
  *             kd_logger.error('Industry data is empty')
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         codes = industry_data['code'].unique().tolist()
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":66
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":68
  *             industry_code=self._industry_code,
  *             columns=['code', 'industry_id1'])
  *         if industry_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Industry data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":70
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":72
  *             return None
  * 
  *         codes = industry_data['code'].unique().tolist()             # <<<<<<<<<<<<<<
  *         gd_overview_data = self._fetch_overview(codes)
  *         if gd_overview_data.empty:
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_industry_data, __pyx_n_s_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_industry_data, __pyx_n_s_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_unique); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_unique); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_tolist); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_tolist); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_codes = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":71
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":73
  * 
  *         codes = industry_data['code'].unique().tolist()
  *         gd_overview_data = self._fetch_overview(codes)             # <<<<<<<<<<<<<<
  *         if gd_overview_data.empty:
  *             kd_logger.error('Glassdoor overview data is empty')
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fetch_overview); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fetch_overview); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, __pyx_v_codes) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_codes);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_gd_overview_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":72
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":74
  *         codes = industry_data['code'].unique().tolist()
  *         gd_overview_data = self._fetch_overview(codes)
  *         if gd_overview_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor overview data is empty')
  *             return None
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_overview_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_overview_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":73
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":75
  *         gd_overview_data = self._fetch_overview(codes)
  *         if gd_overview_data.empty:
  *             kd_logger.error('Glassdoor overview data is empty')             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_error); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_error); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_kp_s_Glassdoor_overview_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_s_Glassdoor_overview_data_is_empty);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":74
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":76
  *         if gd_overview_data.empty:
  *             kd_logger.error('Glassdoor overview data is empty')
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         cids = gd_overview_data['cid'].unique().tolist()
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":72
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":74
  *         codes = industry_data['code'].unique().tolist()
  *         gd_overview_data = self._fetch_overview(codes)
  *         if gd_overview_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor overview data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":76
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":78
  *             return None
  * 
  *         cids = gd_overview_data['cid'].unique().tolist()             # <<<<<<<<<<<<<<
  *         gd_reviews_data = self._fetch_reviews(begin_date=begin_date,
  *                                               end_date=end_date,
  */
-  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gd_overview_data, __pyx_n_s_cid); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_gd_overview_data, __pyx_n_s_cid); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_unique); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_unique); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_tolist); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_tolist); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_cids = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":77
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":79
  * 
  *         cids = gd_overview_data['cid'].unique().tolist()
  *         gd_reviews_data = self._fetch_reviews(begin_date=begin_date,             # <<<<<<<<<<<<<<
  *                                               end_date=end_date,
  *                                               cids=cids)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fetch_reviews); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_fetch_reviews); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_begin_date, __pyx_v_begin_date) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_begin_date, __pyx_v_begin_date) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":78
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":80
  *         cids = gd_overview_data['cid'].unique().tolist()
  *         gd_reviews_data = self._fetch_reviews(begin_date=begin_date,
  *                                               end_date=end_date,             # <<<<<<<<<<<<<<
  *                                               cids=cids)
  *         if gd_reviews_data.empty:
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_end_date, __pyx_v_end_date) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_end_date, __pyx_v_end_date) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":79
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":81
  *         gd_reviews_data = self._fetch_reviews(begin_date=begin_date,
  *                                               end_date=end_date,
  *                                               cids=cids)             # <<<<<<<<<<<<<<
  *         if gd_reviews_data.empty:
  *             kd_logger.error('Glassdoor reviews data is empty')
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_cids, __pyx_v_cids) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_cids, __pyx_v_cids) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":77
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":79
  * 
  *         cids = gd_overview_data['cid'].unique().tolist()
  *         gd_reviews_data = self._fetch_reviews(begin_date=begin_date,             # <<<<<<<<<<<<<<
  *                                               end_date=end_date,
  *                                               cids=cids)
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_gd_reviews_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":80
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":82
  *                                               end_date=end_date,
  *                                               cids=cids)
  *         if gd_reviews_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor reviews data is empty')
  *             return None
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_reviews_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_reviews_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_4) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":81
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":83
  *                                               cids=cids)
  *         if gd_reviews_data.empty:
  *             kd_logger.error('Glassdoor reviews data is empty')             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_kp_s_Glassdoor_reviews_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_Glassdoor_reviews_data_is_empty);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":82
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":84
  *         if gd_reviews_data.empty:
  *             kd_logger.error('Glassdoor reviews data is empty')
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         kd_logger.info('merging glassdoor data...')
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":80
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":82
  *                                               end_date=end_date,
  *                                               cids=cids)
  *         if gd_reviews_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor reviews data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":84
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":86
  *             return None
  * 
  *         kd_logger.info('merging glassdoor data...')             # <<<<<<<<<<<<<<
  *         total_data = gd_reviews_data.merge(gd_overview_data,
  *                                            on=['cid'],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_s_merging_glassdoor_data) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_merging_glassdoor_data);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":85
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":87
  * 
  *         kd_logger.info('merging glassdoor data...')
  *         total_data = gd_reviews_data.merge(gd_overview_data,             # <<<<<<<<<<<<<<
  *                                            on=['cid'],
  *                                            how='left')
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_reviews_data, __pyx_n_s_merge); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gd_reviews_data, __pyx_n_s_merge); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_gd_overview_data);
   __Pyx_GIVEREF(__pyx_v_gd_overview_data);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_gd_overview_data);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":86
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":88
  *         kd_logger.info('merging glassdoor data...')
  *         total_data = gd_reviews_data.merge(gd_overview_data,
  *                                            on=['cid'],             # <<<<<<<<<<<<<<
  *                                            how='left')
  *         return total_data
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_cid);
   __Pyx_GIVEREF(__pyx_n_s_cid);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_cid);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_on, __pyx_t_5) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_on, __pyx_t_5) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_how, __pyx_n_s_left) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_how, __pyx_n_s_left) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":85
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":87
  * 
  *         kd_logger.info('merging glassdoor data...')
  *         total_data = gd_reviews_data.merge(gd_overview_data,             # <<<<<<<<<<<<<<
  *                                            on=['cid'],
  *                                            how='left')
  */
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_total_data = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":88
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":90
  *                                            on=['cid'],
  *                                            how='left')
  *         return total_data             # <<<<<<<<<<<<<<
  * 
  *     def _transform_raw(self, mean_data):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_total_data);
   __pyx_r = __pyx_v_total_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":61
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":63
  *         return gd_reviews_data
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  */
 
@@ -3551,29 +3614,32 @@
   __Pyx_XDECREF(__pyx_v_gd_reviews_data);
   __Pyx_XDECREF(__pyx_v_total_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":90
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":92
  *         return total_data
  * 
  *     def _transform_raw(self, mean_data):             # <<<<<<<<<<<<<<
  *         # save the raw average scores for UI use
  *         raw_data = mean_data.reset_index().set_index([
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_8_transform_raw[] = "Glassdoor._transform_raw(self, mean_data)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw = {"_transform_raw", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_8_transform_raw};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_mean_data = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_transform_raw (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_mean_data,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -3592,32 +3658,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mean_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_transform_raw", 1, 2, 2, 1); __PYX_ERR(0, 90, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_transform_raw", 1, 2, 2, 1); __PYX_ERR(0, 92, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_transform_raw") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_transform_raw") < 0)) __PYX_ERR(0, 92, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_mean_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_transform_raw", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 90, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_transform_raw", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 92, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._transform_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_8_transform_raw(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
 
@@ -3632,44 +3698,47 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_transform_raw", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":92
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":94
  *     def _transform_raw(self, mean_data):
  *         # save the raw average scores for UI use
  *         raw_data = mean_data.reset_index().set_index([             # <<<<<<<<<<<<<<
  *             'date',
  *             'code',
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_set_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_set_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_n_s_date);
   __Pyx_GIVEREF(__pyx_n_s_date);
   PyList_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_date);
   __Pyx_INCREF(__pyx_n_s_code);
   __Pyx_GIVEREF(__pyx_n_s_code);
   PyList_SET_ITEM(__pyx_t_4, 1, __pyx_n_s_code);
@@ -3682,190 +3751,190 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":95
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":97
  *             'date',
  *             'code',
  *         ]).stack().reset_index().rename(columns={             # <<<<<<<<<<<<<<
  *             'level_2': 'name',
  *             0: 'value'
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_stack); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_stack); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_rename); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_rename); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":96
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":98
  *             'code',
  *         ]).stack().reset_index().rename(columns={
  *             'level_2': 'name',             # <<<<<<<<<<<<<<
  *             0: 'value'
  *         })
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_level_2, __pyx_n_s_name) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_int_0, __pyx_n_s_value) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_columns, __pyx_t_2) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_level_2, __pyx_n_s_name) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_int_0, __pyx_n_s_value) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_columns, __pyx_t_2) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":95
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":97
  *             'date',
  *             'code',
  *         ]).stack().reset_index().rename(columns={             # <<<<<<<<<<<<<<
  *             'level_2': 'name',
  *             0: 'value'
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_raw_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":99
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":101
  *             0: 'value'
  *         })
  *         raw_data['date'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             raw_data['date']).dt.strftime('%Y-%m-%d')
  *         raw_data['industry'] = self._industry_code
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":100
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":102
  *         })
  *         raw_data['date'] = pd.to_datetime(
  *             raw_data['date']).dt.strftime('%Y-%m-%d')             # <<<<<<<<<<<<<<
  *         raw_data['industry'] = self._industry_code
  *         return raw_data
  */
-  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_raw_data, __pyx_n_s_date); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_raw_data, __pyx_n_s_date); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strftime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strftime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_s_Y_m_d) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_Y_m_d);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":99
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":101
  *             0: 'value'
  *         })
  *         raw_data['date'] = pd.to_datetime(             # <<<<<<<<<<<<<<
  *             raw_data['date']).dt.strftime('%Y-%m-%d')
  *         raw_data['industry'] = self._industry_code
  */
-  if (unlikely(PyObject_SetItem(__pyx_v_raw_data, __pyx_n_s_date, __pyx_t_2) < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_raw_data, __pyx_n_s_date, __pyx_t_2) < 0)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":101
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":103
  *         raw_data['date'] = pd.to_datetime(
  *             raw_data['date']).dt.strftime('%Y-%m-%d')
  *         raw_data['industry'] = self._industry_code             # <<<<<<<<<<<<<<
  *         return raw_data
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (unlikely(PyObject_SetItem(__pyx_v_raw_data, __pyx_n_s_industry, __pyx_t_2) < 0)) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_raw_data, __pyx_n_s_industry, __pyx_t_2) < 0)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":102
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":104
  *             raw_data['date']).dt.strftime('%Y-%m-%d')
  *         raw_data['industry'] = self._industry_code
  *         return raw_data             # <<<<<<<<<<<<<<
  * 
  *     def _blom_score(self, values_series, threshold=0.9):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_raw_data);
   __pyx_r = __pyx_v_raw_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":90
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":92
  *         return total_data
  * 
  *     def _transform_raw(self, mean_data):             # <<<<<<<<<<<<<<
  *         # save the raw average scores for UI use
  *         raw_data = mean_data.reset_index().set_index([
  */
 
@@ -3882,15 +3951,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_raw_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":104
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":106
  *         return raw_data
  * 
  *     def _blom_score(self, values_series, threshold=0.9):             # <<<<<<<<<<<<<<
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  */
 
@@ -3898,14 +3967,17 @@
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_10_blom_score[] = "Glassdoor._blom_score(self, values_series, threshold=0.9)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score = {"_blom_score", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_10_blom_score};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_values_series = 0;
   PyObject *__pyx_v_threshold = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_blom_score (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_values_series,&__pyx_n_s_threshold,0};
     PyObject* values[3] = {0,0,0};
     values[2] = ((PyObject *)((PyObject*)__pyx_float_0_9));
@@ -3927,25 +3999,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_values_series)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_blom_score", 0, 2, 3, 1); __PYX_ERR(0, 104, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_blom_score", 0, 2, 3, 1); __PYX_ERR(0, 106, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_threshold);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_blom_score") < 0)) __PYX_ERR(0, 104, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_blom_score") < 0)) __PYX_ERR(0, 106, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -3955,15 +4027,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_values_series = values[1];
     __pyx_v_threshold = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_blom_score", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 104, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_blom_score", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 106, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._blom_score", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_10_blom_score(__pyx_self, __pyx_v_self, __pyx_v_values_series, __pyx_v_threshold);
 
@@ -3987,173 +4059,176 @@
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   Py_ssize_t __pyx_t_7;
   Py_ssize_t __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_blom_score", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":105
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":107
  * 
  *     def _blom_score(self, values_series, threshold=0.9):
  *         idx = values_series.index.droplevel(level=0)             # <<<<<<<<<<<<<<
  *         coverage = values_series.isna().sum() / len(values_series)
  *         if coverage > threshold:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_values_series, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_values_series, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_droplevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_droplevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_level, __pyx_int_0) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_level, __pyx_int_0) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_idx = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":106
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":108
  *     def _blom_score(self, values_series, threshold=0.9):
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)             # <<<<<<<<<<<<<<
  *         if coverage > threshold:
  *             scores = [np.nan for _ in range(len(values_series))]
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_values_series, __pyx_n_s_isna); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_values_series, __pyx_n_s_isna); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = PyObject_Length(__pyx_v_values_series); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 106, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_values_series); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_coverage = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":107
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":109
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  *         if coverage > threshold:             # <<<<<<<<<<<<<<
  *             scores = [np.nan for _ in range(len(values_series))]
  *         else:
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_coverage, __pyx_v_threshold, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_coverage, __pyx_v_threshold, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_6) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":108
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":110
  *         coverage = values_series.isna().sum() / len(values_series)
  *         if coverage > threshold:
  *             scores = [np.nan for _ in range(len(values_series))]             # <<<<<<<<<<<<<<
  *         else:
  *             ranks = stats.mstats.rankdata(np.ma.masked_invalid(values_series))
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = PyObject_Length(__pyx_v_values_series); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_v_values_series); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 110, __pyx_L1_error)
     __pyx_t_7 = __pyx_t_5;
     for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
       __pyx_v__ = __pyx_t_8;
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 108, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 110, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_v_scores = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":107
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":109
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  *         if coverage > threshold:             # <<<<<<<<<<<<<<
  *             scores = [np.nan for _ in range(len(values_series))]
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":110
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":112
  *             scores = [np.nan for _ in range(len(values_series))]
  *         else:
  *             ranks = stats.mstats.rankdata(np.ma.masked_invalid(values_series))             # <<<<<<<<<<<<<<
  *             ranks[ranks == 0] = np.nan
  *             n = ranks.size - np.count_nonzero(np.isnan(ranks))
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_stats); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_stats); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_mstats); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_mstats); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_rankdata); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_rankdata); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ma); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ma); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_masked_invalid); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_masked_invalid); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_9, __pyx_v_values_series) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_values_series);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4161,70 +4236,70 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_ranks = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":111
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":113
  *         else:
  *             ranks = stats.mstats.rankdata(np.ma.masked_invalid(values_series))
  *             ranks[ranks == 0] = np.nan             # <<<<<<<<<<<<<<
  *             n = ranks.size - np.count_nonzero(np.isnan(ranks))
  *             scores = stats.norm.ppf((ranks - 3. / 8) / (n + 0.25))
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_nan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_ranks, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_ranks, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyObject_SetItem(__pyx_v_ranks, __pyx_t_1, __pyx_t_3) < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_ranks, __pyx_t_1, __pyx_t_3) < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":112
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":114
  *             ranks = stats.mstats.rankdata(np.ma.masked_invalid(values_series))
  *             ranks[ranks == 0] = np.nan
  *             n = ranks.size - np.count_nonzero(np.isnan(ranks))             # <<<<<<<<<<<<<<
  *             scores = stats.norm.ppf((ranks - 3. / 8) / (n + 0.25))
  *         scores = pd.Series(data=scores, index=idx)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ranks, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ranks, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_count_nonzero); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_count_nonzero); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_isnan); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_isnan); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_10, function);
       }
     }
     __pyx_t_2 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_9, __pyx_v_ranks) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_v_ranks);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_t_10 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -4232,47 +4307,47 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_10, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_n = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":113
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":115
  *             ranks[ranks == 0] = np.nan
  *             n = ranks.size - np.count_nonzero(np.isnan(ranks))
  *             scores = stats.norm.ppf((ranks - 3. / 8) / (n + 0.25))             # <<<<<<<<<<<<<<
  *         scores = pd.Series(data=scores, index=idx)
  *         return scores
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_stats); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_stats); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_norm); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_norm); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ppf); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ppf); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyFloat_FromDouble((3. / 8.0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_3 = PyFloat_FromDouble((3. / 8.0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyNumber_Subtract(__pyx_v_ranks, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Subtract(__pyx_v_ranks, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyFloat_AddObjC(__pyx_v_n, __pyx_float_0_25, 0.25, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFloat_AddObjC(__pyx_v_n, __pyx_float_0_25, 0.25, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_10 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_3)) {
@@ -4281,58 +4356,58 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_10);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_scores = __pyx_t_4;
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":114
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":116
  *             n = ranks.size - np.count_nonzero(np.isnan(ranks))
  *             scores = stats.norm.ppf((ranks - 3. / 8) / (n + 0.25))
  *         scores = pd.Series(data=scores, index=idx)             # <<<<<<<<<<<<<<
  *         return scores
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_Series); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_Series); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_data, __pyx_v_scores) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_index, __pyx_v_idx) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_data, __pyx_v_scores) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_index, __pyx_v_idx) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF_SET(__pyx_v_scores, __pyx_t_10);
   __pyx_t_10 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":115
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":117
  *             scores = stats.norm.ppf((ranks - 3. / 8) / (n + 0.25))
  *         scores = pd.Series(data=scores, index=idx)
  *         return scores             # <<<<<<<<<<<<<<
  * 
  *     def _distribute(self, mean_data):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_scores);
   __pyx_r = __pyx_v_scores;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":104
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":106
  *         return raw_data
  * 
  *     def _blom_score(self, values_series, threshold=0.9):             # <<<<<<<<<<<<<<
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  */
 
@@ -4353,29 +4428,32 @@
   __Pyx_XDECREF(__pyx_v_ranks);
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":117
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_12_distribute[] = "Glassdoor._distribute(self, mean_data)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute = {"_distribute", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_12_distribute};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_mean_data = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_distribute (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_mean_data,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -4394,45 +4472,45 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mean_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_distribute", 1, 2, 2, 1); __PYX_ERR(0, 117, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_distribute", 1, 2, 2, 1); __PYX_ERR(0, 119, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_distribute") < 0)) __PYX_ERR(0, 117, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_distribute") < 0)) __PYX_ERR(0, 119, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_mean_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_distribute", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 117, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_distribute", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 119, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_12_distribute(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":120
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":122
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)             # <<<<<<<<<<<<<<
  *         dt = pd.concat(res, axis=1)
  *         dt['industry'] = self._industry_code
  */
 
@@ -4456,22 +4534,25 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda1", 0);
   __pyx_outer_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 120, __pyx_L1_error) }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_percentile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 122, __pyx_L1_error) }
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_percentile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (unlikely(!__pyx_cur_scope->__pyx_v_res)) { __Pyx_RaiseClosureNameError("res"); __PYX_ERR(0, 120, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_res)) { __Pyx_RaiseClosureNameError("res"); __PYX_ERR(0, 122, __pyx_L1_error) }
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
@@ -4479,40 +4560,40 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_x, __pyx_cur_scope->__pyx_v_res};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_x, __pyx_cur_scope->__pyx_v_res};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_x);
     __Pyx_GIVEREF(__pyx_v_x);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_x);
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_res);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_res);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_cur_scope->__pyx_v_res);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -4527,15 +4608,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":117
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
 
@@ -4545,37 +4626,40 @@
   CYTHON_UNUSED PyObject *__pyx_v__ = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_distribute", 0);
   __pyx_cur_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *)__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute(__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 117, __pyx_L1_error)
+    __PYX_ERR(0, 119, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":118
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":120
  * 
  *     def _distribute(self, mean_data):
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']             # <<<<<<<<<<<<<<
  *         res = []
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_set_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_set_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyList_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_date);
   __Pyx_GIVEREF(__pyx_n_s_date);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_date);
   __Pyx_INCREF(__pyx_n_s_code);
   __Pyx_GIVEREF(__pyx_n_s_code);
   PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_code);
@@ -4591,134 +4675,134 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_dt = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":119
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":121
  *     def _distribute(self, mean_data):
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []             # <<<<<<<<<<<<<<
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)
  *         dt = pd.concat(res, axis=1)
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_cur_scope->__pyx_v_res = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":120
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":122
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)             # <<<<<<<<<<<<<<
  *         dt = pd.concat(res, axis=1)
  *         dt['industry'] = self._industry_code
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dt, __pyx_n_s_unstack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dt, __pyx_n_s_unstack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_apply); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_apply); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_distribute_lambda1, 0, __pyx_n_s_Glassdoor__distribute_locals_lam, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_distribute_lambda1, 0, __pyx_n_s_Glassdoor__distribute_locals_lam, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v__ = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":121
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":123
  *         res = []
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)
  *         dt = pd.concat(res, axis=1)             # <<<<<<<<<<<<<<
  *         dt['industry'] = self._industry_code
  *         return dt
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_concat); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_concat); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_res);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_res);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_cur_scope->__pyx_v_res);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_dt, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":122
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":124
  *         _ = dt.unstack().apply(lambda x: self._percentile(x, res), axis=0)
  *         dt = pd.concat(res, axis=1)
  *         dt['industry'] = self._industry_code             # <<<<<<<<<<<<<<
  *         return dt
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyObject_SetItem(__pyx_v_dt, __pyx_n_s_industry, __pyx_t_1) < 0)) __PYX_ERR(0, 122, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_dt, __pyx_n_s_industry, __pyx_t_1) < 0)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":123
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":125
  *         dt = pd.concat(res, axis=1)
  *         dt['industry'] = self._industry_code
  *         return dt             # <<<<<<<<<<<<<<
  * 
  *     def _percentile(self, x, res):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_dt);
   __pyx_r = __pyx_v_dt;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":117
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
 
@@ -4735,15 +4819,15 @@
   __Pyx_XDECREF(__pyx_v__);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":125
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":127
  *         return dt
  * 
  *     def _percentile(self, x, res):             # <<<<<<<<<<<<<<
  *         name = str(x.name)
  *         x = x.dropna()
  */
 
@@ -4751,14 +4835,17 @@
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_percentile[] = "Glassdoor._percentile(self, x, res)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile = {"_percentile", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_percentile};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_x = 0;
   PyObject *__pyx_v_res = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_percentile (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_x,&__pyx_n_s_res,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -4779,40 +4866,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_x)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_percentile", 1, 3, 3, 1); __PYX_ERR(0, 125, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_percentile", 1, 3, 3, 1); __PYX_ERR(0, 127, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_res)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_percentile", 1, 3, 3, 2); __PYX_ERR(0, 125, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_percentile", 1, 3, 3, 2); __PYX_ERR(0, 127, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_percentile") < 0)) __PYX_ERR(0, 125, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_percentile") < 0)) __PYX_ERR(0, 127, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_x = values[1];
     __pyx_v_res = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_percentile", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 125, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_percentile", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 127, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._percentile", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_14_percentile(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_res);
 
@@ -4828,182 +4915,185 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_percentile", 0);
   __Pyx_INCREF(__pyx_v_x);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":126
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":128
  * 
  *     def _percentile(self, x, res):
  *         name = str(x.name)             # <<<<<<<<<<<<<<
  *         x = x.dropna()
  *         rt = CSQuantiles(name).transform(x.reset_index().set_index('date'),
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_name = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":127
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":129
  *     def _percentile(self, x, res):
  *         name = str(x.name)
  *         x = x.dropna()             # <<<<<<<<<<<<<<
  *         rt = CSQuantiles(name).transform(x.reset_index().set_index('date'),
  *                                          name=name,
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_dropna); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_dropna); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_x, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":128
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":130
  *         name = str(x.name)
  *         x = x.dropna()
  *         rt = CSQuantiles(name).transform(x.reset_index().set_index('date'),             # <<<<<<<<<<<<<<
  *                                          name=name,
  *                                          category_field='code')
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_CSQuantiles); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_CSQuantiles); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_transform); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_transform); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_set_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_set_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_n_s_date) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_s_date);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":129
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":131
  *         x = x.dropna()
  *         rt = CSQuantiles(name).transform(x.reset_index().set_index('date'),
  *                                          name=name,             # <<<<<<<<<<<<<<
  *                                          category_field='code')
  *         res.append(rt.reset_index().set_index(['date', 'code']))
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_category_field, __pyx_n_s_code) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_category_field, __pyx_n_s_code) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":128
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":130
  *         name = str(x.name)
  *         x = x.dropna()
  *         rt = CSQuantiles(name).transform(x.reset_index().set_index('date'),             # <<<<<<<<<<<<<<
  *                                          name=name,
  *                                          category_field='code')
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_rt = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":131
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":133
  *                                          name=name,
  *                                          category_field='code')
  *         res.append(rt.reset_index().set_index(['date', 'code']))             # <<<<<<<<<<<<<<
  * 
  *     def _calculate_distribute(self, mean_data):
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_rt, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_rt, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_set_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_set_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_date);
   __Pyx_GIVEREF(__pyx_n_s_date);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_date);
   __Pyx_INCREF(__pyx_n_s_code);
   __Pyx_GIVEREF(__pyx_n_s_code);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_code);
@@ -5016,21 +5106,21 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_1, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_res, __pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_res, __pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":125
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":127
  *         return dt
  * 
  *     def _percentile(self, x, res):             # <<<<<<<<<<<<<<
  *         name = str(x.name)
  *         x = x.dropna()
  */
 
@@ -5050,29 +5140,32 @@
   __Pyx_XDECREF(__pyx_v_rt);
   __Pyx_XDECREF(__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":133
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":135
  *         res.append(rt.reset_index().set_index(['date', 'code']))
  * 
  *     def _calculate_distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16_calculate_distribute[] = "Glassdoor._calculate_distribute(self, mean_data)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute = {"_calculate_distribute", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16_calculate_distribute};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_mean_data = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_calculate_distribute (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_mean_data,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -5091,32 +5184,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mean_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_calculate_distribute", 1, 2, 2, 1); __PYX_ERR(0, 133, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calculate_distribute", 1, 2, 2, 1); __PYX_ERR(0, 135, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_calculate_distribute") < 0)) __PYX_ERR(0, 133, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_calculate_distribute") < 0)) __PYX_ERR(0, 135, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_mean_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_calculate_distribute", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 133, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_calculate_distribute", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 135, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._calculate_distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16_calculate_distribute(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
 
@@ -5134,204 +5227,207 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_calculate_distribute", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":134
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":136
  * 
  *     def _calculate_distribute(self, mean_data):
  *         kd_logger.info('calculating distribute...')             # <<<<<<<<<<<<<<
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  *         dist_data = self._distribute(mean_data=mean_data)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_calculating_distribute) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_calculating_distribute);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":135
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":137
  *     def _calculate_distribute(self, mean_data):
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])             # <<<<<<<<<<<<<<
  *         dist_data = self._distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_to_datetime); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_mean_data, __pyx_n_s_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_mean_data, __pyx_n_s_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_n_s_date, __pyx_t_1) < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_n_s_date, __pyx_t_1) < 0)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":136
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":138
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  *         dist_data = self._distribute(mean_data=mean_data)             # <<<<<<<<<<<<<<
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_distribute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_distribute); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_mean_data, __pyx_v_mean_data) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_mean_data, __pyx_v_mean_data) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_dist_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":137
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":139
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  *         dist_data = self._distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('distribute data is empty')
  *             return None
  */
   __pyx_t_6 = (__pyx_v_dist_data == Py_None);
   __pyx_t_7 = (__pyx_t_6 != 0);
   if (!__pyx_t_7) {
   } else {
     __pyx_t_5 = __pyx_t_7;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dist_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dist_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = __pyx_t_7;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_5) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":138
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":140
  *         dist_data = self._distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')             # <<<<<<<<<<<<<<
  *             return None
  *         dist_data = dist_data.reset_index().set_index(
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_kp_s_distribute_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_distribute_data_is_empty);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":139
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":141
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')
  *             return None             # <<<<<<<<<<<<<<
  *         dist_data = dist_data.reset_index().set_index(
  *             ['date', 'code', 'industry']).stack().reset_index()
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":137
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":139
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  *         dist_data = self._distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('distribute data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":140
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":142
  *             kd_logger.error('distribute data is empty')
  *             return None
  *         dist_data = dist_data.reset_index().set_index(             # <<<<<<<<<<<<<<
  *             ['date', 'code', 'industry']).stack().reset_index()
  *         dist_data = dist_data.rename(columns={'level_3': 'name', 0: 'value'})
  */
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_dist_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_dist_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_9) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_set_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_set_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":141
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":143
  *             return None
  *         dist_data = dist_data.reset_index().set_index(
  *             ['date', 'code', 'industry']).stack().reset_index()             # <<<<<<<<<<<<<<
  *         dist_data = dist_data.rename(columns={'level_3': 'name', 0: 'value'})
  *         dist_data['date'] = dist_data['date'].dt.strftime('%Y-%m-%d')
  */
-  __pyx_t_4 = PyList_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_n_s_date);
   __Pyx_GIVEREF(__pyx_n_s_date);
   PyList_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_date);
   __Pyx_INCREF(__pyx_n_s_code);
   __Pyx_GIVEREF(__pyx_n_s_code);
   PyList_SET_ITEM(__pyx_t_4, 1, __pyx_n_s_code);
@@ -5347,126 +5443,126 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_2 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_stack); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_stack); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF_SET(__pyx_v_dist_data, __pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":142
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":144
  *         dist_data = dist_data.reset_index().set_index(
  *             ['date', 'code', 'industry']).stack().reset_index()
  *         dist_data = dist_data.rename(columns={'level_3': 'name', 0: 'value'})             # <<<<<<<<<<<<<<
  *         dist_data['date'] = dist_data['date'].dt.strftime('%Y-%m-%d')
  *         return dist_data
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dist_data, __pyx_n_s_rename); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dist_data, __pyx_n_s_rename); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_level_3, __pyx_n_s_name) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_0, __pyx_n_s_value) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_columns, __pyx_t_1) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_level_3, __pyx_n_s_name) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_0, __pyx_n_s_value) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_columns, __pyx_t_1) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF_SET(__pyx_v_dist_data, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":143
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":145
  *             ['date', 'code', 'industry']).stack().reset_index()
  *         dist_data = dist_data.rename(columns={'level_3': 'name', 0: 'value'})
  *         dist_data['date'] = dist_data['date'].dt.strftime('%Y-%m-%d')             # <<<<<<<<<<<<<<
  *         return dist_data
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dist_data, __pyx_n_s_date); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dist_data, __pyx_n_s_date); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_dt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_dt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strftime); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strftime); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_3, __pyx_kp_s_Y_m_d) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_s_Y_m_d);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_dist_data, __pyx_n_s_date, __pyx_t_1) < 0)) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_dist_data, __pyx_n_s_date, __pyx_t_1) < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":144
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":146
  *         dist_data = dist_data.rename(columns={'level_3': 'name', 0: 'value'})
  *         dist_data['date'] = dist_data['date'].dt.strftime('%Y-%m-%d')
  *         return dist_data             # <<<<<<<<<<<<<<
  * 
  *     def _format_mean(self, mean_data):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_dist_data);
   __pyx_r = __pyx_v_dist_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":133
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":135
  *         res.append(rt.reset_index().set_index(['date', 'code']))
  * 
  *     def _calculate_distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  */
 
@@ -5483,29 +5579,32 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_dist_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":146
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":148
  *         return dist_data
  * 
  *     def _format_mean(self, mean_data):             # <<<<<<<<<<<<<<
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_18_format_mean[] = "Glassdoor._format_mean(self, mean_data)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean = {"_format_mean", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_18_format_mean};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_mean_data = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_format_mean (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_mean_data,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
@@ -5524,32 +5623,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mean_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_format_mean", 1, 2, 2, 1); __PYX_ERR(0, 146, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_format_mean", 1, 2, 2, 1); __PYX_ERR(0, 148, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_format_mean") < 0)) __PYX_ERR(0, 146, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_format_mean") < 0)) __PYX_ERR(0, 148, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_mean_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_format_mean", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 146, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_format_mean", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 148, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor._format_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_18_format_mean(__pyx_self, __pyx_v_self, __pyx_v_mean_data);
 
@@ -5560,74 +5659,77 @@
 
 static PyObject *__pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_18_format_mean(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_mean_data) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_format_mean", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":147
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":149
  * 
  *     def _format_mean(self, mean_data):
  *         mean_data['industry'] = self._industry_code             # <<<<<<<<<<<<<<
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  *         return mean_data
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_industry_code_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_n_s_industry, __pyx_t_1) < 0)) __PYX_ERR(0, 147, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_n_s_industry, __pyx_t_1) < 0)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":148
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":150
  *     def _format_mean(self, mean_data):
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')             # <<<<<<<<<<<<<<
  *         return mean_data
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_mean_data, __pyx_n_s_date); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_mean_data, __pyx_n_s_date); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strftime); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strftime); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_s_Y_m_d) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_s_Y_m_d);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_n_s_date, __pyx_t_1) < 0)) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_n_s_date, __pyx_t_1) < 0)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":149
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":151
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  *         return mean_data             # <<<<<<<<<<<<<<
  * 
  *     def calculate_result(self, total_data, threshold=0.9):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_mean_data);
   __pyx_r = __pyx_v_mean_data;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":146
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":148
  *         return dist_data
  * 
  *     def _format_mean(self, mean_data):             # <<<<<<<<<<<<<<
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  */
 
@@ -5640,15 +5742,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":151
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
 
@@ -5656,14 +5758,17 @@
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_20calculate_result[] = "Glassdoor.calculate_result(self, total_data, threshold=0.9)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result = {"calculate_result", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_20calculate_result};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_total_data = 0;
   PyObject *__pyx_v_threshold = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("calculate_result (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_total_data,&__pyx_n_s_threshold,0};
     PyObject* values[3] = {0,0,0};
     values[2] = ((PyObject *)((PyObject*)__pyx_float_0_9));
@@ -5685,25 +5790,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_total_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("calculate_result", 0, 2, 3, 1); __PYX_ERR(0, 151, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calculate_result", 0, 2, 3, 1); __PYX_ERR(0, 153, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_threshold);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_result") < 0)) __PYX_ERR(0, 151, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "calculate_result") < 0)) __PYX_ERR(0, 153, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -5713,28 +5818,28 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_total_data = values[1];
     __pyx_v_threshold = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calculate_result", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 151, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calculate_result", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 153, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.calculate_result", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_20calculate_result(__pyx_self, __pyx_v_self, __pyx_v_total_data, __pyx_v_threshold);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":162
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":164
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(             # <<<<<<<<<<<<<<
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  */
 
@@ -5757,66 +5862,69 @@
   struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *__pyx_outer_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda2", 0);
   __pyx_outer_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 162, __pyx_L1_error) }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_blom_score); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 164, __pyx_L1_error) }
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_blom_score); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":163
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":165
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))             # <<<<<<<<<<<<<<
  *             if isinstance(col_score, pd.DataFrame):
  *                 col_score = col_score.stack()
  */
-  if (unlikely(!__pyx_cur_scope->__pyx_v_col_name)) { __Pyx_RaiseClosureNameError("col_name"); __PYX_ERR(0, 163, __pyx_L1_error) }
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_cur_scope->__pyx_v_col_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_v_col_name)) { __Pyx_RaiseClosureNameError("col_name"); __PYX_ERR(0, 165, __pyx_L1_error) }
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_cur_scope->__pyx_v_col_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":162
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":164
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(             # <<<<<<<<<<<<<<
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":163
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":165
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))             # <<<<<<<<<<<<<<
  *             if isinstance(col_score, pd.DataFrame):
  *                 col_score = col_score.stack()
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (unlikely(!__pyx_cur_scope->__pyx_v_threshold)) { __Pyx_RaiseClosureNameError("threshold"); __PYX_ERR(0, 163, __pyx_L1_error) }
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_threshold, __pyx_cur_scope->__pyx_v_threshold) < 0) __PYX_ERR(0, 163, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_v_threshold)) { __Pyx_RaiseClosureNameError("threshold"); __PYX_ERR(0, 165, __pyx_L1_error) }
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_threshold, __pyx_cur_scope->__pyx_v_threshold) < 0) __PYX_ERR(0, 165, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":162
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":164
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(             # <<<<<<<<<<<<<<
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
@@ -5831,15 +5939,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":151
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
 
@@ -5857,40 +5965,43 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   PyObject *(*__pyx_t_10)(PyObject *);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_result", 0);
   __pyx_cur_scope = (struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *)__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result(__pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 151, __pyx_L1_error)
+    __PYX_ERR(0, 153, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_threshold = __pyx_v_threshold;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_threshold);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_threshold);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":153
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":155
  *     def calculate_result(self, total_data, threshold=0.9):
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()             # <<<<<<<<<<<<<<
  *         raw_data = self._transform_raw(mean_data=mean_data)
  *         if raw_data is None or raw_data.empty:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_total_data, __pyx_n_s_groupby); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_total_data, __pyx_n_s_groupby); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_n_s_date);
   __Pyx_GIVEREF(__pyx_n_s_date);
   PyList_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_date);
   __Pyx_INCREF(__pyx_n_s_code);
   __Pyx_GIVEREF(__pyx_n_s_code);
   PyList_SET_ITEM(__pyx_t_4, 1, __pyx_n_s_code);
@@ -5903,588 +6014,617 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_mean); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_mean); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_mean_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":154
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":156
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  *         raw_data = self._transform_raw(mean_data=mean_data)             # <<<<<<<<<<<<<<
  *         if raw_data is None or raw_data.empty:
  *             kd_logger.error('raw data is empty')
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_transform_raw); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_transform_raw); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mean_data, __pyx_v_mean_data) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mean_data, __pyx_v_mean_data) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_raw_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":155
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":157
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  *         raw_data = self._transform_raw(mean_data=mean_data)
  *         if raw_data is None or raw_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('raw data is empty')
  *             return None
  */
   __pyx_t_7 = (__pyx_v_raw_data == Py_None);
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (!__pyx_t_8) {
   } else {
     __pyx_t_6 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_raw_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_raw_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 157, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_6 = __pyx_t_8;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_6) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":156
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":158
  *         raw_data = self._transform_raw(mean_data=mean_data)
  *         if raw_data is None or raw_data.empty:
  *             kd_logger.error('raw data is empty')             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_s_raw_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_raw_data_is_empty);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":157
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":159
  *         if raw_data is None or raw_data.empty:
  *             kd_logger.error('raw data is empty')
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         kd_logger.info('calculating blom score...')
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":155
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":157
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  *         raw_data = self._transform_raw(mean_data=mean_data)
  *         if raw_data is None or raw_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('raw data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":159
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":161
  *             return None
  * 
  *         kd_logger.info('calculating blom score...')             # <<<<<<<<<<<<<<
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_kp_s_calculating_blom_score) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_calculating_blom_score);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":160
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":162
  * 
  *         kd_logger.info('calculating blom score...')
  *         for col_name in self._factors_sets:             # <<<<<<<<<<<<<<
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_factors_sets); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_factors_sets); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
     __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_9 = 0;
     __pyx_t_10 = NULL;
   } else {
-    __pyx_t_9 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __pyx_t_9 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_10 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __pyx_t_10 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 162, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (likely(!__pyx_t_10)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 160, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 162, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 160, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 162, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_10(__pyx_t_3);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 160, __pyx_L1_error)
+          else __PYX_ERR(0, 162, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_col_name);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_col_name, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":161
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":163
  *         kd_logger.info('calculating blom score...')
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(             # <<<<<<<<<<<<<<
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_sort_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_sort_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_n_s_date);
     __Pyx_GIVEREF(__pyx_n_s_date);
     PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_date);
     __Pyx_INCREF(__pyx_n_s_code);
     __Pyx_GIVEREF(__pyx_n_s_code);
     PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_code);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_by, __pyx_t_5) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_by, __pyx_t_5) < 0) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_groupby); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_groupby); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":162
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":164
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(             # <<<<<<<<<<<<<<
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  */
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_date);
     __Pyx_GIVEREF(__pyx_n_s_date);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_date);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_by, __pyx_t_1) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_by, __pyx_t_1) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":161
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":163
  *         kd_logger.info('calculating blom score...')
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(             # <<<<<<<<<<<<<<
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":162
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":164
  *         for col_name in self._factors_sets:
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(             # <<<<<<<<<<<<<<
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_apply); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_apply); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16calculate_result_lambda2, 0, __pyx_n_s_Glassdoor_calculate_result_local, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_16calculate_result_lambda2, 0, __pyx_n_s_Glassdoor_calculate_result_local, ((PyObject*)__pyx_cur_scope), __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_1);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF_SET(__pyx_v_col_score, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":164
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":166
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):             # <<<<<<<<<<<<<<
  *                 col_score = col_score.stack()
  *             col_score.name = col_name
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pd); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pd); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DataFrame); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DataFrame); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_6 = PyObject_IsInstance(__pyx_v_col_score, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_6 = PyObject_IsInstance(__pyx_v_col_score, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_8 = (__pyx_t_6 != 0);
     if (__pyx_t_8) {
 
-      /* "seleya/mfc/alchemy/qrank/glassdoor.py":165
+      /* "seleya/mfc/alchemy/qrank/glassdoor.py":167
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):
  *                 col_score = col_score.stack()             # <<<<<<<<<<<<<<
  *             col_score.name = col_name
  *             mean_data[col_name] = col_score
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_col_score, __pyx_n_s_stack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_col_score, __pyx_n_s_stack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_5 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF_SET(__pyx_v_col_score, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "seleya/mfc/alchemy/qrank/glassdoor.py":164
+      /* "seleya/mfc/alchemy/qrank/glassdoor.py":166
  *                 by=['date']).apply(lambda x: self._blom_score(
  *                     x[col_name], threshold=threshold))
  *             if isinstance(col_score, pd.DataFrame):             # <<<<<<<<<<<<<<
  *                 col_score = col_score.stack()
  *             col_score.name = col_name
  */
     }
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":166
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":168
  *             if isinstance(col_score, pd.DataFrame):
  *                 col_score = col_score.stack()
  *             col_score.name = col_name             # <<<<<<<<<<<<<<
  *             mean_data[col_name] = col_score
  *         mean_data = mean_data.stack().reset_index().rename(columns={
  */
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_col_score, __pyx_n_s_name, __pyx_cur_scope->__pyx_v_col_name) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_col_score, __pyx_n_s_name, __pyx_cur_scope->__pyx_v_col_name) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":167
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":169
  *                 col_score = col_score.stack()
  *             col_score.name = col_name
  *             mean_data[col_name] = col_score             # <<<<<<<<<<<<<<
  *         mean_data = mean_data.stack().reset_index().rename(columns={
  *             'level_2': 'name',
  */
-    if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_cur_scope->__pyx_v_col_name, __pyx_v_col_score) < 0)) __PYX_ERR(0, 167, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_mean_data, __pyx_cur_scope->__pyx_v_col_name, __pyx_v_col_score) < 0)) __PYX_ERR(0, 169, __pyx_L1_error)
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":160
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":162
  * 
  *         kd_logger.info('calculating blom score...')
  *         for col_name in self._factors_sets:             # <<<<<<<<<<<<<<
  *             col_score = mean_data.sort_values(by=['date', 'code']).groupby(
  *                 by=['date']).apply(lambda x: self._blom_score(
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":168
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":170
  *             col_score.name = col_name
  *             mean_data[col_name] = col_score
  *         mean_data = mean_data.stack().reset_index().rename(columns={             # <<<<<<<<<<<<<<
  *             'level_2': 'name',
  *             0: 'value'
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_stack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_mean_data, __pyx_n_s_stack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_5 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 168, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_rename); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_rename); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":169
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":171
  *             mean_data[col_name] = col_score
  *         mean_data = mean_data.stack().reset_index().rename(columns={
  *             'level_2': 'name',             # <<<<<<<<<<<<<<
  *             0: 'value'
  *         })
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_level_2, __pyx_n_s_name) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_int_0, __pyx_n_s_value) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_t_5) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_level_2, __pyx_n_s_name) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_int_0, __pyx_n_s_value) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_columns, __pyx_t_5) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":168
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":170
  *             col_score.name = col_name
  *             mean_data[col_name] = col_score
  *         mean_data = mean_data.stack().reset_index().rename(columns={             # <<<<<<<<<<<<<<
  *             'level_2': 'name',
  *             0: 'value'
  */
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_mean_data, __pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":173
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":175
  *         })
  * 
  *         dist_data = self._calculate_distribute(mean_data=mean_data)             # <<<<<<<<<<<<<<
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_calculate_distribute); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_calculate_distribute); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mean_data, __pyx_v_mean_data) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mean_data, __pyx_v_mean_data) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_dist_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":174
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":176
  * 
  *         dist_data = self._calculate_distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('distribute data is empty')
  *             return None
  */
   __pyx_t_6 = (__pyx_v_dist_data == Py_None);
   __pyx_t_7 = (__pyx_t_6 != 0);
   if (!__pyx_t_7) {
   } else {
     __pyx_t_8 = __pyx_t_7;
     goto __pyx_L10_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_dist_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_dist_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_8 = __pyx_t_7;
   __pyx_L10_bool_binop_done:;
   if (__pyx_t_8) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":175
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":177
  *         dist_data = self._calculate_distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_error); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_error); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_s_distribute_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s_distribute_data_is_empty);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":176
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":178
  *         if dist_data is None or dist_data.empty:
  *             kd_logger.error('distribute data is empty')
  *             return None             # <<<<<<<<<<<<<<
  * 
- *         return raw_data, self._format_mean(mean_data), dist_data
+ *         kd_logger.info('calculating success...')
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":174
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":176
  * 
  *         dist_data = self._calculate_distribute(mean_data=mean_data)
  *         if dist_data is None or dist_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('distribute data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":178
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":180
  *             return None
  * 
+ *         kd_logger.info('calculating success...')             # <<<<<<<<<<<<<<
+ *         return raw_data, self._format_mean(mean_data), dist_data
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_s_calculating_success) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_calculating_success);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":181
+ * 
+ *         kd_logger.info('calculating success...')
  *         return raw_data, self._format_mean(mean_data), dist_data             # <<<<<<<<<<<<<<
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_format_mean); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 178, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_3);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self, __pyx_n_s_format_mean); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_v_mean_data) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_mean_data);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_v_mean_data) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_mean_data);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 178, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_raw_data);
   __Pyx_GIVEREF(__pyx_v_raw_data);
-  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_raw_data);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_raw_data);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_v_dist_data);
   __Pyx_GIVEREF(__pyx_v_dist_data);
-  PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_dist_data);
+  PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_dist_data);
   __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_5;
-  __pyx_t_5 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":151
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
 
@@ -6504,15 +6644,15 @@
   __Pyx_XDECREF(__pyx_v_dist_data);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "seleya/mfc/alchemy/qrank/glassdoor.py":180
+/* "seleya/mfc/alchemy/qrank/glassdoor.py":183
  *         return raw_data, self._format_mean(mean_data), dist_data
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):             # <<<<<<<<<<<<<<
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:
  */
 
@@ -6521,14 +6661,17 @@
 static char __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_22run[] = "Glassdoor.run(self, begin_date, end_date, threshold=0.9)";
 static PyMethodDef __pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_23run = {"run", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_23run, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_22run};
 static PyObject *__pyx_pw_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_23run(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_begin_date = 0;
   PyObject *__pyx_v_end_date = 0;
   PyObject *__pyx_v_threshold = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("run (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_begin_date,&__pyx_n_s_end_date,&__pyx_n_s_threshold,0};
     PyObject* values[4] = {0,0,0,0};
     values[3] = ((PyObject *)((PyObject*)__pyx_float_0_9));
@@ -6552,31 +6695,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_begin_date)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("run", 0, 3, 4, 1); __PYX_ERR(0, 180, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("run", 0, 3, 4, 1); __PYX_ERR(0, 183, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end_date)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("run", 0, 3, 4, 2); __PYX_ERR(0, 180, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("run", 0, 3, 4, 2); __PYX_ERR(0, 183, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_threshold);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "run") < 0)) __PYX_ERR(0, 180, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "run") < 0)) __PYX_ERR(0, 183, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -6588,15 +6731,15 @@
     __pyx_v_self = values[0];
     __pyx_v_begin_date = values[1];
     __pyx_v_end_date = values[2];
     __pyx_v_threshold = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("run", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 180, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("run", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 183, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("seleya.mfc.alchemy.qrank.glassdoo.Glassdoor.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_22run(__pyx_self, __pyx_v_self, __pyx_v_begin_date, __pyx_v_end_date, __pyx_v_threshold);
 
@@ -6613,24 +6756,27 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("run", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":181
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":184
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):
  *         total_data = self.prepare_data(begin_date, end_date)             # <<<<<<<<<<<<<<
  *         if total_data is None or total_data.empty:
  *             kd_logger.error('Glassdoor data is empty')
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_prepare_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_prepare_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -6639,153 +6785,153 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_begin_date, __pyx_v_end_date};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_begin_date, __pyx_v_end_date};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 184, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_begin_date);
     __Pyx_GIVEREF(__pyx_v_begin_date);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_begin_date);
     __Pyx_INCREF(__pyx_v_end_date);
     __Pyx_GIVEREF(__pyx_v_end_date);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_end_date);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_total_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":182
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":185
  *     def run(self, begin_date, end_date, threshold=0.9):
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor data is empty')
  *             return None
  */
   __pyx_t_7 = (__pyx_v_total_data == Py_None);
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (!__pyx_t_8) {
   } else {
     __pyx_t_6 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_total_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_total_data, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_6 = __pyx_t_8;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_6) {
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":183
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":186
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:
  *             kd_logger.error('Glassdoor data is empty')             # <<<<<<<<<<<<<<
  *             return None
  *         return self.calculate_result(total_data=total_data,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, __pyx_kp_s_Glassdoor_data_is_empty) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_s_Glassdoor_data_is_empty);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":184
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":187
  *         if total_data is None or total_data.empty:
  *             kd_logger.error('Glassdoor data is empty')
  *             return None             # <<<<<<<<<<<<<<
  *         return self.calculate_result(total_data=total_data,
  *                                      threshold=threshold)
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "seleya/mfc/alchemy/qrank/glassdoor.py":182
+    /* "seleya/mfc/alchemy/qrank/glassdoor.py":185
  *     def run(self, begin_date, end_date, threshold=0.9):
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:             # <<<<<<<<<<<<<<
  *             kd_logger.error('Glassdoor data is empty')
  *             return None
  */
   }
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":185
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":188
  *             kd_logger.error('Glassdoor data is empty')
  *             return None
  *         return self.calculate_result(total_data=total_data,             # <<<<<<<<<<<<<<
  *                                      threshold=threshold)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_calculate_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_calculate_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_total_data, __pyx_v_total_data) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_total_data, __pyx_v_total_data) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":186
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":189
  *             return None
  *         return self.calculate_result(total_data=total_data,
  *                                      threshold=threshold)             # <<<<<<<<<<<<<<
  */
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_threshold, __pyx_v_threshold) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_threshold, __pyx_v_threshold) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":185
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":188
  *             kd_logger.error('Glassdoor data is empty')
  *             return None
  *         return self.calculate_result(total_data=total_data,             # <<<<<<<<<<<<<<
  *                                      threshold=threshold)
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":180
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":183
  *         return raw_data, self._format_mean(mean_data), dist_data
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):             # <<<<<<<<<<<<<<
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:
  */
 
@@ -6852,15 +6998,20 @@
 
 static PyTypeObject __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews = {
   PyVarObject_HEAD_INIT(0, 0)
   "seleya.mfc.alchemy.qrank.glassdoo.__pyx_scope_struct___fetch_reviews", /*tp_name*/
   sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -6902,14 +7053,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
+  #if PY_VERSION_HEX >= 0x030800b1
+  0, /*tp_vectorcall*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  0, /*tp_print*/
+  #endif
 };
 
 static struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute *__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute[8];
 static int __pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute = 0;
 
 static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -6963,15 +7120,20 @@
 
 static PyTypeObject __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute = {
   PyVarObject_HEAD_INIT(0, 0)
   "seleya.mfc.alchemy.qrank.glassdoo.__pyx_scope_struct_1__distribute", /*tp_name*/
   sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -7013,14 +7175,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
+  #if PY_VERSION_HEX >= 0x030800b1
+  0, /*tp_vectorcall*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  0, /*tp_print*/
+  #endif
 };
 
 static struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result *__pyx_freelist_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result[8];
 static int __pyx_freecount_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result = 0;
 
 static PyObject *__pyx_tp_new_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -7081,15 +7249,20 @@
 
 static PyTypeObject __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result = {
   PyVarObject_HEAD_INIT(0, 0)
   "seleya.mfc.alchemy.qrank.glassdoo.__pyx_scope_struct_2_calculate_result", /*tp_name*/
   sizeof(struct __pyx_obj_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -7131,14 +7304,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
+  #if PY_VERSION_HEX >= 0x030800b1
+  0, /*tp_vectorcall*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  0, /*tp_print*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 static int __pyx_import_star_set(PyObject *o, PyObject* py_name, char *name) {
@@ -7203,19 +7382,20 @@
                 err = -1;
             else
                 PyErr_Clear();
             break;
         }
         if (skip_leading_underscores &&
 #if PY_MAJOR_VERSION < 3
-            PyString_Check(name) &&
+            likely(PyString_Check(name)) &&
             PyString_AS_STRING(name)[0] == '_')
 #else
-            PyUnicode_Check(name) &&
-            PyUnicode_AS_UNICODE(name)[0] == '_')
+            likely(PyUnicode_Check(name)) &&
+            likely(__Pyx_PyUnicode_GET_LENGTH(name)) &&
+            __Pyx_PyUnicode_READ_CHAR(name, 0) == '_')
 #endif
         {
             Py_DECREF(name);
             continue;
         }
         value = PyObject_GetAttr(v, name);
         if (value == NULL)
@@ -7320,15 +7500,15 @@
   {&__pyx_n_s_CSQuantiles, __pyx_k_CSQuantiles, sizeof(__pyx_k_CSQuantiles), 0, 0, 1, 1},
   {&__pyx_n_s_DISAPPROVE, __pyx_k_DISAPPROVE, sizeof(__pyx_k_DISAPPROVE), 0, 0, 1, 1},
   {&__pyx_n_s_DataFrame, __pyx_k_DataFrame, sizeof(__pyx_k_DataFrame), 0, 0, 1, 1},
   {&__pyx_kp_s_Fetching_glassdoor_overview_data, __pyx_k_Fetching_glassdoor_overview_data, sizeof(__pyx_k_Fetching_glassdoor_overview_data), 0, 0, 1, 0},
   {&__pyx_kp_s_Fetching_glassdoor_reviews_data, __pyx_k_Fetching_glassdoor_reviews_data, sizeof(__pyx_k_Fetching_glassdoor_reviews_data), 0, 0, 1, 0},
   {&__pyx_kp_s_Fetching_industry_data, __pyx_k_Fetching_industry_data, sizeof(__pyx_k_Fetching_industry_data), 0, 0, 1, 0},
   {&__pyx_n_s_GDOveriew, __pyx_k_GDOveriew, sizeof(__pyx_k_GDOveriew), 0, 0, 1, 1},
-  {&__pyx_n_s_GDReviews, __pyx_k_GDReviews, sizeof(__pyx_k_GDReviews), 0, 0, 1, 1},
+  {&__pyx_n_s_GDReviewsBase, __pyx_k_GDReviewsBase, sizeof(__pyx_k_GDReviewsBase), 0, 0, 1, 1},
   {&__pyx_n_s_Glassdoor, __pyx_k_Glassdoor, sizeof(__pyx_k_Glassdoor), 0, 0, 1, 1},
   {&__pyx_n_s_Glassdoor___init, __pyx_k_Glassdoor___init, sizeof(__pyx_k_Glassdoor___init), 0, 0, 1, 1},
   {&__pyx_n_s_Glassdoor__blom_score, __pyx_k_Glassdoor__blom_score, sizeof(__pyx_k_Glassdoor__blom_score), 0, 0, 1, 1},
   {&__pyx_n_s_Glassdoor__calculate_distribute, __pyx_k_Glassdoor__calculate_distribute, sizeof(__pyx_k_Glassdoor__calculate_distribute), 0, 0, 1, 1},
   {&__pyx_n_s_Glassdoor__distribute, __pyx_k_Glassdoor__distribute, sizeof(__pyx_k_Glassdoor__distribute), 0, 0, 1, 1},
   {&__pyx_n_s_Glassdoor__distribute_locals_lam, __pyx_k_Glassdoor__distribute_locals_lam, sizeof(__pyx_k_Glassdoor__distribute_locals_lam), 0, 0, 1, 1},
   {&__pyx_n_s_Glassdoor__fetch_overview, __pyx_k_Glassdoor__fetch_overview, sizeof(__pyx_k_Glassdoor__fetch_overview), 0, 0, 1, 1},
@@ -7361,14 +7541,15 @@
   {&__pyx_n_s_begin_date, __pyx_k_begin_date, sizeof(__pyx_k_begin_date), 0, 0, 1, 1},
   {&__pyx_n_s_blom_score, __pyx_k_blom_score, sizeof(__pyx_k_blom_score), 0, 0, 1, 1},
   {&__pyx_n_s_by, __pyx_k_by, sizeof(__pyx_k_by), 0, 0, 1, 1},
   {&__pyx_n_s_calculate_distribute, __pyx_k_calculate_distribute, sizeof(__pyx_k_calculate_distribute), 0, 0, 1, 1},
   {&__pyx_n_s_calculate_result, __pyx_k_calculate_result, sizeof(__pyx_k_calculate_result), 0, 0, 1, 1},
   {&__pyx_kp_s_calculating_blom_score, __pyx_k_calculating_blom_score, sizeof(__pyx_k_calculating_blom_score), 0, 0, 1, 0},
   {&__pyx_kp_s_calculating_distribute, __pyx_k_calculating_distribute, sizeof(__pyx_k_calculating_distribute), 0, 0, 1, 0},
+  {&__pyx_kp_s_calculating_success, __pyx_k_calculating_success, sizeof(__pyx_k_calculating_success), 0, 0, 1, 0},
   {&__pyx_n_s_category_field, __pyx_k_category_field, sizeof(__pyx_k_category_field), 0, 0, 1, 1},
   {&__pyx_n_s_cid, __pyx_k_cid, sizeof(__pyx_k_cid), 0, 0, 1, 1},
   {&__pyx_n_s_cids, __pyx_k_cids, sizeof(__pyx_k_cids), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_code, __pyx_k_code, sizeof(__pyx_k_code), 0, 0, 1, 1},
   {&__pyx_n_s_codes, __pyx_k_codes, sizeof(__pyx_k_codes), 0, 0, 1, 1},
   {&__pyx_n_s_col, __pyx_k_col, sizeof(__pyx_k_col), 0, 0, 1, 1},
@@ -7437,14 +7618,15 @@
   {&__pyx_n_s_norm, __pyx_k_norm, sizeof(__pyx_k_norm), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_n_s_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
   {&__pyx_n_s_on, __pyx_k_on, sizeof(__pyx_k_on), 0, 0, 1, 1},
   {&__pyx_n_s_pandas, __pyx_k_pandas, sizeof(__pyx_k_pandas), 0, 0, 1, 1},
   {&__pyx_n_s_pd, __pyx_k_pd, sizeof(__pyx_k_pd), 0, 0, 1, 1},
+  {&__pyx_n_s_pdb, __pyx_k_pdb, sizeof(__pyx_k_pdb), 0, 0, 1, 1},
   {&__pyx_n_s_percentile, __pyx_k_percentile, sizeof(__pyx_k_percentile), 0, 0, 1, 1},
   {&__pyx_n_s_ppf, __pyx_k_ppf, sizeof(__pyx_k_ppf), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_prepare_data, __pyx_k_prepare_data, sizeof(__pyx_k_prepare_data), 0, 0, 1, 1},
   {&__pyx_n_s_probability_cols, __pyx_k_probability_cols, sizeof(__pyx_k_probability_cols), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
@@ -7496,189 +7678,189 @@
   {&__pyx_n_s_unstack, __pyx_k_unstack, sizeof(__pyx_k_unstack), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_values_series, __pyx_k_values_series, sizeof(__pyx_k_values_series), 0, 0, 1, 1},
   {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 10, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 110, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":10
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":11
  * 
  * 
  * class Glassdoor(object):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, industry_code):
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_builtin_object); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_builtin_object); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":12
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":13
  * class Glassdoor(object):
  * 
  *     def __init__(self, industry_code):             # <<<<<<<<<<<<<<
  *         self._industry_code = industry_code
  *         self._mapping_dict = {
  */
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_industry_code); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_industry_code); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_init, 12, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_init, 13, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 13, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":33
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":34
  *         self._factors_sets = self._probability_cols + self._mean_cols
  * 
  *     def _fetch_overview(self, codes):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  */
-  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_codes, __pyx_n_s_gd_overview_data); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_codes, __pyx_n_s_gd_overview_data); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_fetch_overview, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_fetch_overview, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 34, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":41
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
-  __pyx_tuple__7 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_begin_date, __pyx_n_s_end_date, __pyx_n_s_cids, __pyx_n_s_columns, __pyx_n_s_gd_reviews_data, __pyx_n_s_col); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_begin_date, __pyx_n_s_end_date, __pyx_n_s_cids, __pyx_n_s_columns, __pyx_n_s_gd_reviews_data, __pyx_n_s_col); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_fetch_reviews, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_fetch_reviews, 42, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 42, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":61
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":63
  *         return gd_reviews_data
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  */
-  __pyx_tuple__9 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_begin_date, __pyx_n_s_end_date, __pyx_n_s_industry_data, __pyx_n_s_codes, __pyx_n_s_gd_overview_data, __pyx_n_s_cids, __pyx_n_s_gd_reviews_data, __pyx_n_s_total_data); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_begin_date, __pyx_n_s_end_date, __pyx_n_s_industry_data, __pyx_n_s_codes, __pyx_n_s_gd_overview_data, __pyx_n_s_cids, __pyx_n_s_gd_reviews_data, __pyx_n_s_total_data); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_prepare_data, 61, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 61, __pyx_L1_error)
-  __pyx_tuple__11 = PyTuple_Pack(2, ((PyObject *)Py_None), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_prepare_data, 63, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(2, ((PyObject *)Py_None), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":90
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":92
  *         return total_data
  * 
  *     def _transform_raw(self, mean_data):             # <<<<<<<<<<<<<<
  *         # save the raw average scores for UI use
  *         raw_data = mean_data.reset_index().set_index([
  */
-  __pyx_tuple__12 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_mean_data, __pyx_n_s_raw_data); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_mean_data, __pyx_n_s_raw_data); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_transform_raw, 90, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_transform_raw, 92, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 92, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":104
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":106
  *         return raw_data
  * 
  *     def _blom_score(self, values_series, threshold=0.9):             # <<<<<<<<<<<<<<
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  */
-  __pyx_tuple__15 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_values_series, __pyx_n_s_threshold, __pyx_n_s_idx, __pyx_n_s_coverage, __pyx_n_s_scores, __pyx_n_s_ranks, __pyx_n_s_n, __pyx_n_s__14); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_values_series, __pyx_n_s_threshold, __pyx_n_s_idx, __pyx_n_s_coverage, __pyx_n_s_scores, __pyx_n_s_ranks, __pyx_n_s_n, __pyx_n_s__14); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_blom_score, 104, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 104, __pyx_L1_error)
-  __pyx_tuple__17 = PyTuple_Pack(1, ((PyObject*)__pyx_float_0_9)); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_blom_score, 106, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, ((PyObject*)__pyx_float_0_9)); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":117
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
-  __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_mean_data, __pyx_n_s_dt, __pyx_n_s_res, __pyx_n_s__14); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_mean_data, __pyx_n_s_dt, __pyx_n_s_res, __pyx_n_s__14); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_distribute, 117, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_distribute, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 119, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":125
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":127
  *         return dt
  * 
  *     def _percentile(self, x, res):             # <<<<<<<<<<<<<<
  *         name = str(x.name)
  *         x = x.dropna()
  */
-  __pyx_tuple__20 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_res, __pyx_n_s_name, __pyx_n_s_rt); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_res, __pyx_n_s_name, __pyx_n_s_rt); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_percentile, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_percentile, 127, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 127, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":133
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":135
  *         res.append(rt.reset_index().set_index(['date', 'code']))
  * 
  *     def _calculate_distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  */
-  __pyx_tuple__22 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_mean_data, __pyx_n_s_dist_data); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_mean_data, __pyx_n_s_dist_data); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_calculate_distribute, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_calculate_distribute, 135, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 135, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":146
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":148
  *         return dist_data
  * 
  *     def _format_mean(self, mean_data):             # <<<<<<<<<<<<<<
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  */
-  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_mean_data); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_mean_data); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_format_mean, 146, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_format_mean, 148, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 148, __pyx_L1_error)
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":151
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
-  __pyx_tuple__26 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_total_data, __pyx_n_s_threshold, __pyx_n_s_mean_data, __pyx_n_s_raw_data, __pyx_n_s_col_name, __pyx_n_s_col_score, __pyx_n_s_dist_data); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_total_data, __pyx_n_s_threshold, __pyx_n_s_mean_data, __pyx_n_s_raw_data, __pyx_n_s_col_name, __pyx_n_s_col_score, __pyx_n_s_dist_data); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_calculate_result, 151, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 151, __pyx_L1_error)
-  __pyx_tuple__28 = PyTuple_Pack(1, ((PyObject*)__pyx_float_0_9)); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_calculate_result, 153, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(1, ((PyObject*)__pyx_float_0_9)); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":180
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":183
  *         return raw_data, self._format_mean(mean_data), dist_data
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):             # <<<<<<<<<<<<<<
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:
  */
-  __pyx_tuple__29 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_begin_date, __pyx_n_s_end_date, __pyx_n_s_threshold, __pyx_n_s_total_data); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_begin_date, __pyx_n_s_end_date, __pyx_n_s_threshold, __pyx_n_s_total_data); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(4, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_run, 180, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 180, __pyx_L1_error)
-  __pyx_tuple__31 = PyTuple_Pack(1, ((PyObject*)__pyx_float_0_9)); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(4, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_seleya_mfc_alchemy_qrank_glassdo_2, __pyx_n_s_run, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(1, ((PyObject*)__pyx_float_0_9)); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -7726,30 +7908,39 @@
   /*--- Function export code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews.tp_print = 0;
+  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews.tp_dictoffset && __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews = &__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct___fetch_reviews;
-  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
+  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute.tp_print = 0;
+  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute.tp_dictoffset && __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute = &__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_1__distribute;
-  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
+  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result.tp_print = 0;
+  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result.tp_dictoffset && __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result = &__pyx_type_6seleya_3mfc_7alchemy_5qrank_8glassdoo___pyx_scope_struct_2_calculate_result;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
@@ -7778,25 +7969,27 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
+#ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#elif PY_MAJOR_VERSION < 3
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" void
+#else
+#define __Pyx_PyMODINIT_FUNC void
 #endif
 #else
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyObject *
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
 #else
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initglassdoo(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initglassdoo(void)
@@ -7872,14 +8065,17 @@
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_glassdoo(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'glassdoo' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -7939,18 +8135,17 @@
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #if CYTHON_COMPILING_IN_PYPY
   Py_INCREF(__pyx_b);
-  #endif
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_seleya__mfc__alchemy__qrank__glassdoo) {
@@ -7968,15 +8163,15 @@
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() != 0)) goto __pyx_L1_error;
+  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -8041,15 +8236,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "seleya/mfc/alchemy/qrank/glassdoor.py":6
  * import scipy.stats as stats
  * from ultron.sentry.api import *
  * from seleya import SurfaceDBAPI             # <<<<<<<<<<<<<<
  * from seleya.utilities.kd_logger import kd_logger
- * 
+ * import pdb
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_SurfaceDBAPI);
   __Pyx_GIVEREF(__pyx_n_s_SurfaceDBAPI);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_SurfaceDBAPI);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_seleya, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
@@ -8061,15 +8256,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "seleya/mfc/alchemy/qrank/glassdoor.py":7
  * from ultron.sentry.api import *
  * from seleya import SurfaceDBAPI
  * from seleya.utilities.kd_logger import kd_logger             # <<<<<<<<<<<<<<
- * 
+ * import pdb
  * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_kd_logger);
   __Pyx_GIVEREF(__pyx_n_s_kd_logger);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_kd_logger);
@@ -8078,184 +8273,196 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_kd_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_kd_logger, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":10
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":8
+ * from seleya import SurfaceDBAPI
+ * from seleya.utilities.kd_logger import kd_logger
+ * import pdb             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pdb, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pdb, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":11
  * 
  * 
  * class Glassdoor(object):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, industry_code):
  */
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_tuple__2, __pyx_n_s_Glassdoor, __pyx_n_s_Glassdoor, (PyObject *) NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_tuple__2, __pyx_n_s_Glassdoor, __pyx_n_s_Glassdoor, (PyObject *) NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":12
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":13
  * class Glassdoor(object):
  * 
  *     def __init__(self, industry_code):             # <<<<<<<<<<<<<<
  *         self._industry_code = industry_code
  *         self._mapping_dict = {
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__, 0, __pyx_n_s_Glassdoor___init, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_1__init__, 0, __pyx_n_s_Glassdoor___init, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":33
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":34
  *         self._factors_sets = self._probability_cols + self._mean_cols
  * 
  *     def _fetch_overview(self, codes):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor overview data...')
  *         gd_overview_data = SurfaceDBAPI.GDOveriew().fetch(
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview, 0, __pyx_n_s_Glassdoor__fetch_overview, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_3_fetch_overview, 0, __pyx_n_s_Glassdoor__fetch_overview, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_fetch_overview, __pyx_t_3) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_fetch_overview, __pyx_t_3) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":41
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":42
  *         return gd_overview_data
  * 
  *     def _fetch_reviews(self, begin_date, end_date, cids):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching glassdoor reviews data...')
  *         columns = ['id', 'cid', 'reviewId', 'reviewDateTime'
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_5_fetch_reviews, 0, __pyx_n_s_Glassdoor__fetch_reviews, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_5_fetch_reviews, 0, __pyx_n_s_Glassdoor__fetch_reviews, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_fetch_reviews, __pyx_t_3) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_fetch_reviews, __pyx_t_3) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":61
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":63
  *         return gd_reviews_data
  * 
  *     def prepare_data(self, begin_date=None, end_date=None):             # <<<<<<<<<<<<<<
  *         kd_logger.info('Fetching industry data...')
  *         industry_data = SurfaceDBAPI.Industry().fetch(
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data, 0, __pyx_n_s_Glassdoor_prepare_data, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_7prepare_data, 0, __pyx_n_s_Glassdoor_prepare_data, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__11);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_prepare_data, __pyx_t_3) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_prepare_data, __pyx_t_3) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":90
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":92
  *         return total_data
  * 
  *     def _transform_raw(self, mean_data):             # <<<<<<<<<<<<<<
  *         # save the raw average scores for UI use
  *         raw_data = mean_data.reset_index().set_index([
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw, 0, __pyx_n_s_Glassdoor__transform_raw, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_9_transform_raw, 0, __pyx_n_s_Glassdoor__transform_raw, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_transform_raw, __pyx_t_3) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_transform_raw, __pyx_t_3) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":104
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":106
  *         return raw_data
  * 
  *     def _blom_score(self, values_series, threshold=0.9):             # <<<<<<<<<<<<<<
  *         idx = values_series.index.droplevel(level=0)
  *         coverage = values_series.isna().sum() / len(values_series)
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score, 0, __pyx_n_s_Glassdoor__blom_score, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_11_blom_score, 0, __pyx_n_s_Glassdoor__blom_score, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__17);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_blom_score, __pyx_t_3) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_blom_score, __pyx_t_3) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":117
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":119
  *         return scores
  * 
  *     def _distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         dt = mean_data.set_index(['date', 'code', 'name'])['value']
  *         res = []
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute, 0, __pyx_n_s_Glassdoor__distribute, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_13_distribute, 0, __pyx_n_s_Glassdoor__distribute, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_distribute, __pyx_t_3) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_distribute, __pyx_t_3) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":125
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":127
  *         return dt
  * 
  *     def _percentile(self, x, res):             # <<<<<<<<<<<<<<
  *         name = str(x.name)
  *         x = x.dropna()
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile, 0, __pyx_n_s_Glassdoor__percentile, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_15_percentile, 0, __pyx_n_s_Glassdoor__percentile, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_percentile, __pyx_t_3) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_percentile, __pyx_t_3) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":133
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":135
  *         res.append(rt.reset_index().set_index(['date', 'code']))
  * 
  *     def _calculate_distribute(self, mean_data):             # <<<<<<<<<<<<<<
  *         kd_logger.info('calculating distribute...')
  *         mean_data['date'] = pd.to_datetime(mean_data['date'])
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute, 0, __pyx_n_s_Glassdoor__calculate_distribute, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_17_calculate_distribute, 0, __pyx_n_s_Glassdoor__calculate_distribute, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_calculate_distribute, __pyx_t_3) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_calculate_distribute, __pyx_t_3) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":146
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":148
  *         return dist_data
  * 
  *     def _format_mean(self, mean_data):             # <<<<<<<<<<<<<<
  *         mean_data['industry'] = self._industry_code
  *         mean_data['date'] = mean_data['date'].dt.strftime('%Y-%m-%d')
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean, 0, __pyx_n_s_Glassdoor__format_mean, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_19_format_mean, 0, __pyx_n_s_Glassdoor__format_mean, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_format_mean, __pyx_t_3) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_format_mean, __pyx_t_3) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":151
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":153
  *         return mean_data
  * 
  *     def calculate_result(self, total_data, threshold=0.9):             # <<<<<<<<<<<<<<
  *         # aggregate means by year and cid
  *         mean_data = total_data.groupby(['date', 'code']).mean()
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result, 0, __pyx_n_s_Glassdoor_calculate_result, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_21calculate_result, 0, __pyx_n_s_Glassdoor_calculate_result, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__28);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_calculate_result, __pyx_t_3) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_calculate_result, __pyx_t_3) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":180
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":183
  *         return raw_data, self._format_mean(mean_data), dist_data
  * 
  *     def run(self, begin_date, end_date, threshold=0.9):             # <<<<<<<<<<<<<<
  *         total_data = self.prepare_data(begin_date, end_date)
  *         if total_data is None or total_data.empty:
  */
-  __pyx_t_3 = __Pyx_CyFunction_NewEx(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_23run, 0, __pyx_n_s_Glassdoor_run, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6seleya_3mfc_7alchemy_5qrank_8glassdoo_9Glassdoor_23run, 0, __pyx_n_s_Glassdoor_run, NULL, __pyx_n_s_seleya_mfc_alchemy_qrank_glassdo, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__31);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_run, __pyx_t_3) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_run, __pyx_t_3) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "seleya/mfc/alchemy/qrank/glassdoor.py":10
+  /* "seleya/mfc/alchemy/qrank/glassdoor.py":11
  * 
  * 
  * class Glassdoor(object):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, industry_code):
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_Glassdoor, __pyx_tuple__2, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_Glassdoor, __pyx_tuple__2, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Glassdoor, __pyx_t_3) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Glassdoor, __pyx_t_3) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "seleya/mfc/alchemy/qrank/glassdoor.py":1
  * # -*- coding: utf-8 -*-             # <<<<<<<<<<<<<<
  * import numpy as np
@@ -8396,15 +8603,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
+        if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -8423,15 +8630,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -8439,15 +8646,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -8491,30 +8698,34 @@
         return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
 #endif
     return PyObject_SetAttr(obj, attr_name, value);
 }
 #endif
 
 /* PyDictVersioning */
-#if CYTHON_USE_DICT_VERSIONS
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
-    return dict ? __PYX_GET_DICT_VERSION(dict) : 0;
+    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
     PyObject **dictptr = NULL;
     Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
     if (offset) {
-        dictptr = (offset > 0) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
+#if CYTHON_COMPILING_IN_CPYTHON
+        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
+#else
+        dictptr = _PyObject_GetDictPtr(obj);
+#endif
     }
     return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
 }
 static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
-    if (!dict || tp_dict_version != __PYX_GET_DICT_VERSION(dict))
+    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
         return 0;
     return obj_dict_version == __Pyx_get_object_dict_version(obj);
 }
 #endif
 
 /* GetModuleGlobalName */
 #if CYTHON_USE_DICT_VERSIONS
@@ -8601,15 +8812,15 @@
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
 #if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs) {
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
 #endif
@@ -8672,20 +8883,20 @@
     }
     else {
         d = NULL;
         nd = 0;
     }
 #if PY_MAJOR_VERSION >= 3
     result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, nargs,
+                               args, (int)nargs,
                                k, (int)nk,
                                d, (int)nd, kwdefs, closure);
 #else
     result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, nargs,
+                               args, (int)nargs,
                                k, (int)nk,
                                d, (int)nd, closure);
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
@@ -8980,15 +9191,15 @@
     return cached_type;
 bad:
     Py_XDECREF(cached_type);
     cached_type = NULL;
     goto done;
 }
 
-/* CythonFunction */
+/* CythonFunctionShared */
 #include <structmember.h>
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *closure)
 {
     if (unlikely(op->func_doc == NULL)) {
         if (op->func.m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
@@ -9287,18 +9498,17 @@
     {0, 0, 0, 0}
 };
 #if PY_VERSION_HEX < 0x030500A0
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
 #else
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func.m_weakreflist)
 #endif
-static PyObject *__Pyx_CyFunction_New(PyTypeObject *type, PyMethodDef *ml, int flags, PyObject* qualname,
-                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
-    __pyx_CyFunctionObject *op = PyObject_GC_New(__pyx_CyFunctionObject, type);
-    if (op == NULL)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    if (unlikely(op == NULL))
         return NULL;
     op->flags = flags;
     __Pyx_CyFunction_weakreflist(op) = NULL;
     op->func.m_ml = ml;
     op->func.m_self = (PyObject *) op;
     Py_XINCREF(closure);
     op->func_closure = closure;
@@ -9311,20 +9521,20 @@
     op->func_doc = NULL;
     op->func_classobj = NULL;
     op->func_globals = globals;
     Py_INCREF(op->func_globals);
     Py_XINCREF(code);
     op->func_code = code;
     op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
     op->defaults = NULL;
     op->defaults_tuple = NULL;
     op->defaults_kwdict = NULL;
     op->defaults_getter = NULL;
     op->func_annotations = NULL;
-    PyObject_GC_Track(op);
     return (PyObject *) op;
 }
 static int
 __Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
 {
     Py_CLEAR(m->func_closure);
     Py_CLEAR(m->func.m_module);
@@ -9379,26 +9589,28 @@
         for (i = 0; i < m->defaults_pyobjects; i++)
             Py_VISIT(pydefaults[i]);
     }
     return 0;
 }
 static PyObject *__Pyx_CyFunction_descr_get(PyObject *func, PyObject *obj, PyObject *type)
 {
+#if PY_MAJOR_VERSION < 3
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     if (m->flags & __Pyx_CYFUNCTION_STATICMETHOD) {
         Py_INCREF(func);
         return func;
     }
     if (m->flags & __Pyx_CYFUNCTION_CLASSMETHOD) {
         if (type == NULL)
             type = (PyObject *)(Py_TYPE(obj));
         return __Pyx_PyMethod_New(func, type, (PyObject *)(Py_TYPE(type)));
     }
     if (obj == Py_None)
         obj = NULL;
+#endif
     return __Pyx_PyMethod_New(func, obj, type);
 }
 static PyObject*
 __Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
 {
 #if PY_MAJOR_VERSION >= 3
     return PyUnicode_FromFormat("<cyfunction %U at %p>",
@@ -9543,14 +9755,20 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030800b1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+    0,
+#endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
@@ -9558,14 +9776,15 @@
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->defaults = PyObject_Malloc(size);
     if (unlikely(!m->defaults))
         return PyErr_NoMemory();
     memset(m->defaults, 0, size);
     m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
     return m->defaults;
 }
 static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->defaults_tuple = tuple;
     Py_INCREF(tuple);
 }
@@ -9576,14 +9795,27 @@
 }
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->func_annotations = dict;
     Py_INCREF(dict);
 }
 
+/* CythonFunction */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* DictGetItem */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
     PyObject *value;
     value = PyDict_GetItemWithError(d, key);
     if (unlikely(!value)) {
         if (!PyErr_Occurred()) {
@@ -9941,15 +10173,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.')) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -10122,15 +10354,15 @@
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -10226,15 +10458,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
```

### Comparing `Finance-Seleya-1.1.2/seleya/utilities/api_base.py` & `Finance-Seleya-1.1.3/seleya/utilities/api_base.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/seleya/utilities/kd_logger.py` & `Finance-Seleya-1.1.3/seleya/utilities/kd_logger.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.2/setup.py` & `Finance-Seleya-1.1.3/setup.py`

 * *Files identical despite different names*

