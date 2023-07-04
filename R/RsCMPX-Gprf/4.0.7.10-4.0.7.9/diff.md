# Comparing `tmp/RsCMPX_Gprf-4.0.7.10.tar.gz` & `tmp/RsCMPX_Gprf-4.0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RsCMPX_Gprf-4.0.7.10.tar", last modified: Sun May 16 18:22:56 2021, max compression
+gzip compressed data, was "dist\RsCMPX_Gprf-4.0.7.9.tar", last modified: Mon Dec 28 20:25:19 2020, max compression
```

## Comparing `RsCMPX_Gprf-4.0.7.10.tar` & `RsCMPX_Gprf-4.0.7.9.tar`

### file list

```diff
@@ -1,845 +1,855 @@
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.267001 RsCMPX_Gprf-4.0.7.10/
--rw-rw-rw-   0        0        0     2487 2021-05-16 18:22:56.267001 RsCMPX_Gprf-4.0.7.10/PKG-INFO
--rw-rw-rw-   0        0        0     1644 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/README.md
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.141206 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.190076 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/CustomFiles/
--rw-rw-rw-   0        0        0        0 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/CustomFiles/__init__.py
--rw-rw-rw-   0        0        0     3304 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/CustomFiles/events.py
--rw-rw-rw-   0        0        0     4517 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/CustomFiles/reliability.py
--rw-rw-rw-   0        0        0    18659 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/CustomFiles/utilities.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.293799 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/
--rw-rw-rw-   0        0        0     1253 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.315740 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/
--rw-rw-rw-   0        0        0     1035 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/System.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.328705 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/System_/
--rw-rw-rw-   0        0        0     1633 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/System_/Attenuation.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/System_/__init__.py
--rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.339677 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/
--rw-rw-rw-   0        0        0     1063 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.350647 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/
--rw-rw-rw-   0        0        0     1231 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.369598 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/
--rw-rw-rw-   0        0        0     1195 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/Rx.py
--rw-rw-rw-   0        0        0     1195 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/Tx.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/__init__.py
--rw-rw-rw-   0        0        0     1007 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.383560 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/
--rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.395527 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/
--rw-rw-rw-   0        0        0     1075 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.411484 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.422456 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor_/
--rw-rw-rw-   0        0        0     2784 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor_/Zero.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/__init__.py
--rw-rw-rw-   0        0        0     2371 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.471325 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/
--rw-rw-rw-   0        0        0     1278 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.493269 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/
--rw-rw-rw-   0        0        0     1007 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.506233 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator_/
--rw-rw-rw-   0        0        0     2426 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator_/Spath.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator_/__init__.py
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.517203 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement_/
--rw-rw-rw-   0        0        0     2431 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement_/Spath.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/__init__.py
--rw-rw-rw-   0        0        0     1017 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Lte.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.528173 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Lte_/
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.539144 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement_/
--rw-rw-rw-   0        0        0     2294 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement_/Spath.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Lte_/__init__.py
--rw-rw-rw-   0        0        0     1029 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrMmw.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.550114 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.561085 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement_/
--rw-rw-rw-   0        0        0     2300 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement_/Spath.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/__init__.py
--rw-rw-rw-   0        0        0     1029 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrSub.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.572057 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.583027 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement_/
--rw-rw-rw-   0        0        0     2300 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement_/Spath.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/__init__.py
--rw-rw-rw-   0        0        0     1035 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/System.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.595992 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/System_/
--rw-rw-rw-   0        0        0      810 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/System_/Attenuation.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/System_/__init__.py
--rw-rw-rw-   0        0        0     1474 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.606963 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment_/
--rw-rw-rw-   0        0        0     1205 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment_/Connectors.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment_/__init__.py
--rw-rw-rw-   0        0        0     1017 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Uwb.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.614941 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.625456 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement_/
--rw-rw-rw-   0        0        0     2294 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement_/Spath.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/__init__.py
--rw-rw-rw-   0        0        0     1517 2021-05-16 18:22:45.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.645403 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/
--rw-rw-rw-   0        0        0     1281 2021-05-16 18:22:45.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.661361 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/
--rw-rw-rw-   0        0        0     1382 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Generator.py
--rw-rw-rw-   0        0        0     4793 2021-05-16 18:22:45.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.727757 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/
--rw-rw-rw-   0        0        0     4067 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.741720 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/
--rw-rw-rw-   0        0        0     1368 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/IqFile.py
--rw-rw-rw-   0        0        0     3143 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/Sall.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/__init__.py
--rw-rw-rw-   0        0        0     1250 2021-05-16 18:22:45.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Correction.py
--rw-rw-rw-   0        0        0     8999 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.760669 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/
--rw-rw-rw-   0        0        0     2454 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Attenuation.py
--rw-rw-rw-   0        0        0     2075 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Auto.py
--rw-rw-rw-   0        0        0     3232 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Average.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/__init__.py
--rw-rw-rw-   0        0        0    12387 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.767650 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn_/
--rw-rw-rw-   0        0        0     5314 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn_/PeakSearch.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn_/__init__.py
--rw-rw-rw-   0        0        0    15899 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.793582 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/
--rw-rw-rw-   0        0        0     2431 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.807544 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/
--rw-rw-rw-   0        0        0     1846 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/Bandpass.py
--rw-rw-rw-   0        0        0     1638 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/Gauss.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/__init__.py
--rw-rw-rw-   0        0        0     1363 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/IqSettings.py
--rw-rw-rw-   0        0        0     6651 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.821019 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/
--rw-rw-rw-   0        0        0     2724 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/EnvelopePower.py
--rw-rw-rw-   0        0        0     2668 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/Frequency.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/__init__.py
--rw-rw-rw-   0        0        0     1463 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/Trigger.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/__init__.py
--rw-rw-rw-   0        0        0    10961 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.833982 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/
--rw-rw-rw-   0        0        0     7101 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.853931 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/
--rw-rw-rw-   0        0        0     3730 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/EnvelopePower.py
--rw-rw-rw-   0        0        0     3046 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/Frequency.py
--rw-rw-rw-   0        0        0     3111 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/Retrigger.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/__init__.py
--rw-rw-rw-   0        0        0     1447 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/Trigger.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/__init__.py
--rw-rw-rw-   0        0        0     6127 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.862906 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/
--rw-rw-rw-   0        0        0     1850 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.872880 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor_/
--rw-rw-rw-   0        0        0     1949 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor_/Frequency.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/__init__.py
--rw-rw-rw-   0        0        0     3042 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.890832 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/
--rw-rw-rw-   0        0        0     1025 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.898810 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy_/
--rw-rw-rw-   0        0        0     2644 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy_/Frequency.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy_/__init__.py
--rw-rw-rw-   0        0        0      995 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.909781 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/
--rw-rw-rw-   0        0        0     1027 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.918756 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy_/
--rw-rw-rw-   0        0        0     2987 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy_/Frequency.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/__init__.py
--rw-rw-rw-   0        0        0     1273 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/View.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/__init__.py
--rw-rw-rw-   0        0        0    11195 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.948187 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/
--rw-rw-rw-   0        0        0      893 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/Catalog.py
--rw-rw-rw-   0        0        0     2865 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.962150 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/
--rw-rw-rw-   0        0        0     1462 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/Bandpass.py
--rw-rw-rw-   0        0        0     1438 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/Gauss.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/__init__.py
--rw-rw-rw-   0        0        0    11921 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.995062 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/
--rw-rw-rw-   0        0        0     3696 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/EnvelopePower.py
--rw-rw-rw-   0        0        0     3012 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Frequency.py
--rw-rw-rw-   0        0        0     3457 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/IqData.py
--rw-rw-rw-   0        0        0     3197 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Irepetition.py
--rw-rw-rw-   0        0        0     2819 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/ParameterSetList.py
--rw-rw-rw-   0        0        0     3073 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Retrigger.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/__init__.py
--rw-rw-rw-   0        0        0     3396 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.021993 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/
--rw-rw-rw-   0        0        0     1116 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Catalog.py
--rw-rw-rw-   0        0        0     1752 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.044929 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/
--rw-rw-rw-   0        0        0     1041 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.053906 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass_/
--rw-rw-rw-   0        0        0     3528 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass_/Bandwidth.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass_/__init__.py
--rw-rw-rw-   0        0        0     2722 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandwidth.py
--rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.063879 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss_/
--rw-rw-rw-   0        0        0     3552 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss_/Bandwidth.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss_/__init__.py
--rw-rw-rw-   0        0        0     4314 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/TypePy.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/__init__.py
--rw-rw-rw-   0        0        0     3382 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Mlength.py
--rw-rw-rw-   0        0        0     2500 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/PdefSet.py
--rw-rw-rw-   0        0        0     3044 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Slength.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/__init__.py
--rw-rw-rw-   0        0        0     1433 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/Trigger.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/__init__.py
--rw-rw-rw-   0        0        0     6952 2021-05-16 18:22:45.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/RfSettings.py
--rw-rw-rw-   0        0        0     1424 2021-05-16 18:22:45.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Scenario.py
--rw-rw-rw-   0        0        0     5212 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.080834 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/
--rw-rw-rw-   0        0        0     3561 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.099783 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/
--rw-rw-rw-   0        0        0     2111 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Rbw.py
--rw-rw-rw-   0        0        0     2181 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Swt.py
--rw-rw-rw-   0        0        0     2151 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Vbw.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/__init__.py
--rw-rw-rw-   0        0        0     4628 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.110754 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency_/
--rw-rw-rw-   0        0        0     2358 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency_/Span.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency_/__init__.py
--rw-rw-rw-   0        0        0     3762 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.125714 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/
--rw-rw-rw-   0        0        0     3232 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/Rbw.py
--rw-rw-rw-   0        0        0     2139 2021-05-16 18:22:46.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/Vbw.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/__init__.py
--rw-rw-rw-   0        0        0     2445 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.134690 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/
--rw-rw-rw-   0        0        0     1099 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.144663 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/
--rw-rw-rw-   0        0        0     1037 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.153641 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable_/
--rw-rw-rw-   0        0        0     1626 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable_/Info.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/__init__.py
--rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.163613 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/
--rw-rw-rw-   0        0        0     1535 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.180568 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/
--rw-rw-rw-   0        0        0     1231 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.193533 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/
--rw-rw-rw-   0        0        0     1802 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/Rx.py
--rw-rw-rw-   0        0        0     1802 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/Tx.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/__init__.py
--rw-rw-rw-   0        0        0     1880 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/Direction.py
--rw-rw-rw-   0        0        0     2350 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/Info.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/__init__.py
--rw-rw-rw-   0        0        0     1274 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.208493 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/
--rw-rw-rw-   0        0        0     1035 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/System.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.216472 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/System_/
--rw-rw-rw-   0        0        0     1642 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/System_/Attenuation.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/System_/__init__.py
--rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/Tenvironment.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.225447 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/Tenvironment_/
--rw-rw-rw-   0        0        0     1293 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/Tenvironment_/Spath.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/Tenvironment_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/__init__.py
--rw-rw-rw-   0        0        0     1942 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.252376 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/
--rw-rw-rw-   0        0        0     1001 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.262351 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/
--rw-rw-rw-   0        0        0     1029 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.271326 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System_/
--rw-rw-rw-   0        0        0     1227 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System_/Connectors.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/__init__.py
--rw-rw-rw-   0        0        0     1041 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Generic.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.280301 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/
--rw-rw-rw-   0        0        0     1011 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.289279 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement_/
--rw-rw-rw-   0        0        0     1184 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement_/Dapi.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/__init__.py
--rw-rw-rw-   0        0        0     1278 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.305235 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/
--rw-rw-rw-   0        0        0     2283 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.322192 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/
--rw-rw-rw-   0        0        0     1222 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Correction.py
--rw-rw-rw-   0        0        0     1204 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Rms.py
--rw-rw-rw-   0        0        0     2055 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Snumber.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/__init__.py
--rw-rw-rw-   0        0        0     1810 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.332163 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement_/
--rw-rw-rw-   0        0        0     2039 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement_/Snumber.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/__init__.py
--rw-rw-rw-   0        0        0      967 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Meas.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.340142 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Meas_/
--rw-rw-rw-   0        0        0      753 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Meas_/Scpi.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Meas_/__init__.py
--rw-rw-rw-   0        0        0     1613 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.362083 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/
--rw-rw-rw-   0        0        0     1280 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.376046 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/
--rw-rw-rw-   0        0        0     1271 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/Generator.py
--rw-rw-rw-   0        0        0     1289 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/Measurement.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/__init__.py
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.384025 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte_/
--rw-rw-rw-   0        0        0     1283 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte_/Measurement.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte_/__init__.py
--rw-rw-rw-   0        0        0     1031 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.393998 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw_/
--rw-rw-rw-   0        0        0     1295 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw_/Measurement.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw_/__init__.py
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.402975 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb_/
--rw-rw-rw-   0        0        0     1283 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb_/Measurement.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/__init__.py
--rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.410952 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/
--rw-rw-rw-   0        0        0     3060 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.454836 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/
--rw-rw-rw-   0        0        0     6191 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.463812 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/
--rw-rw-rw-   0        0        0     1811 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.472788 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State_/
--rw-rw-rw-   0        0        0     1200 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/__init__.py
--rw-rw-rw-   0        0        0     8585 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.480767 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/
--rw-rw-rw-   0        0        0     1812 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.489744 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State_/
--rw-rw-rw-   0        0        0     1201 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/__init__.py
--rw-rw-rw-   0        0        0     7220 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.520660 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/
--rw-rw-rw-   0        0        0     1838 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Icomponent.py
--rw-rw-rw-   0        0        0     1241 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.533626 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/
--rw-rw-rw-   0        0        0     2606 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/Average.py
--rw-rw-rw-   0        0        0     2606 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/Current.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/__init__.py
--rw-rw-rw-   0        0        0     1721 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.554570 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/
--rw-rw-rw-   0        0        0     2027 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Average.py
--rw-rw-rw-   0        0        0     2027 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Current.py
--rw-rw-rw-   0        0        0     2027 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Maximum.py
--rw-rw-rw-   0        0        0     2027 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Minimum.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/__init__.py
--rw-rw-rw-   0        0        0     1838 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Qcomponent.py
--rw-rw-rw-   0        0        0     1817 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.564544 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State_/
--rw-rw-rw-   0        0        0     1206 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/__init__.py
--rw-rw-rw-   0        0        0     8904 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.592469 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/
--rw-rw-rw-   0        0        0     1538 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Bin.py
--rw-rw-rw-   0        0        0      937 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Reliability.py
--rw-rw-rw-   0        0        0     1814 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.600447 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State_/
--rw-rw-rw-   0        0        0     1203 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State_/__init__.py
--rw-rw-rw-   0        0        0      913 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/SymbolRate.py
--rw-rw-rw-   0        0        0     1649 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Talignment.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/__init__.py
--rw-rw-rw-   0        0        0     7646 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.636352 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/
--rw-rw-rw-   0        0        0     1785 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/FreqError.py
--rw-rw-rw-   0        0        0     1724 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Icomponent.py
--rw-rw-rw-   0        0        0     1701 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Level.py
--rw-rw-rw-   0        0        0     2910 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/OfError.py
--rw-rw-rw-   0        0        0     1701 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Phase.py
--rw-rw-rw-   0        0        0     1724 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Qcomponent.py
--rw-rw-rw-   0        0        0     1806 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.645328 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State_/
--rw-rw-rw-   0        0        0     1195 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/__init__.py
--rw-rw-rw-   0        0        0     6302 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.657296 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/
--rw-rw-rw-   0        0        0     1814 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.665274 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor_/
--rw-rw-rw-   0        0        0     4968 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor_/Power.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor_/__init__.py
--rw-rw-rw-   0        0        0     1796 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.675249 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State_/
--rw-rw-rw-   0        0        0     1185 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/__init__.py
--rw-rw-rw-   0        0        0     3167 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.704170 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/
--rw-rw-rw-   0        0        0     1102 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Clear.py
--rw-rw-rw-   0        0        0     1672 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.727110 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/
--rw-rw-rw-   0        0        0     1596 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Frequency.py
--rw-rw-rw-   0        0        0     1561 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Gain.py
--rw-rw-rw-   0        0        0     2372 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/State.py
--rw-rw-rw-   0        0        0     1235 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.742071 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/
--rw-rw-rw-   0        0        0     1621 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/Frequency.py
--rw-rw-rw-   0        0        0     1586 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/Gain.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/__init__.py
--rw-rw-rw-   0        0        0     1644 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Open.py
--rw-rw-rw-   0        0        0     1651 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Short.py
--rw-rw-rw-   0        0        0     1483 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.750048 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State_/
--rw-rw-rw-   0        0        0      942 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/__init__.py
--rw-rw-rw-   0        0        0     9209 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.813878 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/
--rw-rw-rw-   0        0        0     1145 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/AmplitudeProbDensity.py
--rw-rw-rw-   0        0        0     4467 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.822854 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average_/
--rw-rw-rw-   0        0        0     1613 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average_/Rms.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average_/__init__.py
--rw-rw-rw-   0        0        0     2329 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.839810 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/
--rw-rw-rw-   0        0        0     1725 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Power.py
--rw-rw-rw-   0        0        0     1333 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Probability.py
--rw-rw-rw-   0        0        0     1478 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Sample.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/__init__.py
--rw-rw-rw-   0        0        0     4951 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.857761 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/
--rw-rw-rw-   0        0        0     1649 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Maximum.py
--rw-rw-rw-   0        0        0     1649 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Minimum.py
--rw-rw-rw-   0        0        0     1613 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Rms.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/__init__.py
--rw-rw-rw-   0        0        0     1163 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ElapsedStats.py
--rw-rw-rw-   0        0        0     2935 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.865740 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData_/
--rw-rw-rw-   0        0        0     1493 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData_/Bin.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData_/__init__.py
--rw-rw-rw-   0        0        0     1973 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqInfo.py
--rw-rw-rw-   0        0        0     2221 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.899649 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/
--rw-rw-rw-   0        0        0     4299 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Average.py
--rw-rw-rw-   0        0        0     4299 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Current.py
--rw-rw-rw-   0        0        0     1015 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.909622 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum_/
--rw-rw-rw-   0        0        0     4376 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum_/Current.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum_/__init__.py
--rw-rw-rw-   0        0        0     1015 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.919597 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum_/
--rw-rw-rw-   0        0        0     4376 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum_/Current.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum_/__init__.py
--rw-rw-rw-   0        0        0     1236 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.935553 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/
--rw-rw-rw-   0        0        0     4349 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/Maximum.py
--rw-rw-rw-   0        0        0     4349 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/Minimum.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/__init__.py
--rw-rw-rw-   0        0        0     4341 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/StandardDev.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/__init__.py
--rw-rw-rw-   0        0        0     1255 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.949516 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/
--rw-rw-rw-   0        0        0     3951 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/Current.py
--rw-rw-rw-   0        0        0     1649 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/Maximum.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/__init__.py
--rw-rw-rw-   0        0        0     1255 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.962482 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/
--rw-rw-rw-   0        0        0     3951 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/Current.py
--rw-rw-rw-   0        0        0     1649 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/Minimum.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/__init__.py
--rw-rw-rw-   0        0        0     1234 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.977442 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/
--rw-rw-rw-   0        0        0     3924 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/Maximum.py
--rw-rw-rw-   0        0        0     3924 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/Minimum.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/__init__.py
--rw-rw-rw-   0        0        0     4553 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.985421 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev_/
--rw-rw-rw-   0        0        0     1669 2021-05-16 18:22:48.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev_/Current.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev_/__init__.py
--rw-rw-rw-   0        0        0     1799 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:54.995393 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State_/
--rw-rw-rw-   0        0        0     1188 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/__init__.py
--rw-rw-rw-   0        0        0     4759 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.034291 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/
--rw-rw-rw-   0        0        0     1739 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.057229 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Average.py
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Current.py
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Maximum.py
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Minimum.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/__init__.py
--rw-rw-rw-   0        0        0     1814 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.064212 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker_/
--rw-rw-rw-   0        0        0     2305 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker_/Npeak.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker_/__init__.py
--rw-rw-rw-   0        0        0     1739 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.085155 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Average.py
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Current.py
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Maximum.py
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Minimum.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/__init__.py
--rw-rw-rw-   0        0        0     1739 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.111086 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Average.py
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Current.py
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Maximum.py
--rw-rw-rw-   0        0        0     1643 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Minimum.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/__init__.py
--rw-rw-rw-   0        0        0     1279 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.125047 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/
--rw-rw-rw-   0        0        0     2019 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/Npeak.py
--rw-rw-rw-   0        0        0     2019 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/Speak.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/__init__.py
--rw-rw-rw-   0        0        0     1703 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.148984 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/
--rw-rw-rw-   0        0        0     1619 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Average.py
--rw-rw-rw-   0        0        0     1619 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Current.py
--rw-rw-rw-   0        0        0     1619 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Maximum.py
--rw-rw-rw-   0        0        0     1619 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Minimum.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/__init__.py
--rw-rw-rw-   0        0        0     1730 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.174915 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/
--rw-rw-rw-   0        0        0     1637 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Average.py
--rw-rw-rw-   0        0        0     1637 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Current.py
--rw-rw-rw-   0        0        0     1637 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Maximum.py
--rw-rw-rw-   0        0        0     1637 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Minimum.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/__init__.py
--rw-rw-rw-   0        0        0     1492 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.181896 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State_/
--rw-rw-rw-   0        0        0      951 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/__init__.py
--rw-rw-rw-   0        0        0      989 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.190873 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/
--rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.198851 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.207827 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement_/
--rw-rw-rw-   0        0        0     4700 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement_/Ploss.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/__init__.py
--rw-rw-rw-   0        0        0      993 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.216803 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/
--rw-rw-rw-   0        0        0     1035 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/System.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.226776 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/System_/
--rw-rw-rw-   0        0        0     1099 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.233758 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation_/
--rw-rw-rw-   0        0        0     1305 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation_/CorrectionTable.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/System_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/__init__.py
--rw-rw-rw-   0        0        0     1274 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.248718 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/
--rw-rw-rw-   0        0        0     1035 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/System.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.257695 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/System_/
--rw-rw-rw-   0        0        0     1099 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.265673 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation_/
--rw-rw-rw-   0        0        0     1263 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation_/CorrectionTable.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/System_/__init__.py
--rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/Tenvironment.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.276643 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/
--rw-rw-rw-   0        0        0     1063 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.285619 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/
--rw-rw-rw-   0        0        0     2399 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/CorrectionTable.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/__init__.py
--rw-rw-rw-   0        0        0      983 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.294597 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/
--rw-rw-rw-   0        0        0     1023 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.302575 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.314543 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/
--rw-rw-rw-   0        0        0     1001 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.322521 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power_/
--rw-rw-rw-   0        0        0     1626 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power_/Current.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/__init__.py
--rw-rw-rw-   0        0        0     1628 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.347454 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/
--rw-rw-rw-   0        0        0     1279 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.360420 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/
--rw-rw-rw-   0        0        0     3811 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.374383 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/
--rw-rw-rw-   0        0        0     1442 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/RfSettings.py
--rw-rw-rw-   0        0        0     4800 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/Scenario.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/__init__.py
--rw-rw-rw-   0        0        0     3846 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.389343 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/
--rw-rw-rw-   0        0        0     1434 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/RfSettings.py
--rw-rw-rw-   0        0        0     6441 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.402308 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/
--rw-rw-rw-   0        0        0      881 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/Catalog.py
--rw-rw-rw-   0        0        0     1212 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/MaProtocol.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/__init__.py
--rw-rw-rw-   0        0        0     1029 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrMmw.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.412282 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrMmw_/
--rw-rw-rw-   0        0        0     1225 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrMmw_/Measurement.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrMmw_/__init__.py
--rw-rw-rw-   0        0        0     1029 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrSub.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.420261 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrSub_/
--rw-rw-rw-   0        0        0     1225 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrSub_/Measurement.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrSub_/__init__.py
--rw-rw-rw-   0        0        0     1017 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Uwb.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.429237 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Uwb_/
--rw-rw-rw-   0        0        0     1213 2021-05-16 18:22:47.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Uwb_/Measurement.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Uwb_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/__init__.py
--rw-rw-rw-   0        0        0      979 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.437215 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/
--rw-rw-rw-   0        0        0     1009 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.447188 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/
--rw-rw-rw-   0        0        0     4131 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.494063 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/
--rw-rw-rw-   0        0        0     9135 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.527996 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/
--rw-rw-rw-   0        0        0     4006 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/File.py
--rw-rw-rw-   0        0        0     2006 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Marker.py
--rw-rw-rw-   0        0        0     3261 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Msegment.py
--rw-rw-rw-   0        0        0     2651 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Samples.py
--rw-rw-rw-   0        0        0     2263 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Segments.py
--rw-rw-rw-   0        0        0     2674 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.536949 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker_/
--rw-rw-rw-   0        0        0     1117 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker_/Clist.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/__init__.py
--rw-rw-rw-   0        0        0     2117 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.550911 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/
--rw-rw-rw-   0        0        0     2579 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/Level.py
--rw-rw-rw-   0        0        0     3625 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/Ofrequency.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/__init__.py
--rw-rw-rw-   0        0        0     3383 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/IqSettings.py
--rw-rw-rw-   0        0        0    10348 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.615738 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/
--rw-rw-rw-   0        0        0     2468 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Dgain.py
--rw-rw-rw-   0        0        0     2441 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Dtime.py
--rw-rw-rw-   0        0        0     1089 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Esingle.py
--rw-rw-rw-   0        0        0     3139 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Fill.py
--rw-rw-rw-   0        0        0     2500 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Frequency.py
--rw-rw-rw-   0        0        0     2384 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.624716 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment_/
--rw-rw-rw-   0        0        0     1802 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment_/Enabling.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment_/__init__.py
--rw-rw-rw-   0        0        0     2524 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Irepetition.py
--rw-rw-rw-   0        0        0     2532 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Modulation.py
--rw-rw-rw-   0        0        0     2522 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Reenabling.py
--rw-rw-rw-   0        0        0     2512 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/RfLevel.py
--rw-rw-rw-   0        0        0     1071 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Rlist.py
--rw-rw-rw-   0        0        0     1071 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Slist.py
--rw-rw-rw-   0        0        0     2164 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Sstop.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/__init__.py
--rw-rw-rw-   0        0        0     2637 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Reliability.py
--rw-rw-rw-   0        0        0     4543 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/RfSettings.py
--rw-rw-rw-   0        0        0     6868 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.668599 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/
--rw-rw-rw-   0        0        0     8251 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.733425 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/
--rw-rw-rw-   0        0        0     1628 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Check.py
--rw-rw-rw-   0        0        0     1755 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/CrcProtect.py
--rw-rw-rw-   0        0        0     1228 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Download.py
--rw-rw-rw-   0        0        0     1508 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Duration.py
--rw-rw-rw-   0        0        0     1537 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Paratio.py
--rw-rw-rw-   0        0        0     1622 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Path.py
--rw-rw-rw-   0        0        0     1511 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Poffset.py
--rw-rw-rw-   0        0        0     1687 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Reliability.py
--rw-rw-rw-   0        0        0     1726 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Rmessage.py
--rw-rw-rw-   0        0        0     1582 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Roption.py
--rw-rw-rw-   0        0        0     1503 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Samples.py
--rw-rw-rw-   0        0        0     1518 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/SymbolRate.py
--rw-rw-rw-   0        0        0     1585 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Waveform.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/__init__.py
--rw-rw-rw-   0        0        0     1956 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.743399 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone_/
--rw-rw-rw-   0        0        0     3544 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone_/Ofrequency.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone_/__init__.py
--rw-rw-rw-   0        0        0     5649 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.809223 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/
--rw-rw-rw-   0        0        0     2839 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Acycles.py
--rw-rw-rw-   0        0        0     2843 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Dgain.py
--rw-rw-rw-   0        0        0     2813 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Dtime.py
--rw-rw-rw-   0        0        0     2442 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.831164 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/
--rw-rw-rw-   0        0        0     1282 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Call.py
--rw-rw-rw-   0        0        0     1129 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Insert.py
--rw-rw-rw-   0        0        0     1118 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Mdown.py
--rw-rw-rw-   0        0        0     1102 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Mup.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/__init__.py
--rw-rw-rw-   0        0        0     3814 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.854104 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/
--rw-rw-rw-   0        0        0     1383 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Apply.py
--rw-rw-rw-   0        0        0     3563 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Dgain.py
--rw-rw-rw-   0        0        0     3751 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Frequency.py
--rw-rw-rw-   0        0        0     3500 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Lrms.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/__init__.py
--rw-rw-rw-   0        0        0     3156 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Frequency.py
--rw-rw-rw-   0        0        0     3604 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Itransition.py
--rw-rw-rw-   0        0        0     4876 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Lincrement.py
--rw-rw-rw-   0        0        0     2765 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Lrms.py
--rw-rw-rw-   0        0        0     4256 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.867068 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/
--rw-rw-rw-   0        0        0     2380 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Catalog.py
--rw-rw-rw-   0        0        0     2935 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.876044 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index_/
--rw-rw-rw-   0        0        0     2179 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/__init__.py
--rw-rw-rw-   0        0        0     1531 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/SymbolRate.py
--rw-rw-rw-   0        0        0     1512 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Ttime.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/__init__.py
--rw-rw-rw-   0        0        0     1001 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.885021 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker_/
--rw-rw-rw-   0        0        0     3886 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker_/Delays.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker_/__init__.py
--rw-rw-rw-   0        0        0     2706 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Reliability.py
--rw-rw-rw-   0        0        0     1427 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Rmarker.py
--rw-rw-rw-   0        0        0     2058 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/State.py
--rw-rw-rw-   0        0        0     2171 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Tdd.py
--rw-rw-rw-   0        0        0     1824 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.894993 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker_/
--rw-rw-rw-   0        0        0     3645 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker_/Delay.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/__init__.py
--rw-rw-rw-   0        0        0     1878 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/State.py
--rw-rw-rw-   0        0        0     2047 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Tdd.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/__init__.py
--rw-rw-rw-   0        0        0     1033 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.902973 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/
--rw-rw-rw-   0        0        0     1097 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/Attenuation.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.911949 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/Attenuation_/
--rw-rw-rw-   0        0        0     1411 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.920925 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable_/
--rw-rw-rw-   0        0        0     1062 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/Attenuation_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/__init__.py
--rw-rw-rw-   0        0        0     1021 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Tenvironment.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.929901 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Tenvironment_/
--rw-rw-rw-   0        0        0      780 2021-05-16 18:22:51.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Tenvironment_/Spath.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Tenvironment_/__init__.py
--rw-rw-rw-   0        0        0      984 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.940872 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/
--rw-rw-rw-   0        0        0     1279 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.955833 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/
--rw-rw-rw-   0        0        0     1252 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.968797 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/
--rw-rw-rw-   0        0        0     5480 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.988743 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/
--rw-rw-rw-   0        0        0      870 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Catalog.py
--rw-rw-rw-   0        0        0     1009 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:55.997719 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual_/
--rw-rw-rw-   0        0        0     1129 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual_/Execute.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual_/__init__.py
--rw-rw-rw-   0        0        0     2007 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.007695 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/
--rw-rw-rw-   0        0        0     1011 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.015672 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual_/
--rw-rw-rw-   0        0        0     1185 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual_/Execute.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/__init__.py
--rw-rw-rw-   0        0        0     2473 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.033625 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/
--rw-rw-rw-   0        0        0     2184 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/IsMeas.py
--rw-rw-rw-   0        0        0     2228 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/IsTrigger.py
--rw-rw-rw-   0        0        0     1009 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.043598 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual_/
--rw-rw-rw-   0        0        0     1247 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual_/Execute.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/__init__.py
--rw-rw-rw-   0        0        0     2060 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.071523 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/
--rw-rw-rw-   0        0        0    10672 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.080500 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn_/
--rw-rw-rw-   0        0        0     1057 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn_/Catalog.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn_/__init__.py
--rw-rw-rw-   0        0        0     8477 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.088477 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder_/
--rw-rw-rw-   0        0        0     1055 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder_/Catalog.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder_/__init__.py
--rw-rw-rw-   0        0        0     9111 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.096456 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot_/
--rw-rw-rw-   0        0        0     1045 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot_/Catalog.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot_/__init__.py
--rw-rw-rw-   0        0        0     9373 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.111418 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/
--rw-rw-rw-   0        0        0     1035 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/Catalog.py
--rw-rw-rw-   0        0        0     1061 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.120394 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList_/
--rw-rw-rw-   0        0        0     2932 2021-05-16 18:22:49.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList_/Offset.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/__init__.py
--rw-rw-rw-   0        0        0     6183 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.130366 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum_/
--rw-rw-rw-   0        0        0      891 2021-05-16 18:22:50.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum_/Catalog.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:56.260021 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/
--rw-rw-rw-   0        0        0      541 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgLinkedEventArgs.py
--rw-rw-rw-   0        0        0     4003 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgSingle.py
--rw-rw-rw-   0        0        0     1061 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgSingleList.py
--rw-rw-rw-   0        0        0     1000 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py
--rw-rw-rw-   0        0        0     9026 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgStringComposer.py
--rw-rw-rw-   0        0        0     5624 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgStruct.py
--rw-rw-rw-   0        0        0     3354 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgStructList.py
--rw-rw-rw-   0        0        0     2446 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgStructStringParser.py
--rw-rw-rw-   0        0        0     5176 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/CommandsGroup.py
--rw-rw-rw-   0        0        0    20227 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/Conversions.py
--rw-rw-rw-   0        0        0     3618 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ConverterFromScpiString.py
--rw-rw-rw-   0        0        0     4409 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ConverterToScpiString.py
--rw-rw-rw-   0        0        0    10299 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/Core.py
--rw-rw-rw-   0        0        0    38340 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/Instrument.py
--rw-rw-rw-   0        0        0     3918 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/InstrumentErrors.py
--rw-rw-rw-   0        0        0     2081 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/InstrumentOptions.py
--rw-rw-rw-   0        0        0     5101 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/InstrumentSettings.py
--rw-rw-rw-   0        0        0     3380 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/InternalLinker.py
--rw-rw-rw-   0        0        0     4331 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/IoTransferEventArgs.py
--rw-rw-rw-   0        0        0     3841 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/RepeatedCapability.py
--rw-rw-rw-   0        0        0     4719 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/StreamReader.py
--rw-rw-rw-   0        0        0     4938 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/StreamWriter.py
--rw-rw-rw-   0        0        0     1040 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/StructBase.py
--rw-rw-rw-   0        0        0     2893 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/Types.py
--rw-rw-rw-   0        0        0     4530 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/Utilities.py
--rw-rw-rw-   0        0        0     4850 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/VisaPluginSocketIo.py
--rw-rw-rw-   0        0        0    44232 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/VisaSession.py
--rw-rw-rw-   0        0        0     6999 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/VisaSessionSim.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/__init__.py
--rw-rw-rw-   0        0        0    11532 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/RsCMPX_Gprf.py
--rw-rw-rw-   0        0        0      825 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/__init__.py
--rw-rw-rw-   0        0        0    12119 2021-05-16 18:22:42.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/enums.py
--rw-rw-rw-   0        0        0     2000 2021-05-16 18:22:43.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/repcap.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:22:53.166139 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf.egg-info/
--rw-rw-rw-   0        0        0     2487 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    44946 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-05-16 18:22:56.269993 RsCMPX_Gprf-4.0.7.10/setup.cfg
--rw-rw-rw-   0        0        0      863 2021-05-16 18:22:52.000000 RsCMPX_Gprf-4.0.7.10/setup.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.675992 RsCMPX_Gprf-4.0.7.9/
+-rw-rw-rw-   0        0        0     2316 2020-12-28 20:25:19.674995 RsCMPX_Gprf-4.0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1569 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/README.md
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.779556 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.802495 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/CustomFiles/
+-rw-rw-rw-   0        0        0        0 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/CustomFiles/__init__.py
+-rw-rw-rw-   0        0        0     2132 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/CustomFiles/events.py
+-rw-rw-rw-   0        0        0     4646 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/CustomFiles/reliability.py
+-rw-rw-rw-   0        0        0    17351 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/CustomFiles/utilities.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.854357 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/
+-rw-rw-rw-   0        0        0     1253 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.860340 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/
+-rw-rw-rw-   0        0        0     1035 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/System.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.864330 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/System_/
+-rw-rw-rw-   0        0        0     1099 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/System_/Attenuation.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.872309 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/System_/Attenuation_/
+-rw-rw-rw-   0        0        0     1314 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/System_/Attenuation_/CorrectionTable.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/System_/Attenuation_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/System_/__init__.py
+-rw-rw-rw-   0        0        0     1023 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.876299 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/
+-rw-rw-rw-   0        0        0     1063 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.881286 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/
+-rw-rw-rw-   0        0        0     1231 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.889263 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/
+-rw-rw-rw-   0        0        0     1195 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/Rx.py
+-rw-rw-rw-   0        0        0     1195 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/Tx.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/__init__.py
+-rw-rw-rw-   0        0        0     1007 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.894250 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/
+-rw-rw-rw-   0        0        0     1023 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.898240 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/
+-rw-rw-rw-   0        0        0     1075 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.903226 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/
+-rw-rw-rw-   0        0        0     1019 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.908212 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor_/
+-rw-rw-rw-   0        0        0     2784 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor_/Zero.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/__init__.py
+-rw-rw-rw-   0        0        0     2371 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.927162 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/
+-rw-rw-rw-   0        0        0     1278 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.935140 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/
+-rw-rw-rw-   0        0        0     1007 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.940127 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator_/
+-rw-rw-rw-   0        0        0     2426 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator_/Spath.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator_/__init__.py
+-rw-rw-rw-   0        0        0     1019 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.944117 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement_/
+-rw-rw-rw-   0        0        0     2431 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement_/Spath.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0     1017 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Lte.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.950607 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Lte_/
+-rw-rw-rw-   0        0        0     1019 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.955593 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement_/
+-rw-rw-rw-   0        0        0     2294 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement_/Spath.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Lte_/__init__.py
+-rw-rw-rw-   0        0        0     1029 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrMmw.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.960580 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/
+-rw-rw-rw-   0        0        0     1019 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.965568 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement_/
+-rw-rw-rw-   0        0        0     2300 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement_/Spath.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/__init__.py
+-rw-rw-rw-   0        0        0     1029 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrSub.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.970553 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/
+-rw-rw-rw-   0        0        0     1019 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.975540 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement_/
+-rw-rw-rw-   0        0        0     2300 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement_/Spath.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/__init__.py
+-rw-rw-rw-   0        0        0     1035 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/System.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.979529 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/System_/
+-rw-rw-rw-   0        0        0      810 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/System_/Attenuation.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/System_/__init__.py
+-rw-rw-rw-   0        0        0     1474 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.984516 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment_/
+-rw-rw-rw-   0        0        0     1205 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment_/Connectors.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment_/__init__.py
+-rw-rw-rw-   0        0        0     1017 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Uwb.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.988506 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/
+-rw-rw-rw-   0        0        0     1019 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.992495 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement_/
+-rw-rw-rw-   0        0        0     2294 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement_/Spath.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/__init__.py
+-rw-rw-rw-   0        0        0     1517 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.001500 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/
+-rw-rw-rw-   0        0        0     1281 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.007455 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/
+-rw-rw-rw-   0        0        0     1382 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Generator.py
+-rw-rw-rw-   0        0        0     4793 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.038371 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/
+-rw-rw-rw-   0        0        0     4067 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.045353 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/
+-rw-rw-rw-   0        0        0     1373 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/IqFile.py
+-rw-rw-rw-   0        0        0     3143 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/Sall.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/__init__.py
+-rw-rw-rw-   0        0        0     1250 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Correction.py
+-rw-rw-rw-   0        0        0     9004 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.057321 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/
+-rw-rw-rw-   0        0        0     2444 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Attenuation.py
+-rw-rw-rw-   0        0        0     2075 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Auto.py
+-rw-rw-rw-   0        0        0     3232 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Average.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/__init__.py
+-rw-rw-rw-   0        0        0    12392 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.062307 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn_/
+-rw-rw-rw-   0        0        0     5314 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn_/PeakSearch.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn_/__init__.py
+-rw-rw-rw-   0        0        0    15904 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.075273 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/
+-rw-rw-rw-   0        0        0     2431 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.086246 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/
+-rw-rw-rw-   0        0        0     1851 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/Bandpass.py
+-rw-rw-rw-   0        0        0     1638 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/Gauss.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/__init__.py
+-rw-rw-rw-   0        0        0     1363 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/IqSettings.py
+-rw-rw-rw-   0        0        0     6651 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.092227 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/
+-rw-rw-rw-   0        0        0     2724 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/EnvelopePower.py
+-rw-rw-rw-   0        0        0     2668 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/Frequency.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/__init__.py
+-rw-rw-rw-   0        0        0     1463 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/Trigger.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/__init__.py
+-rw-rw-rw-   0        0        0    10966 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.098213 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/
+-rw-rw-rw-   0        0        0     7101 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.108185 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/
+-rw-rw-rw-   0        0        0     3730 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/EnvelopePower.py
+-rw-rw-rw-   0        0        0     3046 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/Frequency.py
+-rw-rw-rw-   0        0        0     3111 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/ReTrigger.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/__init__.py
+-rw-rw-rw-   0        0        0     1447 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/Trigger.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/__init__.py
+-rw-rw-rw-   0        0        0     6132 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.112175 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/
+-rw-rw-rw-   0        0        0     1850 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.117162 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor_/
+-rw-rw-rw-   0        0        0     1949 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor_/Frequency.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/__init__.py
+-rw-rw-rw-   0        0        0     3037 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.125169 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/
+-rw-rw-rw-   0        0        0     1025 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.130127 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy_/
+-rw-rw-rw-   0        0        0     2644 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy_/Frequency.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy_/__init__.py
+-rw-rw-rw-   0        0        0      995 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.135115 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/
+-rw-rw-rw-   0        0        0     1027 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.139104 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy_/
+-rw-rw-rw-   0        0        0     2987 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy_/Frequency.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/__init__.py
+-rw-rw-rw-   0        0        0     1273 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/View.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/__init__.py
+-rw-rw-rw-   0        0        0    11200 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.156057 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/
+-rw-rw-rw-   0        0        0      893 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/Catalog.py
+-rw-rw-rw-   0        0        0     2865 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.163038 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/
+-rw-rw-rw-   0        0        0     1462 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/Bandpass.py
+-rw-rw-rw-   0        0        0     1438 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/Gauss.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/__init__.py
+-rw-rw-rw-   0        0        0    11921 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.179995 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/
+-rw-rw-rw-   0        0        0     3696 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/EnvelopePower.py
+-rw-rw-rw-   0        0        0     3012 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Frequency.py
+-rw-rw-rw-   0        0        0     3457 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/IqData.py
+-rw-rw-rw-   0        0        0     3197 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Irepetition.py
+-rw-rw-rw-   0        0        0     2819 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/ParameterSetList.py
+-rw-rw-rw-   0        0        0     3073 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/ReTrigger.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/__init__.py
+-rw-rw-rw-   0        0        0     3396 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.192959 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/
+-rw-rw-rw-   0        0        0     1116 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Catalog.py
+-rw-rw-rw-   0        0        0     1752 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.205924 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/
+-rw-rw-rw-   0        0        0     1041 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.211908 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass_/
+-rw-rw-rw-   0        0        0     3528 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass_/Bandwidth.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass_/__init__.py
+-rw-rw-rw-   0        0        0     2722 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandwidth.py
+-rw-rw-rw-   0        0        0     1023 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.216894 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss_/
+-rw-rw-rw-   0        0        0     3552 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss_/Bandwidth.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss_/__init__.py
+-rw-rw-rw-   0        0        0     4314 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/TypePy.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/__init__.py
+-rw-rw-rw-   0        0        0     3382 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Mlength.py
+-rw-rw-rw-   0        0        0     2500 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/PdefSet.py
+-rw-rw-rw-   0        0        0     3044 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Slength.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/__init__.py
+-rw-rw-rw-   0        0        0     1433 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/Trigger.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/__init__.py
+-rw-rw-rw-   0        0        0     6938 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/RfSettings.py
+-rw-rw-rw-   0        0        0     1424 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Scenario.py
+-rw-rw-rw-   0        0        0     5217 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.226868 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/
+-rw-rw-rw-   0        0        0     3561 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.235845 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/
+-rw-rw-rw-   0        0        0     2111 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Rbw.py
+-rw-rw-rw-   0        0        0     2181 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Swt.py
+-rw-rw-rw-   0        0        0     2151 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Vbw.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/__init__.py
+-rw-rw-rw-   0        0        0     4628 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.240830 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency_/
+-rw-rw-rw-   0        0        0     2358 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency_/Span.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency_/__init__.py
+-rw-rw-rw-   0        0        0     3762 2020-12-28 20:25:11.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.248810 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/
+-rw-rw-rw-   0        0        0     3232 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/Rbw.py
+-rw-rw-rw-   0        0        0     2139 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/Vbw.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0     2445 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.252799 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/
+-rw-rw-rw-   0        0        0     1099 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.257787 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/
+-rw-rw-rw-   0        0        0     1037 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.261775 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable_/
+-rw-rw-rw-   0        0        0     1626 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable_/Info.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/__init__.py
+-rw-rw-rw-   0        0        0     1023 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.267759 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/
+-rw-rw-rw-   0        0        0     1535 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.279728 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/
+-rw-rw-rw-   0        0        0     1231 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.287705 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/
+-rw-rw-rw-   0        0        0     1802 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/Rx.py
+-rw-rw-rw-   0        0        0     1802 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/Tx.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/__init__.py
+-rw-rw-rw-   0        0        0     1880 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/Direction.py
+-rw-rw-rw-   0        0        0     2350 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/Info.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/__init__.py
+-rw-rw-rw-   0        0        0     1274 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.295684 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/
+-rw-rw-rw-   0        0        0     1035 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/System.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.299674 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/System_/
+-rw-rw-rw-   0        0        0     1099 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/System_/Attenuation.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.304660 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/System_/Attenuation_/
+-rw-rw-rw-   0        0        0     1323 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/System_/Attenuation_/CorrectionTable.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/System_/Attenuation_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/System_/__init__.py
+-rw-rw-rw-   0        0        0     1023 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/Tenvironment.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.309647 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/Tenvironment_/
+-rw-rw-rw-   0        0        0     1293 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/Tenvironment_/Spath.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/Tenvironment_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/__init__.py
+-rw-rw-rw-   0        0        0     1942 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.324607 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/
+-rw-rw-rw-   0        0        0     1001 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.328597 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/
+-rw-rw-rw-   0        0        0     1029 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.333583 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System_/
+-rw-rw-rw-   0        0        0     1227 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System_/Connectors.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/__init__.py
+-rw-rw-rw-   0        0        0     1041 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Generic.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.338569 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/
+-rw-rw-rw-   0        0        0     1011 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.343556 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement_/
+-rw-rw-rw-   0        0        0     1184 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement_/Dapi.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/__init__.py
+-rw-rw-rw-   0        0        0     1278 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.350538 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/
+-rw-rw-rw-   0        0        0     2283 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.359514 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/
+-rw-rw-rw-   0        0        0     1222 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Correction.py
+-rw-rw-rw-   0        0        0     1204 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Rms.py
+-rw-rw-rw-   0        0        0     2055 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Snumber.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/__init__.py
+-rw-rw-rw-   0        0        0     1810 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.362505 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement_/
+-rw-rw-rw-   0        0        0     2039 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement_/Snumber.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0      967 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Meas.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.368519 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Meas_/
+-rw-rw-rw-   0        0        0      753 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Meas_/Scpi.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Meas_/__init__.py
+-rw-rw-rw-   0        0        0     1613 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.379460 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/
+-rw-rw-rw-   0        0        0     1280 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.388436 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/
+-rw-rw-rw-   0        0        0     1271 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/Generator.py
+-rw-rw-rw-   0        0        0     1289 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/Measurement.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0     1019 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.393423 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte_/
+-rw-rw-rw-   0        0        0     1283 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte_/Measurement.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte_/__init__.py
+-rw-rw-rw-   0        0        0     1031 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.400404 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw_/
+-rw-rw-rw-   0        0        0     1295 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw_/Measurement.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw_/__init__.py
+-rw-rw-rw-   0        0        0     1019 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.405390 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb_/
+-rw-rw-rw-   0        0        0     1283 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb_/Measurement.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/__init__.py
+-rw-rw-rw-   0        0        0     1023 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.410377 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/
+-rw-rw-rw-   0        0        0     3060 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.436307 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/
+-rw-rw-rw-   0        0        0     6191 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.440297 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/
+-rw-rw-rw-   0        0        0     1811 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.446281 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State_/
+-rw-rw-rw-   0        0        0     1200 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/__init__.py
+-rw-rw-rw-   0        0        0     8585 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.452266 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/
+-rw-rw-rw-   0        0        0     1812 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.457251 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State_/
+-rw-rw-rw-   0        0        0     1201 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/__init__.py
+-rw-rw-rw-   0        0        0     7220 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.476201 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/
+-rw-rw-rw-   0        0        0     1838 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Icomponent.py
+-rw-rw-rw-   0        0        0     1241 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.492158 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/
+-rw-rw-rw-   0        0        0     2606 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/Average.py
+-rw-rw-rw-   0        0        0     2606 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/Current.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/__init__.py
+-rw-rw-rw-   0        0        0     1721 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.512106 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/
+-rw-rw-rw-   0        0        0     2027 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Average.py
+-rw-rw-rw-   0        0        0     2027 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Current.py
+-rw-rw-rw-   0        0        0     2027 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Maximum.py
+-rw-rw-rw-   0        0        0     2027 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Minimum.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/__init__.py
+-rw-rw-rw-   0        0        0     1838 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Qcomponent.py
+-rw-rw-rw-   0        0        0     1817 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.520084 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State_/
+-rw-rw-rw-   0        0        0     1206 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/__init__.py
+-rw-rw-rw-   0        0        0     8904 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.537038 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/
+-rw-rw-rw-   0        0        0     1538 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Bin.py
+-rw-rw-rw-   0        0        0      937 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Reliability.py
+-rw-rw-rw-   0        0        0     1814 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.542054 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State_/
+-rw-rw-rw-   0        0        0     1203 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State_/__init__.py
+-rw-rw-rw-   0        0        0      913 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/SymbolRate.py
+-rw-rw-rw-   0        0        0     1649 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Talignment.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/__init__.py
+-rw-rw-rw-   0        0        0     7646 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.562969 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/
+-rw-rw-rw-   0        0        0     1785 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/FreqError.py
+-rw-rw-rw-   0        0        0     1724 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Icomponent.py
+-rw-rw-rw-   0        0        0     1701 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Level.py
+-rw-rw-rw-   0        0        0     2910 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/OfError.py
+-rw-rw-rw-   0        0        0     1701 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Phase.py
+-rw-rw-rw-   0        0        0     1724 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Qcomponent.py
+-rw-rw-rw-   0        0        0     1806 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.567956 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State_/
+-rw-rw-rw-   0        0        0     1195 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/__init__.py
+-rw-rw-rw-   0        0        0     6302 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.574936 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/
+-rw-rw-rw-   0        0        0     1814 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.579923 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor_/
+-rw-rw-rw-   0        0        0     4968 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor_/Power.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor_/__init__.py
+-rw-rw-rw-   0        0        0     1796 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.584910 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State_/
+-rw-rw-rw-   0        0        0     1185 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/__init__.py
+-rw-rw-rw-   0        0        0     3167 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.604857 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/
+-rw-rw-rw-   0        0        0     1102 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Clear.py
+-rw-rw-rw-   0        0        0     1672 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.620815 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/
+-rw-rw-rw-   0        0        0     1596 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Frequency.py
+-rw-rw-rw-   0        0        0     1561 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Gain.py
+-rw-rw-rw-   0        0        0     2372 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/State.py
+-rw-rw-rw-   0        0        0     1235 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.629791 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/
+-rw-rw-rw-   0        0        0     1621 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/Frequency.py
+-rw-rw-rw-   0        0        0     1586 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/Gain.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/__init__.py
+-rw-rw-rw-   0        0        0     1644 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Open.py
+-rw-rw-rw-   0        0        0     1651 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Short.py
+-rw-rw-rw-   0        0        0     1483 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.636772 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State_/
+-rw-rw-rw-   0        0        0      942 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/__init__.py
+-rw-rw-rw-   0        0        0     9209 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.674671 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/
+-rw-rw-rw-   0        0        0     1145 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/AmplitudeProbDensity.py
+-rw-rw-rw-   0        0        0     4467 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.678659 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average_/
+-rw-rw-rw-   0        0        0     1613 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average_/Rms.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average_/__init__.py
+-rw-rw-rw-   0        0        0     2329 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.690627 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/
+-rw-rw-rw-   0        0        0     1725 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Power.py
+-rw-rw-rw-   0        0        0     1333 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Probability.py
+-rw-rw-rw-   0        0        0     1478 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Sample.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/__init__.py
+-rw-rw-rw-   0        0        0     4951 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.704591 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/
+-rw-rw-rw-   0        0        0     1649 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Maximum.py
+-rw-rw-rw-   0        0        0     1649 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Minimum.py
+-rw-rw-rw-   0        0        0     1613 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Rms.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/__init__.py
+-rw-rw-rw-   0        0        0     1163 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ElapsedStats.py
+-rw-rw-rw-   0        0        0     2935 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.710575 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData_/
+-rw-rw-rw-   0        0        0     1493 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData_/Bin.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData_/__init__.py
+-rw-rw-rw-   0        0        0     1973 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqInfo.py
+-rw-rw-rw-   0        0        0     2221 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.737502 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/
+-rw-rw-rw-   0        0        0     4299 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Average.py
+-rw-rw-rw-   0        0        0     4299 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Current.py
+-rw-rw-rw-   0        0        0     1015 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.742489 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum_/
+-rw-rw-rw-   0        0        0     4376 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum_/Current.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum_/__init__.py
+-rw-rw-rw-   0        0        0     1015 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.747476 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum_/
+-rw-rw-rw-   0        0        0     4376 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum_/Current.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum_/__init__.py
+-rw-rw-rw-   0        0        0     1236 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.758446 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/
+-rw-rw-rw-   0        0        0     4349 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/Maximum.py
+-rw-rw-rw-   0        0        0     4349 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/Minimum.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/__init__.py
+-rw-rw-rw-   0        0        0     4341 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/StandardDev.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/__init__.py
+-rw-rw-rw-   0        0        0     1255 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.767423 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/
+-rw-rw-rw-   0        0        0     3951 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/Current.py
+-rw-rw-rw-   0        0        0     1649 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/Maximum.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/__init__.py
+-rw-rw-rw-   0        0        0     1255 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.775401 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/
+-rw-rw-rw-   0        0        0     3951 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/Current.py
+-rw-rw-rw-   0        0        0     1649 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/Minimum.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/__init__.py
+-rw-rw-rw-   0        0        0     1234 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.784378 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/
+-rw-rw-rw-   0        0        0     3924 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/Maximum.py
+-rw-rw-rw-   0        0        0     3924 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/Minimum.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/__init__.py
+-rw-rw-rw-   0        0        0     4553 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.791359 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev_/
+-rw-rw-rw-   0        0        0     1669 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev_/Current.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev_/__init__.py
+-rw-rw-rw-   0        0        0     1799 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.798340 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State_/
+-rw-rw-rw-   0        0        0     1188 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/__init__.py
+-rw-rw-rw-   0        0        0     4759 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.829256 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/
+-rw-rw-rw-   0        0        0     1739 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.842222 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Average.py
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Current.py
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Maximum.py
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Minimum.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/__init__.py
+-rw-rw-rw-   0        0        0     1814 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.847208 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker_/
+-rw-rw-rw-   0        0        0     2305 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker_/Npeak.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker_/__init__.py
+-rw-rw-rw-   0        0        0     1739 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.861172 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Average.py
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Current.py
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Maximum.py
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Minimum.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/__init__.py
+-rw-rw-rw-   0        0        0     1739 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.874137 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Average.py
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Current.py
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Maximum.py
+-rw-rw-rw-   0        0        0     1643 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Minimum.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/__init__.py
+-rw-rw-rw-   0        0        0     1279 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.881118 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/
+-rw-rw-rw-   0        0        0     2019 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/Npeak.py
+-rw-rw-rw-   0        0        0     2019 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/Speak.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/__init__.py
+-rw-rw-rw-   0        0        0     1703 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.896078 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/
+-rw-rw-rw-   0        0        0     1619 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Average.py
+-rw-rw-rw-   0        0        0     1619 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Current.py
+-rw-rw-rw-   0        0        0     1619 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Maximum.py
+-rw-rw-rw-   0        0        0     1619 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Minimum.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/__init__.py
+-rw-rw-rw-   0        0        0     1730 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.915027 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/
+-rw-rw-rw-   0        0        0     1637 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Average.py
+-rw-rw-rw-   0        0        0     1637 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Current.py
+-rw-rw-rw-   0        0        0     1637 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Maximum.py
+-rw-rw-rw-   0        0        0     1637 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Minimum.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/__init__.py
+-rw-rw-rw-   0        0        0     1492 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.922009 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State_/
+-rw-rw-rw-   0        0        0      951 2020-12-28 20:25:13.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0      989 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.928990 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/
+-rw-rw-rw-   0        0        0     1023 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.935973 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/
+-rw-rw-rw-   0        0        0     1019 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.942953 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement_/
+-rw-rw-rw-   0        0        0     4700 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement_/Ploss.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/__init__.py
+-rw-rw-rw-   0        0        0      993 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.948938 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/
+-rw-rw-rw-   0        0        0     1035 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/System.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.954923 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/System_/
+-rw-rw-rw-   0        0        0     1099 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.959908 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation_/
+-rw-rw-rw-   0        0        0     1305 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation_/CorrectionTable.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/System_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/__init__.py
+-rw-rw-rw-   0        0        0     1274 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.968884 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/
+-rw-rw-rw-   0        0        0     1035 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/System.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.975865 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/System_/
+-rw-rw-rw-   0        0        0     1099 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.981849 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation_/
+-rw-rw-rw-   0        0        0     1263 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation_/CorrectionTable.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/System_/__init__.py
+-rw-rw-rw-   0        0        0     1023 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.987832 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/
+-rw-rw-rw-   0        0        0     1063 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:18.993817 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/
+-rw-rw-rw-   0        0        0     1231 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/CorrectionTable.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.003790 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/CorrectionTable_/
+-rw-rw-rw-   0        0        0     1213 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/CorrectionTable_/Rx.py
+-rw-rw-rw-   0        0        0     1213 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/CorrectionTable_/Tx.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/CorrectionTable_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/__init__.py
+-rw-rw-rw-   0        0        0      983 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.011769 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/
+-rw-rw-rw-   0        0        0     1023 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.018750 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/
+-rw-rw-rw-   0        0        0     1019 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.024736 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/
+-rw-rw-rw-   0        0        0     1001 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.030719 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power_/
+-rw-rw-rw-   0        0        0     1626 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power_/Current.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/__init__.py
+-rw-rw-rw-   0        0        0     1628 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.045679 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/
+-rw-rw-rw-   0        0        0     1279 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.058643 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/
+-rw-rw-rw-   0        0        0     3811 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.067620 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/
+-rw-rw-rw-   0        0        0     1442 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/RfSettings.py
+-rw-rw-rw-   0        0        0     4800 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/Scenario.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/__init__.py
+-rw-rw-rw-   0        0        0     3846 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.076596 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/
+-rw-rw-rw-   0        0        0     1434 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/RfSettings.py
+-rw-rw-rw-   0        0        0     6441 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.085573 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/
+-rw-rw-rw-   0        0        0      881 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/Catalog.py
+-rw-rw-rw-   0        0        0     1212 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/MaProtocol.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0     1029 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrMmw.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.091556 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrMmw_/
+-rw-rw-rw-   0        0        0     1225 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrMmw_/Measurement.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrMmw_/__init__.py
+-rw-rw-rw-   0        0        0     1029 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrSub.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.097540 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrSub_/
+-rw-rw-rw-   0        0        0     1225 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrSub_/Measurement.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrSub_/__init__.py
+-rw-rw-rw-   0        0        0     1017 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Uwb.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.103523 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Uwb_/
+-rw-rw-rw-   0        0        0     1213 2020-12-28 20:25:12.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Uwb_/Measurement.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Uwb_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/__init__.py
+-rw-rw-rw-   0        0        0      979 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.108510 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/
+-rw-rw-rw-   0        0        0     1009 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.115494 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/
+-rw-rw-rw-   0        0        0     4136 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.153390 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/
+-rw-rw-rw-   0        0        0     9151 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.178323 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/
+-rw-rw-rw-   0        0        0     4006 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/File.py
+-rw-rw-rw-   0        0        0     2006 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Marker.py
+-rw-rw-rw-   0        0        0     3261 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Msegment.py
+-rw-rw-rw-   0        0        0     2651 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Samples.py
+-rw-rw-rw-   0        0        0     2263 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Segments.py
+-rw-rw-rw-   0        0        0     2674 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.184308 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker_/
+-rw-rw-rw-   0        0        0     1117 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker_/Clist.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/__init__.py
+-rw-rw-rw-   0        0        0     2117 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.191288 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/
+-rw-rw-rw-   0        0        0     2579 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/Level.py
+-rw-rw-rw-   0        0        0     3625 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/Ofrequency.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/__init__.py
+-rw-rw-rw-   0        0        0     3383 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/IqSettings.py
+-rw-rw-rw-   0        0        0    10353 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.229187 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/
+-rw-rw-rw-   0        0        0     2468 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Dgain.py
+-rw-rw-rw-   0        0        0     2435 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Dtime.py
+-rw-rw-rw-   0        0        0     1089 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Esingle.py
+-rw-rw-rw-   0        0        0     3139 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Fill.py
+-rw-rw-rw-   0        0        0     2500 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Frequency.py
+-rw-rw-rw-   0        0        0     2384 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.236169 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment_/
+-rw-rw-rw-   0        0        0     1802 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment_/Enabling.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment_/__init__.py
+-rw-rw-rw-   0        0        0     2524 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Irepetition.py
+-rw-rw-rw-   0        0        0     2532 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Modulation.py
+-rw-rw-rw-   0        0        0     2522 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Reenabling.py
+-rw-rw-rw-   0        0        0     2512 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/RfLevel.py
+-rw-rw-rw-   0        0        0     1071 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Rlist.py
+-rw-rw-rw-   0        0        0     1071 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Slist.py
+-rw-rw-rw-   0        0        0     2164 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Sstop.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/__init__.py
+-rw-rw-rw-   0        0        0     2637 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Reliability.py
+-rw-rw-rw-   0        0        0     4543 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/RfSettings.py
+-rw-rw-rw-   0        0        0     6868 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.270078 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/
+-rw-rw-rw-   0        0        0     8251 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.310968 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/
+-rw-rw-rw-   0        0        0     1628 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Check.py
+-rw-rw-rw-   0        0        0     1755 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/CrcProtect.py
+-rw-rw-rw-   0        0        0     1228 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Download.py
+-rw-rw-rw-   0        0        0     1508 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Duration.py
+-rw-rw-rw-   0        0        0     1537 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Paratio.py
+-rw-rw-rw-   0        0        0     1622 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Path.py
+-rw-rw-rw-   0        0        0     1511 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Poffset.py
+-rw-rw-rw-   0        0        0     1687 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Reliability.py
+-rw-rw-rw-   0        0        0     1726 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Rmessage.py
+-rw-rw-rw-   0        0        0     1582 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Roption.py
+-rw-rw-rw-   0        0        0     1503 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Samples.py
+-rw-rw-rw-   0        0        0     1518 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/SymbolRate.py
+-rw-rw-rw-   0        0        0     1585 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Waveform.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/__init__.py
+-rw-rw-rw-   0        0        0     1956 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.318947 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone_/
+-rw-rw-rw-   0        0        0     3544 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone_/Ofrequency.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone_/__init__.py
+-rw-rw-rw-   0        0        0     5649 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.367817 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/
+-rw-rw-rw-   0        0        0     2839 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Acycles.py
+-rw-rw-rw-   0        0        0     2843 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Dgain.py
+-rw-rw-rw-   0        0        0     2813 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Dtime.py
+-rw-rw-rw-   0        0        0     2442 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.384771 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/
+-rw-rw-rw-   0        0        0     1282 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Call.py
+-rw-rw-rw-   0        0        0     1129 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Insert.py
+-rw-rw-rw-   0        0        0     1118 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Mdown.py
+-rw-rw-rw-   0        0        0     1102 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Mup.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/__init__.py
+-rw-rw-rw-   0        0        0     3814 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.397736 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/
+-rw-rw-rw-   0        0        0     1383 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Apply.py
+-rw-rw-rw-   0        0        0     3563 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Dgain.py
+-rw-rw-rw-   0        0        0     3751 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Frequency.py
+-rw-rw-rw-   0        0        0     3500 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Lrms.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/__init__.py
+-rw-rw-rw-   0        0        0     3156 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Frequency.py
+-rw-rw-rw-   0        0        0     3604 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Itransition.py
+-rw-rw-rw-   0        0        0     4876 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Lincrement.py
+-rw-rw-rw-   0        0        0     2765 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Lrms.py
+-rw-rw-rw-   0        0        0     4256 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.407710 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/
+-rw-rw-rw-   0        0        0     2380 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Catalog.py
+-rw-rw-rw-   0        0        0     2935 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.412697 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index_/
+-rw-rw-rw-   0        0        0     2179 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/__init__.py
+-rw-rw-rw-   0        0        0     1531 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/SymbolRate.py
+-rw-rw-rw-   0        0        0     1512 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Ttime.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/__init__.py
+-rw-rw-rw-   0        0        0     1001 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.418681 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker_/
+-rw-rw-rw-   0        0        0     3886 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker_/Delays.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker_/__init__.py
+-rw-rw-rw-   0        0        0     2706 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Reliability.py
+-rw-rw-rw-   0        0        0     1427 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Rmarker.py
+-rw-rw-rw-   0        0        0     2058 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/State.py
+-rw-rw-rw-   0        0        0     2171 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Tdd.py
+-rw-rw-rw-   0        0        0     1824 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.423667 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker_/
+-rw-rw-rw-   0        0        0     3645 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker_/Delay.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/__init__.py
+-rw-rw-rw-   0        0        0     1878 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/State.py
+-rw-rw-rw-   0        0        0     2047 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Tdd.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/__init__.py
+-rw-rw-rw-   0        0        0     1033 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.427657 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/
+-rw-rw-rw-   0        0        0     1097 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/Attenuation.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.432644 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/Attenuation_/
+-rw-rw-rw-   0        0        0     1411 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.438628 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable_/
+-rw-rw-rw-   0        0        0     1062 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable_/All.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/Attenuation_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/__init__.py
+-rw-rw-rw-   0        0        0     1021 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Tenvironment.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.445608 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Tenvironment_/
+-rw-rw-rw-   0        0        0      780 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Tenvironment_/Spath.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Tenvironment_/__init__.py
+-rw-rw-rw-   0        0        0      984 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.452591 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/
+-rw-rw-rw-   0        0        0     1279 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.462564 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/
+-rw-rw-rw-   0        0        0     1252 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.473536 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/
+-rw-rw-rw-   0        0        0     5484 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.486499 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/
+-rw-rw-rw-   0        0        0      870 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Catalog.py
+-rw-rw-rw-   0        0        0     1009 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.491485 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual_/
+-rw-rw-rw-   0        0        0     1129 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual_/Execute.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual_/__init__.py
+-rw-rw-rw-   0        0        0     2007 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.497469 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/
+-rw-rw-rw-   0        0        0     1011 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.502457 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual_/
+-rw-rw-rw-   0        0        0     1185 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual_/Execute.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/__init__.py
+-rw-rw-rw-   0        0        0     2473 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.512429 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/
+-rw-rw-rw-   0        0        0     2184 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/IsMeas.py
+-rw-rw-rw-   0        0        0     2228 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/IsTrigger.py
+-rw-rw-rw-   0        0        0     1009 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.518414 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual_/
+-rw-rw-rw-   0        0        0     1247 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual_/Execute.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/__init__.py
+-rw-rw-rw-   0        0        0     2060 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.534371 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/
+-rw-rw-rw-   0        0        0    10672 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.541352 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn_/
+-rw-rw-rw-   0        0        0     1057 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn_/Catalog.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn_/__init__.py
+-rw-rw-rw-   0        0        0     8477 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.549331 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder_/
+-rw-rw-rw-   0        0        0     1055 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder_/Catalog.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder_/__init__.py
+-rw-rw-rw-   0        0        0     9111 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.556312 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot_/
+-rw-rw-rw-   0        0        0     1045 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot_/Catalog.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot_/__init__.py
+-rw-rw-rw-   0        0        0     9373 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.565290 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/
+-rw-rw-rw-   0        0        0     1035 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/Catalog.py
+-rw-rw-rw-   0        0        0     1061 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.574267 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList_/
+-rw-rw-rw-   0        0        0     2932 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList_/Offset.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/__init__.py
+-rw-rw-rw-   0        0        0     6183 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.580248 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum_/
+-rw-rw-rw-   0        0        0      891 2020-12-28 20:25:14.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum_/Catalog.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/__init__.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:19.671006 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/
+-rw-rw-rw-   0        0        0      560 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgLinkedEventArgs.py
+-rw-rw-rw-   0        0        0     4106 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgSingle.py
+-rw-rw-rw-   0        0        0     1086 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgSingleList.py
+-rw-rw-rw-   0        0        0     1028 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py
+-rw-rw-rw-   0        0        0     9241 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgStringComposer.py
+-rw-rw-rw-   0        0        0     5762 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgStruct.py
+-rw-rw-rw-   0        0        0     3433 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgStructList.py
+-rw-rw-rw-   0        0        0     2502 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgStructStringParser.py
+-rw-rw-rw-   0        0        0     5309 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/CommandsGroup.py
+-rw-rw-rw-   0        0        0    20352 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/Conversions.py
+-rw-rw-rw-   0        0        0     3693 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ConverterFromScpiString.py
+-rw-rw-rw-   0        0        0     4489 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ConverterToScpiString.py
+-rw-rw-rw-   0        0        0    10071 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/Core.py
+-rw-rw-rw-   0        0        0    35553 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/Instrument.py
+-rw-rw-rw-   0        0        0     4021 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/InstrumentErrors.py
+-rw-rw-rw-   0        0        0     2161 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/InstrumentOptions.py
+-rw-rw-rw-   0        0        0     5258 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/InstrumentSettings.py
+-rw-rw-rw-   0        0        0     3467 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/InternalLinker.py
+-rw-rw-rw-   0        0        0     4435 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/IoTransferEventArgs.py
+-rw-rw-rw-   0        0        0     3747 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/RepeatedCapability.py
+-rw-rw-rw-   0        0        0     4847 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/StreamReader.py
+-rw-rw-rw-   0        0        0     5074 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/StreamWriter.py
+-rw-rw-rw-   0        0        0     1069 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/StructBase.py
+-rw-rw-rw-   0        0        0     3002 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/Types.py
+-rw-rw-rw-   0        0        0     4669 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/Utilities.py
+-rw-rw-rw-   0        0        0     5025 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/VisaPluginSocketIo.py
+-rw-rw-rw-   0        0        0    44245 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/VisaSession.py
+-rw-rw-rw-   0        0        0     7168 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/VisaSessionSim.py
+-rw-rw-rw-   0        0        0        0 2020-12-25 17:14:40.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/__init__.py
+-rw-rw-rw-   0        0        0    11471 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/RsCMPX_Gprf.py
+-rw-rw-rw-   0        0        0      848 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/__init__.py
+-rw-rw-rw-   0        0        0    12119 2020-12-28 20:25:04.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/enums.py
+-rw-rw-rw-   0        0        0     2000 2020-12-28 20:25:04.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/repcap.py
+drwxrwxrwx   0        0        0        0 2020-12-28 20:25:17.791525 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf.egg-info/
+-rw-rw-rw-   0        0        0     2316 2020-12-28 20:25:17.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    45476 2020-12-28 20:25:17.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-12-28 20:25:17.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2020-12-28 20:25:17.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2020-12-28 20:25:17.000000 RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-12-28 20:25:19.677988 RsCMPX_Gprf-4.0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0      888 2020-12-28 20:25:15.000000 RsCMPX_Gprf-4.0.7.9/setup.py
```

### Comparing `RsCMPX_Gprf-4.0.7.10/PKG-INFO` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 Metadata-Version: 2.1
-Name: RsCMPX_Gprf
-Version: 4.0.7.10
+Name: RsCMPX-Gprf
+Version: 4.0.7.9
 Summary: CMX/CMP Global Purpose RF Remote-control Module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 Author-email: Customer.Support@rohde-schwarz.com
 License: MIT
-Description: Rohde & Schwarz CMX/CMP Global Purpose RF RsCMPX_Gprf instrument driver.
+Description: Rohde & Schwarz CMX/CMP Global Purpose RF RsCMPX_Gprf instrument driver Version 4.0.7.9
         
-        Supported instruments: CMX500, CMP200
-        
-        The package is hosted here: https://pypi.org/project/RsCMPX_Gprf/
-        
-        Documentation: https://RsCMPX_Gprf.readthedocs.io/
-        
-        Examples: https://github.com/Rohde-Schwarz/Examples/
+        Check out the module documentation on https://RsCMPX_Gprf.readthedocs.io/
         
         --------------------------------------------------------------------------------
         
         Currently supported CMX/CMP subsystems:
         
         - Base: `RsCmpx_Base <https://RsCmpx_Base.readthedocs.io/>`_
         - GPRF: `RsCmpx_Gprf <https://RsCmpx_Gprf.readthedocs.io/>`_
@@ -31,19 +25,19 @@
         In case you require support for more subsystems, please contact our customer support on customersupport@rohde-schwarz.com
         with the topic "Auto-generated Python drivers" in the email subject. This will speed up the response process
         
         --------------------------------------------------------------------------------
         
         Release Notes: for the whole RsCmpx_xxx group:
         
-        Latest release notes summary: Added documentation on ReadTheDocs
+        Latest release notes summary: Added documentation on ReadTheDocs.io
         
         Version 4.0.7.4
         
-        - Added documentation on ReadTheDocs
+        - Added documentation on ReadTheDocs.io
         
         Version 4.0.7.3
         
         - Added new subsystems NrFr2Meas, UwbMeas, Signaling
         
         Version 4.0.7.2
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/CustomFiles/events.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/CustomFiles/events.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,37 +17,23 @@
 	@io_events_include_data.setter
 	def io_events_include_data(self, value: bool) -> None:
 		"""If True, the on_write and on_read events include also the sent/received data.
 		Default value is False, to avoid handling potentially big data."""
 		self._core.io.io_events_include_data = value
 
 	@property
-	def before_write_handler(self) -> Callable:
-		"""Returns the handler of before_write events. \n
-		:return: current before_write_handler"""
-		return self._core.io.before_write_handler
-
-	@before_write_handler.setter
-	def before_write_handler(self, handler: Callable) -> None:
-		"""Sets handler for before_write events.
-		The before_write event is invoked before each write operation (only once, not for every chunk)
-		Event prototype: handler(io: Instrument, cmd: str)
-		:param handler: new handler"""
-		self._core.io.before_write_handler = handler
-
-	@property
 	def on_write_handler(self) -> Callable:
 		"""Returns the handler of on_write events. \n
 		:return: current on_write_handler"""
 		return self._core.io.on_write_handler
 
 	@on_write_handler.setter
 	def on_write_handler(self, handler: Callable) -> None:
 		"""Sets handler for on_write events.
-		The on_write event is invoked every time the driver performs a write operation to the instrument (for each write chunk)
+		The on_write event is invoked every time the driver performs a write operation to the instrument.
 		Event arguments type: IoTransferEventArgs
 		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
 		:param handler: new handler for all write operations"""
 		self._core.io.on_write_handler = handler
 
 	@property
 	def on_read_handler(self) -> Callable:
@@ -59,21 +45,7 @@
 	def on_read_handler(self, handler: Callable) -> None:
 		"""Sets handler for on_read events.
 		The on_read event is invoked every time the driver performs a read operation to the instrument.
 		Event arguments type: IoTransferEventArgs
 		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
 		:param handler: new handler for all read operations"""
 		self._core.io.on_read_handler = handler
-
-	@property
-	def before_query_handler(self) -> Callable:
-		"""Returns the handler of before_query events. \n
-		:return: current before_query_handler"""
-		return self._core.io.before_query_handler
-
-	@before_query_handler.setter
-	def before_query_handler(self, handler: Callable) -> None:
-		"""Sets handler for before_query events.
-		The before_query event is invoked before each query operation (only once, not for every chunk)
-		Event prototype: handler(io: Instrument, query: str)
-		:param handler: new handler"""
-		self._core.io.before_query_handler = handler
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/CustomFiles/reliability.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/CustomFiles/reliability.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import time
-from typing import Callable
-
-from ..Internal import ArgLinkedEventArgs
-from ..Internal import Core
-
-codes_table = {
-				0:       'OK',
-				1:       'Measurement Timeout',
-				2:       'Capture Buffer Overflow',
-				3:       'Over-driven',
-				4:       'Under-driven',
-				6:       'Trigger Timeout',
-				7:       'Acquisition Error',
-				8:       'Sync Error',
-				9:       'Uncalibrated',
-				15:      'Reference Frequency Error',
-				16:      'RF Not Available',
-				17:      'RF Level not Settled',
-				18:      'RF Frequency not Settled',
-				19:      'Call not Established',
-				20:      'Call Type not Usable',
-				21:      'Call Lost',
-				23:      'Missing Option',
-				24:      'Invalid RF Setting',
-				26:      'Resource Conflict',
-				27:      'No Sensor Connected',
-				28:      'Unexpected Parameter Change',
-				30:      'File not Found',
-				31:      'No DTM reply',
-				32:      'ACL Disconnected',
-				40:      'ARB File CRC Error',
-				42:      'ARB Header Tag Invalid',
-				43:      'ARB Segment Overflow',
-				44:      'ARB File not Found',
-				45:      'ARB Memory Overflow',
-				46:      'ARB Sample Rate out of Range',
-				47:      'ARB Cycles out of Range',
-				50:      'Startup Error',
-				51:      'No Reply',
-				52:      'Connection Error',
-				53:      'Configuration Error',
-				54:      'Filesystem Error',
-				60:      'Invalid RF-Connector Setting',
-				93:      'OCXO Oven Temperature too low',
-				101:     'Firmware Error',
-				102:     'Unidentified Error',
-				103:     'Parameter Error',
-				104:     'Not Functional'}
-
-
-class ReliabilityEventArgs:
-	"""Arguments for reliability indicator event."""
-
-	def __init__(self, timestamp, code: int, message: str, context: str):
-		self.timestamp = timestamp
-		self.message = message
-		self.code = code
-		self.message = message
-		self.context = context
-
-
-class Reliability:
-	"""Reliability class that handles all the necessary tasks related to reliability indicator."""
-
-	def __init__(self, core: Core):
-		self._core = core
-		self._last_value = 0
-		self._last_context = ''
-		self._last_timestamp = None
-		self._exception_on_error = False
-		# noinspection PyTypeChecker
-		self._on_update_handler: Callable = None
-		self._core.set_link_handler('Reliability', self._permanent_on_update_handler)
-
-	@property
-	def last_value(self):
-		"""Returns the last updated Reliability code."""
-		return self._last_value
-
-	@property
-	def last_context(self) -> str:
-		"""Returns the last updated Context of the reliability code - usually the SCPI query on which the instrument responded with the Reliability code."""
-		return self._last_context
-
-	@property
-	def last_timestamp(self) -> time:
-		"""Returns the time of the last Reliability update."""
-		return self._last_timestamp
-
-	@property
-	def last_message(self) -> str:
-		"""Returns the LastValue of the reliability table converted to human-readable string."""
-		if self._last_value in codes_table:
-			return codes_table[self._last_value]
-		else:
-			return f'Undefined reliability code {self._last_value}.'
-
-	@property
-	def exception_on_error(self) -> bool:
-		"""see the exception_on_error.setter."""
-		return self._exception_on_error
-
-	@exception_on_error.setter
-	def exception_on_error(self, value) -> None:
-		"""If True, (default is False) the object throws an exception if the updated reliability is not 0 (non-OK)."""
-		self._exception_on_error = value
-
-	def on_update_handler(self, handler: Callable) -> None:
-		"""Register the handler for on_update event.
-		This handler is invoked with each update of the reliability indicator.
-		Handler API: handler(event_args: ReliabilityEventArgs)"""
-		self._on_update_handler = handler
-
-	def _permanent_on_update_handler(self, event_args: ArgLinkedEventArgs):
-		"""Permanent on_update handler. Takes care of updating all the 'last_xxx' values and calling a user-defined updated_handler."""
-		self._last_value = int(str(event_args.value))
-		self._last_context = event_args.context
-		self._last_timestamp = event_args.timestamp
-
-		if self._on_update_handler:
-			# Call the additional handler if registered
-			rel_events_args = ReliabilityEventArgs(self._last_timestamp, self._last_value, self.last_message, self._last_context)
-			self._on_update_handler(rel_events_args)
-
-		if self._exception_on_error and self._last_value != 0:
-			raise Exception(
-				f'Reliability indicator error. Time: {time.strftime("%H:%M:%S", time.localtime(self._last_timestamp))}, '
-				f'Context: {self._last_context}, Value {self._last_value}: {self.last_message}')
+import time
+from typing import Callable
+
+from ..Internal import ArgLinkedEventArgs
+from ..Internal import Core
+
+codes_table = {
+				0:       'OK',
+				1:       'Measurement Timeout',
+				2:       'Capture Buffer Overflow',
+				3:       'Over-driven',
+				4:       'Under-driven',
+				6:       'Trigger Timeout',
+				7:       'Acquisition Error',
+				8:       'Sync Error',
+				9:       'Uncalibrated',
+				15:      'Reference Frequency Error',
+				16:      'RF Not Available',
+				17:      'RF Level not Settled',
+				18:      'RF Frequency not Settled',
+				19:      'Call not Established',
+				20:      'Call Type not Usable',
+				21:      'Call Lost',
+				23:      'Missing Option',
+				24:      'Invalid RF Setting',
+				26:      'Resource Conflict',
+				27:      'No Sensor Connected',
+				28:      'Unexpected Parameter Change',
+				30:      'File not Found',
+				31:      'No DTM reply',
+				32:      'ACL Disconnected',
+				40:      'ARB File CRC Error',
+				42:      'ARB Header Tag Invalid',
+				43:      'ARB Segment Overflow',
+				44:      'ARB File not Found',
+				45:      'ARB Memory Overflow',
+				46:      'ARB Sample Rate out of Range',
+				47:      'ARB Cycles out of Range',
+				50:      'Startup Error',
+				51:      'No Reply',
+				52:      'Connection Error',
+				53:      'Configuration Error',
+				54:      'Filesystem Error',
+				60:      'Invalid RF-Connector Setting',
+				93:      'OCXO Oven Temperature too low',
+				101:     'Firmware Error',
+				102:     'Unidentified Error',
+				103:     'Parameter Error',
+				104:     'Not Functional'}
+
+
+class ReliabilityEventArgs:
+	"""Arguments for reliability indicator event."""
+
+	def __init__(self, timestamp, code: int, message: str, context: str):
+		self.timestamp = timestamp
+		self.message = message
+		self.code = code
+		self.message = message
+		self.context = context
+
+
+class Reliability:
+	"""Reliability class that handles all the necessary tasks related to reliability indicator."""
+
+	def __init__(self, core: Core):
+		self._core = core
+		self._last_value = 0
+		self._last_context = ''
+		self._last_timestamp = None
+		self._exception_on_error = False
+		# noinspection PyTypeChecker
+		self._on_update_handler: Callable = None
+		self._core.set_link_handler('Reliability', self._permanent_on_update_handler)
+
+	@property
+	def last_value(self):
+		"""Returns the last updated Reliability code."""
+		return self._last_value
+
+	@property
+	def last_context(self) -> str:
+		"""Returns the last updated Context of the reliability code - usually the SCPI query on which the instrument responded with the Reliability code."""
+		return self._last_context
+
+	@property
+	def last_timestamp(self) -> time:
+		"""Returns the time of the last Reliability update."""
+		return self._last_timestamp
+
+	@property
+	def last_message(self) -> str:
+		"""Returns the LastValue of the reliability table converted to human-readable string."""
+		if self._last_value in codes_table:
+			return codes_table[self._last_value]
+		else:
+			return f'Undefined reliability code {self._last_value}.'
+
+	@property
+	def exception_on_error(self) -> bool:
+		"""see the exception_on_error.setter."""
+		return self._exception_on_error
+
+	@exception_on_error.setter
+	def exception_on_error(self, value) -> None:
+		"""If True, (default is False) the object throws an exception if the updated reliability is not 0 (non-OK)."""
+		self._exception_on_error = value
+
+	def on_update_handler(self, handler: Callable) -> None:
+		"""Register the handler for on_update event.
+		This handler is invoked with each update of the reliability indicator.
+		Handler API: handler(event_args: ReliabilityEventArgs)"""
+		self._on_update_handler = handler
+
+	def _permanent_on_update_handler(self, event_args: ArgLinkedEventArgs):
+		"""Permanent on_update handler. Takes care of updating all the 'last_xxx' values and calling a user-defined updated_handler."""
+		self._last_value = int(str(event_args.value))
+		self._last_context = event_args.context
+		self._last_timestamp = event_args.timestamp
+
+		if self._on_update_handler:
+			# Call the additional handler if registered
+			rel_events_args = ReliabilityEventArgs(self._last_timestamp, self._last_value, self.last_message, self._last_context)
+			self._on_update_handler(rel_events_args)
+
+		if self._exception_on_error and self._last_value != 0:
+			raise Exception(
+				f'Reliability indicator error. Time: {time.strftime("%H:%M:%S", time.localtime(self._last_timestamp))}, '
+				f'Context: {self._last_context}, Value {self._last_value}: {self.last_message}')
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/CustomFiles/utilities.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/CustomFiles/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,19 +48,18 @@
 		return self._core.io.firmware_version
 
 	@property
 	def instrument_serial_number(self) -> str:
 		"""Returns instrument's serial_number."""
 		return self._core.io.serial_number
 
-	def query_opc(self, timeout: int = 0) -> int:
+	def query_opc(self) -> int:
 		"""SCPI command: *OPC?
-		Queries the instrument's OPC bit and hence it waits until the instrument reports operation complete.
-		If you define timeout > 0, the VISA timeout is set to that value just for this method call."""
-		return self._core.io.query_opc(timeout)
+		Queries the instrument's OPC bit and hence it waits until the instrument reports operation complete."""
+		return self._core.io.query_opc()
 
 	@property
 	def instrument_status_checking(self) -> bool:
 		"""See the instrument_status_checking.setter."""
 		return self._core.io.query_instr_status
 
 	@instrument_status_checking.setter
@@ -176,19 +175,14 @@
 		Stops further commands processing until all commands sent before *WAI have been executed."""
 		return self._core.io.write('*WAI')
 
 	def write_str(self, cmd: str) -> None:
 		"""Writes the command to the instrument."""
 		self._core.io.write(cmd)
 
-	def write(self, cmd: str) -> None:
-		"""This method is an alias to the write_str().
-		Writes the command to the instrument as string."""
-		self._core.io.write(cmd)
-
 	def write_int(self, cmd: str, param: int) -> None:
 		"""Writes the command to the instrument followed by the integer parameter:
 		e.g.: cmd = 'SELECT:INPUT' param = '2', result command = 'SELECT:INPUT 2'"""
 		self._core.io.write(f'{cmd} {param}')
 
 	def write_int_with_opc(self, cmd: str, param: int, timeout: int = None) -> None:
 		"""Writes the command with OPC to the instrument followed by the integer parameter:
@@ -219,20 +213,14 @@
 		self._core.io.write_with_opc(f'{cmd} {Conv.bool_to_str(param)}', timeout)
 
 	def query_str(self, query: str) -> str:
 		"""Sends the query to the instrument and returns the response as string.
 		The response is trimmed of any trailing LF characters and has no length limit."""
 		return self._core.io.query_str(query)
 
-	def query(self, query: str) -> str:
-		"""This method is an alias to the query_str().
-		Sends the query to the instrument and returns the response as string.
-		The response is trimmed of any trailing LF characters and has no length limit."""
-		return self._core.io.query_str(query)
-
 	def query_bool(self, query: str) -> bool:
 		"""Sends the query to the instrument and returns the response as boolean."""
 		return self._core.io.query_bool(query)
 
 	def query_int(self, query: str) -> int:
 		"""Sends the query to the instrument and returns the response as integer."""
 		return self._core.io.query_int(query)
@@ -242,33 +230,20 @@
 		return self._core.io.query_float(query)
 
 	def write_str_with_opc(self, cmd: str, timeout: int = None) -> None:
 		"""Writes the opc-synced command to the instrument.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		self._core.io.write_with_opc(cmd, timeout)
 
-	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
-		"""This method is an alias to the write_str_with_opc().
-		Writes the opc-synced command to the instrument.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		self._core.io.write_with_opc(cmd, timeout)
-
 	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
 		"""Sends the opc-synced query to the instrument and returns the response as string.
 		The response is trimmed of any trailing LF characters and has no length limit.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		return self._core.io.query_str_with_opc(query, timeout)
 
-	def query_with_opc(self, query: str, timeout: int = None) -> str:
-		"""This method is an alias to the query_str_with_opc().
-		Sends the opc-synced query to the instrument and returns the response as string.
-		The response is trimmed of any trailing LF characters and has no length limit.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		return self._core.io.query_str_with_opc(query, timeout)
-
 	def query_bool_with_opc(self, query: str, timeout: int = None) -> bool:
 		"""Sends the opc-synced query to the instrument and returns the response as boolean.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		return self._core.io.query_bool_with_opc(query, timeout)
 
 	def query_int_with_opc(self, query: str, timeout: int = None) -> int:
 		"""Sends the opc-synced query to the instrument and returns the response as integer.
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/System.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/System.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/System_/Attenuation.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable_/Info.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 from typing import List
 
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.Types import DataType
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
+from ......Internal.Types import DataType
+from ......Internal.StructBase import StructBase
+from ......Internal.ArgStruct import ArgStruct
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Attenuation:
-	"""Attenuation commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Info:
+	"""Info commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("attenuation", core, parent)
+		self._base = CommandsGroup("info", core, parent)
 
 	# noinspection PyTypeChecker
-	class CorrectionTableStruct(StructBase):
-		"""Structure for setting input parameters. Contains optional set arguments. Fields: \n
-			- Name: str: No parameter help available
+	class GetStruct(StructBase):
+		"""Response structure. Fields: \n
 			- Frequency: List[float]: No parameter help available
 			- Attenuation: List[float]: No parameter help available"""
 		__meta_args_list = [
-			ArgStruct.scalar_str('Name'),
-			ArgStruct('Frequency', DataType.FloatList, None, True, True, 1),
-			ArgStruct('Attenuation', DataType.FloatList, None, True, True, 1)]
+			ArgStruct('Frequency', DataType.FloatList, None, False, True, 1),
+			ArgStruct('Attenuation', DataType.FloatList, None, False, True, 1)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Name: str = None
 			self.Frequency: List[float] = None
 			self.Attenuation: List[float] = None
 
-	def set_correction_table(self, value: CorrectionTableStruct) -> None:
-		"""SCPI: ADD:SYSTem:ATTenuation:CTABle \n
-		Snippet: driver.add.system.attenuation.set_correction_table(value = CorrectionTableStruct()) \n
+	def get(self, name: str) -> GetStruct:
+		"""SCPI: [CONFigure]:SYSTem:ATTenuation:CTABle:INFO \n
+		Snippet: value: GetStruct = driver.configure.system.attenuation.correctionTable.info.get(name = '1') \n
 		No command help available \n
-			:param value: see the help for CorrectionTableStruct structure arguments.
-		"""
-		self._core.io.write_struct('ADD:SYSTem:ATTenuation:CTABle', value)
+			:param name: No help available
+			:return: structure: for return value, see the help for GetStruct structure arguments."""
+		param = Conversions.value_to_quoted_str(name)
+		return self._core.io.query_struct(f'CONFigure:SYSTem:ATTenuation:CTABle:INFO? {param}', self.__class__.GetStruct())
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/Rx.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/Tx.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor_/Zero.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Calibration_/Gprf_/Measurement_/ExtPwrSensor_/Zero.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Generator_/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Gprf_/Measurement_/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Lte.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Lte.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Lte_/Measurement_/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrMmw.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrMmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrMmw_/Measurement_/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrSub.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrSub.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/NrSub_/Measurement_/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/System.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/System.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("system", core, parent)
 
 	@property
 	def attenuation(self):
-		"""attenuation commands group. 0 Sub-classes, 1 commands."""
+		"""attenuation commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_attenuation'):
 			from .System_.Attenuation import Attenuation
 			self._attenuation = Attenuation(self._core, self._base)
 		return self._attenuation
 
 	def clone(self) -> 'System':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/System_/Attenuation.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/System_/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment_/Connectors.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Tenvironment_/Connectors.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Uwb.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Uwb.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Catalog_/Uwb_/Measurement_/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Generator.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Generator.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/IqFile.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/IqFile.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 class IqFile:
 	"""IqFile commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("iqFile", core, parent)
 
-	def set(self, filename: str) -> None:
+	def set(self, file_name: str) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:CANalyzer:IQFile \n
-		Snippet: driver.configure.gprf.measurement.canalyzer.iqFile.set(filename = '1') \n
+		Snippet: driver.configure.gprf.measurement.canalyzer.iqFile.set(file_name = '1') \n
 		Saves the I/Q data for the current step to the selected file. \n
-			:param filename: Name and path of the target file.
+			:param file_name: Name and path of the target file.
 		"""
-		param = Conversions.value_to_quoted_str(filename)
+		param = Conversions.value_to_quoted_str(file_name)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:CANalyzer:IQFile {param}')
 
 	def get(self) -> str:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:CANalyzer:IQFile \n
 		Snippet: value: str = driver.configure.gprf.measurement.canalyzer.iqFile.get() \n
 		Saves the I/Q data for the current step to the selected file. \n
-			:return: filename_return: No help available"""
+			:return: file_name_return: No help available"""
 		response = self._core.io.query_str(f'CONFigure:GPRF:MEASurement<Instance>:CANalyzer:IQFile?')
 		return trim_str_response(response)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/Sall.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Canalyzer_/Sall.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Correction.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Correction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,33 +43,33 @@
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:return: tcd_timeout: No help available
+			:return: tcd_time_out: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:EPSensor:TOUT?')
 		return Conversions.str_to_float(response)
 
-	def set_timeout(self, tcd_timeout: float) -> None:
+	def set_timeout(self, tcd_time_out: float) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:EPSensor:TOUT \n
-		Snippet: driver.configure.gprf.measurement.extPwrSensor.set_timeout(tcd_timeout = 1.0) \n
+		Snippet: driver.configure.gprf.measurement.extPwrSensor.set_timeout(tcd_time_out = 1.0) \n
 		Defines a timeout for the measurement. The timer is started when the measurement is initiated via a READ or INIT command.
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:param tcd_timeout: No help available
+			:param tcd_time_out: No help available
 		"""
-		param = Conversions.decimal_value_to_str(tcd_timeout)
+		param = Conversions.decimal_value_to_str(tcd_time_out)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:EPSensor:TOUT {param}')
 
 	# noinspection PyTypeChecker
 	def get_resolution(self) -> enums.PwrSensorResolution:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:EPSensor:RESolution \n
 		Snippet: value: enums.PwrSensorResolution = driver.configure.gprf.measurement.extPwrSensor.get_resolution() \n
 		Defines the number of digits of the displayed power results. This command does not affect the remote control results. \n
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Attenuation.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Attenuation.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 		self._core = core
 		self._base = CommandsGroup("attenuation", core, parent)
 
 	def get_state(self) -> bool:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:EPSensor:ATTenuation:STATe \n
 		Snippet: value: bool = driver.configure.gprf.measurement.extPwrSensor.attenuation.get_state() \n
 		Enables or disables the result correction for an external input attenuation. \n
-			:return: attenuator_state: No help available
+			:return: attenuat_state: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:EPSensor:ATTenuation:STATe?')
 		return Conversions.str_to_bool(response)
 
-	def set_state(self, attenuator_state: bool) -> None:
+	def set_state(self, attenuat_state: bool) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:EPSensor:ATTenuation:STATe \n
-		Snippet: driver.configure.gprf.measurement.extPwrSensor.attenuation.set_state(attenuator_state = False) \n
+		Snippet: driver.configure.gprf.measurement.extPwrSensor.attenuation.set_state(attenuat_state = False) \n
 		Enables or disables the result correction for an external input attenuation. \n
-			:param attenuator_state: No help available
+			:param attenuat_state: No help available
 		"""
-		param = Conversions.bool_to_str(attenuator_state)
+		param = Conversions.bool_to_str(attenuat_state)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:EPSensor:ATTenuation:STATe {param}')
 
 	def get_value(self) -> float:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:EPSensor:ATTenuation \n
 		Snippet: value: float = driver.configure.gprf.measurement.extPwrSensor.attenuation.get_value() \n
 		Specifies an external input attenuation factor for correction of the power results. \n
 			:return: attenuation: No help available
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Auto.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Auto.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/ExtPwrSensor_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,33 +27,33 @@
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:return: tcd_timeout: No help available
+			:return: tcd_time_out: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:FFTSanalyzer:TOUT?')
 		return Conversions.str_to_float(response)
 
-	def set_timeout(self, tcd_timeout: float) -> None:
+	def set_timeout(self, tcd_time_out: float) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:FFTSanalyzer:TOUT \n
-		Snippet: driver.configure.gprf.measurement.fftSpecAn.set_timeout(tcd_timeout = 1.0) \n
+		Snippet: driver.configure.gprf.measurement.fftSpecAn.set_timeout(tcd_time_out = 1.0) \n
 		Defines a timeout for the measurement. The timer is started when the measurement is initiated via a READ or INIT command.
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:param tcd_timeout: No help available
+			:param tcd_time_out: No help available
 		"""
-		param = Conversions.decimal_value_to_str(tcd_timeout)
+		param = Conversions.decimal_value_to_str(tcd_time_out)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:FFTSanalyzer:TOUT {param}')
 
 	# noinspection PyTypeChecker
 	def get_amode(self) -> enums.AveragingMode:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:FFTSanalyzer:AMODe \n
 		Snippet: value: enums.AveragingMode = driver.configure.gprf.measurement.fftSpecAn.get_amode() \n
 		Selects the averaging mode for the average spectrum trace. \n
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn_/PeakSearch.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/FftSpecAn_/PeakSearch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,33 +73,33 @@
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:return: tcd_timeout: No help available
+			:return: tcd_time_out: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:IQRecorder:TOUT?')
 		return Conversions.str_to_float(response)
 
-	def set_timeout(self, tcd_timeout: float) -> None:
+	def set_timeout(self, tcd_time_out: float) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQRecorder:TOUT \n
-		Snippet: driver.configure.gprf.measurement.iqRecorder.set_timeout(tcd_timeout = 1.0) \n
+		Snippet: driver.configure.gprf.measurement.iqRecorder.set_timeout(tcd_time_out = 1.0) \n
 		Defines a timeout for the measurement. The timer is started when the measurement is initiated via a READ or INIT command.
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:param tcd_timeout: No help available
+			:param tcd_time_out: No help available
 		"""
-		param = Conversions.decimal_value_to_str(tcd_timeout)
+		param = Conversions.decimal_value_to_str(tcd_time_out)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:IQRecorder:TOUT {param}')
 
 	def get_ratio(self) -> float:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQRecorder:RATio \n
 		Snippet: value: float = driver.configure.gprf.measurement.iqRecorder.get_ratio() \n
 		Specifies a factor to reduce the sampling rate and to increase the measurement duration. The sampling rate resulting from
 		the filter settings is multiplied with the specified ratio. \n
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/Bandpass.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/Bandpass.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 		self._core = core
 		self._base = CommandsGroup("bandpass", core, parent)
 
 	def get_bandwidth(self) -> float:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQRecorder:FILTer:BANDpass:BWIDth \n
 		Snippet: value: float = driver.configure.gprf.measurement.iqRecorder.filterPy.bandpass.get_bandwidth() \n
 		Selects the bandwidth for a bandpass filter. \n
-			:return: bandpass_bw: Only the following values can be configured: IF unit: 31.25 MHz, 62.5 MHz, 125 MHz, 250 MHz, 500 MHz, 1000 MHz R&S CMW: 1 kHz, 10 kHz, 100 kHz, 1 MHz, 10 MHz, 40 MHz, 160 MHz Other values are rounded to the next allowed value.
+			:return: band_pass_bw: Only the following values can be configured: IF unit: 31.25 MHz, 62.5 MHz, 125 MHz, 250 MHz, 500 MHz, 1000 MHz R&S CMW: 1 kHz, 10 kHz, 100 kHz, 1 MHz, 10 MHz, 40 MHz, 160 MHz Other values are rounded to the next allowed value.
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:IQRecorder:FILTer:BANDpass:BWIDth?')
 		return Conversions.str_to_float(response)
 
-	def set_bandwidth(self, bandpass_bw: float) -> None:
+	def set_bandwidth(self, band_pass_bw: float) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQRecorder:FILTer:BANDpass:BWIDth \n
-		Snippet: driver.configure.gprf.measurement.iqRecorder.filterPy.bandpass.set_bandwidth(bandpass_bw = 1.0) \n
+		Snippet: driver.configure.gprf.measurement.iqRecorder.filterPy.bandpass.set_bandwidth(band_pass_bw = 1.0) \n
 		Selects the bandwidth for a bandpass filter. \n
-			:param bandpass_bw: Only the following values can be configured: IF unit: 31.25 MHz, 62.5 MHz, 125 MHz, 250 MHz, 500 MHz, 1000 MHz R&S CMW: 1 kHz, 10 kHz, 100 kHz, 1 MHz, 10 MHz, 40 MHz, 160 MHz Other values are rounded to the next allowed value.
+			:param band_pass_bw: Only the following values can be configured: IF unit: 31.25 MHz, 62.5 MHz, 125 MHz, 250 MHz, 500 MHz, 1000 MHz R&S CMW: 1 kHz, 10 kHz, 100 kHz, 1 MHz, 10 MHz, 40 MHz, 160 MHz Other values are rounded to the next allowed value.
 		"""
-		param = Conversions.decimal_value_to_str(bandpass_bw)
+		param = Conversions.decimal_value_to_str(band_pass_bw)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:IQRecorder:FILTer:BANDpass:BWIDth {param}')
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/Gauss.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/FilterPy_/Gauss.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/IqSettings.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/IqSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/EnvelopePower.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/EnvelopePower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/Trigger.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/Trigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,33 +35,33 @@
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:return: tcd_timeout: No help available
+			:return: tcd_time_out: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:IQVSlot:TOUT?')
 		return Conversions.str_to_float(response)
 
-	def set_timeout(self, tcd_timeout: float) -> None:
+	def set_timeout(self, tcd_time_out: float) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQVSlot:TOUT \n
-		Snippet: driver.configure.gprf.measurement.iqVsSlot.set_timeout(tcd_timeout = 1.0) \n
+		Snippet: driver.configure.gprf.measurement.iqVsSlot.set_timeout(tcd_time_out = 1.0) \n
 		Defines a timeout for the measurement. The timer is started when the measurement is initiated via a READ or INIT command.
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:param tcd_timeout: No help available
+			:param tcd_time_out: No help available
 		"""
-		param = Conversions.decimal_value_to_str(tcd_timeout)
+		param = Conversions.decimal_value_to_str(tcd_time_out)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:IQVSlot:TOUT {param}')
 
 	# noinspection PyTypeChecker
 	def get_repetition(self) -> enums.Repeat:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQVSlot:REPetition \n
 		Snippet: value: enums.Repeat = driver.configure.gprf.measurement.iqVsSlot.get_repetition() \n
 		Specifies the repetition mode of the measurement. The repetition mode specifies whether the measurement is stopped after
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 		"""envelopePower commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_envelopePower'):
 			from .ListPy_.EnvelopePower import EnvelopePower
 			self._envelopePower = EnvelopePower(self._core, self._base)
 		return self._envelopePower
 
 	@property
-	def retrigger(self):
-		"""retrigger commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_retrigger'):
-			from .ListPy_.Retrigger import Retrigger
-			self._retrigger = Retrigger(self._core, self._base)
-		return self._retrigger
+	def reTrigger(self):
+		"""reTrigger commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_reTrigger'):
+			from .ListPy_.ReTrigger import ReTrigger
+			self._reTrigger = ReTrigger(self._core, self._base)
+		return self._reTrigger
 
 	def get_start(self) -> int:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQVSlot:LIST:STARt \n
 		Snippet: value: int = driver.configure.gprf.measurement.iqVsSlot.listPy.get_start() \n
 		Selects the first subsweep to be measured. The <StartIndex> must not be greater than the <StopIndex>. The total number of
 		steps must not exceed 3000 (step count times number of subsweeps) . \n
 			:return: start_index: No help available
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/EnvelopePower.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/EnvelopePower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/Retrigger.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/ReTrigger.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,53 +5,53 @@
 from .......Internal import Conversions
 from .......Internal.Types import DataType
 from .......Internal.ArgSingleList import ArgSingleList
 from .......Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Retrigger:
-	"""Retrigger commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ReTrigger:
+	"""ReTrigger commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("retrigger", core, parent)
+		self._base = CommandsGroup("reTrigger", core, parent)
 
 	def set(self, index: int, retrigger: bool) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQVSlot:LIST:RETRigger \n
-		Snippet: driver.configure.gprf.measurement.iqVsSlot.listPy.retrigger.set(index = 1, retrigger = False) \n
+		Snippet: driver.configure.gprf.measurement.iqVsSlot.listPy.reTrigger.set(index = 1, retrigger = False) \n
 		Configures the retrigger mechanism for subsweep <Index>. The setting is only relevant for trigger mode Retrigger
 		Preselect. \n
 			:param index: No help available
 			:param retrigger: No help available
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('index', index, DataType.Integer), ArgSingle('retrigger', retrigger, DataType.Boolean))
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:IQVSlot:LIST:RETRigger {param}'.rstrip())
 
 	def get(self, index: int) -> bool:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQVSlot:LIST:RETRigger \n
-		Snippet: value: bool = driver.configure.gprf.measurement.iqVsSlot.listPy.retrigger.get(index = 1) \n
+		Snippet: value: bool = driver.configure.gprf.measurement.iqVsSlot.listPy.reTrigger.get(index = 1) \n
 		Configures the retrigger mechanism for subsweep <Index>. The setting is only relevant for trigger mode Retrigger
 		Preselect. \n
 			:param index: No help available
 			:return: retrigger: No help available"""
 		param = Conversions.decimal_value_to_str(index)
 		response = self._core.io.query_str(f'CONFigure:GPRF:MEASurement<Instance>:IQVSlot:LIST:RETRigger? {param}')
 		return Conversions.str_to_bool(response)
 
 	def get_all(self) -> List[bool]:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQVSlot:LIST:RETRigger:ALL \n
-		Snippet: value: List[bool] = driver.configure.gprf.measurement.iqVsSlot.listPy.retrigger.get_all() \n
+		Snippet: value: List[bool] = driver.configure.gprf.measurement.iqVsSlot.listPy.reTrigger.get_all() \n
 		Configures the retrigger mechanism for all subsweeps. The setting is only relevant for trigger mode Retrigger Preselect. \n
 			:return: retrigger: Comma-separated list of values, one value per subsweep
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:IQVSlot:LIST:RETRigger:ALL?')
 		return Conversions.str_to_bool_list(response)
 
 	def set_all(self, retrigger: List[bool]) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQVSlot:LIST:RETRigger:ALL \n
-		Snippet: driver.configure.gprf.measurement.iqVsSlot.listPy.retrigger.set_all(retrigger = [True, False, True]) \n
+		Snippet: driver.configure.gprf.measurement.iqVsSlot.listPy.reTrigger.set_all(retrigger = [True, False, True]) \n
 		Configures the retrigger mechanism for all subsweeps. The setting is only relevant for trigger mode Retrigger Preselect. \n
 			:param retrigger: Comma-separated list of values, one value per subsweep
 		"""
 		param = Conversions.list_to_csv_str(retrigger)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:IQVSlot:LIST:RETRigger:ALL {param}')
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/Trigger.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/Trigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,33 +70,33 @@
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:return: tcd_timeout: No help available
+			:return: tcd_time_out: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:NRPM:TOUT?')
 		return Conversions.str_to_float(response)
 
-	def set_timeout(self, tcd_timeout: float) -> None:
+	def set_timeout(self, tcd_time_out: float) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:NRPM:TOUT \n
-		Snippet: driver.configure.gprf.measurement.nrpm.set_timeout(tcd_timeout = 1.0) \n
+		Snippet: driver.configure.gprf.measurement.nrpm.set_timeout(tcd_time_out = 1.0) \n
 		Defines a timeout for the measurement. The timer is started when the measurement is initiated via a READ or INIT command.
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:param tcd_timeout: No help available
+			:param tcd_time_out: No help available
 		"""
-		param = Conversions.decimal_value_to_str(tcd_timeout)
+		param = Conversions.decimal_value_to_str(tcd_time_out)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:NRPM:TOUT {param}')
 
 	def clone(self) -> 'Nrpm':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = Nrpm(self._core, self._base.parent)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,26 +35,26 @@
 			self._mpath = Mpath(self._core, self._base)
 		return self._mpath
 
 	def get_tmode(self) -> bool:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:PLOSs:TMODe \n
 		Snippet: value: bool = driver.configure.gprf.measurement.ploss.get_tmode() \n
 		No command help available \n
-			:return: test_mode: No help available
+			:return: testmode: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:PLOSs:TMODe?')
 		return Conversions.str_to_bool(response)
 
-	def set_tmode(self, test_mode: bool) -> None:
+	def set_tmode(self, testmode: bool) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:PLOSs:TMODe \n
-		Snippet: driver.configure.gprf.measurement.ploss.set_tmode(test_mode = False) \n
+		Snippet: driver.configure.gprf.measurement.ploss.set_tmode(testmode = False) \n
 		No command help available \n
-			:param test_mode: No help available
+			:param testmode: No help available
 		"""
-		param = Conversions.bool_to_str(test_mode)
+		param = Conversions.bool_to_str(testmode)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:PLOSs:TMODe {param}')
 
 	def get_trace(self) -> bool:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:PLOSs:TRACe \n
 		Snippet: value: bool = driver.configure.gprf.measurement.ploss.get_trace() \n
 		No command help available \n
 			:return: trace_mode: No help available
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath_/ListPy_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/View.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/View.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,33 +79,33 @@
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:return: tcd_timeout: No help available
+			:return: tcd_time_out: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:POWer:TOUT?')
 		return Conversions.str_to_float(response)
 
-	def set_timeout(self, tcd_timeout: float) -> None:
+	def set_timeout(self, tcd_time_out: float) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:POWer:TOUT \n
-		Snippet: driver.configure.gprf.measurement.power.set_timeout(tcd_timeout = 1.0) \n
+		Snippet: driver.configure.gprf.measurement.power.set_timeout(tcd_time_out = 1.0) \n
 		Defines a timeout for the measurement. The timer is started when the measurement is initiated via a READ or INIT command.
 		It is not started if the measurement is initiated manually (ON | OFF key or RESTART | STOP key) . When the measurement
 		has completed the first measurement cycle (first single shot) , the statistical depth is reached and the timer is reset.
 		If the first measurement cycle has not been completed when the timer expires, the measurement is stopped. The measurement
 		state changes to RDY. The reliability indicator is set to 1, indicating that a measurement timeout occurred.
 		Still running READ, FETCh or CALCulate commands are completed, returning the available results. At least for some results,
 		there are no values at all or the statistical depth has not been reached. A timeout of 0 s corresponds to an infinite
 		measurement timeout. \n
-			:param tcd_timeout: No help available
+			:param tcd_time_out: No help available
 		"""
-		param = Conversions.decimal_value_to_str(tcd_timeout)
+		param = Conversions.decimal_value_to_str(tcd_time_out)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:POWer:TOUT {param}')
 
 	def get_slength(self) -> float:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:POWer:SLENgth \n
 		Snippet: value: float = driver.configure.gprf.measurement.power.get_slength() \n
 		Sets the time between the beginning of two consecutive measurement lengths. \n
 			:return: step_length: No help available
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/Bandpass.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/Bandpass.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/Gauss.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/Gauss.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 		"""envelopePower commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_envelopePower'):
 			from .ListPy_.EnvelopePower import EnvelopePower
 			self._envelopePower = EnvelopePower(self._core, self._base)
 		return self._envelopePower
 
 	@property
-	def retrigger(self):
-		"""retrigger commands group. 0 Sub-classes, 2 commands."""
-		if not hasattr(self, '_retrigger'):
-			from .ListPy_.Retrigger import Retrigger
-			self._retrigger = Retrigger(self._core, self._base)
-		return self._retrigger
+	def reTrigger(self):
+		"""reTrigger commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_reTrigger'):
+			from .ListPy_.ReTrigger import ReTrigger
+			self._reTrigger = ReTrigger(self._core, self._base)
+		return self._reTrigger
 
 	@property
 	def irepetition(self):
 		"""irepetition commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_irepetition'):
 			from .ListPy_.Irepetition import Irepetition
 			self._irepetition = Irepetition(self._core, self._base)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/EnvelopePower.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/EnvelopePower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/IqData.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/IqData.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Irepetition.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Irepetition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/ParameterSetList.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/ParameterSetList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Retrigger.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/ReTrigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,51 +5,51 @@
 from .......Internal import Conversions
 from .......Internal.Types import DataType
 from .......Internal.ArgSingleList import ArgSingleList
 from .......Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Retrigger:
-	"""Retrigger commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class ReTrigger:
+	"""ReTrigger commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("retrigger", core, parent)
+		self._base = CommandsGroup("reTrigger", core, parent)
 
 	def set(self, index: int, retrigger: bool) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:RETRigger \n
-		Snippet: driver.configure.gprf.measurement.power.listPy.retrigger.set(index = 1, retrigger = False) \n
+		Snippet: driver.configure.gprf.measurement.power.listPy.reTrigger.set(index = 1, retrigger = False) \n
 		Configures the retrigger mechanism for segment <Index>. The setting is only relevant for trigger mode Retrigger Preselect. \n
 			:param index: No help available
 			:param retrigger: No help available
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('index', index, DataType.Integer), ArgSingle('retrigger', retrigger, DataType.Boolean))
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:RETRigger {param}'.rstrip())
 
 	def get(self, index: int) -> bool:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:RETRigger \n
-		Snippet: value: bool = driver.configure.gprf.measurement.power.listPy.retrigger.get(index = 1) \n
+		Snippet: value: bool = driver.configure.gprf.measurement.power.listPy.reTrigger.get(index = 1) \n
 		Configures the retrigger mechanism for segment <Index>. The setting is only relevant for trigger mode Retrigger Preselect. \n
 			:param index: No help available
 			:return: retrigger: No help available"""
 		param = Conversions.decimal_value_to_str(index)
 		response = self._core.io.query_str(f'CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:RETRigger? {param}')
 		return Conversions.str_to_bool(response)
 
 	def get_all(self) -> List[bool]:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:RETRigger:ALL \n
-		Snippet: value: List[bool] = driver.configure.gprf.measurement.power.listPy.retrigger.get_all() \n
+		Snippet: value: List[bool] = driver.configure.gprf.measurement.power.listPy.reTrigger.get_all() \n
 		Configures the retrigger mechanism for all segments. The setting is only relevant for trigger mode Retrigger Preselect. \n
 			:return: retrigger: Comma-separated list of values, one value per segment
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:RETRigger:ALL?')
 		return Conversions.str_to_bool_list(response)
 
 	def set_all(self, retrigger: List[bool]) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:RETRigger:ALL \n
-		Snippet: driver.configure.gprf.measurement.power.listPy.retrigger.set_all(retrigger = [True, False, True]) \n
+		Snippet: driver.configure.gprf.measurement.power.listPy.reTrigger.set_all(retrigger = [True, False, True]) \n
 		Configures the retrigger mechanism for all segments. The setting is only relevant for trigger mode Retrigger Preselect. \n
 			:param retrigger: Comma-separated list of values, one value per segment
 		"""
 		param = Conversions.list_to_csv_str(retrigger)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:RETRigger:ALL {param}')
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass_/Bandwidth.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandpass_/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandwidth.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss_/Bandwidth.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/Gauss_/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/TypePy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy_/TypePy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Mlength.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Mlength.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/PdefSet.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/PdefSet.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Slength.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Slength.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/Trigger.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/Trigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/RfSettings.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/RfSettings.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,26 +29,26 @@
 		param = Conversions.decimal_value_to_str(analyzer_freq)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:RFSettings:FREQuency {param}')
 
 	def get_envelope_power(self) -> float:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:RFSettings:ENPower \n
 		Snippet: value: float = driver.configure.gprf.measurement.rfSettings.get_envelope_power() \n
 		Sets the expected nominal power of the measured RF signal. \n
-			:return: exp_nominal_power: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+			:return: exp_nom_pwr: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:RFSettings:ENPower?')
 		return Conversions.str_to_float(response)
 
-	def set_envelope_power(self, exp_nominal_power: float) -> None:
+	def set_envelope_power(self, exp_nom_pwr: float) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:RFSettings:ENPower \n
-		Snippet: driver.configure.gprf.measurement.rfSettings.set_envelope_power(exp_nominal_power = 1.0) \n
+		Snippet: driver.configure.gprf.measurement.rfSettings.set_envelope_power(exp_nom_pwr = 1.0) \n
 		Sets the expected nominal power of the measured RF signal. \n
-			:param exp_nominal_power: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+			:param exp_nom_pwr: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
 		"""
-		param = Conversions.decimal_value_to_str(exp_nominal_power)
+		param = Conversions.decimal_value_to_str(exp_nom_pwr)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:RFSettings:ENPower {param}')
 
 	def get_eattenuation(self) -> float:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:RFSettings:EATTenuation \n
 		Snippet: value: float = driver.configure.gprf.measurement.rfSettings.get_eattenuation() \n
 		Defines an external attenuation (or gain, if the value is negative) , to be applied to the input connector. \n
 			:return: rf_input_ext_att: No help available
@@ -101,24 +101,24 @@
 		Snippet: driver.configure.gprf.measurement.rfSettings.set_ml_offset(mix_lev_offset = 1.0) \n
 		No command help available \n
 			:param mix_lev_offset: No help available
 		"""
 		param = Conversions.decimal_value_to_str(mix_lev_offset)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:RFSettings:MLOFfset {param}')
 
-	def get_foffset(self) -> float:
+	def get_freq_offset(self) -> float:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:RFSettings:FOFFset \n
-		Snippet: value: float = driver.configure.gprf.measurement.rfSettings.get_foffset() \n
+		Snippet: value: float = driver.configure.gprf.measurement.rfSettings.get_freq_offset() \n
 		No command help available \n
 			:return: freq_offset: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:RFSettings:FOFFset?')
 		return Conversions.str_to_float(response)
 
-	def set_foffset(self, freq_offset: float) -> None:
+	def set_freq_offset(self, freq_offset: float) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:RFSettings:FOFFset \n
-		Snippet: driver.configure.gprf.measurement.rfSettings.set_foffset(freq_offset = 1.0) \n
+		Snippet: driver.configure.gprf.measurement.rfSettings.set_freq_offset(freq_offset = 1.0) \n
 		No command help available \n
 			:param freq_offset: No help available
 		"""
 		param = Conversions.decimal_value_to_str(freq_offset)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:RFSettings:FOFFset {param}')
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Scenario.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Scenario.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,26 +74,26 @@
 		param = Conversions.enum_scalar_to_str(repetition, enums.Repeat)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:SPECtrum:REPetition {param}')
 
 	def get_timeout(self) -> float:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:SPECtrum:TOUT \n
 		Snippet: value: float = driver.configure.gprf.measurement.spectrum.get_timeout() \n
 		No command help available \n
-			:return: tcd_timeout: No help available
+			:return: tcd_time_out: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:SPECtrum:TOUT?')
 		return Conversions.str_to_float(response)
 
-	def set_timeout(self, tcd_timeout: float) -> None:
+	def set_timeout(self, tcd_time_out: float) -> None:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:SPECtrum:TOUT \n
-		Snippet: driver.configure.gprf.measurement.spectrum.set_timeout(tcd_timeout = 1.0) \n
+		Snippet: driver.configure.gprf.measurement.spectrum.set_timeout(tcd_time_out = 1.0) \n
 		No command help available \n
-			:param tcd_timeout: No help available
+			:param tcd_time_out: No help available
 		"""
-		param = Conversions.decimal_value_to_str(tcd_timeout)
+		param = Conversions.decimal_value_to_str(tcd_time_out)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:SPECtrum:TOUT {param}')
 
 	def get_scount(self) -> int:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:SPECtrum:SCOunt \n
 		Snippet: value: int = driver.configure.gprf.measurement.spectrum.get_scount() \n
 		No command help available \n
 			:return: statistic_count: No help available
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Rbw.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Rbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Swt.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Swt.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Vbw.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/FreqSweep_/Vbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency_/Span.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/Frequency_/Span.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/Rbw.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/Rbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/Vbw.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Spectrum_/ZeroSpan_/Vbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/System_/Attenuation_/CorrectionTable_/Info.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power_/Current.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from typing import List
 
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
 from ......Internal.Types import DataType
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Info:
-	"""Info commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Current:
+	"""Current commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("info", core, parent)
+		self._base = CommandsGroup("current", core, parent)
 
 	# noinspection PyTypeChecker
-	class GetStruct(StructBase):
+	class FetchStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Frequency: List[float]: No parameter help available
-			- Attenuation: List[float]: No parameter help available"""
+			- Reliability: int: No parameter help available
+			- Stat_Count: int: No parameter help available
+			- Power_Current_Rms: List[float]: No parameter help available"""
 		__meta_args_list = [
-			ArgStruct('Frequency', DataType.FloatList, None, False, True, 1),
-			ArgStruct('Attenuation', DataType.FloatList, None, False, True, 1)]
+			ArgStruct.scalar_int('Reliability', 'Reliability'),
+			ArgStruct.scalar_int('Stat_Count'),
+			ArgStruct('Power_Current_Rms', DataType.FloatList, None, False, True, 1)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Frequency: List[float] = None
-			self.Attenuation: List[float] = None
-
-	def get(self, name: str) -> GetStruct:
-		"""SCPI: [CONFigure]:SYSTem:ATTenuation:CTABle:INFO \n
-		Snippet: value: GetStruct = driver.configure.system.attenuation.correctionTable.info.get(name = '1') \n
+			self.Reliability: int = None
+			self.Stat_Count: int = None
+			self.Power_Current_Rms: List[float] = None
+
+	def fetch(self) -> FetchStruct:
+		"""SCPI: FETCh:RESults:GPRF:MEASurement<Instance>:POWer:CURRent \n
+		Snippet: value: FetchStruct = driver.results.gprf.measurement.power.current.fetch() \n
 		No command help available \n
-			:param name: No help available
-			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		param = Conversions.value_to_quoted_str(name)
-		return self._core.io.query_struct(f'CONFigure:SYSTem:ATTenuation:CTABle:INFO? {param}', self.__class__.GetStruct())
+			:return: structure: for return value, see the help for FetchStruct structure arguments."""
+		return self._core.io.query_struct(f'FETCh:RESults:GPRF:MEASurement<Instance>:POWer:CURRent?', self.__class__.FetchStruct())
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/Rx.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/Tx.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/Direction.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/Direction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/Info.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/Info.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/System.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/System.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("system", core, parent)
 
 	@property
 	def attenuation(self):
-		"""attenuation commands group. 0 Sub-classes, 1 commands."""
+		"""attenuation commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_attenuation'):
 			from .System_.Attenuation import Attenuation
 			self._attenuation = Attenuation(self._core, self._base)
 		return self._attenuation
 
 	def clone(self) -> 'System':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/System_/Attenuation.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation_/CorrectionTable.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,27 @@
 from typing import List
 
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.Types import DataType
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Types import DataType
+from .....Internal.ArgSingleList import ArgSingleList
+from .....Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Attenuation:
-	"""Attenuation commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class CorrectionTable:
+	"""CorrectionTable commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("attenuation", core, parent)
+		self._base = CommandsGroup("correctionTable", core, parent)
 
-	# noinspection PyTypeChecker
-	class CorrectionTableStruct(StructBase):
-		"""Structure for setting input parameters. Contains optional set arguments. Fields: \n
-			- Name: str: No parameter help available
-			- Frequency: List[float]: No parameter help available
-			- Attenuation: List[float]: No parameter help available"""
-		__meta_args_list = [
-			ArgStruct.scalar_str('Name'),
-			ArgStruct('Frequency', DataType.FloatList, None, True, True, 1),
-			ArgStruct('Attenuation', DataType.FloatList, None, True, True, 1)]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Name: str = None
-			self.Frequency: List[float] = None
-			self.Attenuation: List[float] = None
-
-	def set_correction_table(self, value: CorrectionTableStruct) -> None:
-		"""SCPI: CREate:SYSTem:ATTenuation:CTABle \n
-		Snippet: driver.create.system.attenuation.set_correction_table(value = CorrectionTableStruct()) \n
+	def set(self, name: str, frequency: List[float], attenuation: List[float]) -> None:
+		"""SCPI: MODify:SYSTem:ATTenuation:CTABle \n
+		Snippet: driver.modify.system.attenuation.correctionTable.set(name = '1', frequency = [1.1, 2.2, 3.3], attenuation = [1.1, 2.2, 3.3]) \n
 		No command help available \n
-			:param value: see the help for CorrectionTableStruct structure arguments.
+			:param name: No help available
+			:param frequency: No help available
+			:param attenuation: No help available
 		"""
-		self._core.io.write_struct('CREate:SYSTem:ATTenuation:CTABle', value)
+		param = ArgSingleList().compose_cmd_string(ArgSingle('name', name, DataType.String), ArgSingle.as_open_list('frequency', frequency, DataType.FloatList), ArgSingle.as_open_list('attenuation', attenuation, DataType.FloatList))
+		self._core.io.write(f'MODify:SYSTem:ATTenuation:CTABle {param}'.rstrip())
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/Tenvironment.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Create_/Tenvironment_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/Tenvironment_/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System_/Connectors.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Catalog_/System_/Connectors.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Generic.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Generic.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement_/Dapi.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Generic_/Measurement_/Dapi.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Correction.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Correction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Rms.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Rms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Snumber.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Generator_/Snumber.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement_/Snumber.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Gprf_/Measurement_/Snumber.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Meas.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Meas.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Meas_/Scpi.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Meas_/Scpi.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/Generator.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/Generator.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Gprf_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Lte_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/NrMmw_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Diagnostic_/Route_/Uwb_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Canalyzer_/State_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/ExtPwrSensor_/State_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Icomponent.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Icomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Peaks_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Power_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Qcomponent.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/Qcomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/FftSpecAn_/State_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Bin.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Bin.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Reliability.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/State_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/SymbolRate.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/SymbolRate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Talignment.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqRecorder_/Talignment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/FreqError.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/FreqError.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Icomponent.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Icomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Level.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Level.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/OfError.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/OfError.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Phase.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Phase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Qcomponent.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/Qcomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/IqVsSlot_/State_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor_/Power.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/Sensor_/Power.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Nrpm_/State_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Clear.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Clear.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Gain.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Gain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/Gain.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Eval_/Trace_/Gain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Open.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Open.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Short.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/Short.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Ploss_/State_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/AmplitudeProbDensity.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/AmplitudeProbDensity.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average_/Rms.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Average_/Rms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Power.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Power.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Probability.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Probability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Sample.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/CumulativeDistribFnc_/Sample.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Rms.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Current_/Rms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ElapsedStats.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ElapsedStats.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData_/Bin.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqData_/Bin.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqInfo.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/IqInfo.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Maximum_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Minimum_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/Peak_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/StandardDev.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/ListPy_/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Maximum_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Minimum_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/Peak_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/StandardDev_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Power_/State_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Average_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker_/Npeak.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Marker_/Npeak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Maximum_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Minimum_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/Npeak.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/Npeak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/Speak.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/ReferenceMarker_/Speak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Rms_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Average.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Maximum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Minimum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/Sample_/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Gprf_/Measurement_/Spectrum_/State_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement_/Ploss.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Initiate_/Gprf_/Measurement_/Ploss.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/System.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Modify_/System.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/System_/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Modify_/System_/Attenuation_/CorrectionTable.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Add_/System_/Attenuation_/CorrectionTable.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 class CorrectionTable:
 	"""CorrectionTable commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("correctionTable", core, parent)
 
-	def set(self, name: str, frequency: List[float], attenuation: List[float]) -> None:
-		"""SCPI: MODify:SYSTem:ATTenuation:CTABle \n
-		Snippet: driver.modify.system.attenuation.correctionTable.set(name = '1', frequency = [1.1, 2.2, 3.3], attenuation = [1.1, 2.2, 3.3]) \n
+	def set(self, name: str, frequency: List[float] = None, attenuation: List[float] = None) -> None:
+		"""SCPI: ADD:SYSTem:ATTenuation:CTABle \n
+		Snippet: driver.add.system.attenuation.correctionTable.set(name = '1', frequency = [1.1, 2.2, 3.3], attenuation = [1.1, 2.2, 3.3]) \n
 		No command help available \n
 			:param name: No help available
 			:param frequency: No help available
 			:param attenuation: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('name', name, DataType.String), ArgSingle.as_open_list('frequency', frequency, DataType.FloatList), ArgSingle.as_open_list('attenuation', attenuation, DataType.FloatList))
-		self._core.io.write(f'MODify:SYSTem:ATTenuation:CTABle {param}'.rstrip())
+		param = ArgSingleList().compose_cmd_string(ArgSingle('name', name, DataType.String), ArgSingle('frequency', frequency, DataType.FloatList, True, True, 1), ArgSingle('attenuation', attenuation, DataType.FloatList, True, True, 1))
+		self._core.io.write(f'ADD:SYSTem:ATTenuation:CTABle {param}'.rstrip())
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/System.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/System.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Create_/System_/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation_/CorrectionTable.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation_/CorrectionTable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/Tenvironment.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("spath", core, parent)
 
 	@property
 	def correctionTable(self):
-		"""correctionTable commands group. 0 Sub-classes, 2 commands."""
+		"""correctionTable commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_correctionTable'):
 			from .Spath_.CorrectionTable import CorrectionTable
 			self._correctionTable = CorrectionTable(self._core, self._base)
 		return self._correctionTable
 
 	def clone(self) -> 'Spath':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power_/Current.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Segments.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,54 @@
-from typing import List
-
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal.Types import DataType
+from ......Internal import Conversions
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Current:
-	"""Current commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class Segments:
+	"""Segments commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("current", core, parent)
+		self._base = CommandsGroup("segments", core, parent)
+
+	def get_next(self) -> int:
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:NEXT \n
+		Snippet: value: int = driver.source.gprf.generator.arb.segments.get_next() \n
+		No command help available \n
+			:return: segment_number: No help available
+		"""
+		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:NEXT?')
+		return Conversions.str_to_int(response)
+
+	def set_next(self, segment_number: int) -> None:
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:NEXT \n
+		Snippet: driver.source.gprf.generator.arb.segments.set_next(segment_number = 1) \n
+		No command help available \n
+			:param segment_number: No help available
+		"""
+		param = Conversions.decimal_value_to_str(segment_number)
+		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:NEXT {param}')
 
 	# noinspection PyTypeChecker
-	class FetchStruct(StructBase):
-		"""Response structure. Fields: \n
-			- Reliability: int: No parameter help available
-			- Stat_Count: int: No parameter help available
-			- Power_Current_Rms: List[float]: No parameter help available"""
+	class CurrentStruct(StructBase):
+		"""Structure for reading output parameters. Fields: \n
+			- Segment_Number: int: No parameter help available
+			- Segment_Name: str: No parameter help available"""
 		__meta_args_list = [
-			ArgStruct.scalar_int('Reliability', 'Reliability'),
-			ArgStruct.scalar_int('Stat_Count'),
-			ArgStruct('Power_Current_Rms', DataType.FloatList, None, False, True, 1)]
+			ArgStruct.scalar_int('Segment_Number'),
+			ArgStruct.scalar_str('Segment_Name')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Reliability: int = None
-			self.Stat_Count: int = None
-			self.Power_Current_Rms: List[float] = None
-
-	def fetch(self) -> FetchStruct:
-		"""SCPI: FETCh:RESults:GPRF:MEASurement<Instance>:POWer:CURRent \n
-		Snippet: value: FetchStruct = driver.results.gprf.measurement.power.current.fetch() \n
+			self.Segment_Number: int = None
+			self.Segment_Name: str = None
+
+	def get_current(self) -> CurrentStruct:
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:CURRent \n
+		Snippet: value: CurrentStruct = driver.source.gprf.generator.arb.segments.get_current() \n
 		No command help available \n
-			:return: structure: for return value, see the help for FetchStruct structure arguments."""
-		return self._core.io.query_struct(f'FETCh:RESults:GPRF:MEASurement<Instance>:POWer:CURRent?', self.__class__.FetchStruct())
+			:return: structure: for return value, see the help for CurrentStruct structure arguments.
+		"""
+		return self._core.io.query_struct('SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:CURRent?', self.__class__.CurrentStruct())
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/RfSettings.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/Scenario.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Generator_/Scenario.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/RfSettings.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/MaProtocol.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Gprf_/Measurement_/Scenario_/MaProtocol.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrMmw.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrMmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrMmw_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrMmw_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrSub.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrSub.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/NrSub_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/NrSub_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Uwb.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Uwb.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Route_/Uwb_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Route_/Uwb_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,26 +85,26 @@
 		return self._sequencer
 
 	# noinspection PyTypeChecker
 	def get_bb_mode(self) -> enums.BasebandMode:
 		"""SCPI: SOURce:GPRF:GENerator<Instance>:BBMode \n
 		Snippet: value: enums.BasebandMode = driver.source.gprf.generator.get_bb_mode() \n
 		Selects the baseband mode for the generator signal. \n
-			:return: baseband_mode: CW: unmodulated CW signal DTONe: dual-tone signal ARB: ARB generator processing a waveform file
+			:return: base_band_mode: CW: unmodulated CW signal DTONe: dual-tone signal ARB: ARB generator processing a waveform file
 		"""
 		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:BBMode?')
 		return Conversions.str_to_scalar_enum(response, enums.BasebandMode)
 
-	def set_bb_mode(self, baseband_mode: enums.BasebandMode) -> None:
+	def set_bb_mode(self, base_band_mode: enums.BasebandMode) -> None:
 		"""SCPI: SOURce:GPRF:GENerator<Instance>:BBMode \n
-		Snippet: driver.source.gprf.generator.set_bb_mode(baseband_mode = enums.BasebandMode.ARB) \n
+		Snippet: driver.source.gprf.generator.set_bb_mode(base_band_mode = enums.BasebandMode.ARB) \n
 		Selects the baseband mode for the generator signal. \n
-			:param baseband_mode: CW: unmodulated CW signal DTONe: dual-tone signal ARB: ARB generator processing a waveform file
+			:param base_band_mode: CW: unmodulated CW signal DTONe: dual-tone signal ARB: ARB generator processing a waveform file
 		"""
-		param = Conversions.enum_scalar_to_str(baseband_mode, enums.BasebandMode)
+		param = Conversions.enum_scalar_to_str(base_band_mode, enums.BasebandMode)
 		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:BBMode {param}')
 
 	def clone(self) -> 'Generator':
 		"""Clones the group by creating new object from it and its whole existing sub-groups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = Generator(self._core, self._base.parent)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,26 +61,26 @@
 	def segments(self):
 		"""segments commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_segments'):
 			from .Arb_.Segments import Segments
 			self._segments = Segments(self._core, self._base)
 		return self._segments
 
-	def get_foffset(self) -> float:
+	def get_freq_offset(self) -> float:
 		"""SCPI: SOURce:GPRF:GENerator<Instance>:ARB:FOFFset \n
-		Snippet: value: float = driver.source.gprf.generator.arb.get_foffset() \n
+		Snippet: value: float = driver.source.gprf.generator.arb.get_freq_offset() \n
 		No command help available \n
 			:return: frequency_offset: No help available
 		"""
 		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:ARB:FOFFset?')
 		return Conversions.str_to_float(response)
 
-	def set_foffset(self, frequency_offset: float) -> None:
+	def set_freq_offset(self, frequency_offset: float) -> None:
 		"""SCPI: SOURce:GPRF:GENerator<Instance>:ARB:FOFFset \n
-		Snippet: driver.source.gprf.generator.arb.set_foffset(frequency_offset = 1.0) \n
+		Snippet: driver.source.gprf.generator.arb.set_freq_offset(frequency_offset = 1.0) \n
 		No command help available \n
 			:param frequency_offset: No help available
 		"""
 		param = Conversions.decimal_value_to_str(frequency_offset)
 		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:ARB:FOFFset {param}')
 
 	# noinspection PyTypeChecker
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/File.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/File.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Marker.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Marker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Msegment.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Msegment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Samples.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Samples.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/Segments.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Samples.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,33 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.StructBase import StructBase
-from ......Internal.ArgStruct import ArgStruct
+from typing import List
+
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Segments:
-	"""Segments commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class Samples:
+	"""Samples commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("segments", core, parent)
-
-	def get_next(self) -> int:
-		"""SCPI: SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:NEXT \n
-		Snippet: value: int = driver.source.gprf.generator.arb.segments.get_next() \n
-		No command help available \n
-			:return: segment_number: No help available
-		"""
-		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:NEXT?')
-		return Conversions.str_to_int(response)
+		self._base = CommandsGroup("samples", core, parent)
 
-	def set_next(self, segment_number: int) -> None:
-		"""SCPI: SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:NEXT \n
-		Snippet: driver.source.gprf.generator.arb.segments.set_next(segment_number = 1) \n
-		No command help available \n
-			:param segment_number: No help available
+	def get_all(self) -> List[int]:
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:APOol:SAMPles:ALL \n
+		Snippet: value: List[int] = driver.source.gprf.generator.sequencer.apool.samples.get_all() \n
+		Queries the numbers of samples in the ARB files of the file pool. \n
+			:return: samples: Comma-separated list of values, one value per file
 		"""
-		param = Conversions.decimal_value_to_str(segment_number)
-		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:NEXT {param}')
+		response = self._core.io.query_bin_or_ascii_int_list('SOURce:GPRF:GENerator<Instance>:SEQuencer:APOol:SAMPles:ALL?')
+		return response
 
-	# noinspection PyTypeChecker
-	class CurrentStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Segment_Number: int: No parameter help available
-			- Segment_Name: str: No parameter help available"""
-		__meta_args_list = [
-			ArgStruct.scalar_int('Segment_Number'),
-			ArgStruct.scalar_str('Segment_Name')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Segment_Number: int = None
-			self.Segment_Name: str = None
-
-	def get_current(self) -> CurrentStruct:
-		"""SCPI: SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:CURRent \n
-		Snippet: value: CurrentStruct = driver.source.gprf.generator.arb.segments.get_current() \n
-		No command help available \n
-			:return: structure: for return value, see the help for CurrentStruct structure arguments.
-		"""
-		return self._core.io.query_struct('SOURce:GPRF:GENerator<Instance>:ARB:SEGMents:CURRent?', self.__class__.CurrentStruct())
+	def get(self, index: int) -> int:
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:APOol:SAMPles \n
+		Snippet: value: int = driver.source.gprf.generator.sequencer.apool.samples.get(index = 1) \n
+		Queries the number of samples in the ARB file with the specified <Index>. \n
+			:param index: No help available
+			:return: samples: Number of samples"""
+		param = Conversions.decimal_value_to_str(index)
+		response = self._core.io.query_str(f'SOURce:GPRF:GENerator<Instance>:SEQuencer:APOol:SAMPles? {param}')
+		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker_/Clist.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Arb_/UdMarker_/Clist.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/Level.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/Level.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/Ofrequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Dtone_/Ofrequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/IqSettings.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/IqSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,26 +125,26 @@
 		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:LIST:AINDex?')
 		return Conversions.str_to_int(response)
 
 	def get_goto(self) -> int:
 		"""SCPI: SOURce:GPRF:GENerator<Instance>:LIST:GOTO \n
 		Snippet: value: int = driver.source.gprf.generator.listPy.get_goto() \n
 		No command help available \n
-			:return: goto_index: No help available
+			:return: go_to_index: No help available
 		"""
 		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:LIST:GOTO?')
 		return Conversions.str_to_int(response)
 
-	def set_goto(self, goto_index: int) -> None:
+	def set_goto(self, go_to_index: int) -> None:
 		"""SCPI: SOURce:GPRF:GENerator<Instance>:LIST:GOTO \n
-		Snippet: driver.source.gprf.generator.listPy.set_goto(goto_index = 1) \n
+		Snippet: driver.source.gprf.generator.listPy.set_goto(go_to_index = 1) \n
 		No command help available \n
-			:param goto_index: No help available
+			:param go_to_index: No help available
 		"""
-		param = Conversions.decimal_value_to_str(goto_index)
+		param = Conversions.decimal_value_to_str(go_to_index)
 		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:LIST:GOTO {param}')
 
 	# noinspection PyTypeChecker
 	def get_repetition(self) -> enums.RepeatMode:
 		"""SCPI: SOURce:GPRF:GENerator<Instance>:LIST:REPetition \n
 		Snippet: value: enums.RepeatMode = driver.source.gprf.generator.listPy.get_repetition() \n
 		No command help available \n
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Dgain.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Dgain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Dtime.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Dtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 class Dtime:
 	"""Dtime commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("dtime", core, parent)
 
-	def set(self, index: int, dwell_time: float) -> None:
+	def set(self, index: int, dwelltime: float) -> None:
 		"""SCPI: SOURce:GPRF:GENerator<Instance>:LIST:DTIMe \n
-		Snippet: driver.source.gprf.generator.listPy.dtime.set(index = 1, dwell_time = 1.0) \n
+		Snippet: driver.source.gprf.generator.listPy.dtime.set(index = 1, dwelltime = 1.0) \n
 		No command help available \n
 			:param index: No help available
-			:param dwell_time: No help available
+			:param dwelltime: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('index', index, DataType.Integer), ArgSingle('dwell_time', dwell_time, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('index', index, DataType.Integer), ArgSingle('dwelltime', dwelltime, DataType.Float))
 		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:LIST:DTIMe {param}'.rstrip())
 
 	def get(self, index: int) -> float:
 		"""SCPI: SOURce:GPRF:GENerator<Instance>:LIST:DTIMe \n
 		Snippet: value: float = driver.source.gprf.generator.listPy.dtime.get(index = 1) \n
 		No command help available \n
 			:param index: No help available
-			:return: dwell_time: No help available"""
+			:return: dwelltime: No help available"""
 		param = Conversions.decimal_value_to_str(index)
 		response = self._core.io.query_str(f'SOURce:GPRF:GENerator<Instance>:LIST:DTIMe? {param}')
 		return Conversions.str_to_float(response)
 
 	def get_all(self) -> List[float]:
 		"""SCPI: SOURce:GPRF:GENerator<Instance>:LIST:DTIMe:ALL \n
 		Snippet: value: List[float] = driver.source.gprf.generator.listPy.dtime.get_all() \n
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Esingle.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Esingle.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Fill.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Fill.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment_/Enabling.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Increment_/Enabling.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Irepetition.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Irepetition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Modulation.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Modulation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Reenabling.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Reenabling.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/RfLevel.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/RfLevel.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Rlist.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Rlist.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Slist.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Slist.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Sstop.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/ListPy_/Sstop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Reliability.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/RfSettings.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Check.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Check.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/CrcProtect.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/CrcProtect.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Download.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Download.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Duration.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Duration.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Paratio.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Paratio.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Path.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Path.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Poffset.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Poffset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Reliability.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Rmessage.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Rmessage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Roption.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Roption.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Samples.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Tdd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,50 @@
-from typing import List
-
-from .......Internal.Core import Core
-from .......Internal.CommandsGroup import CommandsGroup
-from .......Internal import Conversions
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
+from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Samples:
-	"""Samples commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class Tdd:
+	"""Tdd commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("samples", core, parent)
+		self._base = CommandsGroup("tdd", core, parent)
+
+	def get_mode(self) -> bool:
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MODE \n
+		Snippet: value: bool = driver.source.gprf.generator.sequencer.tdd.get_mode() \n
+		No command help available \n
+			:return: tdd_mode: No help available
+		"""
+		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MODE?')
+		return Conversions.str_to_bool(response)
 
-	def get_all(self) -> List[int]:
-		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:APOol:SAMPles:ALL \n
-		Snippet: value: List[int] = driver.source.gprf.generator.sequencer.apool.samples.get_all() \n
-		Queries the numbers of samples in the ARB files of the file pool. \n
-			:return: samples: Comma-separated list of values, one value per file
+	def set_mode(self, tdd_mode: bool) -> None:
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MODE \n
+		Snippet: driver.source.gprf.generator.sequencer.tdd.set_mode(tdd_mode = False) \n
+		No command help available \n
+			:param tdd_mode: No help available
 		"""
-		response = self._core.io.query_bin_or_ascii_int_list('SOURce:GPRF:GENerator<Instance>:SEQuencer:APOol:SAMPles:ALL?')
-		return response
+		param = Conversions.bool_to_str(tdd_mode)
+		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MODE {param}')
 
-	def get(self, index: int) -> int:
-		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:APOol:SAMPles \n
-		Snippet: value: int = driver.source.gprf.generator.sequencer.apool.samples.get(index = 1) \n
-		Queries the number of samples in the ARB file with the specified <Index>. \n
-			:param index: No help available
-			:return: samples: Number of samples"""
-		param = Conversions.decimal_value_to_str(index)
-		response = self._core.io.query_str(f'SOURce:GPRF:GENerator<Instance>:SEQuencer:APOol:SAMPles? {param}')
-		return Conversions.str_to_int(response)
+	# noinspection PyTypeChecker
+	def get_marker(self) -> enums.TddMarker:
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MARKer \n
+		Snippet: value: enums.TddMarker = driver.source.gprf.generator.sequencer.tdd.get_marker() \n
+		No command help available \n
+			:return: tdd_marker: No help available
+		"""
+		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MARKer?')
+		return Conversions.str_to_scalar_enum(response, enums.TddMarker)
+
+	def set_marker(self, tdd_marker: enums.TddMarker) -> None:
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MARKer \n
+		Snippet: driver.source.gprf.generator.sequencer.tdd.set_marker(tdd_marker = enums.TddMarker.NONE) \n
+		No command help available \n
+			:param tdd_marker: No help available
+		"""
+		param = Conversions.enum_scalar_to_str(tdd_marker, enums.TddMarker)
+		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MARKer {param}')
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/SymbolRate.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/SymbolRate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Waveform.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Apool_/Waveform.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone_/Ofrequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Dtone_/Ofrequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Acycles.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Acycles.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Dgain.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Dgain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Dtime.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Dtime.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Call.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Call.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Insert.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Insert.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Mdown.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Mdown.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Mup.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Entry_/Mup.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Apply.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Apply.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Dgain.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Dgain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Lrms.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Fill_/Lrms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Frequency.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Itransition.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Itransition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Lincrement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Lincrement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Lrms.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Lrms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Signal_/Index_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/SymbolRate.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/SymbolRate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Ttime.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/ListPy_/Ttime.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker_/Delays.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Marker_/Delays.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Reliability.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Rmarker.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Rmarker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Tdd.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Tdd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ...... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class Tdd:
 	"""Tdd commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._base = CommandsGroup("tdd", core, parent)
 
 	def get_mode(self) -> bool:
-		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MODE \n
-		Snippet: value: bool = driver.source.gprf.generator.sequencer.tdd.get_mode() \n
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:TDD:MODE \n
+		Snippet: value: bool = driver.source.gprf.generator.tdd.get_mode() \n
 		No command help available \n
 			:return: tdd_mode: No help available
 		"""
-		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MODE?')
+		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:TDD:MODE?')
 		return Conversions.str_to_bool(response)
 
 	def set_mode(self, tdd_mode: bool) -> None:
-		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MODE \n
-		Snippet: driver.source.gprf.generator.sequencer.tdd.set_mode(tdd_mode = False) \n
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:TDD:MODE \n
+		Snippet: driver.source.gprf.generator.tdd.set_mode(tdd_mode = False) \n
 		No command help available \n
 			:param tdd_mode: No help available
 		"""
 		param = Conversions.bool_to_str(tdd_mode)
-		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MODE {param}')
+		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:TDD:MODE {param}')
 
 	# noinspection PyTypeChecker
 	def get_marker(self) -> enums.TddMarker:
-		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MARKer \n
-		Snippet: value: enums.TddMarker = driver.source.gprf.generator.sequencer.tdd.get_marker() \n
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:TDD:MARKer \n
+		Snippet: value: enums.TddMarker = driver.source.gprf.generator.tdd.get_marker() \n
 		No command help available \n
 			:return: tdd_marker: No help available
 		"""
-		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MARKer?')
+		response = self._core.io.query_str('SOURce:GPRF:GENerator<Instance>:TDD:MARKer?')
 		return Conversions.str_to_scalar_enum(response, enums.TddMarker)
 
 	def set_marker(self, tdd_marker: enums.TddMarker) -> None:
-		"""SCPI: SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MARKer \n
-		Snippet: driver.source.gprf.generator.sequencer.tdd.set_marker(tdd_marker = enums.TddMarker.NONE) \n
+		"""SCPI: SOURce:GPRF:GENerator<Instance>:TDD:MARKer \n
+		Snippet: driver.source.gprf.generator.tdd.set_marker(tdd_marker = enums.TddMarker.NONE) \n
 		No command help available \n
 			:param tdd_marker: No help available
 		"""
 		param = Conversions.enum_scalar_to_str(tdd_marker, enums.TddMarker)
-		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:SEQuencer:TDD:MARKer {param}')
+		self._core.io.write(f'SOURce:GPRF:GENerator<Instance>:TDD:MARKer {param}')
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker_/Delay.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/Sequencer_/Wmarker_/Delay.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/State.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Source_/Gprf_/Generator_/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/Attenuation.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable_/All.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/System_/Attenuation_/CorrectionTable_/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Tenvironment.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Tenvironment_/Spath.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Tenvironment_/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,26 +88,26 @@
 		Snippet: driver.trigger.gprf.generator.arb.set_source(source = '1') \n
 		No command help available \n
 			:param source: No help available
 		"""
 		param = Conversions.value_to_quoted_str(source)
 		self._core.io.write(f'TRIGger:GPRF:GENerator<Instance>:ARB:SOURce {param}')
 
-	def get_retrigger(self) -> bool:
+	def get_re_trigger(self) -> bool:
 		"""SCPI: TRIGger:GPRF:GENerator<Instance>:ARB:RETRigger \n
-		Snippet: value: bool = driver.trigger.gprf.generator.arb.get_retrigger() \n
+		Snippet: value: bool = driver.trigger.gprf.generator.arb.get_re_trigger() \n
 		No command help available \n
 			:return: retrigger: No help available
 		"""
 		response = self._core.io.query_str('TRIGger:GPRF:GENerator<Instance>:ARB:RETRigger?')
 		return Conversions.str_to_bool(response)
 
-	def set_retrigger(self, retrigger: bool) -> None:
+	def set_re_trigger(self, retrigger: bool) -> None:
 		"""SCPI: TRIGger:GPRF:GENerator<Instance>:ARB:RETRigger \n
-		Snippet: driver.trigger.gprf.generator.arb.set_retrigger(retrigger = False) \n
+		Snippet: driver.trigger.gprf.generator.arb.set_re_trigger(retrigger = False) \n
 		No command help available \n
 			:param retrigger: No help available
 		"""
 		param = Conversions.bool_to_str(retrigger)
 		self._core.io.write(f'TRIGger:GPRF:GENerator<Instance>:ARB:RETRigger {param}')
 
 	def get_autostart(self) -> bool:
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual_/Execute.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Manual_/Execute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual_/Execute.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Arb_/Segments_/Manual_/Execute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/IsMeas.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/IsMeas.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/IsTrigger.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/IsTrigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual_/Execute.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Generator_/Sequencer_/Manual_/Execute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/FftSpecAn_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqRecorder_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/IqVsSlot_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList_/Offset.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Power_/ParameterSetList_/Offset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum_/Catalog.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Implementations/Trigger_/Gprf_/Measurement_/Spectrum_/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgSingle.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgSingle.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from .ConverterFromScpiString import ConverterFromScpiString
-from .ConverterToScpiString import ConverterToScpiString
-from .Types import DataType
-
-
-class ArgSingle(object):
-	"""Single Argument outside a structure - used for composing query arguments.
-	Contains the argument value as well (self.value)."""
-
-	def __init__(self, name: str, value, data_type: DataType, is_optional: bool = False, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
-		self.name = name if name else ''
-		self.argument_ix = None
-		self.value = value
-		self.data_type = data_type
-		self.is_optional = is_optional
-		self.is_open_list = is_open_list
-		self.repetition = repetition
-		self.intern_link = intern_link
-		self.conv_from_scpi_string = None
-		self.conv_to_scpi_string = None
-
-		if self.data_type == DataType.Enum:
-			self.assert_mandatory_has_value(self)
-			if self.value is not None:
-				self.enum_type = type(self.value)
-				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
-				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
-		elif self.data_type == DataType.EnumList:
-			self.assert_mandatory_has_value(self)
-			if self.value is not None:
-				self.enum_type = type(self.value[0])
-				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
-				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
-		else:
-			self.conv_from_scpi_string = ConverterFromScpiString(self.data_type)
-			self.conv_to_scpi_string = ConverterToScpiString(self.data_type)
-
-		self.check_consistency()
-
-	@classmethod
-	def as_open_list(cls, name: str, value: object, data_type: DataType) -> 'ArgSingle':
-		"""Creates new ArgSingle of open list type.Use this method for all non-interleaved list types. \n
-		:param name: name of the argument.
-		:param value: value of the argument.
-		:param data_type: data type of the argument.
-		:return: ArgSingle object of an open list type."""
-		return cls(name, value, data_type, False, True, 1, None)
-
-	def __str__(self):
-		opt = '~' if self.is_optional else ''
-		name = f" '{self.name}'" if self.name != '' else ''
-		out = f"SingleArg {opt}{self.data_type.name}{name}"
-
-		if self.is_open_list is False and self.repetition > 1:
-			out += f' [{self.repetition}]'
-		elif self.is_open_list is True:
-			out += f' [{self.repetition}...]'
-		if self.intern_link:
-			out += f", Linking: '{self.intern_link}'"
-		if self.value:
-			out += f', value: {self.value}'
-		else:
-			out += ", <no value>"
-		if self.intern_link:
-			out += f", Linking: '{self.intern_link}'"
-		return out
-
-	# noinspection PyUnusedLocal
-	def has_value(self, value_obj=None) -> bool:
-		"""Returns true, if the argument has value."""
-		return self.value is not None
-
-	# noinspection PyUnusedLocal
-	def assert_is_optional(self, obj=None) -> None:
-		"""Asserts that the parameter is optional.
-		If not, the method throws an exception."""
-		if self.is_optional:
-			return
-		raise Exception(f'Single argument is not optional: {self}')
-
-	# noinspection PyUnusedLocal
-	def assert_mandatory_has_value(self, value_obj=None) -> None:
-		"""Asserts that if the parameter is mandatory, it must have value assigned.
-		If not, the method throws an exception."""
-		if self.is_optional:
-			return
-		if self.value is None:
-			raise ValueError(f'Mandatory single argument has no value: {self}')
-
-	def set_scalar_value_from_str(self, string: str) -> None:
-		"""Sets scalar value from input string"""
-		self.value = self.conv_from_scpi_string.get_value(string)
-
-	def check_consistency(self) -> None:
-		"""Checks the consistency of the object"""
-		if self.value is None:
-			return
-		if isinstance(self.value, list):
-			if self.data_type.is_scalar:
-				raise Exception(f'Argument real data type is list, but it is declared as {self.data_type}. Value: {self.value}')
-		else:
-			if self.data_type.is_list:
-				raise Exception(f'Argument real data type is scalar, but it is declared as {self.data_type}. Value: {self.value}')
+from .ConverterFromScpiString import ConverterFromScpiString
+from .ConverterToScpiString import ConverterToScpiString
+from .Types import DataType
+
+
+class ArgSingle(object):
+	"""Single Argument outside a structure - used for composing query arguments.
+	Contains the argument value as well (self.value)."""
+
+	def __init__(self, name: str, value, data_type: DataType, is_optional: bool = False, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
+		self.name = name if name else ''
+		self.argument_ix = None
+		self.value = value
+		self.data_type = data_type
+		self.is_optional = is_optional
+		self.is_open_list = is_open_list
+		self.repetition = repetition
+		self.intern_link = intern_link
+		self.conv_from_scpi_string = None
+		self.conv_to_scpi_string = None
+
+		if self.data_type == DataType.Enum:
+			self.assert_mandatory_has_value(self)
+			if self.value is not None:
+				self.enum_type = type(self.value)
+				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
+				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
+		elif self.data_type == DataType.EnumList:
+			self.assert_mandatory_has_value(self)
+			if self.value is not None:
+				self.enum_type = type(self.value[0])
+				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
+				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
+		else:
+			self.conv_from_scpi_string = ConverterFromScpiString(self.data_type)
+			self.conv_to_scpi_string = ConverterToScpiString(self.data_type)
+
+		self.check_consistency()
+
+	@classmethod
+	def as_open_list(cls, name: str, value: object, data_type: DataType) -> 'ArgSingle':
+		"""Creates new ArgSingle of open list type.Use this method for all non-interleaved list types. \n
+		:param name: name of the argument.
+		:param value: value of the argument.
+		:param data_type: data type of the argument.
+		:return: ArgSingle object of an open list type."""
+		return cls(name, value, data_type, False, True, 1, None)
+
+	def __str__(self):
+		opt = '~' if self.is_optional else ''
+		name = f" '{self.name}'" if self.name != '' else ''
+		out = f"SingleArg {opt}{self.data_type.name}{name}"
+
+		if self.is_open_list is False and self.repetition > 1:
+			out += f' [{self.repetition}]'
+		elif self.is_open_list is True:
+			out += f' [{self.repetition}...]'
+		if self.intern_link:
+			out += f", Linking: '{self.intern_link}'"
+		if self.value:
+			out += f', value: {self.value}'
+		else:
+			out += ", <no value>"
+		if self.intern_link:
+			out += f", Linking: '{self.intern_link}'"
+		return out
+
+	# noinspection PyUnusedLocal
+	def has_value(self, value_obj=None) -> bool:
+		"""Returns true, if the argument has value."""
+		return self.value is not None
+
+	# noinspection PyUnusedLocal
+	def assert_is_optional(self, obj=None) -> None:
+		"""Asserts that the parameter is optional.
+		If not, the method throws an exception."""
+		if self.is_optional:
+			return
+		raise Exception(f'Single argument is not optional: {self}')
+
+	# noinspection PyUnusedLocal
+	def assert_mandatory_has_value(self, value_obj=None) -> None:
+		"""Asserts that if the parameter is mandatory, it must have value assigned.
+		If not, the method throws an exception."""
+		if self.is_optional:
+			return
+		if self.value is None:
+			raise ValueError(f'Mandatory single argument has no value: {self}')
+
+	def set_scalar_value_from_str(self, string: str) -> None:
+		"""Sets scalar value from input string"""
+		self.value = self.conv_from_scpi_string.get_value(string)
+
+	def check_consistency(self) -> None:
+		"""Checks the consistency of the object"""
+		if self.value is None:
+			return
+		if isinstance(self.value, list):
+			if self.data_type.is_scalar:
+				raise Exception(f'Argument real data type is list, but it is declared as {self.data_type}. Value: {self.value}')
+		else:
+			if self.data_type.is_list:
+				raise Exception(f'Argument real data type is scalar, but it is declared as {self.data_type}. Value: {self.value}')
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgSingleList.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgSingleList.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from .ArgSingle import ArgSingle
-from .ArgStringComposer import compose_cmd_string_from_single_args
-
-
-class ArgSingleList(object):
-	"""Contains methods for composing cmd string for the list of single arguments.
-	Used in methods with 1+ set or query arguments.
-	The instance does not have a fixed args list, you can use the instance method compose_cmd_string with different arguments."""
-
-	def __init__(self):
-		self.args = None
-
-	def compose_cmd_string(self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None, arg7: ArgSingle = None, arg8: ArgSingle = None, arg9: ArgSingle = None):
-		"""Composes the string cmd argument from the arguments list.
-		Same treatment as in the ArgStructList.compose_cmd_string().
-		The difference is in handling the value of the argument."""
-		self.args = dict()
-
-		ix = 0
-		for arg in [arg1, arg2, arg3, arg4, arg5, arg6, arg7, arg8, arg9]:
-			if arg:
-				self.args[ix] = arg
-				ix += 1
-
-		return compose_cmd_string_from_single_args(self.args)
+from .ArgSingle import ArgSingle
+from .ArgStringComposer import compose_cmd_string_from_single_args
+
+
+class ArgSingleList(object):
+	"""Contains methods for composing cmd string for the list of single arguments.
+	Used in methods with 1+ set or query arguments.
+	The instance does not have a fixed args list, you can use the instance method compose_cmd_string with different arguments."""
+
+	def __init__(self):
+		self.args = None
+
+	def compose_cmd_string(self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None, arg7: ArgSingle = None, arg8: ArgSingle = None, arg9: ArgSingle = None):
+		"""Composes the string cmd argument from the arguments list.
+		Same treatment as in the ArgStructList.compose_cmd_string().
+		The difference is in handling the value of the argument."""
+		self.args = dict()
+
+		ix = 0
+		for arg in [arg1, arg2, arg3, arg4, arg5, arg6, arg7, arg8, arg9]:
+			if arg:
+				self.args[ix] = arg
+				ix += 1
+
+		return compose_cmd_string_from_single_args(self.args)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from .Types import DataType
-
-
-class ArgSingleSuppressed(object):
-	"""Single suppressed Argument - used in Query_XxXx_Suppressed() to remove it from the returned value.
-	It does not contain:
-	- 'value' attribute, since this is discarded or linked internally directly  in the Query_XxXx_Suppressed().
-	- 'is_optional' attribute, since it is always mandatory."""
-
-	def __init__(self, argument_ix: int, data_type: DataType, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
-		self.name = ''
-		self.argument_ix = argument_ix
-		self.data_type = data_type
-		self.is_open_list = is_open_list
-		self.repetition = repetition
-		self.intern_link = intern_link
-
-	def __str__(self):
-		out = f"{self.data_type.name} '{self.name}' SuppressedArg"
-		if self.is_open_list is False and self.repetition > 1:
-			out += f' [{self.repetition}]'
-		elif self.is_open_list is True:
-			out += f' [{self.repetition}...]'
-
-		if self.intern_link:
-			out += f", Linking: '{self.intern_link}'"
-
-		return out
+from .Types import DataType
+
+
+class ArgSingleSuppressed(object):
+	"""Single suppressed Argument - used in Query_XxXx_Suppressed() to remove it from the returned value.
+	It does not contain:
+	- 'value' attribute, since this is discarded or linked internally directly  in the Query_XxXx_Suppressed().
+	- 'is_optional' attribute, since it is always mandatory."""
+
+	def __init__(self, argument_ix: int, data_type: DataType, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
+		self.name = ''
+		self.argument_ix = argument_ix
+		self.data_type = data_type
+		self.is_open_list = is_open_list
+		self.repetition = repetition
+		self.intern_link = intern_link
+
+	def __str__(self):
+		out = f"{self.data_type.name} '{self.name}' SuppressedArg"
+		if self.is_open_list is False and self.repetition > 1:
+			out += f' [{self.repetition}]'
+		elif self.is_open_list is True:
+			out += f' [{self.repetition}...]'
+
+		if self.intern_link:
+			out += f", Linking: '{self.intern_link}'"
+
+		return out
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgStringComposer.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgStringComposer.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-"""Provides:
-- class SingleComposer - for composing SCPI string parameters from ArgSingle
-- class StructComposer - for composing SCPI string parameters from ArgStruct
-- function compose_cmd_string_from_struct_args - takes ArgStruct values and converts it to a SCPI string parameter.
-- function compose_cmd_string_from_single_args - takes ArgSingle[] values and converts them to a SCPI string parameter.
-The composing of the SCPI parameter string is similar for the ArgStruct and ArgSingle[] objects, therefore they share the same module."""
-
-from typing import Dict
-
-from .ArgSingle import ArgSingle
-from .ArgStruct import ArgStruct
-from .Utilities import get_plural_string
-
-
-class SingleComposer:
-	"""Composes strings for single argument.
-	Provides Composer interface with 3 functions:
-	- from_scalar_arg
-	- from_list_arg
-	- get_arg_list_size"""
-
-	@staticmethod
-	def from_scalar_arg(arg: ArgSingle) -> str:
-		"""Takes argument's scalar value and converts it to a SCPI parameter string."""
-		if not arg.is_optional and arg.value is None:
-			raise ValueError(f"StructArgComposer.from_scalar_arg() - mandatory argument's '{arg.name}' value is None")
-		assert arg.data_type.is_scalar, f"StructArgComposer.from_scalar_arg() - argument '{arg.name}' must be scalar. Data type: '{arg.data_type}'"
-		if arg.value is None:
-			return ''
-		return arg.conv_to_scpi_string.get_value(arg.value)
-
-	@staticmethod
-	def from_list_arg(arg: ArgSingle, start_ix=0, items_count=-1) -> str:
-		"""Takes argument's List of elements and converts it to a csv-string of SCPI parameters.
-		start_ix defines where to start in the list.
-		items_count defines how many items to take. -1 means all of them"""
-		if not arg.is_optional and arg.value is None:
-			raise ValueError(f"StructArgComposer.from_list_arg() - mandatory argument's '{arg.name}' value is None")
-		assert arg.data_type.is_list, f"StructArgComposer.from_list_arg() - argument must be list. Data type: '{arg.data_type}'"
-		if not arg.is_optional:
-			assert arg.value is not None, f"StructArgComposer.from_list_arg() - mandatory argument's '{arg.name}' value is None"
-		if arg.value is None:
-			return ''
-		if start_ix == 0 and items_count < 0:
-			return arg.conv_to_scpi_string.get_value(arg.value)
-		elif items_count < 0:
-			return arg.conv_to_scpi_string.get_value(arg.value[start_ix])
-		elif items_count == 0:
-			return ''
-		elif items_count > 0:
-			return arg.conv_to_scpi_string.get_value(arg.value[start_ix: start_ix + items_count])
-
-	@staticmethod
-	def get_arg_list_size(arg: ArgSingle) -> int:
-		"""Returns list size of the argument assuming it is a list.
-		If the argument is not a list, the method returns -1."""
-		if arg.data_type.is_scalar:
-			return -1
-		else:
-			return len(arg.value)
-
-
-class StructComposer:
-	"""Composes strings for structure arguments.
-	Provides Composer interface with 3 functions:
-	- from_scalar_arg
-	- from_list_arg
-	- get_arg_list_size \n
-	The StructComposer constructor has the owning struct instance as parameter, because this is needed to access the argument value."""
-
-	def __init__(self, struct):
-		self.struct = struct
-
-	def from_scalar_arg(self, arg: ArgStruct) -> str:
-		"""Returns a single argument value converted to string."""
-		assert arg.data_type.is_scalar, f"StructArgComposer.from_scalar_arg() - argument must be scalar. Data type: '{arg.data_type}'"
-		return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name))
-
-	def from_list_arg(self, arg: ArgStruct, start_ix=0, items_count=-1) -> str:
-		"""Returns csv-string with all the elements from the argument value."""
-		assert arg.data_type.is_list, f"StructArgComposer.from_list_arg() - argument must be list. Data type: '{arg.data_type}'"
-		if start_ix == 0 and items_count < 0:
-			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name))
-		elif items_count < 0:
-			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name)[start_ix])
-		elif items_count == 0:
-			return ''
-		elif items_count > 0:
-			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name)[start_ix: start_ix + items_count])
-
-	def get_arg_list_size(self, arg: ArgStruct) -> int:
-		"""Returns list size of the argument assuming it is a list.
-		If the argument is not a list, the method returns -1."""
-		if arg.data_type.is_scalar:
-			return -1
-		else:
-			return len(getattr(self.struct, arg.name))
-
-
-def compose_cmd_string_from_struct_args(args: Dict[int, ArgStruct], composer: StructComposer, values_obj: object) -> str:
-	"""Returns SCPI-composed string based on the structure args specification."""
-	arg_count = len(args)
-	string_arg = []
-	arg_ix = 0
-	opt_null_ix = -1
-
-	# Non-repeated arguments - single values or arrays which are not open lists
-	# Non-open lists or scalars must be at the beginning of the definition
-	# Once the first open list argument is detected, continue further
-	while arg_ix < arg_count and args[arg_ix].is_open_list is False:
-		arg = args[arg_ix]
-		if arg.has_value(values_obj) is False:
-			arg.assert_is_optional(values_obj)
-			# The optional argument, which has no value. End the entire string_arg composition
-			opt_null_ix = arg_ix
-			break
-
-		if arg.repetition <= 1:
-			# No list, but scalar value
-			string_arg.append(composer.from_scalar_arg(arg))
-		else:
-			string_arg.append(composer.from_list_arg(arg, 0, arg.repetition))
-
-		arg_ix += 1
-	# End of non-repeated arguments
-
-	# If the optional argument without a value was not found, check if there are some more arguments to go through
-	if opt_null_ix < 0 and arg_ix < arg_count:
-		# Still some args to go
-		arg = args[arg_ix]
-		if arg.is_open_list:
-			# The previous loop ended because the next argument had is_open_list = True
-			if arg_ix == (arg_count - 1):
-				if arg.has_value(values_obj):
-					# The last argument, ignore the repetitions and convert the whole list to string
-					string_arg.append(composer.from_list_arg(arg))
-				else:
-					# The optional argument, which has no value. End the entire string_arg composition
-					arg.assert_is_optional(values_obj)
-					opt_null_ix = arg_ix
-			else:
-				# More than one arguments remaining. Loop through them interleaving the result strings
-				# Interleaving arguments must all have values
-
-				# Check if each list has at least Repetition number of elements
-				cycles_error = False
-				alignments_error = False
-				cycle = -1
-				data = {}
-				for x in range(arg_ix, arg_count):
-					arg = args[x]
-					curr_size: int = composer.get_arg_list_size(arg)
-					curr_cycle: int = curr_size // arg.repetition
-					curr_align: int = curr_size % arg.repetition
-					data[x] = (curr_size, curr_cycle, curr_align)
-
-					if curr_size < 0:
-						raise Exception(
-							f"Argument '{arg.name}' has repetitions, therefore it must be declared as a list. Current Declaration: '{arg.data_type}'")
-
-					if arg.repetition > curr_size:
-						raise Exception(f"Argument '{arg.name}' has repetitions {arg.repetition}, but its list size is only {curr_size}")
-
-					# noinspection PyChainedComparisons
-					if cycle >= 0 and curr_cycle != cycle:
-						cycles_error = True
-
-					cycle = curr_cycle
-
-					if curr_align != 0:
-						alignments_error = True
-
-				if cycles_error:
-					message = 'Arguments interleaving is not aligned - all the cycles must be the same. Actual cycles:\n'
-					for x in range(arg_ix, arg_count):
-						message += f'{args[x].name}[{data[x][0]}] sliced by {get_plural_string("element", args[x].repetition)} ' \
-							f'results in {data[x][0] / args[x].repetition} cycles\n'
-
-					raise Exception(message)
-
-				if alignments_error:
-					message = 'At least one argument has a list size not dividable by the defined repetitions:\n'
-					for x in range(arg_ix, arg_count):
-						message += f'{args[x].name}[{data[x][0]}] modulo {args[x].repetition}x results in {data[x][0] % args[x].repetition}\n'
-
-					raise Exception(message)
-
-				for x in range(cycle):
-					for y in range(arg_ix, arg_count):
-						arg = args[y]
-						string_arg.append(composer.from_list_arg(arg, arg.repetition * x, arg.repetition))
-
-	if opt_null_ix >= 0:
-		# Check the rest of the optional values, all of them must be without a value
-		rest = []
-		for y in range(opt_null_ix, arg_count):
-			arg = args[y]
-			if arg.has_value(values_obj):
-				rest.append(arg.name)
-
-		if len(rest):
-			msg = f"Optional Argument '{args[opt_null_ix].name}' has no value, but the further ones do. " \
-				f"If you skip an optional argument, you have to skip all the ones following it. " \
-				f"Clear the values for the rest of the argument(s):\n{', '.join(rest)}"
-			raise Exception(msg)
-
-	return ','.join(string_arg)
-
-
-def compose_cmd_string_from_single_args(args: Dict[int, ArgSingle]) -> str:
-	"""Returns SCPI-composed string based on the single args specification.
-	We can use the same function as for the struct arguments, with the difference of providing a SingleComposer.
-	Parameter value_obj is set to None, since each argument holds the value itself."""
-	# noinspection PyTypeChecker
-	return compose_cmd_string_from_struct_args(args, SingleComposer(), None)
+"""Provides:
+- class SingleComposer - for composing SCPI string parameters from ArgSingle
+- class StructComposer - for composing SCPI string parameters from ArgStruct
+- function compose_cmd_string_from_struct_args - takes ArgStruct values and converts it to a SCPI string parameter.
+- function compose_cmd_string_from_single_args - takes ArgSingle[] values and converts them to a SCPI string parameter.
+The composing of the SCPI parameter string is similar for the ArgStruct and ArgSingle[] objects, therefore they share the same module."""
+
+from typing import Dict
+
+from .ArgSingle import ArgSingle
+from .ArgStruct import ArgStruct
+from .Utilities import get_plural_string
+
+
+class SingleComposer:
+	"""Composes strings for single argument.
+	Provides Composer interface with 3 functions:
+	- from_scalar_arg
+	- from_list_arg
+	- get_arg_list_size"""
+
+	@staticmethod
+	def from_scalar_arg(arg: ArgSingle) -> str:
+		"""Takes argument's scalar value and converts it to a SCPI parameter string."""
+		if not arg.is_optional and arg.value is None:
+			raise ValueError(f"StructArgComposer.from_scalar_arg() - mandatory argument's '{arg.name}' value is None")
+		assert arg.data_type.is_scalar, f"StructArgComposer.from_scalar_arg() - argument '{arg.name}' must be scalar. Data type: '{arg.data_type}'"
+		if arg.value is None:
+			return ''
+		return arg.conv_to_scpi_string.get_value(arg.value)
+
+	@staticmethod
+	def from_list_arg(arg: ArgSingle, start_ix=0, items_count=-1) -> str:
+		"""Takes argument's List of elements and converts it to a csv-string of SCPI parameters.
+		start_ix defines where to start in the list.
+		items_count defines how many items to take. -1 means all of them"""
+		if not arg.is_optional and arg.value is None:
+			raise ValueError(f"StructArgComposer.from_list_arg() - mandatory argument's '{arg.name}' value is None")
+		assert arg.data_type.is_list, f"StructArgComposer.from_list_arg() - argument must be list. Data type: '{arg.data_type}'"
+		if not arg.is_optional:
+			assert arg.value is not None, f"StructArgComposer.from_list_arg() - mandatory argument's '{arg.name}' value is None"
+		if arg.value is None:
+			return ''
+		if start_ix == 0 and items_count < 0:
+			return arg.conv_to_scpi_string.get_value(arg.value)
+		elif items_count < 0:
+			return arg.conv_to_scpi_string.get_value(arg.value[start_ix])
+		elif items_count == 0:
+			return ''
+		elif items_count > 0:
+			return arg.conv_to_scpi_string.get_value(arg.value[start_ix: start_ix + items_count])
+
+	@staticmethod
+	def get_arg_list_size(arg: ArgSingle) -> int:
+		"""Returns list size of the argument assuming it is a list.
+		If the argument is not a list, the method returns -1."""
+		if arg.data_type.is_scalar:
+			return -1
+		else:
+			return len(arg.value)
+
+
+class StructComposer:
+	"""Composes strings for structure arguments.
+	Provides Composer interface with 3 functions:
+	- from_scalar_arg
+	- from_list_arg
+	- get_arg_list_size \n
+	The StructComposer constructor has the owning struct instance as parameter, because this is needed to access the argument value."""
+
+	def __init__(self, struct):
+		self.struct = struct
+
+	def from_scalar_arg(self, arg: ArgStruct) -> str:
+		"""Returns a single argument value converted to string."""
+		assert arg.data_type.is_scalar, f"StructArgComposer.from_scalar_arg() - argument must be scalar. Data type: '{arg.data_type}'"
+		return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name))
+
+	def from_list_arg(self, arg: ArgStruct, start_ix=0, items_count=-1) -> str:
+		"""Returns csv-string with all the elements from the argument value."""
+		assert arg.data_type.is_list, f"StructArgComposer.from_list_arg() - argument must be list. Data type: '{arg.data_type}'"
+		if start_ix == 0 and items_count < 0:
+			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name))
+		elif items_count < 0:
+			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name)[start_ix])
+		elif items_count == 0:
+			return ''
+		elif items_count > 0:
+			return arg.conv_to_scpi_string.get_value(getattr(self.struct, arg.name)[start_ix: start_ix + items_count])
+
+	def get_arg_list_size(self, arg: ArgStruct) -> int:
+		"""Returns list size of the argument assuming it is a list.
+		If the argument is not a list, the method returns -1."""
+		if arg.data_type.is_scalar:
+			return -1
+		else:
+			return len(getattr(self.struct, arg.name))
+
+
+def compose_cmd_string_from_struct_args(args: Dict[int, ArgStruct], composer: StructComposer, values_obj: object) -> str:
+	"""Returns SCPI-composed string based on the structure args specification."""
+	arg_count = len(args)
+	string_arg = []
+	arg_ix = 0
+	opt_null_ix = -1
+
+	# Non-repeated arguments - single values or arrays which are not open lists
+	# Non-open lists or scalars must be at the beginning of the definition
+	# Once the first open list argument is detected, continue further
+	while arg_ix < arg_count and args[arg_ix].is_open_list is False:
+		arg = args[arg_ix]
+		if arg.has_value(values_obj) is False:
+			arg.assert_is_optional(values_obj)
+			# The optional argument, which has no value. End the entire string_arg composition
+			opt_null_ix = arg_ix
+			break
+
+		if arg.repetition <= 1:
+			# No list, but scalar value
+			string_arg.append(composer.from_scalar_arg(arg))
+		else:
+			string_arg.append(composer.from_list_arg(arg, 0, arg.repetition))
+
+		arg_ix += 1
+	# End of non-repeated arguments
+
+	# If the optional argument without a value was not found, check if there are some more arguments to go through
+	if opt_null_ix < 0 and arg_ix < arg_count:
+		# Still some args to go
+		arg = args[arg_ix]
+		if arg.is_open_list:
+			# The previous loop ended because the next argument had is_open_list = True
+			if arg_ix == (arg_count - 1):
+				if arg.has_value(values_obj):
+					# The last argument, ignore the repetitions and convert the whole list to string
+					string_arg.append(composer.from_list_arg(arg))
+				else:
+					# The optional argument, which has no value. End the entire string_arg composition
+					arg.assert_is_optional(values_obj)
+					opt_null_ix = arg_ix
+			else:
+				# More than one arguments remaining. Loop through them interleaving the result strings
+				# Interleaving arguments must all have values
+
+				# Check if each list has at least Repetition number of elements
+				cycles_error = False
+				alignments_error = False
+				cycle = -1
+				data = {}
+				for x in range(arg_ix, arg_count):
+					arg = args[x]
+					curr_size: int = composer.get_arg_list_size(arg)
+					curr_cycle: int = curr_size // arg.repetition
+					curr_align: int = curr_size % arg.repetition
+					data[x] = (curr_size, curr_cycle, curr_align)
+
+					if curr_size < 0:
+						raise Exception(
+							f"Argument '{arg.name}' has repetitions, therefore it must be declared as a list. Current Declaration: '{arg.data_type}'")
+
+					if arg.repetition > curr_size:
+						raise Exception(f"Argument '{arg.name}' has repetitions {arg.repetition}, but its list size is only {curr_size}")
+
+					# noinspection PyChainedComparisons
+					if cycle >= 0 and curr_cycle != cycle:
+						cycles_error = True
+
+					cycle = curr_cycle
+
+					if curr_align != 0:
+						alignments_error = True
+
+				if cycles_error:
+					message = 'Arguments interleaving is not aligned - all the cycles must be the same. Actual cycles:\n'
+					for x in range(arg_ix, arg_count):
+						message += f'{args[x].name}[{data[x][0]}] sliced by {get_plural_string("element", args[x].repetition)} ' \
+							f'results in {data[x][0] / args[x].repetition} cycles\n'
+
+					raise Exception(message)
+
+				if alignments_error:
+					message = 'At least one argument has a list size not dividable by the defined repetitions:\n'
+					for x in range(arg_ix, arg_count):
+						message += f'{args[x].name}[{data[x][0]}] modulo {args[x].repetition}x results in {data[x][0] % args[x].repetition}\n'
+
+					raise Exception(message)
+
+				for x in range(cycle):
+					for y in range(arg_ix, arg_count):
+						arg = args[y]
+						string_arg.append(composer.from_list_arg(arg, arg.repetition * x, arg.repetition))
+
+	if opt_null_ix >= 0:
+		# Check the rest of the optional values, all of them must be without a value
+		rest = []
+		for y in range(opt_null_ix, arg_count):
+			arg = args[y]
+			if arg.has_value(values_obj):
+				rest.append(arg.name)
+
+		if len(rest):
+			msg = f"Optional Argument '{args[opt_null_ix].name}' has no value, but the further ones do. " \
+				f"If you skip an optional argument, you have to skip all the ones following it. " \
+				f"Clear the values for the rest of the argument(s):\n{', '.join(rest)}"
+			raise Exception(msg)
+
+	return ','.join(string_arg)
+
+
+def compose_cmd_string_from_single_args(args: Dict[int, ArgSingle]) -> str:
+	"""Returns SCPI-composed string based on the single args specification.
+	We can use the same function as for the struct arguments, with the difference of providing a SingleComposer.
+	Parameter value_obj is set to None, since each argument holds the value itself."""
+	# noinspection PyTypeChecker
+	return compose_cmd_string_from_struct_args(args, SingleComposer(), None)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgStruct.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgStruct.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-from .ConverterFromScpiString import ConverterFromScpiString
-from .ConverterToScpiString import ConverterToScpiString
-from .Types import DataType
-
-
-class ArgStruct(object):
-	"""Describes an argument in data structures.
-	This info is used to parse a string query response to the output structure,
-	or to parse the output structure to the string parameter for writing.
-	Contains reference to the value in the owning structure."""
-
-	def __init__(self, name: str, data_type: DataType, enum_type=None, is_optional=False, is_open_list=False, repetition=1, intern_link: str = None):
-		self.argument_ix = None
-		self.name = name
-		self.data_type = data_type
-		self.is_optional = is_optional
-		self.is_open_list = is_open_list
-		self.repetition = repetition
-		self.intern_link = intern_link
-		self.enum_type = enum_type
-		self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
-		self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
-
-	@classmethod
-	def scalar_int(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar integer argument."""
-		return cls(name, DataType.Integer, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_int_ext(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar extended integer argument."""
-		return cls(name, DataType.IntegerExt, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_str(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar string argument."""
-		return cls(name, DataType.String, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_raw_str(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar raw string argument."""
-		return cls(name, DataType.RawString, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_bool(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar boolean argument."""
-		return cls(name, DataType.Boolean, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_float(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar float argument."""
-		return cls(name, DataType.Float, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_float_ext(cls, name: str, intern_link: str = None):
-		"""Describes mandatory scalar extended float argument."""
-		return cls(name, DataType.FloatExt, None, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_enum(cls, name: str, enum_type, intern_link: str = None):
-		"""Describes mandatory scalar float argument."""
-		return cls(name, DataType.Enum, enum_type, False, False, 1, intern_link)
-
-	@classmethod
-	def scalar_str_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar string argument."""
-		return cls(name, DataType.String, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_raw_str_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar raw string argument."""
-		return cls(name, DataType.RawString, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_bool_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar boolean argument."""
-		return cls(name, DataType.Boolean, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_int_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar integer argument."""
-		return cls(name, DataType.Integer, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_int_ext_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar extended integer argument."""
-		return cls(name, DataType.IntegerExt, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_float_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar float argument."""
-		return cls(name, DataType.Float, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_float_ext_optional(cls, name: str, intern_link: str = None):
-		"""Describes optional scalar extended float argument."""
-		return cls(name, DataType.FloatExt, None, True, False, 1, intern_link)
-
-	@classmethod
-	def scalar_enum_optional(cls, name: str, enum_type, intern_link: str = None):
-		"""Describes optional scalar float argument."""
-		return cls(name, DataType.Enum, enum_type, True, False, 1, intern_link)
-
-	def __str__(self):
-		opt = '~' if self.is_optional else ''
-		name = f" '{self.name}'" if self.name != '' else ''
-		out = f"StructArg {opt}{self.data_type.name}{name}"
-
-		if self.is_open_list is False and self.repetition > 1:
-			out += f' [{self.repetition}]'
-		elif self.is_open_list is True:
-			out += f' [{self.repetition}...]'
-		if self.intern_link:
-			out += f", Linking: '{self.intern_link}'"
-		return out
-
-	def has_value(self, obj) -> bool:
-		"""Returns True, if the entered object attribute has value."""
-		return getattr(obj, self.name) is not None
-
-	def assert_is_optional(self, obj) -> None:
-		"""Asserts that the parameter is optional.
-		If not, the method throws an exception."""
-		if self.is_optional:
-			return
-		value = getattr(obj, self.name)
-		if value is None:
-			raise Exception(f"Structure '{obj}', argument without value is not optional: {self}")
-		else:
-			raise Exception(f"Structure '{obj}', argument is not optional: {self}', value '{value}'")
-
-	def assert_mandatory_has_value(self, obj) -> None:
-		"""Asserts that if the parameter is mandatory, it must have value assigned.
-		If not, the method throws an exception."""
-		if self.is_optional:
-			return
-		if getattr(obj, self.name) is None:
-			raise ValueError(f"Mandatory structure '{obj}' argument '{self.name}' has no value.")
+from .ConverterFromScpiString import ConverterFromScpiString
+from .ConverterToScpiString import ConverterToScpiString
+from .Types import DataType
+
+
+class ArgStruct(object):
+	"""Describes an argument in data structures.
+	This info is used to parse a string query response to the output structure,
+	or to parse the output structure to the string parameter for writing.
+	Contains reference to the value in the owning structure."""
+
+	def __init__(self, name: str, data_type: DataType, enum_type=None, is_optional=False, is_open_list=False, repetition=1, intern_link: str = None):
+		self.argument_ix = None
+		self.name = name
+		self.data_type = data_type
+		self.is_optional = is_optional
+		self.is_open_list = is_open_list
+		self.repetition = repetition
+		self.intern_link = intern_link
+		self.enum_type = enum_type
+		self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
+		self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
+
+	@classmethod
+	def scalar_int(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar integer argument."""
+		return cls(name, DataType.Integer, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_int_ext(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar extended integer argument."""
+		return cls(name, DataType.IntegerExt, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_str(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar string argument."""
+		return cls(name, DataType.String, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_raw_str(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar raw string argument."""
+		return cls(name, DataType.RawString, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_bool(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar boolean argument."""
+		return cls(name, DataType.Boolean, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_float(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar float argument."""
+		return cls(name, DataType.Float, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_float_ext(cls, name: str, intern_link: str = None):
+		"""Describes mandatory scalar extended float argument."""
+		return cls(name, DataType.FloatExt, None, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_enum(cls, name: str, enum_type, intern_link: str = None):
+		"""Describes mandatory scalar float argument."""
+		return cls(name, DataType.Enum, enum_type, False, False, 1, intern_link)
+
+	@classmethod
+	def scalar_str_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar string argument."""
+		return cls(name, DataType.String, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_raw_str_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar raw string argument."""
+		return cls(name, DataType.RawString, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_bool_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar boolean argument."""
+		return cls(name, DataType.Boolean, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_int_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar integer argument."""
+		return cls(name, DataType.Integer, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_int_ext_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar extended integer argument."""
+		return cls(name, DataType.IntegerExt, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_float_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar float argument."""
+		return cls(name, DataType.Float, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_float_ext_optional(cls, name: str, intern_link: str = None):
+		"""Describes optional scalar extended float argument."""
+		return cls(name, DataType.FloatExt, None, True, False, 1, intern_link)
+
+	@classmethod
+	def scalar_enum_optional(cls, name: str, enum_type, intern_link: str = None):
+		"""Describes optional scalar float argument."""
+		return cls(name, DataType.Enum, enum_type, True, False, 1, intern_link)
+
+	def __str__(self):
+		opt = '~' if self.is_optional else ''
+		name = f" '{self.name}'" if self.name != '' else ''
+		out = f"StructArg {opt}{self.data_type.name}{name}"
+
+		if self.is_open_list is False and self.repetition > 1:
+			out += f' [{self.repetition}]'
+		elif self.is_open_list is True:
+			out += f' [{self.repetition}...]'
+		if self.intern_link:
+			out += f", Linking: '{self.intern_link}'"
+		return out
+
+	def has_value(self, obj) -> bool:
+		"""Returns True, if the entered object attribute has value."""
+		return getattr(obj, self.name) is not None
+
+	def assert_is_optional(self, obj) -> None:
+		"""Asserts that the parameter is optional.
+		If not, the method throws an exception."""
+		if self.is_optional:
+			return
+		value = getattr(obj, self.name)
+		if value is None:
+			raise Exception(f"Structure '{obj}', argument without value is not optional: {self}")
+		else:
+			raise Exception(f"Structure '{obj}', argument is not optional: {self}', value '{value}'")
+
+	def assert_mandatory_has_value(self, obj) -> None:
+		"""Asserts that if the parameter is mandatory, it must have value assigned.
+		If not, the method throws an exception."""
+		if self.is_optional:
+			return
+		if getattr(obj, self.name) is None:
+			raise ValueError(f"Mandatory structure '{obj}' argument '{self.name}' has no value.")
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgStructList.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgStructList.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from .ArgStringComposer import StructComposer, compose_cmd_string_from_struct_args
-from .ArgStructStringParser import ArgStructStringParser
-from .StructBase import StructBase
-
-
-class ArgStructList(object):
-	"""Contains methods for composing cmd string and parsing cmd response to the provided structure instance."""
-
-	RAW_DATA_PROP_NAME = 'RawReturnData'
-
-	def __init__(self, struct):
-		self.__struct = struct
-		self.args = self.__get_struct_arg_attrs()
-
-	def __str__(self):
-		return f"'{self.__struct.__class__.__name__}', {len(self.args)} args: [ {', '.join([self.args[x].name for x in self.args])} ]"
-
-	def __get_struct_arg_attrs(self):
-		"""Fills self.args with the dictionary of ArgStruct list.
-		Dictionary key is the argument order (argument_ix)."""
-		# noinspection PyUnresolvedReferences,PyProtectedMember
-		args_list = StructBase._StructBase__get_meta_args_list(None, self.__struct)
-		# meta_data = getattr(self.__struct, '_{}__meta_args_list'.format(self.__struct.__class__.__name__))
-		args = dict()
-		for x in args_list:
-			args[x.argument_ix] = x
-
-		return args
-
-	def parse_from_cmd_response(self, content: str):
-		"""Fills the structure from the entered string content (command response)."""
-		if hasattr(self.__struct, ArgStructList.RAW_DATA_PROP_NAME):
-			setattr(self.__struct, ArgStructList.RAW_DATA_PROP_NAME, content)
-
-		parser = ArgStructStringParser(self.__struct, content)
-		arg_count = len(self.args)
-		arg_ix = 0
-
-		# Non-repeated arguments
-		while arg_ix < arg_count and self.args[arg_ix].is_open_list is False:
-			arg = self.args[arg_ix]
-			if arg.repetition <= 1:
-				# No list, but scalar value
-				parser.to_scalar_value(arg)
-			else:
-				# List with a fixed size, not repeated
-				parser.to_list_value(arg, True, 0, arg.repetition, arg.repetition, 1)
-
-			arg_ix += 1
-
-		if arg_ix < arg_count:
-			arg = self.args[arg_ix]
-			# Still some args to go
-			if arg.is_open_list is True:
-				# The previous loop ended because the next argument had is_open_list True
-				if arg_ix == (arg_count - 1):
-					# This is the last argument, ignore the repetitions and take the whole rest of the elements
-					parser.to_list_value(arg, True, 0, parser.remaining, parser.remaining, 1)
-				else:
-					# More than one arguments remaining. Loop through them interleaving the result strings
-					open_list_args = {key: value for key, value in self.args.items() if key >= arg_ix}
-
-					# Accumulate the number of repetitions from all the open_list_args
-					period: int = sum(open_list_args[ix].repetition for ix in open_list_args)
-					reminder: int = parser.remaining % period
-					if reminder != 0:
-						raise Exception(
-							f'Arguments parsing is not aligned - source string elements remaining to parse {parser.remaining}'
-							f'is not dividable by the summary Period {period} of all the open list arguments:\n' + '\n'.join(['{}'.format(x) for x in open_list_args]))
-					# Go through the arguments and accumulate the list content
-					offset = 0
-					for x in open_list_args:
-						arg = open_list_args[x]
-						parser.to_list_value(arg, False, offset, arg.repetition, period, -1)
-						offset += arg.repetition
-
-	def compose_cmd_string(self):
-		"""Composes the string argument from the structure for sending to the instrument."""
-		return compose_cmd_string_from_struct_args(self.args, StructComposer(self.__struct), self.__struct)
+from .ArgStringComposer import StructComposer, compose_cmd_string_from_struct_args
+from .ArgStructStringParser import ArgStructStringParser
+from .StructBase import StructBase
+
+
+class ArgStructList(object):
+	"""Contains methods for composing cmd string and parsing cmd response to the provided structure instance."""
+
+	RAW_DATA_PROP_NAME = 'RawReturnData'
+
+	def __init__(self, struct):
+		self.__struct = struct
+		self.args = self.__get_struct_arg_attrs()
+
+	def __str__(self):
+		return f"'{self.__struct.__class__.__name__}', {len(self.args)} args: [ {', '.join([self.args[x].name for x in self.args])} ]"
+
+	def __get_struct_arg_attrs(self):
+		"""Fills self.args with the dictionary of ArgStruct list.
+		Dictionary key is the argument order (argument_ix)."""
+		# noinspection PyUnresolvedReferences,PyProtectedMember
+		args_list = StructBase._StructBase__get_meta_args_list(None, self.__struct)
+		# meta_data = getattr(self.__struct, '_{}__meta_args_list'.format(self.__struct.__class__.__name__))
+		args = dict()
+		for x in args_list:
+			args[x.argument_ix] = x
+
+		return args
+
+	def parse_from_cmd_response(self, content: str):
+		"""Fills the structure from the entered string content (command response)."""
+		if hasattr(self.__struct, ArgStructList.RAW_DATA_PROP_NAME):
+			setattr(self.__struct, ArgStructList.RAW_DATA_PROP_NAME, content)
+
+		parser = ArgStructStringParser(self.__struct, content)
+		arg_count = len(self.args)
+		arg_ix = 0
+
+		# Non-repeated arguments
+		while arg_ix < arg_count and self.args[arg_ix].is_open_list is False:
+			arg = self.args[arg_ix]
+			if arg.repetition <= 1:
+				# No list, but scalar value
+				parser.to_scalar_value(arg)
+			else:
+				# List with a fixed size, not repeated
+				parser.to_list_value(arg, True, 0, arg.repetition, arg.repetition, 1)
+
+			arg_ix += 1
+
+		if arg_ix < arg_count:
+			arg = self.args[arg_ix]
+			# Still some args to go
+			if arg.is_open_list is True:
+				# The previous loop ended because the next argument had is_open_list True
+				if arg_ix == (arg_count - 1):
+					# This is the last argument, ignore the repetitions and take the whole rest of the elements
+					parser.to_list_value(arg, True, 0, parser.remaining, parser.remaining, 1)
+				else:
+					# More than one arguments remaining. Loop through them interleaving the result strings
+					open_list_args = {key: value for key, value in self.args.items() if key >= arg_ix}
+
+					# Accumulate the number of repetitions from all the open_list_args
+					period: int = sum(open_list_args[ix].repetition for ix in open_list_args)
+					reminder: int = parser.remaining % period
+					if reminder != 0:
+						raise Exception(
+							f'Arguments parsing is not aligned - source string elements remaining to parse {parser.remaining}'
+							f'is not dividable by the summary Period {period} of all the open list arguments:\n' + '\n'.join(['{}'.format(x) for x in open_list_args]))
+					# Go through the arguments and accumulate the list content
+					offset = 0
+					for x in open_list_args:
+						arg = open_list_args[x]
+						parser.to_list_value(arg, False, offset, arg.repetition, period, -1)
+						offset += arg.repetition
+
+	def compose_cmd_string(self):
+		"""Composes the string argument from the structure for sending to the instrument."""
+		return compose_cmd_string_from_struct_args(self.args, StructComposer(self.__struct), self.__struct)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ArgStructStringParser.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ArgStructStringParser.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from . import Utilities
-from .ArgStruct import ArgStruct
-
-
-class ArgStructStringParser:
-	"""Class for parsing a response from the instrument to an output structure of arguments.
-	It is used by the ArgStructList class for filling structures with return values."""
-
-	def __init__(self, struct, value: str):
-		self.struct = struct
-		self.elements = value.split(',')
-		self.count = len(self.elements)
-		self.position = 0
-
-	@property
-	def remaining(self) -> int:
-		"""Remaining items to parse."""
-		return self.count - self.position
-
-	def to_scalar_value(self, arg: ArgStruct):
-		"""Parses the current element to a scalar argument."""
-		assert arg.data_type.is_scalar, f'to_scalar_value() method only works with scalar values. Data type: {arg.data_type}'
-		if self.position >= self.count:
-			raise Exception(
-				f"Cannot parse a scalar value to structure argument. Response contains only {self.count} elements, "
-				f"argument '{arg.name}' has position {self.position + 1}.\n"
-				f"Response (commas replaced by new lines):\n" + Utilities.truncate_string_from_end('\n'.join(self.elements), 1000))
-		string = self.elements[self.position]
-		value = arg.conv_from_scpi_string.get_one_element_value(string)
-		setattr(self.struct, arg.name, value)
-		self.position += 1
-
-	def to_list_value(self, arg: ArgStruct, increase_pos: bool, offset: int, count: int, period: int, cycles: int) -> None:
-		"""Parses more elements to the list argument - slicing."""
-		assert arg.data_type.is_list, f'to_list_value method only works with list values. Data type: {arg.data_type}'
-		if cycles < 0:
-			cycles = self.remaining // period
-		if self.position >= self.count:
-			raise Exception(
-				f"Cannot parse an list value to the argument '{arg.name}', "
-				f"because the element position {self.position} is over the parsed list length {self.count}")
-		if (self.position + offset + count) > self.count:
-			raise Exception(
-				f"Cannot parse the whole list value to the argument '{arg.name}', because the element position {self.position} "
-				f"plus the argument offset {offset} and argument length {count} would be over the parsed list length {self.count}")
-
-		result = []
-		for cycle in range(cycles):
-			start_ix = self.position + (cycle * period) + offset
-			for i in range(count):
-				result.append(arg.conv_from_scpi_string.get_one_element_value(self.elements[start_ix + i]))
-
-		if increase_pos:
-			self.position += count
-
-		setattr(self.struct, arg.name, result)
+from . import Utilities
+from .ArgStruct import ArgStruct
+
+
+class ArgStructStringParser:
+	"""Class for parsing a response from the instrument to an output structure of arguments.
+	It is used by the ArgStructList class for filling structures with return values."""
+
+	def __init__(self, struct, value: str):
+		self.struct = struct
+		self.elements = value.split(',')
+		self.count = len(self.elements)
+		self.position = 0
+
+	@property
+	def remaining(self) -> int:
+		"""Remaining items to parse."""
+		return self.count - self.position
+
+	def to_scalar_value(self, arg: ArgStruct):
+		"""Parses the current element to a scalar argument."""
+		assert arg.data_type.is_scalar, f'to_scalar_value() method only works with scalar values. Data type: {arg.data_type}'
+		if self.position >= self.count:
+			raise Exception(
+				f"Cannot parse a scalar value to structure argument. Response contains only {self.count} elements, "
+				f"argument '{arg.name}' has position {self.position + 1}.\n"
+				f"Response (commas replaced by new lines):\n" + Utilities.truncate_string_from_end('\n'.join(self.elements), 1000))
+		string = self.elements[self.position]
+		value = arg.conv_from_scpi_string.get_one_element_value(string)
+		setattr(self.struct, arg.name, value)
+		self.position += 1
+
+	def to_list_value(self, arg: ArgStruct, increase_pos: bool, offset: int, count: int, period: int, cycles: int) -> None:
+		"""Parses more elements to the list argument - slicing."""
+		assert arg.data_type.is_list, f'to_list_value method only works with list values. Data type: {arg.data_type}'
+		if cycles < 0:
+			cycles = self.remaining // period
+		if self.position >= self.count:
+			raise Exception(
+				f"Cannot parse an list value to the argument '{arg.name}', "
+				f"because the element position {self.position} is over the parsed list length {self.count}")
+		if (self.position + offset + count) > self.count:
+			raise Exception(
+				f"Cannot parse the whole list value to the argument '{arg.name}', because the element position {self.position} "
+				f"plus the argument offset {offset} and argument length {count} would be over the parsed list length {self.count}")
+
+		result = []
+		for cycle in range(cycles):
+			start_ix = self.position + (cycle * period) + offset
+			for i in range(count):
+				result.append(arg.conv_from_scpi_string.get_one_element_value(self.elements[start_ix + i]))
+
+		if increase_pos:
+			self.position += count
+
+		setattr(self.struct, arg.name, result)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/CommandsGroup.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/CommandsGroup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from enum import Enum
-from typing import List
-from .Core import Core
-from .RepeatedCapability import RepeatedCapability as RepCap
-from .InstrumentErrors import DriverValueError
-
-
-class CommandsGroup:
-	"""Contains methods dealing with RepCaps and Group object cloning"""
-
-	def __init__(self, group_name: str, core: Core, parent: 'CommandsGroup'):
-		"""Constructor with header name, group property name and the start value"""
-
-		self.group_name = group_name
-		self._core = core
-		self.parent = parent
-		self.io = core.io
-		self.existing_children = []
-		self.rep_cap: RepCap or None = None
-		self.multi_repcap_types: str = ''
-		if parent:
-			parent.existing_children.append(self)
-
-	def __str__(self):
-		"""String representation of the CommandsGroup"""
-		out = f"SCPI Commands Group {self.group_name}"
-		if self.has_repcap():
-			out += f', RepCap {self.rep_cap.name} = {self.rep_cap.get_enum_value()}'
-		return out
-
-	def has_repcap(self) -> bool:
-		"""Returns True, if the group has a RepCap.
-		Returns False for a group with MultiRepCaps"""
-		return self.rep_cap is not None
-
-	def has_multi_repcaps(self) -> bool:
-		"""Returns True for a group with MultiRepCaps"""
-		return self.multi_repcap_types != ''
-
-	def add_existing_child(self, child: 'CommandsGroup') -> None:
-		"""Adds the child to the parent's list of created children.
-		This is used when the group is cloned, where the whole existing tree of groups have to be recreated"""
-		self.existing_children.append(child)
-
-	def set_repcap_enum_value(self, enum_value: Enum) -> None:
-		"""Sets RepCap value as enum
-		Default is not allowed."""
-		try:
-			self.rep_cap.set_enum_value(enum_value)
-		except ValueError:
-			raise DriverValueError(self.io.resource_name, f"Commands group RepCap value '{self.rep_cap.name}.Default' cannot be set. Please select a concrete value.")
-
-	def get_repcap_enum_value(self) -> Enum:
-		"""Returns RepCap value as enum"""
-		return self.rep_cap.get_enum_value()
-
-	def get_repcap_cmd_value(self, enum_value: Enum, enum_type) -> str:
-		"""Returns the current string of RepCapCmdValue for the entered RepCapEnumName
-		The enum_value can be a repcap of the current CommandsGroup or any of their parents"""
-		# Use the static functions of the RepeatedCapability to get the non-default value
-		# It is faster, since there is no need to use the RepCap instance
-		if not RepCap.clsm_is_default_value(enum_value, enum_type):
-			return RepCap.clsm_get_cmd_string_value(enum_value, enum_type)
-		# Default value - get it from the group or the parent groups
-		group = self
-		while group is not None:
-			if group.has_repcap():
-				if group.rep_cap.matches_type(enum_type):
-					return group.rep_cap.get_cmd_string_value()
-			group = group.parent
-
-		# repCapEnumName not found in single repcaps. Check the multiRepCaps
-		group = self
-		while group is not None:
-			if group.has_multi_repcaps():
-				if str(enum_type.__name__) in group.multi_repcap_types.split(','):
-					# Found in the multiple repcaps, create more fitting exception message
-					raise DriverValueError(
-						self.io.resource_name,
-						f"You can not use the RepCap value '{enum_value}', "
-						f"because its real value is not defined in any of the parent command groups. Please select a concrete value.")
-			group = group.parent
-
-		# repCapEnumName not found, create exception message
-		group = self
-		groups = []
-		while group is not None:
-			item = group.group_name
-			if group.has_repcap():
-				item += f' => {group.rep_cap.name}'
-			groups.insert(0, item)
-			group = group.parent
-
-		groups_chain = str.join("\n", groups)
-		raise DriverValueError(
-			self.io.resource_name,
-			f"Error replacing RepCaps in the SCPI command:"
-			f"RepCap '{enum_type}' not found in the group chain:\n{groups_chain}")
-
-	def get_owners_chain(self, stop: 'CommandsGroup' = None) -> List['CommandsGroup']:
-		"""Returns the owners chain including itself up to the entered point or up to the root by default"""
-		chain = []
-		group = self
-		while group != stop:
-			chain.append(group)
-			group = group.parent
-		return chain
-
-	def get_self_and_desc_existing_children(self) -> List['CommandsGroup']:
-		"""Get all the existing descendant groups recursively"""
-		all_descendants = [self]
-		for x in self.existing_children:
-			all_descendants.extend(x.get_self_and_desc_existing_children())
-		return all_descendants
-
-	def synchronize_repcaps(self, new_group) -> None:
-		"""Clones the existing group repeated capabilities to the new one.
-		Because of the lazy group properties, the group clones are created by accessing the repcaps in them"""
-		all_existing = filter(lambda grp: grp.has_repcap(), self.get_self_and_desc_existing_children())
-		for x in all_existing:
-			chain = x.get_owners_chain(self)
-			chain.reverse()
-			group = new_group
-			for item in chain:
-				group = getattr(group, item.group_name)
-			fnc = getattr(group, x.rep_cap.method_set_name)
-			fnc(x.rep_cap.get_enum_value())
-
-	def restore_repcaps(self) -> None:
-		"""Sets RepCaps of the Group and its children groups to their initial values"""
-		all_existing = filter(lambda grp: grp.has_repcap(), self.get_self_and_desc_existing_children())
-		for x in all_existing:
-			x.rep_cap.set_to_start_value()
+from enum import Enum
+from typing import List
+from .Core import Core
+from .RepeatedCapability import RepeatedCapability as RepCap
+from .InstrumentErrors import DriverValueError
+
+
+class CommandsGroup:
+	"""Contains methods dealing with RepCaps and Group object cloning"""
+
+	def __init__(self, group_name: str, core: Core, parent: 'CommandsGroup'):
+		"""Constructor with header name, group property name and the start value"""
+
+		self.group_name = group_name
+		self._core = core
+		self.parent = parent
+		self.io = core.io
+		self.existing_children = []
+		self.rep_cap: RepCap or None = None
+		self.multi_repcap_types: str = ''
+		if parent:
+			parent.existing_children.append(self)
+
+	def __str__(self):
+		"""String representation of the CommandsGroup"""
+		out = f"SCPI Commands Group {self.group_name}"
+		if self.has_repcap():
+			out += f', RepCap {self.rep_cap.name} = {self.rep_cap.get_enum_value()}'
+		return out
+
+	def has_repcap(self) -> bool:
+		"""Returns True, if the group has a RepCap.
+		Returns False for a group with MultiRepCaps"""
+		return self.rep_cap is not None
+
+	def has_multi_repcaps(self) -> bool:
+		"""Returns True for a group with MultiRepCaps"""
+		return self.multi_repcap_types != ''
+
+	def add_existing_child(self, child: 'CommandsGroup') -> None:
+		"""Adds the child to the parent's list of created children.
+		This is used when the group is cloned, where the whole existing tree of groups have to be recreated"""
+		self.existing_children.append(child)
+
+	def set_repcap_enum_value(self, enum_value: Enum) -> None:
+		"""Sets RepCap value as enum
+		Default is not allowed."""
+		try:
+			self.rep_cap.set_enum_value(enum_value)
+		except ValueError:
+			raise DriverValueError(self.io.resource_name, f"Commands group RepCap value '{self.rep_cap.name}.Default' cannot be set. Please select a concrete value.")
+
+	def get_repcap_enum_value(self) -> Enum:
+		"""Returns RepCap value as enum"""
+		return self.rep_cap.get_enum_value()
+
+	def get_repcap_cmd_value(self, enum_value: Enum, enum_type) -> str:
+		"""Returns the current string of RepCapCmdValue for the entered RepCapEnumName
+		The enum_value can be a repcap of the current CommandsGroup or any of their parents"""
+		# Use the static functions of the RepeatedCapability to get the non-default value
+		# It is faster, since there is no need to use the RepCap instance
+		if not RepCap.clsm_is_default_value(enum_value, enum_type):
+			return RepCap.clsm_get_cmd_string_value(enum_value, enum_type)
+		# Default value - get it from the group or the parent groups
+		group = self
+		while group is not None:
+			if group.has_repcap():
+				if group.rep_cap.matches_type(enum_type):
+					return group.rep_cap.get_cmd_string_value()
+			group = group.parent
+
+		# repCapEnumName not found in single repcaps. Check the multiRepCaps
+		group = self
+		while group is not None:
+			if group.has_multi_repcaps():
+				if str(enum_type.__name__) in group.multi_repcap_types.split(','):
+					# Found in the multiple repcaps, create more fitting exception message
+					raise DriverValueError(
+						self.io.resource_name,
+						f"You can not use the RepCap value '{enum_value}', "
+						f"because its real value is not defined in any of the parent command groups. Please select a concrete value.")
+			group = group.parent
+
+		# repCapEnumName not found, create exception message
+		group = self
+		groups = []
+		while group is not None:
+			item = group.group_name
+			if group.has_repcap():
+				item += f' => {group.rep_cap.name}'
+			groups.insert(0, item)
+			group = group.parent
+
+		groups_chain = str.join("\n", groups)
+		raise DriverValueError(
+			self.io.resource_name,
+			f"Error replacing RepCaps in the SCPI command:"
+			f"RepCap '{enum_type}' not found in the group chain:\n{groups_chain}")
+
+	def get_owners_chain(self, stop: 'CommandsGroup' = None) -> List['CommandsGroup']:
+		"""Returns the owners chain including itself up to the entered point or up to the root by default"""
+		chain = []
+		group = self
+		while group != stop:
+			chain.append(group)
+			group = group.parent
+		return chain
+
+	def get_self_and_desc_existing_children(self) -> List['CommandsGroup']:
+		"""Get all the existing descendant groups recursively"""
+		all_descendants = [self]
+		for x in self.existing_children:
+			all_descendants.extend(x.get_self_and_desc_existing_children())
+		return all_descendants
+
+	def synchronize_repcaps(self, new_group) -> None:
+		"""Clones the existing group repeated capabilities to the new one.
+		Because of the lazy group properties, the group clones are created by accessing the repcaps in them"""
+		all_existing = filter(lambda grp: grp.has_repcap(), self.get_self_and_desc_existing_children())
+		for x in all_existing:
+			chain = x.get_owners_chain(self)
+			chain.reverse()
+			group = new_group
+			for item in chain:
+				group = getattr(group, item.group_name)
+			fnc = getattr(group, x.rep_cap.method_set_name)
+			fnc(x.rep_cap.get_enum_value())
+
+	def restore_repcaps(self) -> None:
+		"""Sets RepCaps of the Group and its children groups to their initial values"""
+		all_existing = filter(lambda grp: grp.has_repcap(), self.get_self_and_desc_existing_children())
+		for x in all_existing:
+			x.rep_cap.set_to_start_value()
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/Conversions.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/Conversions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,606 +1,589 @@
-import math
-import struct
-import sys
-from enum import Enum
-from typing import List
-
-from . import Utilities
-
-
-class BinFloatFormat(Enum):
-	"""Binary format of a float number."""
-	Single_4bytes = 1
-	Single_4bytes_swapped = 2
-	Double_8bytes = 3
-	Double_8bytes_swapped = 4
-
-
-class BinIntFormat(Enum):
-	"""Binary format of an integer number."""
-	Integer32_4bytes = 1
-	Integer32_4bytes_swapped = 2
-	Integer16_2bytes = 3
-	Integer16_2bytes_swapped = 4
-
-
-def assert_string_data(value: str) -> None:
-	"""Asserts value is string type."""
-	assert isinstance(value, str), f"Input value type must be string. Actual type: {type(value)}, value: {value}"
-
-
-def assert_list_data(value: list) -> None:
-	"""Asserts value is list type."""
-	assert isinstance(value, list), f"Input value type must be a list. Actual type: {type(value)}, value: {value}"
-
-
-def _get_endianness_symbol(swap_endianness: bool) -> str:
-	"""Based on the current endianness returns the symbol used in the 'struct' module."""
-	if swap_endianness is False:
-		return '@'
-	elif swap_endianness is True and sys.byteorder == 'little':
-		return '>'
-	else:
-		return '<'
-
-
-def bytes_to_float32_list(data: bytes, swap_endianness=False) -> List[float]:
-	"""Converts bytes to list of floats - one number is represented by 4 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 4}f'
-	return list(struct.unpack(fmt, data))
-
-
-def bytes_to_double64_list(data: bytes, swap_endianness=False) -> List[float]:
-	"""Converts bytes to list of doubles - one number is represented by 8 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 8}d'
-	return list(struct.unpack(fmt, data))
-
-
-def bytes_to_int32_list(data: bytes, swap_endianness=False) -> List[int]:
-	"""Converts bytes to list of integer32 - one number is represented by 4 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 4}i'
-	return list(struct.unpack(fmt, data))
-
-
-def bytes_to_int16_list(data: bytes, swap_endianness=False) -> List[int]:
-	"""Converts bytes to list of integer16 - one number is represented by 2 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 2}h'
-	return list(struct.unpack(fmt, data))
-
-
-def bytes_to_list_of_floats(data: bytes, fmt: BinFloatFormat) -> List[float]:
-	"""Decodes binary data to a list of floating-point numbers based on the entered format."""
-	if fmt == BinFloatFormat.Single_4bytes:
-		return bytes_to_float32_list(data)
-	elif fmt == BinFloatFormat.Single_4bytes_swapped:
-		return bytes_to_float32_list(data, True)
-	elif fmt == BinFloatFormat.Double_8bytes:
-		return bytes_to_double64_list(data)
-	elif fmt == BinFloatFormat.Double_8bytes_swapped:
-		return bytes_to_double64_list(data, True)
-
-
-def bytes_to_list_of_integers(data: bytes, fmt: BinIntFormat) -> List[int]:
-	"""Decodes binary data to a list of integer numbers based on the entered format."""
-	if fmt == BinIntFormat.Integer32_4bytes:
-		return bytes_to_int32_list(data)
-	elif fmt == BinIntFormat.Integer32_4bytes_swapped:
-		return bytes_to_int32_list(data, True)
-	elif fmt == BinIntFormat.Integer16_2bytes:
-		return bytes_to_int16_list(data)
-	elif fmt == BinIntFormat.Integer16_2bytes_swapped:
-		return bytes_to_int16_list(data, True)
-
-
-def double64_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
-	"""Converts list of doubles to bytes - one number is converted to 8 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}d'
-	return struct.pack(fmt, *data)
-
-
-def float32_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
-	"""Converts list of floats to bytes - one number is converted to 4 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}f'
-	return struct.pack(fmt, *data)
-
-
-def int32_list_to_bytes(data: List[int], swap_endianness=False) -> bytes:
-	"""Converts list of integers 32 to bytes - one number is converted to 4 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}i'
-	return struct.pack(fmt, *data)
-
-
-def int16_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
-	"""Converts list of integers 16 to bytes - one number is converted to 2 bytes."""
-	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}h'
-	return struct.pack(fmt, *data)
-
-
-def list_of_integers_to_bytes(ints: List[int], fmt: BinIntFormat) -> bytes:
-	"""Encodes list of integers to binary data based on the entered format."""
-	if fmt == BinIntFormat.Integer32_4bytes:
-		return int32_list_to_bytes(ints)
-	elif fmt == BinIntFormat.Integer32_4bytes_swapped:
-		return int32_list_to_bytes(ints, True)
-	elif fmt == BinIntFormat.Integer16_2bytes:
-		return int16_list_to_bytes(ints)
-	elif fmt == BinIntFormat.Integer16_2bytes_swapped:
-		return int16_list_to_bytes(ints, True)
-
-
-def list_of_floats_to_bytes(floats: List[float], fmt: BinFloatFormat) -> bytes:
-	"""Encodes list of floats to binary data based on the entered format."""
-	if fmt == BinFloatFormat.Single_4bytes:
-		return float32_list_to_bytes(floats)
-	elif fmt == BinFloatFormat.Single_4bytes_swapped:
-		return float32_list_to_bytes(floats, True)
-	elif fmt == BinFloatFormat.Double_8bytes:
-		return double64_list_to_bytes(floats)
-	elif fmt == BinFloatFormat.Double_8bytes_swapped:
-		return double64_list_to_bytes(floats, True)
-
-
-pure_bool_true_lookup = frozenset(['on', 'On', 'ON', 'true', 'True', 'TRUE'])
-bool_true_lookup = frozenset(['1', 'on', 'On', 'ON', 'true', 'True', 'TRUE'])
-bool_false_lookup = frozenset(['0', 'off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
-pure_bool_false_lookup = frozenset(['off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
-
-
-def str_to_bool(string: str) -> bool:
-	"""Converts string to boolean value.
-	The function robust, and case insensitive.
-	If the string can not be converted to a boolean, the function returns False."""
-	assert_string_data(string)
-	if string in bool_true_lookup:
-		return True
-	if string in bool_false_lookup:
-		return False
-	# If leading/trailing spaces
-	string = string.strip()
-	if string in bool_true_lookup:
-		return True
-	if string in bool_false_lookup:
-		return False
-	# If enclosed by brackets
-	string = Utilities.trim_str_response(string)
-	if string in bool_true_lookup:
-		return True
-	if string in bool_false_lookup:
-		return False
-	return False
-
-
-def string_to_pure_bool(string: str) -> bool or None:
-	"""Converts string to boolean value. Compare to str_to_bool(), the values '1' and '0' are not considered boolean.
-	Also, if the method can not convert the string to boolean, it returns None."""
-	assert_string_data(string)
-	if string in pure_bool_true_lookup:
-		return True
-	if string in pure_bool_false_lookup:
-		return False
-	# If leading/trailing spaces
-	string = string.strip()
-	if string in pure_bool_true_lookup:
-		return True
-	if string in pure_bool_false_lookup:
-		return False
-	# If enclosed by brackets
-	string = Utilities.trim_str_response(string)
-	if string in pure_bool_true_lookup:
-		return True
-	if string in pure_bool_false_lookup:
-		return False
-	return None
-
-
-number_plus_inf_lookup = frozenset(['Inf', 'INF', 'INFINITY', '+Inf', '+INF', '+inf', '+INFINITY', '+Infinity', '+infinity'])
-number_minus_inf_lookup = frozenset(['-Inf', '-INF', '-inf', '-INFINITY', '-Infinity', '-infinity'])
-number_nan_lookup = frozenset(['Nan', 'NAN', 'nan', 'NaN', 'NAV', 'NaV', 'NCAP', 'INV', 'NONE', 'none', 'None', 'DTX', 'UND', 'und'])
-number_max_lookup = frozenset(['OFL', 'ofl', 'Ofl'])
-number_min_lookup = frozenset(['UFL', 'ufl', 'Ufl'])
-int_neg_inf = -(sys.maxsize - 1)
-enum_spec_prefixes = {'_minus': '-', '_plus': '+', '_': ''}
-enum_spec_strings = {'_dash_': '-', '_dot_': '.'}
-
-
-def str_to_int(string: str) -> int:
-	"""Converts string to integer value. Float values are coerced to integer.
-	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
-	assert_string_data(string)
-	string = string.strip()
-	if string == '':
-		return 0
-	value = str_special_values_to_int(string)
-	if value:
-		return value
-
-	# Hexadecimal numbers
-	if string.startswith('#H') or string.startswith('0x'):
-		if ',' in string:
-			return int(string[2:string.find(',')], 16)
-		else:
-			return int(string[2:], 16)
-
-	# Binary numbers
-	if string.startswith('#B') or string.startswith('0b'):
-		if ',' in string:
-			return int(string[2:string.find(',')], 2)
-		else:
-			return int(string[2:], 2)
-
-	# Octal numbers
-	if string.startswith('#Q') or string.startswith('0o'):
-		if ',' in string:
-			return int(string[2:string.find(',')], 8)
-		else:
-			return int(string[2:], 8)
-	# Simulation
-	if string == 'Simulating':
-		return 0
-	return int(round(float(string)))
-
-
-def str_special_values_to_int(string: str) -> int:
-	"""Converts special string values to integer. Returns None if no special value was found."""
-	assert_string_data(string)
-	if string in number_plus_inf_lookup or string in number_max_lookup:
-		return sys.maxsize
-	if string in number_minus_inf_lookup or string in number_min_lookup or string in number_nan_lookup:
-		return int_neg_inf
-	if string == 'OFF':
-		return int_neg_inf + 1
-	if string == 'ON':
-		return int_neg_inf + 2
-	if string == 'OK':
-		return sys.maxsize - 1
-	if string == 'DC':
-		# noinspection PyTypeChecker
-		return int_neg_inf / 100
-	if string == 'ULEU':
-		return int(sys.maxsize / 10)
-	if string == 'ULEL':
-		# noinspection PyTypeChecker
-		return int_neg_inf / 10
-	# noinspection PyTypeChecker
-	return None
-
-
-def str_to_int_or_bool(string: str) -> int or bool:
-	"""Similar to str_to_int, but for special values "ON/OFF" the function returns boolean"""
-	result = string_to_pure_bool(string)
-	if result is not None:
-		return result
-	return str_to_int(string)
-
-
-def str_to_float(string: str) -> float:
-	"""Converts string to float value.
-	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
-	assert_string_data(string)
-	string = string.strip()
-	if string == '':
-		return 0.0
-	if string in number_plus_inf_lookup:
-		return math.inf
-	if string in number_minus_inf_lookup:
-		return -math.inf
-	if string in number_nan_lookup:
-		return math.nan
-	if string in number_max_lookup:
-		return sys.float_info.max
-	if string in number_min_lookup:
-		return -sys.float_info.max
-	if string == 'OFF':
-		return -sys.float_info.epsilon
-	if string == 'ON':
-		return -2*sys.float_info.epsilon
-	if string == 'OK':
-		return sys.float_info.epsilon
-	if string == 'DC' or string == '':
-		return -sys.float_info.max / 100
-	if string == 'ULEU':
-		return sys.float_info.max / 10
-	if string == 'ULEL':
-		return -sys.float_info.max / 10
-	if string == 'Simulating':
-		return 0.0
-	return float(string)
-
-
-def str_to_float_or_bool(string: str) -> float or bool:
-	"""Similar to str_to_float, but for special values "ON/OFF" the function returns boolean"""
-	result = string_to_pure_bool(string)
-	if result is not None:
-		return result
-	return str_to_float(string)
-
-
-def float_to_str(value: float) -> str:
-	"""Converts double number to string using {.12g} formatter."""
-	return format(value, ".12g")
-
-
-def bool_to_str(value: bool) -> str:
-	"""Converts boolean to 'ON' or 'OFF' string."""
-	if type(value) is bool:
-		return 'ON' if value is True else 'OFF'
-	else:
-		raise Exception(f"bool_to_str: unsupported variable type '{type(value)}', value '{value}'. Only boolean values are supported.")
-
-
-def str_enclose_by_quotes(string: str) -> str:
-	"""Returns string enclosed by single quotes."""
-	assert_string_data(string)
-	return "'" + string + "'"
-
-
-def list_to_csv_str(value: list) -> str:
-	"""Converts list of elements to strings separated by commas.
-	Element types can differ on an individual basis.
-	Supported element types:
-	- int
-	- bool
-	- float
-	- string -> string no quotes
-	- enum"""
-	assert_list_data(value)
-	result = []
-	for x in value:
-		el = value_to_str(x)
-		if not el:
-			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_str: '{x}'")
-		result.append(el)
-	return ','.join(result)
-
-
-def list_to_csv_quoted_str(value: list) -> str:
-	"""Converts list of elements to quoted strings separated by commas.
-	Only string elements are enclosed by single quotes
-	Element types can differ on an individual basis.
-	Supported element types:
-	- int
-	- bool
-	- float
-	- string -> string enclosed by quotes
-	- enum"""
-	assert_list_data(value)
-	result = []
-	for x in value:
-		if isinstance(x, str):
-			el = str_enclose_by_quotes(x)
-		else:
-			el = value_to_str(x)
-		if not el:
-			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_quoted_str: '{x}'")
-		result.append(el)
-
-	return ','.join(result)
-
-
-def decimal_value_to_str(x: int or float) -> str:
-	"""Converts scalar decimal value to string.
-	Supported element types:
-	- int
-	- float"""
-	if isinstance(x, int) and type(x) is not bool:
-		return str(x)
-	elif isinstance(x, float):
-		return float_to_str(x)
-	else:
-		raise Exception(f"decimal_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer and float types are supported.")
-
-
-def decimal_or_bool_value_to_str(x: int or float or bool) -> str:
-	"""Converts scalar decimal value to string.
-	Supported element types:
-	- int
-	- float
-	- boolean"""
-	if type(x) is bool:
-		return bool_to_str(x)
-	if isinstance(x, int):
-		return str(x)
-	elif isinstance(x, float):
-		return float_to_str(x)
-	else:
-		raise Exception(f"decimal_or_bool_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer, float and boolean types are supported.")
-
-
-def value_to_str(x: int or bool or float or str or Enum) -> str:
-	"""Converts scalar value to string.
-	Supported element types:
-	- int
-	- bool
-	- float
-	- string
-	- enum"""
-	if isinstance(x, bool):
-		return bool_to_str(x)
-	elif isinstance(x, int):
-		return str(x)
-	elif isinstance(x, float):
-		return float_to_str(x)
-	elif isinstance(x, str):
-		return x
-	elif isinstance(x, Enum):
-		return enum_value_to_scpi_string(x.name)
-	else:
-		raise Exception(f"value_to_str: unsupported variable type '{type(x)}', value '{x}'. Supported types: int, bool, float, str, enum.")
-
-
-def enum_value_to_scpi_string(enum_value: str) -> str:
-	"""Conversion EnumValue -> SCPI_String
-	Unescapes all the special characters that can not be contained in the enum member definition, but can be sent to the instrument as enum string.
-	Use this to send the scpi enum value to the instrument."""
-	for key in enum_spec_prefixes:
-		if enum_value.startswith(key):
-			enum_value = enum_spec_prefixes[key] + enum_value[len(key):]
-	for key in enum_spec_strings:
-		enum_value = enum_value.replace(key, enum_spec_strings[key])
-	return enum_value
-
-
-def value_to_quoted_str(x: int or bool or float or str or Enum) -> str:
-	"""Converts scalar value to string enclosed by single quotes.
-	Supported element types:
-	- int
-	- bool
-	- float
-	- string
-	- enum"""
-	return f"'{value_to_str(x)}'"
-
-
-def str_to_float_list(string: str) -> List[float]:
-	"""Converts string with comma-separated values to list of Floats."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(str_to_float, string.split(','))]
-	return result
-
-
-def str_to_float_or_bool_list(string: str) -> List[float or bool]:
-	"""Converts string with comma-separated values to list of float or boolean values."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(str_to_float_or_bool, string.split(','))]
-	return result
-
-
-def str_to_int_list(string: str) -> List[int]:
-	"""Converts string with comma-separated values to list of Integers."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(str_to_int, string.split(','))]
-	return result
-
-
-def str_to_int_or_bool_list(string: str) -> List[int or bool]:
-	"""Converts string with comma-separated values to list of integer or boolean values."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(str_to_int_or_bool, string.split(','))]
-	return result
-
-
-def str_to_bool_list(string: str) -> List[bool]:
-	"""Converts string with comma-separated values to list of booleans."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(str_to_bool, string.split(','))]
-	return result
-
-
-def str_to_str_list(string: str, clear_one_empty_item: bool = False) -> List[str]:
-	"""Converts string with comma-separated values to list of strings.
-	Each element is trimmed by trim_str_response().
-	If the clear_one_empty_item is set to True (default is False), and the result is exactly one empty string item, the method returns empty list."""
-	assert_string_data(string)
-	if not string:
-		return []
-	result = [*map(Utilities.trim_str_response, string.split(','))]
-	if clear_one_empty_item and len(result) == 1 and result[0] == '':
-		return []
-	return result
-
-
-def _find_in_enum_members(item: str, enum_members: List[str]) -> int:
-	"""Matches a string in the provided list of member strings.
-	The item must be not fully matched.
-	The item is matched if a member string starts with the item (the item is a prefix of the member).
-	Example: item='CONN' will match the enum_member 'CONNected'
-	If the item contains a comma, only the value before comma is considered
-	Returns found index in the enum_members list"""
-	if ',' in item:
-		item = item[:item.index(',')].strip()
-	i = 0
-	for x in enum_members:
-		if x.startswith(item):
-			return i
-		i += 1
-
-	# smart matching:
-	# item = 'MAX' matches enum 'MAXpeak'
-	# item = 'SPECtrum1' matches enum 'SPEC1'
-	# item = 'SPEC' matches enum 'SPECtrum1'
-
-	item = ''.join([c for c in item if not c.islower()])
-	# item must be longer than 1 character
-	if len(item) < 2:
-		return -1
-	i = 0
-	for x in enum_members:
-		x_uc = ''.join([c for c in x if not c.islower()])
-		if x_uc == item:
-			return i
-		i += 1
-	return -1
-
-
-def str_to_scalar_enum_helper(string: str, enum_type: Enum, enum_members=None) -> Enum:
-	"""Converts string to one enum element.
-	enum_members are optional to improve the performance for repeated conversions.
-	If you do not provide them, they are generated inside the function."""
-	value = Utilities.trim_str_response(string)
-	if not enum_members:
-		# noinspection PyTypeChecker
-		enum_members = [x.name for x in enum_type]
-
-	# Search in the enum member and return the index of the matched item
-	ix = _find_in_enum_members(value, enum_members)
-	if ix >= 0:
-		# noinspection PyUnresolvedReferences
-		return enum_type[enum_members[ix]]
-
-	# If the result is -1 (not found), try to replace the special values and search again
-	# This is done to improve the performance, since most of the enums have no special values
-	enum_members_conv = [enum_value_to_scpi_string(x) for x in enum_members]
-	ix = _find_in_enum_members(value, enum_members_conv)
-	if ix >= 0:
-		# noinspection PyUnresolvedReferences
-		return enum_type[enum_members[ix]]
-
-	# If not found, search in the special integer numbers:
-	spec_value = str_special_values_to_int(value)
-	if not spec_value:
-		raise Exception(f"String '{value}' can not be found in the enum type '{enum_type}'")
-	# noinspection PyTypeChecker
-	return spec_value
-
-
-def str_to_list_enum_helper(string: str, enum_type: Enum, enum_members=None) -> List[Enum]:
-	"""Converts string to list of enum elements.
-	enum_members are optional to improve the performance for repeated conversions.
-	If you do not provide them, they are generated inside the function."""
-	if not enum_members:
-		# noinspection PyTypeChecker
-		enum_members = [x.name for x in enum_type]
-	elements = string.split(',')
-	return [str_to_scalar_enum_helper(x, enum_type, enum_members) for x in elements]
-
-
-def enum_scalar_to_str(data, enum_type) -> str:
-	"""Converts enum scalar value to string."""
-	assert isinstance(data, enum_type), f"Expected command parameter {enum_type}, actual data type: {type(data)}. Value: {data}"
-	return value_to_str(data)
-
-
-def enum_list_to_str(data: List, enum_type) -> str:
-	"""Converts enum list to csv-string."""
-	# For enums, check that each element is an enum
-	assert all(isinstance(x, enum_type) for x in data), f"Expected command parameter list of {enum_type}, detected one or more elements of non-enum type. Value: {data}"
-	return list_to_csv_str(data)
-
-
-def str_to_scalar_enum(string: str, enum_type) -> Enum:
-	"""Converts string to one enum element."""
-	return str_to_scalar_enum_helper(string, enum_type)
-
-
-def str_to_list_enum(string: str, enum_type) -> List[Enum]:
-	"""Converts string to list of enum elements."""
-	return str_to_list_enum_helper(string, enum_type)
+import math
+import struct
+import sys
+from enum import Enum
+from typing import List
+
+from . import Utilities
+
+
+class BinFloatFormat(Enum):
+	"""Binary format of a float number."""
+	Single_4bytes = 1
+	Single_4bytes_swapped = 2
+	Double_8bytes = 3
+	Double_8bytes_swapped = 4
+
+
+class BinIntFormat(Enum):
+	"""Binary format of an integer number."""
+	Integer32_4bytes = 1
+	Integer32_4bytes_swapped = 2
+	Integer16_2bytes = 3
+	Integer16_2bytes_swapped = 4
+
+
+def assert_string_data(value: str) -> None:
+	"""Asserts value is string type."""
+	assert isinstance(value, str), f"Input value type must be string. Actual type: {type(value)}, value: {value}"
+
+
+def assert_list_data(value: list) -> None:
+	"""Asserts value is list type."""
+	assert isinstance(value, list), f"Input value type must be a list. Actual type: {type(value)}, value: {value}"
+
+
+def _get_endianness_symbol(swap_endianness: bool) -> str:
+	"""Based on the current endianness returns the symbol used in the 'struct' module."""
+	if swap_endianness is False:
+		return '@'
+	elif swap_endianness is True and sys.byteorder == 'little':
+		return '>'
+	else:
+		return '<'
+
+
+def bytes_to_float32_list(data: bytes, swap_endianness=False) -> List[float]:
+	"""Converts bytes to list of floats - one number is represented by 4 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 4}f'
+	return list(struct.unpack(fmt, data))
+
+
+def bytes_to_double64_list(data: bytes, swap_endianness=False) -> List[float]:
+	"""Converts bytes to list of doubles - one number is represented by 8 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 8}d'
+	return list(struct.unpack(fmt, data))
+
+
+def bytes_to_int32_list(data: bytes, swap_endianness=False) -> List[int]:
+	"""Converts bytes to list of integer32 - one number is represented by 4 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 4}i'
+	return list(struct.unpack(fmt, data))
+
+
+def bytes_to_int16_list(data: bytes, swap_endianness=False) -> List[int]:
+	"""Converts bytes to list of integer16 - one number is represented by 2 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{len(data) // 2}h'
+	return list(struct.unpack(fmt, data))
+
+
+def bytes_to_list_of_floats(data: bytes, fmt: BinFloatFormat) -> List[float]:
+	"""Decodes binary data to a list of floating-point numbers based on the entered format."""
+	if fmt == BinFloatFormat.Single_4bytes:
+		return bytes_to_float32_list(data)
+	elif fmt == BinFloatFormat.Single_4bytes_swapped:
+		return bytes_to_float32_list(data, True)
+	elif fmt == BinFloatFormat.Double_8bytes:
+		return bytes_to_double64_list(data)
+	elif fmt == BinFloatFormat.Double_8bytes_swapped:
+		return bytes_to_double64_list(data, True)
+
+
+def bytes_to_list_of_integers(data: bytes, fmt: BinIntFormat) -> List[int]:
+	"""Decodes binary data to a list of integer numbers based on the entered format."""
+	if fmt == BinIntFormat.Integer32_4bytes:
+		return bytes_to_int32_list(data)
+	elif fmt == BinIntFormat.Integer32_4bytes_swapped:
+		return bytes_to_int32_list(data, True)
+	elif fmt == BinIntFormat.Integer16_2bytes:
+		return bytes_to_int16_list(data)
+	elif fmt == BinIntFormat.Integer16_2bytes_swapped:
+		return bytes_to_int16_list(data, True)
+
+
+def double64_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
+	"""Converts list of doubles to bytes - one number is converted to 8 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}d'
+	return struct.pack(fmt, *data)
+
+
+def float32_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
+	"""Converts list of floats to bytes - one number is converted to 4 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}f'
+	return struct.pack(fmt, *data)
+
+
+def int32_list_to_bytes(data: List[int], swap_endianness=False) -> bytes:
+	"""Converts list of integers 32 to bytes - one number is converted to 4 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}i'
+	return struct.pack(fmt, *data)
+
+
+def int16_list_to_bytes(data: List[float], swap_endianness=False) -> bytes:
+	"""Converts list of integers 16 to bytes - one number is converted to 2 bytes."""
+	fmt = f'{_get_endianness_symbol(swap_endianness)}{str(len(data))}h'
+	return struct.pack(fmt, *data)
+
+
+def list_of_integers_to_bytes(ints: List[int], fmt: BinIntFormat) -> bytes:
+	"""Encodes list of integers to binary data based on the entered format."""
+	if fmt == BinIntFormat.Integer32_4bytes:
+		return int32_list_to_bytes(ints)
+	elif fmt == BinIntFormat.Integer32_4bytes_swapped:
+		return int32_list_to_bytes(ints, True)
+	elif fmt == BinIntFormat.Integer16_2bytes:
+		return int16_list_to_bytes(ints)
+	elif fmt == BinIntFormat.Integer16_2bytes_swapped:
+		return int16_list_to_bytes(ints, True)
+
+
+def list_of_floats_to_bytes(floats: List[float], fmt: BinFloatFormat) -> bytes:
+	"""Encodes list of floats to binary data based on the entered format."""
+	if fmt == BinFloatFormat.Single_4bytes:
+		return float32_list_to_bytes(floats)
+	elif fmt == BinFloatFormat.Single_4bytes_swapped:
+		return float32_list_to_bytes(floats, True)
+	elif fmt == BinFloatFormat.Double_8bytes:
+		return double64_list_to_bytes(floats)
+	elif fmt == BinFloatFormat.Double_8bytes_swapped:
+		return double64_list_to_bytes(floats, True)
+
+
+pure_bool_true_lookup = frozenset(['on', 'On', 'ON', 'true', 'True', 'TRUE'])
+bool_true_lookup = frozenset(['1', 'on', 'On', 'ON', 'true', 'True', 'TRUE'])
+bool_false_lookup = frozenset(['0', 'off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
+pure_bool_false_lookup = frozenset(['off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
+
+
+def str_to_bool(string: str) -> bool:
+	"""Converts string to boolean value.
+	The function robust, and case insensitive.
+	If the string can not be converted to a boolean, the function returns False."""
+	assert_string_data(string)
+	if string in bool_true_lookup:
+		return True
+	if string in bool_false_lookup:
+		return False
+	# If leading/trailing spaces
+	string = string.strip()
+	if string in bool_true_lookup:
+		return True
+	if string in bool_false_lookup:
+		return False
+	# If enclosed by brackets
+	string = Utilities.trim_str_response(string)
+	if string in bool_true_lookup:
+		return True
+	if string in bool_false_lookup:
+		return False
+	return False
+
+
+def string_to_pure_bool(string: str) -> bool or None:
+	"""Converts string to boolean value. Compare to str_to_bool(), the values '1' and '0' are not considered boolean.
+	Also, if the method can not convert the string to boolean, it returns None."""
+	assert_string_data(string)
+	if string in pure_bool_true_lookup:
+		return True
+	if string in pure_bool_false_lookup:
+		return False
+	# If leading/trailing spaces
+	string = string.strip()
+	if string in pure_bool_true_lookup:
+		return True
+	if string in pure_bool_false_lookup:
+		return False
+	# If enclosed by brackets
+	string = Utilities.trim_str_response(string)
+	if string in pure_bool_true_lookup:
+		return True
+	if string in pure_bool_false_lookup:
+		return False
+	return None
+
+
+number_plus_inf_lookup = frozenset(['Inf', 'INF', 'INFINITY', '+Inf', '+INF', '+inf', '+INFINITY', '+Infinity', '+infinity'])
+number_minus_inf_lookup = frozenset(['-Inf', '-INF', '-inf', '-INFINITY', '-Infinity', '-infinity'])
+number_nan_lookup = frozenset(['Nan', 'NAN', 'nan', 'NaN', 'NAV', 'NaV', 'NCAP', 'INV', 'NONE', 'none', 'None', 'DTX', 'UND', 'und'])
+number_max_lookup = frozenset(['OFL', 'ofl', 'Ofl'])
+number_min_lookup = frozenset(['UFL', 'ufl', 'Ufl'])
+int_neg_inf = -(sys.maxsize - 1)
+enum_spec_prefixes = {'_minus': '-', '_plus': '+', '_': ''}
+enum_spec_strings = {'_dash_': '-', '_dot_': '.'}
+
+
+def str_to_int(string: str) -> int:
+	"""Converts string to integer value. Float values are coerced to integer.
+	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
+	assert_string_data(string)
+	string = string.strip()
+	if string == '':
+		return 0
+	value = str_special_values_to_int(string)
+	if value:
+		return value
+
+	# Hexadecimal numbers
+	if string.startswith('#H') or string.startswith('0x'):
+		if ',' in string:
+			return int(string[2:string.find(',')], 16)
+		else:
+			return int(string[2:], 16)
+
+	# Binary numbers
+	if string.startswith('#B') or string.startswith('0b'):
+		if ',' in string:
+			return int(string[2:string.find(',')], 2)
+		else:
+			return int(string[2:], 2)
+
+	# Octal numbers
+	if string.startswith('#Q') or string.startswith('0o'):
+		if ',' in string:
+			return int(string[2:string.find(',')], 8)
+		else:
+			return int(string[2:], 8)
+	# Simulation
+	if string == 'Simulating':
+		return 0
+	return int(round(float(string)))
+
+
+def str_special_values_to_int(string: str) -> int:
+	"""Converts special string values to integer. Returns None if no special value was found."""
+	assert_string_data(string)
+	if string in number_plus_inf_lookup or string in number_max_lookup:
+		return sys.maxsize
+	if string in number_minus_inf_lookup or string in number_min_lookup or string in number_nan_lookup:
+		return int_neg_inf
+	if string == 'OFF':
+		return int_neg_inf + 1
+	if string == 'ON':
+		return int_neg_inf + 2
+	if string == 'OK':
+		return sys.maxsize - 1
+	if string == 'DC':
+		# noinspection PyTypeChecker
+		return int_neg_inf / 100
+	if string == 'ULEU':
+		return int(sys.maxsize / 10)
+	if string == 'ULEL':
+		# noinspection PyTypeChecker
+		return int_neg_inf / 10
+	# noinspection PyTypeChecker
+	return None
+
+
+def str_to_int_or_bool(string: str) -> int or bool:
+	"""Similar to str_to_int, but for special values "ON/OFF" the function returns boolean"""
+	result = string_to_pure_bool(string)
+	if result is not None:
+		return result
+	return str_to_int(string)
+
+
+def str_to_float(string: str) -> float:
+	"""Converts string to float value.
+	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
+	assert_string_data(string)
+	string = string.strip()
+	if string == '':
+		return 0.0
+	if string in number_plus_inf_lookup:
+		return math.inf
+	if string in number_minus_inf_lookup:
+		return -math.inf
+	if string in number_nan_lookup:
+		return math.nan
+	if string in number_max_lookup:
+		return sys.float_info.max
+	if string in number_min_lookup:
+		return -sys.float_info.max
+	if string == 'OFF':
+		return -sys.float_info.epsilon
+	if string == 'ON':
+		return -2*sys.float_info.epsilon
+	if string == 'OK':
+		return sys.float_info.epsilon
+	if string == 'DC' or string == '':
+		return -sys.float_info.max / 100
+	if string == 'ULEU':
+		return sys.float_info.max / 10
+	if string == 'ULEL':
+		return -sys.float_info.max / 10
+	if string == 'Simulating':
+		return 0.0
+	return float(string)
+
+
+def str_to_float_or_bool(string: str) -> float or bool:
+	"""Similar to str_to_float, but for special values "ON/OFF" the function returns boolean"""
+	result = string_to_pure_bool(string)
+	if result is not None:
+		return result
+	return str_to_float(string)
+
+
+def float_to_str(value: float) -> str:
+	"""Converts double number to string using {.12g} formatter."""
+	return format(value, ".12g")
+
+
+def bool_to_str(value: bool) -> str:
+	"""Converts boolean to 'ON' or 'OFF' string."""
+	if type(value) is bool:
+		return 'ON' if value is True else 'OFF'
+	else:
+		raise Exception(f"bool_to_str: unsupported variable type '{type(value)}', value '{value}'. Only boolean values are supported.")
+
+
+def str_enclose_by_quotes(string: str) -> str:
+	"""Returns string enclosed by single quotes."""
+	assert_string_data(string)
+	return "'" + string + "'"
+
+
+def list_to_csv_str(value: list) -> str:
+	"""Converts list of elements to strings separated by commas.
+	Element types can differ on an individual basis.
+	Supported element types:
+	- int
+	- bool
+	- float
+	- string -> string no quotes
+	- enum"""
+	assert_list_data(value)
+	result = []
+	for x in value:
+		el = value_to_str(x)
+		if not el:
+			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_str: '{x}'")
+		result.append(el)
+	return ','.join(result)
+
+
+def list_to_csv_quoted_str(value: list) -> str:
+	"""Converts list of elements to quoted strings separated by commas.
+	Only string elements are enclosed by single quotes
+	Element types can differ on an individual basis.
+	Supported element types:
+	- int
+	- bool
+	- float
+	- string -> string enclosed by quotes
+	- enum"""
+	assert_list_data(value)
+	result = []
+	for x in value:
+		if isinstance(x, str):
+			el = str_enclose_by_quotes(x)
+		else:
+			el = value_to_str(x)
+		if not el:
+			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_quoted_str: '{x}'")
+		result.append(el)
+
+	return ','.join(result)
+
+
+def decimal_value_to_str(x: int or float) -> str:
+	"""Converts scalar decimal value to string.
+	Supported element types:
+	- int
+	- float"""
+	if isinstance(x, int) and type(x) is not bool:
+		return str(x)
+	elif isinstance(x, float):
+		return float_to_str(x)
+	else:
+		raise Exception(f"decimal_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer and float types are supported.")
+
+
+def decimal_or_bool_value_to_str(x: int or float or bool) -> str:
+	"""Converts scalar decimal value to string.
+	Supported element types:
+	- int
+	- float
+	- boolean"""
+	if type(x) is bool:
+		return bool_to_str(x)
+	if isinstance(x, int):
+		return str(x)
+	elif isinstance(x, float):
+		return float_to_str(x)
+	else:
+		raise Exception(f"decimal_or_bool_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer, float and boolean types are supported.")
+
+
+def value_to_str(x: int or bool or float or str or Enum) -> str:
+	"""Converts scalar value to string.
+	Supported element types:
+	- int
+	- bool
+	- float
+	- string
+	- enum"""
+	if isinstance(x, bool):
+		return bool_to_str(x)
+	elif isinstance(x, int):
+		return str(x)
+	elif isinstance(x, float):
+		return float_to_str(x)
+	elif isinstance(x, str):
+		return x
+	elif isinstance(x, Enum):
+		return enum_value_to_scpi_string(x.name)
+	else:
+		raise Exception(f"value_to_str: unsupported variable type '{type(x)}', value '{x}'. Supported types: int, bool, float, str, enum.")
+
+
+def enum_value_to_scpi_string(enum_value: str) -> str:
+	"""Conversion EnumValue -> SCPI_String
+	Unescapes all the special characters that can not be contained in the enum member definition, but can be sent to the instrument as enum string.
+	Use this to send the scpi enum value to the instrument."""
+	for key in enum_spec_prefixes:
+		if enum_value.startswith(key):
+			enum_value = enum_spec_prefixes[key] + enum_value[len(key):]
+	for key in enum_spec_strings:
+		enum_value = enum_value.replace(key, enum_spec_strings[key])
+	return enum_value
+
+
+def value_to_quoted_str(x: int or bool or float or str or Enum) -> str:
+	"""Converts scalar value to string enclosed by single quotes.
+	Supported element types:
+	- int
+	- bool
+	- float
+	- string
+	- enum"""
+	return f"'{value_to_str(x)}'"
+
+
+def str_to_float_list(string: str) -> List[float]:
+	"""Converts string with comma-separated values to list of Floats."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_float, string.split(','))]
+	return result
+
+
+def str_to_float_or_bool_list(string: str) -> List[float or bool]:
+	"""Converts string with comma-separated values to list of float or boolean values."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_float_or_bool, string.split(','))]
+	return result
+
+
+def str_to_int_list(string: str) -> List[int]:
+	"""Converts string with comma-separated values to list of Integers."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_int, string.split(','))]
+	return result
+
+
+def str_to_int_or_bool_list(string: str) -> List[int or bool]:
+	"""Converts string with comma-separated values to list of integer or boolean values."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_int_or_bool, string.split(','))]
+	return result
+
+
+def str_to_bool_list(string: str) -> List[bool]:
+	"""Converts string with comma-separated values to list of booleans."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(str_to_bool, string.split(','))]
+	return result
+
+
+def str_to_str_list(string: str, clear_one_empty_item: bool = False) -> List[str]:
+	"""Converts string with comma-separated values to list of strings.
+	Each element is trimmed by trim_str_response().
+	If the clear_one_empty_item is set to True (default is False), and the result is exactly one empty string item, the method returns empty list."""
+	assert_string_data(string)
+	if not string:
+		return []
+	result = [*map(Utilities.trim_str_response, string.split(','))]
+	if clear_one_empty_item and len(result) == 1 and result[0] == '':
+		return []
+	return result
+
+
+def _find_in_enum_members(item: str, enum_members: List[str]) -> int:
+	"""Matches a string in the provided list of member strings.
+	The item must be not fully matched.
+	The item is matched if a member string starts with the item (the item is a prefix of the member).
+	Example: item='CONN' will match the enum_member 'CONNected'
+	If the item contains a comma, only the value before comma is considered
+	Returns found index in the enum_members list"""
+	if ',' in item:
+		item = item[:item.index(',')].strip()
+	ix = -1
+	i = 0
+	for x in enum_members:
+		if x.startswith(item):
+			return i
+		i += 1
+	return ix
+
+
+def str_to_scalar_enum_helper(string: str, enum_type: Enum, enum_members=None) -> Enum:
+	"""Converts string to one enum element.
+	enum_members are optional to improve the performance for repeated conversions.
+	If you do not provide them, they are generated inside the function."""
+	value = Utilities.trim_str_response(string)
+	if not enum_members:
+		# noinspection PyTypeChecker
+		enum_members = [x.name for x in enum_type]
+
+	# Search in the enum member and return the index of the matched item
+	ix = _find_in_enum_members(value, enum_members)
+	if ix >= 0:
+		return enum_type[enum_members[ix]]
+
+	# If the result is -1 (not found), try to replace the special values and search again
+	# This is done to improve the performance, since most of the enums have no special values
+	enum_members_conv = [enum_value_to_scpi_string(x) for x in enum_members]
+	ix = _find_in_enum_members(value, enum_members_conv)
+	if ix >= 0:
+		return enum_type[enum_members[ix]]
+
+	# If not found, search in the special integer numbers:
+	spec_value = str_special_values_to_int(value)
+	if not spec_value:
+		raise Exception(f"String '{value}' can not be found in the enum type '{enum_type}'")
+	# noinspection PyTypeChecker
+	return spec_value
+
+
+def str_to_list_enum_helper(string: str, enum_type: Enum, enum_members=None) -> List[Enum]:
+	"""Converts string to list of enum elements.
+	enum_members are optional to improve the performance for repeated conversions.
+	If you do not provide them, they are generated inside the function."""
+	if not enum_members:
+		# noinspection PyTypeChecker
+		enum_members = [x.name for x in enum_type]
+	elements = string.split(',')
+	return [str_to_scalar_enum_helper(x, enum_type, enum_members) for x in elements]
+
+
+def enum_scalar_to_str(data, enum_type) -> str:
+	"""Converts enum scalar value to string."""
+	assert isinstance(data, enum_type), f"Expected command parameter {enum_type}, actual data type: {type(data)}. Value: {data}"
+	return value_to_str(data)
+
+
+def enum_list_to_str(data: List, enum_type) -> str:
+	"""Converts enum list to csv-string."""
+	# For enums, check that each element is an enum
+	assert all(isinstance(x, enum_type) for x in data), f"Expected command parameter list of {enum_type}, detected one or more elements of non-enum type. Value: {data}"
+	return list_to_csv_str(data)
+
+
+def str_to_scalar_enum(string: str, enum_type) -> Enum:
+	"""Converts string to one enum element."""
+	return str_to_scalar_enum_helper(string, enum_type)
+
+
+def str_to_list_enum(string: str, enum_type) -> List[Enum]:
+	"""Converts string to list of enum elements."""
+	return str_to_list_enum_helper(string, enum_type)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ConverterFromScpiString.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ConverterFromScpiString.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from enum import Enum
-
-from .Conversions import str_to_bool, str_to_int, str_to_int_or_bool, str_to_float, str_to_float_or_bool, str_to_scalar_enum_helper
-from .Conversions import str_to_str_list, str_to_bool_list, str_to_int_list, str_to_int_or_bool_list, str_to_float_list, str_to_float_or_bool_list, str_to_list_enum_helper
-from .Types import DataType
-from .Utilities import trim_str_response
-
-
-class ConverterFromScpiString:
-	"""Converter from SCPI response string to argument value
-	For list argument types, you must use the method get_one_element_value in a loop for each element.
-	Provides methods:
-	- get_one_element_value(str): returns one scalar value converted from the SCPI string.
-	- get_list_value(str): return complete list value converted from the SCPI string.
-	- get_value(str): calls either get_one_element_value or get_list_value() depending on the data type. \n
-	The reason for the different methods is, that sometimes the list data are interleaved with other arguments.
-	In order to parse them properly, the ArgStructStringParser module must be able to set the argument value element-by-element.
-	On the other side, the driver methods might want to set the whole argument value, because the result scpi string is a single argument response."""
-
-	def __init__(self, data_type: DataType, enum_type: Enum = None):
-		self.enum_type = enum_type
-		self.data_type = data_type
-		self.element_type = self.data_type.element_type
-
-		if self.element_type == DataType.RawString:
-			self.converter = trim_str_response
-			self.list_converter = str_to_str_list
-
-		elif self.element_type == DataType.String:
-			self.converter = trim_str_response
-			self.list_converter = str_to_str_list
-
-		elif self.element_type == DataType.Boolean:
-			self.converter = str_to_bool
-			self.list_converter = str_to_bool_list
-
-		elif self.element_type == DataType.Integer:
-			self.converter = str_to_int
-			self.list_converter = str_to_int_list
-
-		elif self.element_type == DataType.IntegerExt:
-			self.converter = str_to_int_or_bool
-			self.list_converter = str_to_int_or_bool_list
-
-		elif self.element_type == DataType.Float:
-			self.converter = str_to_float
-			self.list_converter = str_to_float_list
-
-		elif self.element_type == DataType.FloatExt:
-			self.converter = str_to_float_or_bool
-			self.list_converter = str_to_float_or_bool_list
-
-		elif self.element_type == DataType.Enum:
-			assert self.enum_type, f"For data type enum, you have to define the enum_type variable."
-			# noinspection PyTypeChecker
-			self.enum_members = [x.name for x in self.enum_type]
-		else:
-			raise Exception(f"Unsupported data type '{data_type}'")
-
-	def get_one_element_value(self, scpi_string: str):
-		"""Returns single element !!! of the argument value converted from the SCPI string (single element)"""
-		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
-		if self.element_type is DataType.Enum:
-			return str_to_scalar_enum_helper(scpi_string, self.enum_type, self.enum_members)
-		return self.converter(scpi_string)
-
-	def get_value(self, scpi_string: str):
-		"""Returns complete value of the argument converted from the SCPI string (list or scalar)"""
-		if not self.data_type.is_list:
-			return self.get_one_element_value(scpi_string)
-
-		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
-		if self.element_type is DataType.Enum:
-			return str_to_list_enum_helper(scpi_string, self.enum_type, self.enum_members)
-		return self.list_converter(scpi_string)
+from enum import Enum
+
+from .Conversions import str_to_bool, str_to_int, str_to_int_or_bool, str_to_float, str_to_float_or_bool, str_to_scalar_enum_helper
+from .Conversions import str_to_str_list, str_to_bool_list, str_to_int_list, str_to_int_or_bool_list, str_to_float_list, str_to_float_or_bool_list, str_to_list_enum_helper
+from .Types import DataType
+from .Utilities import trim_str_response
+
+
+class ConverterFromScpiString:
+	"""Converter from SCPI response string to argument value
+	For list argument types, you must use the method get_one_element_value in a loop for each element.
+	Provides methods:
+	- get_one_element_value(str): returns one scalar value converted from the SCPI string.
+	- get_list_value(str): return complete list value converted from the SCPI string.
+	- get_value(str): calls either get_one_element_value or get_list_value() depending on the data type. \n
+	The reason for the different methods is, that sometimes the list data are interleaved with other arguments.
+	In order to parse them properly, the ArgStructStringParser module must be able to set the argument value element-by-element.
+	On the other side, the driver methods might want to set the whole argument value, because the result scpi string is a single argument response."""
+
+	def __init__(self, data_type: DataType, enum_type: Enum = None):
+		self.enum_type = enum_type
+		self.data_type = data_type
+		self.element_type = self.data_type.element_type
+
+		if self.element_type == DataType.RawString:
+			self.converter = trim_str_response
+			self.list_converter = str_to_str_list
+
+		elif self.element_type == DataType.String:
+			self.converter = trim_str_response
+			self.list_converter = str_to_str_list
+
+		elif self.element_type == DataType.Boolean:
+			self.converter = str_to_bool
+			self.list_converter = str_to_bool_list
+
+		elif self.element_type == DataType.Integer:
+			self.converter = str_to_int
+			self.list_converter = str_to_int_list
+
+		elif self.element_type == DataType.IntegerExt:
+			self.converter = str_to_int_or_bool
+			self.list_converter = str_to_int_or_bool_list
+
+		elif self.element_type == DataType.Float:
+			self.converter = str_to_float
+			self.list_converter = str_to_float_list
+
+		elif self.element_type == DataType.FloatExt:
+			self.converter = str_to_float_or_bool
+			self.list_converter = str_to_float_or_bool_list
+
+		elif self.element_type == DataType.Enum:
+			assert self.enum_type, f"For data type enum, you have to define the enum_type variable."
+			# noinspection PyTypeChecker
+			self.enum_members = [x.name for x in self.enum_type]
+		else:
+			raise Exception(f"Unsupported data type '{data_type}'")
+
+	def get_one_element_value(self, scpi_string: str):
+		"""Returns single element !!! of the argument value converted from the SCPI string (single element)"""
+		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
+		if self.element_type is DataType.Enum:
+			return str_to_scalar_enum_helper(scpi_string, self.enum_type, self.enum_members)
+		return self.converter(scpi_string)
+
+	def get_value(self, scpi_string: str):
+		"""Returns complete value of the argument converted from the SCPI string (list or scalar)"""
+		if not self.data_type.is_list:
+			return self.get_one_element_value(scpi_string)
+
+		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
+		if self.element_type is DataType.Enum:
+			return str_to_list_enum_helper(scpi_string, self.enum_type, self.enum_members)
+		return self.list_converter(scpi_string)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/ConverterToScpiString.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/ConverterToScpiString.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from enum import Enum
-
-from .Conversions import list_to_csv_quoted_str, value_to_quoted_str, list_to_csv_str, value_to_str, enum_list_to_str, enum_scalar_to_str
-from .Types import DataType
-
-
-def value_to_scpi_string(data, data_type: DataType):
-	"""Method to be used in the driver implementation.
-	Convert data to SCPI string parameter: data -> str"""
-	if data_type.is_list:
-		assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
-	else:
-		assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
-	# Strings are enclosed by single quotes
-	if data_type == DataType.StringList:
-		assert all(isinstance(x, str) for x in data), f"Expected command parameter list of strings, detected one or more elements of non-string type. Value: {data}"
-		return list_to_csv_quoted_str(data)
-	elif data_type == DataType.String:
-		assert isinstance(data, str), f"Expected command parameter string, actual data type: {type(data)}. Value: {data}"
-		return value_to_quoted_str(data)
-
-	# Raw string is not enclosed by quotes
-	elif data_type == DataType.RawStringList:
-		assert all(isinstance(x, str) for x in data), f"Expected command parameter list of strings, detected one or more elements of non-string type. Value: {data}"
-		return list_to_csv_str(data)
-	elif data_type == DataType.RawString:
-		assert isinstance(data, str), f"Expected command parameter string, actual data type: {type(data)}. Value: {data}"
-		return value_to_str(data)
-
-	elif data_type == DataType.BooleanList:
-		assert all(type(x) == bool for x in data), f"Expected command parameter list of booleans, detected one or more elements of non-boolean type. Value: {data}"
-		return list_to_csv_str(data)
-	elif data_type == DataType.Boolean:
-		assert type(data) == bool, f"Expected command parameter boolean, actual data type: {type(data)}. Value: {data}"
-		return value_to_str(data)
-
-	# For integer and float, allow them to be mixed
-	elif data_type == DataType.IntegerList or data_type == DataType.FloatList:
-		assert all((isinstance(x, int) or isinstance(x, float)) and type(x) != bool for x in data), f"Expected command parameter list of numbers, detected one or more elements of non-number type. Value: {data}"
-		return list_to_csv_str(data)
-	elif data_type == DataType.Integer or data_type == DataType.Float:
-		assert (isinstance(data, int) or isinstance(data, float)) and type(data) != bool, f"Expected command parameter number, actual data type: {type(data)}. Value: {data}"
-		return value_to_str(data)
-
-	# For integer and float extended, allow them to be mixed including the boolean type
-	elif data_type == DataType.IntegerExtList or data_type == DataType.FloatExtList:
-		assert all((isinstance(x, int) or isinstance(x, float) or isinstance(x, bool)) for x in data), f"Expected command parameter list of numbers or booleans, detected one or more elements of non-number type. Value: {data}"
-		return list_to_csv_str(data)
-	elif data_type == DataType.IntegerExt or data_type == DataType.FloatExt:
-		assert (isinstance(data, int) or isinstance(data, float) or isinstance(data, bool)), f"Expected command parameter number or boolean, actual data type: {type(data)}. Value: {data}"
-		return value_to_str(data)
-	else:
-		raise Exception(f"Unsupported data type: '{type(data_type)}'.")
-
-
-class ConverterToScpiString:
-	"""Converter from argument value to SCPI string.
-	Provides method get_value(arg_value) -> str
-	"""
-
-	def __init__(self, data_type: DataType, enum_type: Enum = None):
-		self.enum_type = enum_type
-		self.data_type = data_type
-		self.element_type = self.data_type.element_type
-		if self.element_type == DataType.Enum:
-			assert self.enum_type, f"For data_type {data_type.name}, you have to define the enum_type variable."
-
-	def get_value(self, data) -> str:
-		"""Returns SCPI string converted from the argument data."""
-		if self.data_type.is_list:
-			assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
-		else:
-			assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
-
-		if self.data_type == DataType.Enum:
-			return enum_scalar_to_str(data, self.enum_type)
-		elif self.data_type == DataType.EnumList:
-			return enum_list_to_str(data, self.enum_type)
-
-		return value_to_scpi_string(data, self.data_type)
+from enum import Enum
+
+from .Conversions import list_to_csv_quoted_str, value_to_quoted_str, list_to_csv_str, value_to_str, enum_list_to_str, enum_scalar_to_str
+from .Types import DataType
+
+
+def value_to_scpi_string(data, data_type: DataType):
+	"""Method to be used in the driver implementation.
+	Convert data to SCPI string parameter: data -> str"""
+	if data_type.is_list:
+		assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
+	else:
+		assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
+	# Strings are enclosed by single quotes
+	if data_type == DataType.StringList:
+		assert all(isinstance(x, str) for x in data), f"Expected command parameter list of strings, detected one or more elements of non-string type. Value: {data}"
+		return list_to_csv_quoted_str(data)
+	elif data_type == DataType.String:
+		assert isinstance(data, str), f"Expected command parameter string, actual data type: {type(data)}. Value: {data}"
+		return value_to_quoted_str(data)
+
+	# Raw string is not enclosed by quotes
+	elif data_type == DataType.RawStringList:
+		assert all(isinstance(x, str) for x in data), f"Expected command parameter list of strings, detected one or more elements of non-string type. Value: {data}"
+		return list_to_csv_str(data)
+	elif data_type == DataType.RawString:
+		assert isinstance(data, str), f"Expected command parameter string, actual data type: {type(data)}. Value: {data}"
+		return value_to_str(data)
+
+	elif data_type == DataType.BooleanList:
+		assert all(type(x) == bool for x in data), f"Expected command parameter list of booleans, detected one or more elements of non-boolean type. Value: {data}"
+		return list_to_csv_str(data)
+	elif data_type == DataType.Boolean:
+		assert type(data) == bool, f"Expected command parameter boolean, actual data type: {type(data)}. Value: {data}"
+		return value_to_str(data)
+
+	# For integer and float, allow them to be mixed
+	elif data_type == DataType.IntegerList or data_type == DataType.FloatList:
+		assert all((isinstance(x, int) or isinstance(x, float)) and type(x) != bool for x in data), f"Expected command parameter list of numbers, detected one or more elements of non-number type. Value: {data}"
+		return list_to_csv_str(data)
+	elif data_type == DataType.Integer or data_type == DataType.Float:
+		assert (isinstance(data, int) or isinstance(data, float)) and type(data) != bool, f"Expected command parameter number, actual data type: {type(data)}. Value: {data}"
+		return value_to_str(data)
+
+	# For integer and float extended, allow them to be mixed including the boolean type
+	elif data_type == DataType.IntegerExtList or data_type == DataType.FloatExtList:
+		assert all((isinstance(x, int) or isinstance(x, float) or isinstance(x, bool)) for x in data), f"Expected command parameter list of numbers or booleans, detected one or more elements of non-number type. Value: {data}"
+		return list_to_csv_str(data)
+	elif data_type == DataType.IntegerExt or data_type == DataType.FloatExt:
+		assert (isinstance(data, int) or isinstance(data, float) or isinstance(data, bool)), f"Expected command parameter number or boolean, actual data type: {type(data)}. Value: {data}"
+		return value_to_str(data)
+	else:
+		raise Exception(f"Unsupported data type: '{type(data_type)}'.")
+
+
+class ConverterToScpiString:
+	"""Converter from argument value to SCPI string.
+	Provides method get_value(arg_value) -> str
+	"""
+
+	def __init__(self, data_type: DataType, enum_type: Enum = None):
+		self.enum_type = enum_type
+		self.data_type = data_type
+		self.element_type = self.data_type.element_type
+		if self.element_type == DataType.Enum:
+			assert self.enum_type, f"For data_type {data_type.name}, you have to define the enum_type variable."
+
+	def get_value(self, data) -> str:
+		"""Returns SCPI string converted from the argument data."""
+		if self.data_type.is_list:
+			assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
+		else:
+			assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
+
+		if self.data_type == DataType.Enum:
+			return enum_scalar_to_str(data, self.enum_type)
+		elif self.data_type == DataType.EnumList:
+			return enum_list_to_str(data, self.enum_type)
+
+		return value_to_scpi_string(data, self.data_type)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/Core.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/Core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,264 +1,252 @@
-import re
-from typing import Callable
-
-from . import InstrumentOptions as Options, Conversions as Conv
-from .ArgSingle import ArgSingle
-from .ArgSingleList import ArgSingleList
-from .Conversions import BinFloatFormat, BinIntFormat
-from .Instrument import Instrument
-from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode
-from .Utilities import parse_token_to_key_and_value, trim_str_response
-
-
-class Core(object):
-	"""Main driver component. Provides: \n
-		- Main core constructor
-		- 'io' interface for all the write / query operations
-		- Command parameters string composer for single arguments...
-		- Link handlers adding / changing / deleting
-
-		Version history:
-
-		1.10.0 (build 46) 03.05.2021
-			- Added methods to Instrument: query_struct_with_opc(), query_str_suppressed_with_opc()
-
-		1.9.0 (build 45) 13.04.2021
-			- Added option to set callbacks before_write and before_query
-			- When a RepCap has a member with integer number 0 defined, the command string interpretation of such member is '0', not empty string
-
-		1.8.0 (build 43) 19.01.2021
-			- Added matching of Enum instrument responses also in short/long form
-
-		1.7.7 (build 42) 26.11.2020
-			- Extended ArgSingleList.compose_cmd_string() to 9 arguments
-
-		1.7.6 (build 41) 23.11.2020
-			- Extended data types for IntegerExt, FloatExt, IntegerExtArray, FloatExtArray
-
-		1.7.5 (build 40) 12.11.2020
-			- Extended Conversions method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
-
-		1.7.4 (build 39) 11.09.2020
-			- Fixed parsing of the instrument errors when an error message contains two double quotes
-
-		1.7.3 (build 38) 21.10.2020
-			- Added 'UND' to the list of float numbers that are represented as NaN
-
-		1.7.2 (build 37) 10.10.2020
-			- SCPI response string conversion to scalar enum: if the string contains ',', the content after it inclusive the comma is ignored
-
-		1.7.1 (build 36) 08.10.2020
-			- Fixed Python 3.8.5+ warnings
-
-		1.7.0 (build 34) 30.09.2020
-			- Added option to set the termination characters for reading and writing. Until now, it was fixed to '\n' (Linefeed)
-			- Replaced 'import visa' with 'import pyvisa' to remove Python 3.8 pyvisa warnings
-
-		Version History:
-		1.6.0 (build 33) 17.09.2020
-			- Added special characters encoding/decoding in enums
-
-		1.4.0 (build 32) 17.09.2020
-			- Added recognition of RsVisa library location for linux when using options string 'SelectVisa=rs'
-			- Fixed bug in reading binary data 16 bit
-
-		1.3.0 (build 31) 04.09.2020
-			- added DRIVERSETUP_QUERYOPT to the driver's option string
-			- *OPT? is no longer performed at the init, but only at the first access to options string.
-				In addition, the *OPT? query is executed with 1000 ms timeout, and the errors are suppressed
-
-		1.2.0 (build 30), 03.08.2020
-			- Fixed NRP-Z session parameters: vxi_capable = False, io_segment_size = 1000000
-
-		1.1.0 (build 29), 20.06.2020
-			- Added RepeatedCapability and base class CommandsGroup
-			- Fixed simulation mode switching
-
-		0.9.3 (build 25), 23.04.2020 - Fixed composition of optional arguments in ArgSingleList and ArgSingle
-		0.9.2 (build 24), 13.11.2019 - Added recognition of special values for enum return strings
-		0.9.1 - Added read / write to file, refactored internals to work with streams
-		0.9.0 - First Version created."""
-
-	driver_version: str = ''
-	"""Placeholder for the driver version string."""
-
-	def __init__(
-			self,
-			resource_name: str,
-			id_query: bool = True,
-			reset: bool = False,
-			driver_options: str = None,
-			user_options: str = None,
-			direct_session: object = None):
-		"""Initializes new driver session. For cleaner code, use the class methods: \n
-		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
-
-		self.core_version = '1.9.0'
-		self.simulating = False
-		self.supported_idn_patterns = []
-		self.supported_instr_models = []
-
-		self._args_single_list = ArgSingleList()
-		sett_dr = self._parse_init_settings_string(driver_options)
-		self._apply_settings_to_core(sett_dr)
-		sett_user = self._parse_init_settings_string(user_options)
-		self._apply_settings_to_core(sett_user)
-
-		# Typical settings for the Core
-		self._instrumentSettings = InstrumentSettings(
-			InstrViClearMode.execute_on_all,  # Instrument viClear mode
-			False,  # Full model name. True: SMW200A, False: SMW
-			0,  # Delay by each write
-			0,  # Delay by each read
-			100000,  # Max chunk read / write size in bytes
-			WaitForOpcMode.stb_poll,  # Waiting for OPC Mode: Status byte polling
-			30000,  # OPC timeout
-			10000,  # VISA timeout
-			60000,  # Self-test timeout
-			Options.ParseMode.Auto,  # *OPT? response parsing mode
-			BinFloatFormat.Single_4bytes,  # Format for parsing of binary float numbers
-			BinIntFormat.Integer32_4bytes,  # Format for parsing of binary integer numbers
-			False  # OPC query after each setting
-		)
-
-		self._instrumentSettings.apply_option_settings(sett_dr)
-		self._instrumentSettings.apply_option_settings(sett_user)
-
-		# Resolve the direct_session to handle. Options for direct_session type:
-		# - VisaSession object, retrieved from the driver's RsInstrument.get_session_handle() method
-		# - string in case of a simulation session
-		handle = direct_session
-		if handle:
-			# Check if the entered 'direct_session' is either the driver object or the Visa session
-			if hasattr(direct_session, 'get_session_handle'):
-				assert hasattr(direct_session, '_core'), f"Direct session is a class type. It must be an instance of the top-level driver class."
-				handle = direct_session.get_session_handle()
-			# Check if the handle is not a simulation mode string
-			if isinstance(handle, str):
-				if "Simulating session, resource name " in handle:
-					self.simulating = True
-					handle = None
-
-		self.io = Instrument(resource_name, self.simulating, self._instrumentSettings, handle)
-		self.io.query_instr_status = True
-
-		self._apply_settings_to_instrument(sett_dr)
-		self._apply_settings_to_instrument(sett_user)
-
-		self.io.set_simulating_cmds()
-
-		if id_query:
-			self.io.fits_idn_pattern(self.supported_idn_patterns, self.supported_instr_models)
-
-		if reset:
-			self.io.reset()
-		else:
-			self.io.check_status()
-
-	@classmethod
-	def from_existing_session(cls, session: object, driver_options: str = None) -> 'Core':
-		"""Creates a new Core object with the entered 'session' reused."""
-		# noinspection PyTypeChecker
-		return cls(None, False, False, driver_options, None, session)
-
-	def __str__(self):
-		return f"Core session '{self.io.resource_name}'"
-
-	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
-		"""Adds / Updates link handler for the entered link_name.
-		Handler API: handler(event_args: ArgLinkedEventArgs)
-		Returns the previous registered handler, or None if no handler was registered before."""
-		return self.io.set_link_handler(link_name, handler)
-
-	def del_link_handler(self, link_name: str) -> Callable:
-		"""Deletes link handler for the link_name.
-		Returns the deleted handler, or None if none existed."""
-		return self.io.del_link_handler(link_name)
-
-	def del_all_link_handlers(self) -> int:
-		"""Deletes all the link handlers.
-		Returns number of deleted links."""
-		return self.io.del_all_link_handlers()
-
-	# noinspection PyMethodMayBeStatic
-	def _parse_init_settings_string(self, text: str) -> dict:
-		"""Parses init string to a dictionary of settings: name -> value."""
-		tokens = {}
-		if not text:
-			return tokens
-
-		# Text enclosed in single brackets '' must have the commas escaped
-		literal_pattern = r"'([^']+)'"
-		while True:
-			# literal loop
-			m = re.search(literal_pattern, text)
-			if not m:
-				break
-			lit_part = '"' + m.group(1).replace(',', '<COMMA_ESC>') + '"'
-			text = text.replace(m.group(0), lit_part)
-
-		# Remove all the class-options enclosed by round brackets e.g. "<groupName>=(<groupTokens>)"
-		group_pattern = r'(\w+)\s*=\s*\(([^\)]*)\)'
-		# Match class-settings, add them as separate keys with groupName_Key
-		while True:
-			# Group loop
-			m = re.search(group_pattern, text)
-			if not m:
-				break
-			text = text.replace(m.group(0), '')
-			group_name = m.group(1).upper()
-			group_tokens = m.group(2).strip().split(',')
-			for token in group_tokens:
-				key, value = parse_token_to_key_and_value(token)
-				if value:
-					tokens[f'{group_name}_{key.upper()}'] = value
-
-		# All groups are removed from the text, now we can use splitting on commas and remove white-space-only elements
-		for token in text.split(','):
-			key, value = parse_token_to_key_and_value(token.replace('<COMMA_ESC>', ','))
-			if value:
-				tokens[key.upper()] = value
-		return tokens
-
-	def _apply_settings_to_core(self, settings: dict) -> None:
-		"""Applies settings relevant for the Core from the dictionary."""
-		value = settings.get('SIMULATE')
-		if value:
-			self.simulating = Conv.str_to_bool(value)
-
-		value = settings.get('SUPPORTEDINSTRMODELS')
-		if value:
-			self.supported_instr_models = [*map(trim_str_response, value.split('/'))]
-
-		value = settings.get('SUPPORTEDIDNPATTERNS')
-		if value:
-			self.supported_idn_patterns = [*map(trim_str_response, value.split('/'))]
-
-	def _apply_settings_to_instrument(self, settings: dict) -> None:
-		"""Applies settings relevant for the Instrument from the dictionary."""
-		value = settings.get('QUERYINSTRUMENTSTATUS')
-		if value:
-			self.io.query_instr_status = Conv.str_to_bool(value)
-
-		value = settings.get('SIMULATIONIDNSTRING')
-		if value and self.simulating:
-			# Use the '*' instead of the ',' in the value to avoid comma as token delimiter
-			self.io.idn_string = value.replace('*', ',')
-
-	def compose_cmd_arg_param(
-			self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None) -> str:
-		"""Composes command parameter string based on the single arguments definition."""
-		return self._args_single_list.compose_cmd_string(arg1, arg2, arg3, arg4, arg5, arg6)
-
-	def get_last_sent_cmd(self) -> str:
-		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
-		return self.io.get_last_sent_cmd()
-
-	def get_session_handle(self):
-		"""Returns the underlying pyvisa session."""
-		return self.io.get_session_handle()
-
-	def close(self):
-		"""Closes the Core session."""
-		self.io.close()
-		self.io = None
+import re
+from typing import Callable
+
+from . import InstrumentOptions as Options, Conversions as Conv
+from .ArgSingle import ArgSingle
+from .ArgSingleList import ArgSingleList
+from .Conversions import BinFloatFormat, BinIntFormat
+from .Instrument import Instrument
+from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode
+from .Utilities import parse_token_to_key_and_value, trim_str_response
+
+
+class Core(object):
+	"""Main driver component. Provides: \n
+		- Main core constructor
+		- 'io' interface for all the write / query operations
+		- Command parameters string composer for single arguments...
+		- Link handlers adding / changing / deleting
+
+		1.7.7 (build 42) 26.11.2020
+			- Extended ArgSingleList.compose_cmd_string() to 9 arguments
+
+		1.7.6 (build 41) 23.11.2020
+			- Extended data types for IntegerExt, FloatExt, IntegerExtArray, FloatExtArray
+
+		1.7.5 (build 40) 12.11.2020
+			- Extended Conversions method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
+
+		1.7.4 (build 39) 11.09.2020
+			- Fixed parsing of the instrument errors when an error message contains two double quotes
+
+		1.7.3 (build 38) 21.10.2020
+			- Added 'UND' to the list of float numbers that are represented as NaN
+
+		1.7.2 (build 37) 10.10.2020
+			- SCPI response string conversion to scalar enum: if the string contains ',', the content after it inclusive the comma is ignored
+
+		1.7.1 (build 36) 08.10.2020
+			- Fixed Python 3.8.5+ warnings
+
+		1.7.0 (build 34) 30.09.2020
+			- Added option to set the termination characters for reading and writing. Until now, it was fixed to '\n' (Linefeed)
+			- Replaced 'import visa' with 'import pyvisa' to remove Python 3.8 pyvisa warnings
+
+		Version History:
+		1.6.0 (build 33) 17.09.2020
+			- Added special characters encoding/decoding in enums
+
+		1.4.0 (build 32) 17.09.2020
+			- Added recognition of RsVisa library location for linux when using options string 'SelectVisa=rs'
+			- Fixed bug in reading binary data 16 bit
+
+		1.3.0 (build 31) 04.09.2020
+			- added DRIVERSETUP_QUERYOPT to the driver's option string
+			- *OPT? is no longer performed at the init, but only at the first access to options string.
+				In addition, the *OPT? query is executed with 1000 ms timeout, and the errors are suppressed
+
+		1.2.0 (build 30), 03.08.2020
+			- Fixed NRP-Z session parameters: vxi_capable = False, io_segment_size = 1000000
+
+		1.1.0 (build 29), 20.06.2020
+			- Added RepeatedCapability and base class CommandsGroup
+			- Fixed simulation mode switching
+
+		0.9.3 (build 25), 23.04.2020 - Fixed composition of optional arguments in ArgSingleList and ArgSingle
+		0.9.2 (build 24), 13.11.2019 - Added recognition of special values for enum return strings
+		0.9.1 - Added read / write to file, refactored internals to work with streams
+		0.9.0 - First Version created."""
+
+	driver_version: str = ''
+	"""Placeholder for the driver version string."""
+
+	def __init__(
+			self,
+			resource_name: str,
+			id_query: bool = True,
+			reset: bool = False,
+			driver_options: str = None,
+			user_options: str = None,
+			direct_session: object = None):
+		"""Initializes new driver session. For cleaner code, use the class methods: \n
+		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
+
+		self.core_version = '1.7.6'
+		self.simulating = False
+		self.supported_idn_patterns = []
+		self.supported_instr_models = []
+
+		self._args_single_list = ArgSingleList()
+		sett_dr = self._parse_init_settings_string(driver_options)
+		self._apply_settings_to_core(sett_dr)
+		sett_user = self._parse_init_settings_string(user_options)
+		self._apply_settings_to_core(sett_user)
+
+		# Typical settings for the Core
+		self._instrumentSettings = InstrumentSettings(
+			InstrViClearMode.execute_on_all,  # Instrument viClear mode
+			False,  # Full model name. True: SMW200A, False: SMW
+			0,  # Delay by each write
+			0,  # Delay by each read
+			100000,  # Max chunk read / write size in bytes
+			WaitForOpcMode.stb_poll,  # Waiting for OPC Mode: Status byte polling
+			30000,  # OPC timeout
+			10000,  # VISA timeout
+			60000,  # Self-test timeout
+			Options.ParseMode.Auto,  # *OPT? response parsing mode
+			BinFloatFormat.Single_4bytes,  # Format for parsing of binary float numbers
+			BinIntFormat.Integer32_4bytes,  # Format for parsing of binary integer numbers
+			False  # OPC query after each setting
+		)
+
+		self._instrumentSettings.apply_option_settings(sett_dr)
+		self._instrumentSettings.apply_option_settings(sett_user)
+
+		# Resolve the direct_session to handle. Options for direct_session type:
+		# - VisaSession object, retrieved from the driver's RsInstrument.get_session_handle() method
+		# - string in case of a simulation session
+		handle = direct_session
+		if handle:
+			# Check if the entered 'direct_session' is either the driver object or the Visa session
+			if hasattr(direct_session, 'get_session_handle'):
+				assert hasattr(direct_session, '_core'), f"Direct session is a class type. It must be an instance of the top-level driver class."
+				handle = direct_session.get_session_handle()
+			# Check if the handle is not a simulation mode string
+			if isinstance(handle, str):
+				if "Simulating session, resource name " in handle:
+					self.simulating = True
+					handle = None
+
+		self.io = Instrument(resource_name, self.simulating, self._instrumentSettings, handle)
+		self.io.query_instr_status = True
+
+		self._apply_settings_to_instrument(sett_dr)
+		self._apply_settings_to_instrument(sett_user)
+
+		self.io.set_simulating_cmds()
+
+		if id_query:
+			self.io.fits_idn_pattern(self.supported_idn_patterns, self.supported_instr_models)
+
+		if reset:
+			self.io.reset()
+		else:
+			self.io.check_status()
+
+	@classmethod
+	def from_existing_session(cls, session: object, driver_options: str = None) -> 'Core':
+		"""Creates a new Core object with the entered 'session' reused."""
+		# noinspection PyTypeChecker
+		return cls(None, False, False, driver_options, None, session)
+
+	def __str__(self):
+		return f"Core session '{self.io.resource_name}'"
+
+	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
+		"""Adds / Updates link handler for the entered link_name.
+		Handler API: handler(event_args: ArgLinkedEventArgs)
+		Returns the previous registered handler, or None if no handler was registered before."""
+		return self.io.set_link_handler(link_name, handler)
+
+	def del_link_handler(self, link_name: str) -> Callable:
+		"""Deletes link handler for the link_name.
+		Returns the deleted handler, or None if none existed."""
+		return self.io.del_link_handler(link_name)
+
+	def del_all_link_handlers(self) -> int:
+		"""Deletes all the link handlers.
+		Returns number of deleted links."""
+		return self.io.del_all_link_handlers()
+
+	# noinspection PyMethodMayBeStatic
+	def _parse_init_settings_string(self, text: str) -> dict:
+		"""Parses init string to a dictionary of settings: name -> value."""
+		tokens = {}
+		if not text:
+			return tokens
+
+		# Text enclosed in single brackets '' must have the commas escaped
+		literal_pattern = r"'([^']+)'"
+		while True:
+			# literal loop
+			m = re.search(literal_pattern, text)
+			if not m:
+				break
+			lit_part = '"' + m.group(1).replace(',', '<COMMA_ESC>') + '"'
+			text = text.replace(m.group(0), lit_part)
+
+		# Remove all the class-options enclosed by round brackets e.g. "<groupName>=(<groupTokens>)"
+		group_pattern = r'(\w+)\s*=\s*\(([^\)]*)\)'
+		# Match class-settings, add them as separate keys with groupName_Key
+		while True:
+			# Group loop
+			m = re.search(group_pattern, text)
+			if not m:
+				break
+			text = text.replace(m.group(0), '')
+			group_name = m.group(1).upper()
+			group_tokens = m.group(2).strip().split(',')
+			for token in group_tokens:
+				key, value = parse_token_to_key_and_value(token)
+				if value:
+					tokens[f'{group_name}_{key.upper()}'] = value
+
+		# All groups are removed from the text, now we can use splitting on commas and remove white-space-only elements
+		for token in text.split(','):
+			key, value = parse_token_to_key_and_value(token.replace('<COMMA_ESC>', ','))
+			if value:
+				tokens[key.upper()] = value
+		return tokens
+
+	def _apply_settings_to_core(self, settings: dict) -> None:
+		"""Applies settings relevant for the Core from the dictionary."""
+		value = settings.get('SIMULATE')
+		if value:
+			self.simulating = Conv.str_to_bool(value)
+
+		value = settings.get('SUPPORTEDINSTRMODELS')
+		if value:
+			self.supported_instr_models = [*map(trim_str_response, value.split('/'))]
+
+		value = settings.get('SUPPORTEDIDNPATTERNS')
+		if value:
+			self.supported_idn_patterns = [*map(trim_str_response, value.split('/'))]
+
+	def _apply_settings_to_instrument(self, settings: dict) -> None:
+		"""Applies settings relevant for the Instrument from the dictionary."""
+		value = settings.get('QUERYINSTRUMENTSTATUS')
+		if value:
+			self.io.query_instr_status = Conv.str_to_bool(value)
+
+		value = settings.get('SIMULATIONIDNSTRING')
+		if value and self.simulating:
+			# Use the '*' instead of the ',' in the value to avoid comma as token delimiter
+			self.io.idn_string = value.replace('*', ',')
+
+	def compose_cmd_arg_param(
+			self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None) -> str:
+		"""Composes command parameter string based on the single arguments definition."""
+		return self._args_single_list.compose_cmd_string(arg1, arg2, arg3, arg4, arg5, arg6)
+
+	def get_last_sent_cmd(self) -> str:
+		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
+		return self.io.get_last_sent_cmd()
+
+	def get_session_handle(self):
+		"""Returns the underlying pyvisa session."""
+		return self.io.get_session_handle()
+
+	def close(self):
+		"""Closes the Core session."""
+		self.io.close()
+		self.io = None
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/Instrument.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/Instrument.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,854 +1,781 @@
-import re
-import threading
-from enum import Enum
-from typing import List, Callable, Tuple, Dict
-
-from . import Utilities, InstrumentSettings, InstrumentOptions, InstrumentErrors, Conversions as Conv
-from .ArgSingleSuppressed import ArgSingleSuppressed
-from .ArgStructList import ArgStructList
-from .InternalLinker import InternalLinker
-from .IoTransferEventArgs import IoTransferEventArgs
-from .StreamReader import StreamReader
-from .StreamWriter import StreamWriter
-from .Utilities import trim_str_response
-from .VisaSession import VisaSession, EventArgsChunk
-from .VisaSessionSim import VisaSessionSim
-from .RepeatedCapability import RepeatedCapability
-
-
-class Instrument(object):
-	"""Model of an Instrument with VISA interface."""
-
-	def __init__(self, resource_name: str, simulate: bool, settings: InstrumentSettings, direct_session=None):
-		"""Opening an instrument session.
-		If simulate is true, it cannot be later switched to false anymore."""
-		self._simulating: bool = simulate
-		self._session = None
-		self._global_repcaps: Dict[str, RepeatedCapability] = {}
-		self._linker = InternalLinker()
-		# noinspection PyTypeChecker
-		self.on_write_handler: Callable = None
-		# noinspection PyTypeChecker
-		self.on_read_handler: Callable = None
-		self._io_events_include_data: bool = False
-		self._lock = None
-		self._before_query_handler = None
-		self._before_write_handler = None
-
-		# Fixed settings
-		self.selftest_timeout = 100000 if settings.selftest_timeout == 0 else settings.selftest_timeout
-		self.idn_model_full_name = settings.idn_model_full_name
-		self.instr_options_parse_mode = settings.instr_options_parse_mode
-
-		# Changeable settings
-		self.resource_name: str = resource_name
-		self._instr_options: InstrumentOptions = None  # Internal private property for the lazy property self.instr_options - see the getter for self.instr_options. Initialized by the first access
-		self.query_instr_status: bool = True
-		self.opc_query_after_write: bool = False
-		self.bin_float_numbers_format = settings.bin_float_numbers_format
-		self.bin_int_numbers_format = settings.bin_int_numbers_format
-		self.opc_query_after_write: bool = settings.opc_query_after_write
-		self.stb_in_error_check: bool = settings.stb_in_error_check
-
-		self.manufacturer: str = 'Rohde&Schwarz'
-		self.model: str = 'R&S Instrument'
-		self.serial_number: str = '100001'
-		self.firmware_version: str = '1.00'
-
-		if self._simulating:
-			self._session = VisaSessionSim(resource_name, settings, direct_session)
-			self._lock = self._session.get_lock()
-			self._instr_options = InstrumentOptions.Options('K0', InstrumentOptions.ParseMode.KeepOriginal)
-			self._session.write('*OPT K0')
-			return
-
-		self._session = VisaSession(resource_name, settings, direct_session)
-		self._lock = self._session.get_lock()
-		with self._lock:
-			self._session.clear_before_read()
-			self.idn_string = Utilities.trim_str_response(self._session.query_str('*IDN?')).strip()
-
-			# NRP-Z session coercing
-			if self._session.is_rsnrp_session():
-				settings.instr_options_parse_mode = InstrumentOptions.ParseMode.Skip
-				self.stb_in_error_check = False
-			self.instr_options_parse_mode = settings.instr_options_parse_mode
-
-	def __str__(self):
-		if self._simulating:
-			return f"Simulated, Model: '{self.model}', ResourceName: '{self.resource_name}'"
-		else:
-			return f"Instrument Model: '{self.model}', ResourceName: '{self.resource_name}'"
-
-	def set_simulating_cmds(self) -> None:
-		"""Updated cached values in the simulating VISA session to properly respond to *IDN? or *OPT?"""
-		if self._simulating:
-			self.write(f'*idn {self.idn_string}')
-			self.write(f'*opt {Conv.list_to_csv_str(self.instr_options.get_all())}')
-			self.write(f'*opc 1')
-			self.write(f'*stb 0')
-			self.write(f'*tst 0,"Passed"')
-			self.write(f'syst:err 0,"No Error"')
-			self.write(f'system:error 0,"No Error"')
-
-	def get_last_sent_cmd(self) -> str:
-		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
-		if self._simulating:
-			# noinspection PyUnresolvedReferences
-			return self._session.get_last_sent_cmd()
-		raise Exception('get_last_sent_cmd() can only be used in simulation mode')
-
-	def assign_lock(self, lock: threading.RLock) -> None:
-		"""Assigns the thread lock provided from by the user. Trickles down to the VisaSession."""
-		self._lock = lock
-		self._session.assign_lock(lock)
-
-	def get_lock(self) -> threading.RLock:
-		"""Returns the current RLock object."""
-		return self._lock
-
-	def clear_lock(self):
-		"""Clears the existing thread lock, making the current session thread-independent from others that might share the current thread lock."""
-		self.assign_lock(threading.RLock())
-
-	@property
-	def visa_manufacturer(self) -> str:
-		"""Returns the visa manufacturer of the current session."""
-		return self._session.manufacturer
-
-	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
-		"""Adds / Updates link handler for the entered link_name.
-		Handler API: handler(event_args: ArgLinkedEventArgs)
-		Returns the previous registered handler, or None if no handler was registered before."""
-		return self._linker.set_handler(link_name, handler)
-
-	def del_link_handler(self, link_name: str) -> Callable:
-		"""Deletes link handler for the link_name.
-		Returns the deleted handler, or None if none existed."""
-		return self._linker.del_handler(link_name)
-
-	def del_all_link_handlers(self) -> int:
-		"""Deletes all the link handlers.
-		Returns number of deleted links."""
-		return self._linker.del_all_handlers()
-
-	@property
-	def idn_string(self) -> str:
-		return self._idn_string
-
-	@idn_string.setter
-	def idn_string(self, value: str) -> None:
-		"""IDN string. Set it to force a different IDN string than the default *IDN? response."""
-		self._idn_string = value
-		self._parse_idn_string(self._idn_string)
-
-	@property
-	def instr_options(self) -> InstrumentOptions:
-		"""Public getter for the lazy property instr_options"""
-		if self._instr_options is None:
-			self._query_options_and_parse(self.instr_options_parse_mode)
-		return self._instr_options
-
-	@property
-	def opc_timeout(self) -> int:
-		"""See the opc_timeout.setter."""
-		return self._session.opc_timeout
-
-	@opc_timeout.setter
-	def opc_timeout(self, value: int) -> None:
-		"""Sets / Gets timeout in milliseconds for all the operations that use OPC synchronization."""
-		self._session.opc_timeout = value
-
-	@property
-	def visa_timeout(self) -> int:
-		"""See the visa_timeout.setter."""
-		return self._session.visa_timeout
-
-	@visa_timeout.setter
-	def visa_timeout(self, value: int) -> None:
-		"""Sets / Gets visa IO timeout in milliseconds."""
-		self._session.visa_timeout = value
-
-	@property
-	def data_chunk_size(self) -> int:
-		"""Returns max chunk size of one data block."""
-		return self._session.data_chunk_size
-
-	@data_chunk_size.setter
-	def data_chunk_size(self, chunk_size: int) -> None:
-		"""Sets the maximum size of one block transferred during write/read operations."""
-		self._session.data_chunk_size = int(chunk_size)
-
-	# noinspection PyMethodMayBeStatic
-	def _sim_cached_value_found(self, value) -> bool:
-		return value != 'Simulating'
-
-	# noinspection PyMethodMayBeStatic
-	def _sim_cached_value_not_found(self, value) -> bool:
-		return value == 'Simulating'
-
-	def _parse_idn_string(self, idn_string: str) -> None:
-		"""Parse the *IDN? response to:
-		- Manufacturer
-		- Model
-		- SerialNumber
-		- FirmwareRevision"""
-		idn_string = idn_string.strip()
-		m = re.search(r'([\w& ]+),([a-zA-Z ]+)([\-0-9a-zA-Z ]*),([^,]+),([\w .\-/]+)', idn_string)
-		if not m:
-			raise Exception(f"The instrument *IDN? string parsing failed. Parsed *IDN? response: '{idn_string}'")
-		self.manufacturer = m.group(1).strip()
-		self.model = m.group(2).strip()
-		self.full_model_name = self.model + m.group(3).strip()
-		self.serial_number = m.group(4).strip()
-		self.firmware_version = m.group(5).strip()
-		if self.idn_model_full_name:
-			self.model = self.full_model_name
-
-	def fits_idn_pattern(self, patterns: List[str], supported_models: List[str]) -> None:
-		"""Throws exception if the current instrument model does not fit  any of the patterns.
-		The supported_models argument is only used for exception messages"""
-		matches = False
-		assert self._idn_string, f'*IDN? was not assigned yet.'
-		for x in patterns:
-			matches = re.search(x, self.idn_string, re.IGNORECASE)
-			if matches:
-				break
-		if not matches:
-			message = f"Instrument is not supported.\n*IDN? string: '{self.idn_string}'"
-			if len(supported_models) > 0:
-				message += f"\nSupported models: '{', '.join(supported_models)}'"
-			if len(patterns) == 1:
-				message += f"\nSupported IDN pattern: '{patterns[0]}'"
-			if len(patterns) > 1:
-				message += "\nSupported IDN patterns:\n" + '\n'.join(patterns)
-			raise InstrumentErrors.UnexpectedResponseException(self.resource_name, message)
-
-	def _query_options_and_parse(self, mode: InstrumentOptions.ParseMode) -> None:
-		"""Queries *OPT? and parses it based on the ParseMode."""
-		if mode == InstrumentOptions.ParseMode.Skip:
-			self._instr_options = InstrumentOptions.Options('', mode)
-			return
-		if self._simulating is False:
-			with self._lock:
-				opts = self._session.query_str_no_tout_err('*OPT?', 1000)
-				if opts is None:
-					opts = 'Cannot read the instrument options - *OPT? query is not supported'
-				self._instr_options = InstrumentOptions.Options(opts, mode)
-
-	@staticmethod
-	def _parse_err_query_response(response: str) -> str:
-		"""Parses entered response string to string error message without the error code.
-		E.g.: response = '-110,"Command error"' returns: 'Command error'."""
-		m = re.match(r'(-?[\d]+).*?"(.*)"', response)
-		if m:
-			return m.group(2)
-		else:
-			return response
-
-	def add_global_repcap(self, name: str, rep_cap: RepeatedCapability) -> None:
-		"""Adds the global repcap name to the list of global repcaps
-		and sets its value to the provided default value."""
-		if name in self._global_repcaps:
-			raise Exception(f"Error adding new global repcap: '{name}' already exists in the list.")
-		self._global_repcaps[name] = rep_cap
-
-	def set_global_repcap_value(self, name: str, enum_value: Enum) -> None:
-		"""Updates the existing global repcap value as enum"""
-		if name not in self._global_repcaps:
-			raise Exception(f"Error updating global repcap: '{name}' does not exist in the list.")
-		self._global_repcaps[name].set_enum_value(enum_value)
-
-	def get_global_repcap_value(self, name: str) -> Enum:
-		"""Returns the current global repcap value as enum"""
-		if name not in self._global_repcaps:
-			raise Exception(f"Error retrieving global repcap: '{name}' does not exist in the list.")
-		return self._global_repcaps[name].get_enum_value()
-
-	def _replace_global_repcaps(self, cmd: str) -> str:
-		"""Replaces all the global repcaps in the command: e.g. '<instance>' => '1'.
-		Returns the replaced command."""
-		for name, value in self._global_repcaps.items():
-			cmd_value = value.get_cmd_string_value()
-			cmd = cmd.replace(name, cmd_value)
-		return cmd
-
-	def query_opc(self, timeout: int = 0) -> bool:
-		"""Sends *OPC? query and returns the result.
-		If you define timeout > 0, the VISA timeout is set to that value just for this method call."""
-		with self._lock:
-			self.start_send_read_event('*OPC?', False)
-			opc: bool = self._session.query_opc(timeout)
-			self.end_send_read_event()
-			return opc
-
-	def query_all_syst_errors(self, include_codes=True) -> List[str]:
-		"""Returns all errors in the instrument's error queue.
-		If include_codes is False, you only get the error messages without the error codes."""
-		with self._lock:
-			self.start_send_read_event('SYST:ERROR?', False)
-			errors = self._session.query_all_syst_errors()
-			if include_codes is False and errors is not None:
-				errors = [self._parse_err_query_response(x) for x in errors]
-			self.end_send_read_event()
-			return errors
-
-	def check_status(self) -> None:
-		"""Throws InstrumentStatusException in case of an error in the instrument's error queue.
-		The procedure is skipped, if the QueryInstrumentStatus is set to false."""
-		with self._lock:
-			if not self.query_instr_status:
-				return
-			call_syst_error = self._session.error_in_error_queue() if self.stb_in_error_check else True
-			if call_syst_error:
-				errors = self.query_all_syst_errors(False)
-				InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, errors)
-
-	def clear_status(self) -> None:
-		"""Clears instrument's status subsystem."""
-		with self._lock:
-			self._session.clear()
-			self._session.clear_before_read()
-
-	def reset(self) -> None:
-		"""Resets the instrument and clears its status."""
-		with self._lock:
-			self.write('*RST', True)
-			self.query_opc()
-			self.clear_status()
-			self.check_status()
-
-	def write(self, cmd: str, block_callback: bool = False) -> None:
-		"""Writes string command to the instrument."""
-		with self._lock:
-			cmd = self._replace_global_repcaps(cmd)
-			self._call_before_write_handler(cmd, block_callback)
-			self._session.write(cmd)
-			if self.opc_query_after_write:
-				self._session.query_opc()
-			if self.on_write_handler:
-				self.send_write_str_event(cmd, False)
-			self.check_status()
-
-	def write_with_opc(self, cmd: str, timeout: int = None, block_callback: bool = False) -> None:
-		"""Writes a OPC-synced command.
-		Also performs error checking if the property self.query_instr_status is set to True.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			cmd = self._replace_global_repcaps(cmd)
-			self._call_before_write_handler(cmd, block_callback)
-			self._session.write_with_opc(cmd, timeout)
-			self._session.query_and_clear_esr()
-			if self.on_write_handler:
-				self.send_write_str_event(cmd, True)
-			self.check_status()
-
-	def write_struct(self, cmd: str, struct: object) -> None:
-		"""Writes command to the instrument with the parameter composed from the entered structure."""
-		with self._lock:
-			worker = ArgStructList(struct)
-			param = worker.compose_cmd_string()
-			cmd += f' {param}'.rstrip()
-			self.write(cmd)
-
-	def write_struct_with_opc(self, cmd: str, struct: object, timeout: int = None) -> None:
-		"""Writes OPC-synced command to the instrument with the parameter composed from the entered structure.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			worker = ArgStructList(struct)
-			param = worker.compose_cmd_string()
-			cmd += f' {param}'.rstrip()
-			self.write_with_opc(cmd, timeout)
-
-	def query_str(self, query: str, block_callback: bool = False) -> str:
-		"""Sends a query and reads response from the instrument.
-		The response is trimmed of any trailing LF characters and has no length limit."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			self._call_pre_query_handler(query, block_callback)
-			response = self._session.query_str(query)
-			self.end_send_read_event()
-			self.check_status()
-			return response
-
-	def query_str_with_opc(self, query: str, timeout: int = None, block_callback: bool = False) -> str:
-		"""Sends a OPC-synced query.
-		Also performs error checking if the self.query_instr_status is true.
-		The response is trimmed of any trailing LF characters and has no length limit.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			self._call_pre_query_handler(query, block_callback)
-			response = self._session.query_str_with_opc(query, timeout)
-			self.end_send_read_event()
-			self._session.query_and_clear_esr()
-			self.check_status()
-			return response
-
-	def query_bin_block_to_stream(self, query: str, stream: StreamWriter) -> None:
-		"""Queries binary data block to the provided stream.
-		Use it for querying data from instrument to a variable or a file.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block(query, stream, True)
-			self.end_send_read_event()
-			self.check_status()
-
-	def query_bin_block(self, query: str) -> bytes:
-		"""Queries binary data block to bytes and returns data as bytes.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			writer = StreamWriter.as_bin_var()
-			self.query_bin_block_to_stream(query, writer)
-			return writer.content
-
-	def query_bin_block_to_file(self, cmd: str, file_path: str, append: bool = False) -> None:
-		"""Queries binary data block to the provided file.
-		If append is False, any existing file content is discarded.
-		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			with StreamWriter.as_bin_file(file_path, append) as writer:
-				self.query_bin_block_to_stream(cmd, writer)
-
-	def query_bin_block_to_stream_with_opc(self, query: str, stream: StreamWriter, timeout: int = None) -> None:
-		"""Sends a OPC-synced query and returns data the provided stream.
-		Use it for querying data from instrument to a variable or a file.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block_with_opc(query, stream, True, timeout)
-			self.end_send_read_event()
-			self._session.query_and_clear_esr()
-			self.check_status()
-
-	def query_bin_block_with_opc(self, query: str, timeout: int = None) -> bytes:
-		"""Sends a OPC-synced query and returns data as bytes.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			with StreamWriter.as_bin_var() as stream:
-				self.query_bin_block_to_stream_with_opc(query, stream, timeout)
-				return stream.content
-
-	def query_bin_block_to_file_with_opc(self, cmd: str, file_path: str, append: bool = False, timeout: int = None) -> None:
-		"""Sends a OPC-synced query and writes the returned data to the provided file.
-		If append is False, any existing file content is discarded.
-		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
-		Throws an exception if the returned data was not a binary data."""
-		with self._lock:
-			with StreamWriter.as_bin_file(file_path, append) as writer:
-				self.query_bin_block_to_stream_with_opc(cmd, writer, timeout)
-
-	def query_int(self, query: str) -> int:
-		"""Sends a query and reads response from the instrument as integer."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0
-			return Conv.str_to_int(string)
-
-	def query_int_with_opc(self, query: str, timeout: int = None) -> int:
-		"""Sends a OPC-synced query and reads response from the instrument as integer number.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0
-			return Conv.str_to_int(string)
-
-	def query_float(self, query: str) -> float:
-		"""Sends a query and reads response from the instrument as float number."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0.0
-			return Conv.str_to_float(string)
-
-	def query_float_with_opc(self, query: str, timeout: int = None) -> float:
-		"""Sends a OPC-synced query and reads response from the instrument as float number.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return 0.0
-			return Conv.str_to_float(string)
-
-	def query_bool(self, query: str) -> bool:
-		"""Sends a query and reads response from the instrument as boolean value."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return False
-			return Conv.str_to_bool(string)
-
-	def query_bool_with_opc(self, query: str, timeout: int = None) -> bool:
-		"""Sends a OPC-synced query and reads response from the instrument as boolean value.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return False
-			return Conv.str_to_bool(string)
-
-	def query_str_list(self, query: str) -> List[str]:
-		"""Sends a query and reads response from the instrument as csv-list."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
-			response = [trim_str_response(x) for x in string.split(',')]
-			return response
-
-	def query_str_list_with_opc(self, query: str, timeout: int = None) -> List[str]:
-		"""Sends a OPC-synced query and reads response from the instrument as csv-list.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
-			response = [trim_str_response(x) for x in string.split(',')]
-			return response
-
-	def write_bin_block_from_stream(self, cmd: str, stream: StreamReader) -> None:
-		"""Writes all the stream content as binary data block to the instrument.
-		Use it for writing data to instrument from a variable or a file.
-		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
-		with self._lock:
-			if self.on_write_handler:
-				self.start_send_write_bin_event(cmd)
-			self._call_pre_query_handler(cmd, False)
-			self._session.write_bin_block(cmd, stream)
-			self.end_send_write_bin_event()
-			self.check_status()
-
-	def write_bin_block(self, cmd: str, payload: bytes) -> None:
-		"""Writes all the payload as binary data block to the instrument.
-		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
-		self.write_bin_block_from_stream(cmd, StreamReader.as_bin_var(payload))
-
-	def write_bin_block_from_file(self, cmd: str, file_path: str) -> None:
-		"""Writes all the file content as binary data block to the instrument.
-		The binary data header is added at the beginning of the transmission automatically, do not include it in the file content!!!"""
-		with StreamReader.as_bin_file(file_path) as reader:
-			self.write_bin_block_from_stream(cmd, reader)
-
-	def query_bin_or_ascii_float_list(self, query: str) -> List[float]:
-		"""Queries a list of floating-point numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32)."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			stream = StreamWriter.as_bin_var()
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block(query, stream, False)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
-			else:
-				result = Conv.str_to_float_list(stream.content)
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_float_list_with_opc(self, query: str, timeout: int = None) -> List[float]:
-		"""Sends a OPC-synced query and reads a list of floating-point numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32).
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			stream = StreamWriter.as_bin_var()
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block_with_opc(query, stream, False, timeout)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
-			else:
-				result = Conv.str_to_float_list(stream.content)
-			self._session.query_and_clear_esr()
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_float_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[float]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return Conv.str_to_float_list(response)
-
-	def query_bin_or_ascii_float_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[float]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
-		If you do not provide timeout, the method uses current opc_timeout.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return Conv.str_to_float_list(response)
-
-	def query_bin_or_ascii_int_list(self, query: str) -> List[int]:
-		"""Queries a list of integer numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32)."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, False)
-			stream = StreamWriter.as_bin_var()
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block(query, stream, False)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
-			else:
-				result = Conv.str_to_int_list(stream.content)
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_int_list_with_opc(self, query: str, timeout: int = None) -> List[int]:
-		"""Sends a OPC-synced query and reads a list of integer numbers that can be returned in ASCII format or in binary format.
-		- For ASCII format, the list numbers are decoded as comma-separated values.
-		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32).
-		If you do not provide timeout, the method uses current opc_timeout."""
-		with self._lock:
-			query = self._replace_global_repcaps(query)
-			self.start_send_read_event(query, True)
-			stream = StreamWriter.as_bin_var()
-			self._call_pre_query_handler(query, False)
-			self._session.query_bin_block_with_opc(query, stream, False, timeout)
-			self.end_send_read_event()
-			if self._simulating and not self._session.cached_to_stream:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			if stream.binary:
-				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
-			else:
-				result = Conv.str_to_int_list(stream.content)
-			self._session.query_and_clear_esr()
-			self.check_status()
-			return result
-
-	def query_bin_or_ascii_int_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[int]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			response = self.query_str(query)
-			if self._simulating:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			response = self._linker.cut_from_response_string(suppressed, response, query)
-			return Conv.str_to_int_list(response)
-
-	def query_bin_or_ascii_int_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[int]:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
-		If you do not provide timeout, the method uses current opc_timeout.
-		The current implementation allows for the rest of the string to be only ASCII format."""
-		with self._lock:
-			response = self.query_str_with_opc(query, timeout)
-			if self._simulating:
-				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
-			response = self._linker.cut_from_response_string(suppressed, response, query)
-			return Conv.str_to_int_list(response)
-
-	def query_struct(self, query: str, struct: object) -> object:
-		"""Queries string of from instrument, and parses it based on the provided structure object.
-		THe method returns the copy of the entered object that it had modified."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return struct
-			struct_list = ArgStructList(struct)
-			struct_list.parse_from_cmd_response(string)
-			self._linker.invoke_struct_intern_links(struct, struct_list.args, query)
-			return struct
-
-	def query_struct_with_opc(self, query: str, struct: object, timeout: int = None) -> object:
-		"""Queries string of from instrument, and parses it based on the provided structure object.
-		THe method returns the copy of the entered object that it had modified."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return struct
-			struct_list = ArgStructList(struct)
-			struct_list.parse_from_cmd_response(string)
-			self._linker.invoke_struct_intern_links(struct, struct_list.args, query)
-			return struct
-
-	def query_str_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> str:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument."""
-		with self._lock:
-			string = self.query_str(query)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return string
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return response
-
-	def query_str_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> str:
-		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument."""
-		with self._lock:
-			string = self.query_str_with_opc(query, timeout)
-			if self._simulating and self._sim_cached_value_not_found(string):
-				return string
-			response = self._linker.cut_from_response_string(suppressed, string, query)
-			return response
-
-	def self_test(self, timeout: int = None) -> Tuple[int, str]:
-		"""Performs instrument's selftest (*TST?).
-		Returns tuple (code:int, message: str). . Code 0 means the self-test passed.
-		You can define the custom timeout in milliseconds. If you do not define it, the default selftest timeout is used (usually 60 secs)."""
-		with self._lock:
-			if timeout is None or timeout == 0:
-				timeout = self.selftest_timeout
-			response = self.query_str_with_opc('*TST?', timeout)
-			m = re.search(r'^(-?[\d]+)(,(.*))?', response)
-			if not m:
-				raise InstrumentErrors.UnexpectedResponseException(self.resource_name, f"Unexpected response to a '*TST?' self-test query: '{response}'")
-			code = Conv.str_to_int(m.group(1))
-			msg = Utilities.trim_str_response(m.group(3))
-			self.check_status()
-			return code, msg
-
-	def get_session_handle(self) -> object:
-		"""Returns the underlying pyvisa session."""
-		return self._session.get_session_handle()
-
-	def close(self) -> None:
-		"""Closes the Instrument session."""
-		with self._lock:
-			self._session.close()
-			self._session = None
-
-	# Events part
-
-	@property
-	def io_events_include_data(self) -> bool:
-		"""If true, the read and write handlers also include read and written data."""
-		return self._io_events_include_data
-
-	@io_events_include_data.setter
-	def io_events_include_data(self, value: bool) -> None:
-		"""If true, the read and write handlers also include read and written data."""
-		self._io_events_include_data = value
-		self._session.io_events_include_data = value
-
-	def event_args_append_instr_info(self, args: IoTransferEventArgs) -> IoTransferEventArgs:
-		"""Appends instrument-related information to the read/write event argument"""
-		args.chunk_size = self.data_chunk_size
-		args.resource_name = self.resource_name
-		return args
-
-	def send_write_str_event(self, cmd: str, opc_sync: bool) -> None:
-		"""Creates and sends write string event. The transfer is marked as done (end_of_transfer = True)."""
-		args = IoTransferEventArgs.write_str(opc_sync, len(cmd), cmd)
-		args.transferred_size = args.total_size
-		args.chunk_ix = 0
-		args.end_of_transfer = True
-		args = self.event_args_append_instr_info(args)
-		if self._io_events_include_data:
-			args.data = cmd
-		self.on_write_handler(args)
-
-	def start_send_read_event(self, query: str, opc_sync: bool) -> None:
-		"""Registers VisaSession.on_read_chunk_handler() which then generates events with each chunk transfer.
-		Event handler for these events is the local function of this method, which sends IoTransferEventArgs further up to the Instrument.on_read_handler()"""
-		if not self.on_read_handler:
-			return
-
-		def _read_chunk_handler(visa_args: EventArgsChunk) -> None:
-			"""Receives events from VisaSession on read chunk transfers, and sends them as IoTransferEventArgs to the Instrument.on_read_handler()"""
-			args.end_of_transfer = visa_args.end_of_transfer
-			args.chunk_ix = visa_args.chunk_ix
-			args.total_chunks = visa_args.total_chunks
-			args.chunk_size = visa_args.chunk_size
-			args.transferred_size = visa_args.transferred_size
-			args.total_size = visa_args.total_size
-			args.data = visa_args.data
-			args.binary = visa_args.binary
-			self.on_read_handler(args)
-
-		args = IoTransferEventArgs.read_chunk(opc_sync, query)
-		args = self.event_args_append_instr_info(args)
-		self._session.on_read_chunk_handler = _read_chunk_handler
-
-	def end_send_read_event(self):
-		"""Unregisters VisaSession.on_read_chunk_handler()"""
-		self._session.on_read_chunk_handler = None
-
-	def start_send_write_bin_event(self, cmd: str) -> None:
-		"""Registers VisaSession.on_write_chunk_handler() which then generates events with each chunk transfer.
-		Event handler for these events is the local function of this method, which sends IoTransferEventArgs further up to the Instrument.on_write_handler()"""
-		if not self.on_write_handler:
-			return
-
-		def _write_chunk_handler(visa_args: EventArgsChunk) -> None:
-			"""Receives events from VisaSession on write chunk transfers, and sends them as IoTransferEventArgs to the Instrument.on_write_handler()"""
-			args.end_of_transfer = visa_args.end_of_transfer
-			args.chunk_ix = visa_args.chunk_ix
-			args.total_chunks = visa_args.total_chunks
-			args.chunk_size = visa_args.chunk_size
-			args.transferred_size = visa_args.transferred_size
-			args.total_size = visa_args.total_size
-			args.data = visa_args.data
-			args.binary = visa_args.binary
-			self.on_write_handler(args)
-
-		args = IoTransferEventArgs.write_bin(cmd)
-		args = self.event_args_append_instr_info(args)
-		self._session.on_write_chunk_handler = _write_chunk_handler
-
-	def end_send_write_bin_event(self):
-		"""Unregisters VisaSession.on_write_chunk_handler()"""
-		self._session.on_write_chunk_handler = None
-
-	def _call_before_write_handler(self, cmd: str, block_callback: bool) -> None:
-		"""Calls the _pre_write_handler if defined. Used in all the base write methods."""
-		if block_callback is False and self._before_write_handler:
-			self._before_write_handler(self, cmd)
-
-	def _call_pre_query_handler(self, query: str, block_callback: bool) -> None:
-		"""Calls the _pre_query_handler if defined. Used in all the base query methods."""
-		if block_callback is False and self._before_query_handler:
-			self._before_query_handler(self, query)
-
-	@property
-	def before_write_handler(self) -> Callable:
-		"""Returns the handler of before_write events. \n
-		:return: current before_write_handler"""
-		return self._before_write_handler
-
-	@before_write_handler.setter
-	def before_write_handler(self, handler: Callable) -> None:
-		"""Sets handler for before_write events.
-		The before_write event is invoked before each write operation (only once, not for every chunk)
-		Event prototype: handler(io: Instrument, cmd: str)
-		:param handler: new handler"""
-		self._before_write_handler = handler
-
-	@property
-	def before_query_handler(self) -> Callable:
-		"""Returns the handler of before_query events. \n
-		:return: current before_query_handler"""
-		return self._before_query_handler
-
-	@before_query_handler.setter
-	def before_query_handler(self, handler: Callable) -> None:
-		"""Sets handler for before_query events.
-		The before_query event is invoked before each query operation (only once, not for every chunk)
-		Event prototype: handler(io: Instrument, query: str)
-		:param handler: new handler"""
-		self._before_query_handler = handler
+import re
+import threading
+from enum import Enum
+from typing import List, Callable, Tuple, Dict
+
+from . import Utilities, InstrumentSettings, InstrumentOptions, InstrumentErrors, Conversions as Conv
+from .ArgSingleSuppressed import ArgSingleSuppressed
+from .ArgStructList import ArgStructList
+from .InternalLinker import InternalLinker
+from .IoTransferEventArgs import IoTransferEventArgs
+from .StreamReader import StreamReader
+from .StreamWriter import StreamWriter
+from .Utilities import trim_str_response
+from .VisaSession import VisaSession, EventArgsChunk
+from .VisaSessionSim import VisaSessionSim
+from .RepeatedCapability import RepeatedCapability
+
+
+class Instrument(object):
+	"""Model of an Instrument with VISA interface."""
+
+	def __init__(self, resource_name: str, simulate: bool, settings: InstrumentSettings, direct_session=None):
+		"""Opening an instrument session.
+		If simulate is true, it cannot be later switched to false anymore."""
+		self._simulating: bool = simulate
+		self._session = None
+		self._global_repcaps: Dict[str, RepeatedCapability] = {}
+		self._linker = InternalLinker()
+		# noinspection PyTypeChecker
+		self.on_write_handler: Callable = None
+		# noinspection PyTypeChecker
+		self.on_read_handler: Callable = None
+		self._io_events_include_data: bool = False
+		self._lock = None
+
+		# Fixed settings
+		self.selftest_timeout = 100000 if settings.selftest_timeout == 0 else settings.selftest_timeout
+		self.idn_model_full_name = settings.idn_model_full_name
+		self.instr_options_parse_mode = settings.instr_options_parse_mode
+
+		# Changeable settings
+		self.resource_name: str = resource_name
+		self._instr_options: InstrumentOptions = None  # Internal private property for the lazy property self.instr_options - see the getter for self.instr_options. Initialized by the first access
+		self.query_instr_status: bool = True
+		self.opc_query_after_write: bool = False
+		self.bin_float_numbers_format = settings.bin_float_numbers_format
+		self.bin_int_numbers_format = settings.bin_int_numbers_format
+		self.opc_query_after_write: bool = settings.opc_query_after_write
+		self.stb_in_error_check: bool = settings.stb_in_error_check
+
+		self.manufacturer: str = 'Rohde&Schwarz'
+		self.model: str = 'R&S Instrument'
+		self.serial_number: str = '100001'
+		self.firmware_version: str = '1.00'
+
+		if self._simulating:
+			self._session = VisaSessionSim(resource_name, settings, direct_session)
+			self._lock = self._session.get_lock()
+			self._instr_options = InstrumentOptions.Options('K0', InstrumentOptions.ParseMode.KeepOriginal)
+			self._session.write("*OPT K0")
+			return
+
+		self._session = VisaSession(resource_name, settings, direct_session)
+		self._lock = self._session.get_lock()
+		with self._lock:
+			self._session.clear_before_read()
+			self.idn_string = Utilities.trim_str_response(self._session.query_str('*IDN?')).strip()
+
+			# NRP-Z session coercing
+			if self._session.is_rsnrp_session():
+				settings.instr_options_parse_mode = InstrumentOptions.ParseMode.Skip
+				self.stb_in_error_check = False
+			self.instr_options_parse_mode = settings.instr_options_parse_mode
+
+	def __str__(self):
+		if self._simulating:
+			return f"Simulated, Model: '{self.model}', ResourceName: '{self.resource_name}'"
+		else:
+			return f"Instrument Model: '{self.model}', ResourceName: '{self.resource_name}'"
+
+	def set_simulating_cmds(self) -> None:
+		"""Updated cached values in the simulating VISA session to properly respond to *IDN? or *OPT?"""
+		if self._simulating:
+			self.write(f'*idn {self.idn_string}')
+			self.write(f'*opt {Conv.list_to_csv_str(self.instr_options.get_all())}')
+			self.write(f'*opc 1')
+			self.write(f'*stb 0')
+			self.write(f'*tst 0,"Passed"')
+			self.write(f'syst:err 0,"No Error"')
+			self.write(f'system:error 0,"No Error"')
+
+	def get_last_sent_cmd(self) -> str:
+		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
+		if self._simulating:
+			# noinspection PyUnresolvedReferences
+			return self._session.get_last_sent_cmd()
+		raise Exception("get_last_sent_cmd() can only be used in simulation mode")
+
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the thread lock provided from by the user. Trickles down to the VisaSession."""
+		self._lock = lock
+		self._session.assign_lock(lock)
+
+	def get_lock(self) -> threading.RLock:
+		"""Returns the current RLock object."""
+		return self._lock
+
+	def clear_lock(self):
+		"""Clears the existing thread lock, making the current session thread-independent from others that might share the current thread lock."""
+		self.assign_lock(threading.RLock())
+
+	@property
+	def visa_manufacturer(self) -> str:
+		"""Returns the visa manufacturer of the current session."""
+		return self._session.manufacturer
+
+	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
+		"""Adds / Updates link handler for the entered link_name.
+		Handler API: handler(event_args: ArgLinkedEventArgs)
+		Returns the previous registered handler, or None if no handler was registered before."""
+		return self._linker.set_handler(link_name, handler)
+
+	def del_link_handler(self, link_name: str) -> Callable:
+		"""Deletes link handler for the link_name.
+		Returns the deleted handler, or None if none existed."""
+		return self._linker.del_handler(link_name)
+
+	def del_all_link_handlers(self) -> int:
+		"""Deletes all the link handlers.
+		Returns number of deleted links."""
+		return self._linker.del_all_handlers()
+
+	@property
+	def idn_string(self) -> str:
+		return self._idn_string
+
+	@idn_string.setter
+	def idn_string(self, value: str) -> None:
+		"""IDN string. Set it to force a different IDN string than the default *IDN? response."""
+		self._idn_string = value
+		self._parse_idn_string(self._idn_string)
+
+	@property
+	def instr_options(self) -> InstrumentOptions:
+		"""Public getter for the lazy property instr_options"""
+		if self._instr_options is None:
+			self._query_options_and_parse(self.instr_options_parse_mode)
+		return self._instr_options
+
+	@property
+	def opc_timeout(self) -> int:
+		"""See the opc_timeout.setter."""
+		return self._session.opc_timeout
+
+	@opc_timeout.setter
+	def opc_timeout(self, value: int) -> None:
+		"""Sets / Gets timeout in milliseconds for all the operations that use OPC synchronization."""
+		self._session.opc_timeout = value
+
+	@property
+	def visa_timeout(self) -> int:
+		"""See the visa_timeout.setter."""
+		return self._session.visa_timeout
+
+	@visa_timeout.setter
+	def visa_timeout(self, value: int) -> None:
+		"""Sets / Gets visa IO timeout in milliseconds."""
+		self._session.visa_timeout = value
+
+	@property
+	def data_chunk_size(self) -> int:
+		"""Returns max chunk size of one data block."""
+		return self._session.data_chunk_size
+
+	@data_chunk_size.setter
+	def data_chunk_size(self, chunk_size: int) -> None:
+		"""Sets the maximum size of one block transferred during write/read operations."""
+		self._session.data_chunk_size = int(chunk_size)
+
+	# noinspection PyMethodMayBeStatic
+	def _sim_cached_value_found(self, value) -> bool:
+		return value != 'Simulating'
+
+	# noinspection PyMethodMayBeStatic
+	def _sim_cached_value_not_found(self, value) -> bool:
+		return value == 'Simulating'
+
+	def _parse_idn_string(self, idn_string: str) -> None:
+		"""Parse the *IDN? response to:
+		- Manufacturer
+		- Model
+		- SerialNumber
+		- FirmwareRevision"""
+		idn_string = idn_string.strip()
+		m = re.search(r'([\w& ]+),([a-zA-Z ]+)([\-0-9a-zA-Z ]*),([^,]+),([\w .\-/]+)', idn_string)
+		if not m:
+			raise Exception(f"The instrument *IDN? string parsing failed. Parsed *IDN? response: '{idn_string}'")
+		self.manufacturer = m.group(1).strip()
+		self.model = m.group(2).strip()
+		self.full_model_name = self.model + m.group(3).strip()
+		self.serial_number = m.group(4).strip()
+		self.firmware_version = m.group(5).strip()
+		if self.idn_model_full_name:
+			self.model = self.full_model_name
+
+	def fits_idn_pattern(self, patterns: List[str], supported_models: List[str]) -> None:
+		"""Throws exception if the current instrument model does not fit  any of the patterns.
+		The supported_models argument is only used for exception messages"""
+		matches = False
+		assert self._idn_string, f'*IDN? was not assigned yet.'
+		for x in patterns:
+			matches = re.search(x, self.idn_string, re.IGNORECASE)
+			if matches:
+				break
+		if not matches:
+			message = f"Instrument is not supported.\n*IDN? string: '{self.idn_string}'"
+			if len(supported_models) > 0:
+				message += f"\nSupported models: '{', '.join(supported_models)}'"
+			if len(patterns) == 1:
+				message += f"\nSupported IDN pattern: '{patterns[0]}'"
+			if len(patterns) > 1:
+				message += "\nSupported IDN patterns:\n" + '\n'.join(patterns)
+			raise InstrumentErrors.UnexpectedResponseException(self.resource_name, message)
+
+	def _query_options_and_parse(self, mode: InstrumentOptions.ParseMode) -> None:
+		"""Queries *OPT? and parses it based on the ParseMode."""
+		if mode == InstrumentOptions.ParseMode.Skip:
+			self._instr_options = InstrumentOptions.Options('', mode)
+			return
+		if self._simulating is False:
+			with self._lock:
+				opts = self._session.query_str_no_tout_err('*OPT?', 1000)
+				if opts is None:
+					opts = 'Cannot read the instrument options - *OPT? query is not supported'
+				self._instr_options = InstrumentOptions.Options(opts, mode)
+
+	@staticmethod
+	def _parse_err_query_response(response: str) -> str:
+		"""Parses entered response string to string error message without the error code.
+		E.g.: response = '-110,"Command error"' returns: 'Command error'."""
+		m = re.match(r'(-?[\d]+).*?"(.*)"', response)
+		if m:
+			return m.group(2)
+		else:
+			return response
+
+	def add_global_repcap(self, name: str, rep_cap: RepeatedCapability) -> None:
+		"""Adds the global repcap name to the list of global repcaps
+		and sets its value to the provided default value."""
+		if name in self._global_repcaps:
+			raise Exception(f"Error adding new global repcap: '{name}' already exists in the list.")
+		self._global_repcaps[name] = rep_cap
+
+	def set_global_repcap_value(self, name: str, enum_value: Enum) -> None:
+		"""Updates the existing global repcap value as enum"""
+		if name not in self._global_repcaps:
+			raise Exception(f"Error updating global repcap: '{name}' does not exist in the list.")
+		self._global_repcaps[name].set_enum_value(enum_value)
+
+	def get_global_repcap_value(self, name: str) -> Enum:
+		"""Returns the current global repcap value as enum"""
+		if name not in self._global_repcaps:
+			raise Exception(f"Error retrieving global repcap: '{name}' does not exist in the list.")
+		return self._global_repcaps[name].get_enum_value()
+
+	def _replace_global_repcaps(self, cmd: str) -> str:
+		"""Replaces all the global repcaps in the command: e.g. '<instance>' => '1'.
+		Returns the replaced command."""
+		for name, value in self._global_repcaps.items():
+			cmd_value = value.get_cmd_string_value()
+			cmd = cmd.replace(name, cmd_value)
+		return cmd
+
+	def query_opc(self) -> bool:
+		"""Sends *OPC? query and returns the result."""
+		with self._lock:
+			self.start_send_read_event('*OPC?', False)
+			opc: bool = self._session.query_opc()
+			self.end_send_read_event()
+			return opc
+
+	def query_all_syst_errors(self, include_codes=True) -> List[str]:
+		"""Returns all errors in the instrument's error queue.
+		If include_codes is False, you only get the error messages without the error codes."""
+		with self._lock:
+			self.start_send_read_event('SYST:ERROR?', False)
+			errors = self._session.query_all_syst_errors()
+			if include_codes is False and errors is not None:
+				errors = [self._parse_err_query_response(x) for x in errors]
+			self.end_send_read_event()
+			return errors
+
+	def check_status(self) -> None:
+		"""Throws InstrumentStatusException in case of an error in the instrument's error queue.
+		The procedure is skipped, if the QueryInstrumentStatus is set to false."""
+		with self._lock:
+			if not self.query_instr_status:
+				return
+			call_syst_error = self._session.error_in_error_queue() if self.stb_in_error_check else True
+			if call_syst_error:
+				errors = self.query_all_syst_errors(False)
+				InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, errors)
+
+	def clear_status(self) -> None:
+		"""Clears instrument's status subsystem."""
+		with self._lock:
+			self._session.clear()
+			self._session.clear_before_read()
+
+	def reset(self) -> None:
+		"""Resets the instrument and clears its status."""
+		with self._lock:
+			self.write("*RST")
+			self.query_opc()
+			self.clear_status()
+			self.check_status()
+
+	def write(self, cmd: str) -> None:
+		"""Writes string command to the instrument."""
+		with self._lock:
+			cmd = self._replace_global_repcaps(cmd)
+			self._session.write(cmd)
+			if self.opc_query_after_write:
+				self._session.query_opc()
+			if self.on_write_handler:
+				self.send_write_str_event(cmd, False)
+			self.check_status()
+
+	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
+		"""Writes a OPC-synced command.
+		Also performs error checking if the property self.query_instr_status is set to True.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			cmd = self._replace_global_repcaps(cmd)
+			self._session.write_with_opc(cmd, timeout)
+			self._session.query_and_clear_esr()
+			if self.on_write_handler:
+				self.send_write_str_event(cmd, True)
+			self.check_status()
+
+	def write_struct(self, cmd: str, struct: object) -> None:
+		"""Writes command to the instrument with the parameter composed from the entered structure."""
+		with self._lock:
+			worker = ArgStructList(struct)
+			param = worker.compose_cmd_string()
+			cmd += f' {param}'.rstrip()
+			self.write(cmd)
+
+	def write_struct_with_opc(self, cmd: str, struct: object, timeout: int = None) -> None:
+		"""Writes OPC-synced command to the instrument with the parameter composed from the entered structure.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			worker = ArgStructList(struct)
+			param = worker.compose_cmd_string()
+			cmd += f' {param}'.rstrip()
+			self.write_with_opc(cmd, timeout)
+
+	def query_str(self, query: str) -> str:
+		"""Sends a query and reads response from the instrument.
+		The response is trimmed of any trailing LF characters and has no length limit."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			response = self._session.query_str(query)
+			self.end_send_read_event()
+			self.check_status()
+			return response
+
+	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
+		"""Sends a OPC-synced query.
+		Also performs error checking if the self.query_instr_status is true.
+		The response is trimmed of any trailing LF characters and has no length limit.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			response = self._session.query_str_with_opc(query, timeout)
+			self.end_send_read_event()
+			self._session.query_and_clear_esr()
+			self.check_status()
+			return response
+
+	def query_bin_block_to_stream(self, query: str, stream: StreamWriter) -> None:
+		"""Queries binary data block to the provided stream.
+		Use it for querying data from instrument to a variable or a file.
+		Throws an exception if the returned data was not a binary data."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			self._session.query_bin_block(query, stream, True)
+			self.end_send_read_event()
+			self.check_status()
+
+	def query_bin_block(self, query: str) -> bytes:
+		"""Queries binary data block to bytes and returns data as bytes.
+		Throws an exception if the returned data was not a binary data."""
+		with self._lock:
+			writer = StreamWriter.as_bin_var()
+			self.query_bin_block_to_stream(query, writer)
+			return writer.content
+
+	def query_bin_block_to_file(self, cmd: str, file_path: str, append: bool = False) -> None:
+		"""Queries binary data block to the provided file.
+		If append is False, any existing file content is discarded.
+		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
+		Throws an exception if the returned data was not a binary data."""
+		with self._lock:
+			with StreamWriter.as_bin_file(file_path, append) as writer:
+				self.query_bin_block_to_stream(cmd, writer)
+
+	def query_bin_block_to_stream_with_opc(self, query: str, stream: StreamWriter, timeout: int = None) -> None:
+		"""Sends a OPC-synced query and returns data the provided stream.
+		Use it for querying data from instrument to a variable or a file.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			self._session.query_bin_block_with_opc(query, stream, True, timeout)
+			self.end_send_read_event()
+			self._session.query_and_clear_esr()
+			self.check_status()
+
+	def query_bin_block_with_opc(self, query: str, timeout: int = None) -> bytes:
+		"""Sends a OPC-synced query and returns data as bytes.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			with StreamWriter.as_bin_var() as stream:
+				self.query_bin_block_to_stream_with_opc(query, stream, timeout)
+				return stream.content
+
+	def query_bin_block_to_file_with_opc(self, cmd: str, file_path: str, append: bool = False, timeout: int = None) -> None:
+		"""Sends a OPC-synced query and writes the returned data to the provided file.
+		If append is False, any existing file content is discarded.
+		If append is True, the new content is added to the end of the existing file, or if the file does not exit, it is created.
+		Throws an exception if the returned data was not a binary data."""
+		with self._lock:
+			with StreamWriter.as_bin_file(file_path, append) as writer:
+				self.query_bin_block_to_stream_with_opc(cmd, writer, timeout)
+
+	def query_int(self, query: str) -> int:
+		"""Sends a query and reads response from the instrument as integer."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0
+			return Conv.str_to_int(string)
+
+	def query_int_with_opc(self, query: str, timeout: int = None) -> int:
+		"""Sends a OPC-synced query and reads response from the instrument as integer number.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0
+			return Conv.str_to_int(string)
+
+	def query_float(self, query: str) -> float:
+		"""Sends a query and reads response from the instrument as float number."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0.0
+			return Conv.str_to_float(string)
+
+	def query_float_with_opc(self, query: str, timeout: int = None) -> float:
+		"""Sends a OPC-synced query and reads response from the instrument as float number.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return 0.0
+			return Conv.str_to_float(string)
+
+	def query_bool(self, query: str) -> bool:
+		"""Sends a query and reads response from the instrument as boolean value."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return False
+			return Conv.str_to_bool(string)
+
+	def query_bool_with_opc(self, query: str, timeout: int = None) -> bool:
+		"""Sends a OPC-synced query and reads response from the instrument as boolean value.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return False
+			return Conv.str_to_bool(string)
+
+	def query_str_list(self, query: str) -> List[str]:
+		"""Sends a query and reads response from the instrument as csv-list."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
+			response = [trim_str_response(x) for x in string.split(',')]
+			return response
+
+	def query_str_list_with_opc(self, query: str, timeout: int = None) -> List[str]:
+		"""Sends a OPC-synced query and reads response from the instrument as csv-list.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				string = 'AAA,BBB,CCC,DDD,EEE,FFF,GGG,HHH,III,JJJ'
+			response = [trim_str_response(x) for x in string.split(',')]
+			return response
+
+	def write_bin_block_from_stream(self, cmd: str, stream: StreamReader) -> None:
+		"""Writes all the stream content as binary data block to the instrument.
+		Use it for writing data to instrument from a variable or a file.
+		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
+		with self._lock:
+			if self.on_write_handler:
+				self.start_send_write_bin_event(cmd)
+			self._session.write_bin_block(cmd, stream)
+			self.end_send_write_bin_event()
+			self.check_status()
+
+	def write_bin_block(self, cmd: str, payload: bytes) -> None:
+		"""Writes all the payload as binary data block to the instrument.
+		The binary data header is added at the beginning of the transmission automatically, do not include it in the payload!!!"""
+		self.write_bin_block_from_stream(cmd, StreamReader.as_bin_var(payload))
+
+	def write_bin_block_from_file(self, cmd: str, file_path: str) -> None:
+		"""Writes all the file content as binary data block to the instrument.
+		The binary data header is added at the beginning of the transmission automatically, do not include it in the file content!!!"""
+		with StreamReader.as_bin_file(file_path) as reader:
+			self.write_bin_block_from_stream(cmd, reader)
+
+	def query_bin_or_ascii_float_list(self, query: str) -> List[float]:
+		"""Queries a list of floating-point numbers that can be returned in ASCII format or in binary format.
+		- For ASCII format, the list numbers are decoded as comma-separated values.
+		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32)."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			stream = StreamWriter.as_bin_var()
+			self._session.query_bin_block(query, stream, False)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
+			else:
+				result = Conv.str_to_float_list(stream.content)
+			self.check_status()
+			return result
+
+	def query_bin_or_ascii_float_list_with_opc(self, query: str, timeout: int = None) -> List[float]:
+		"""Sends a OPC-synced query and reads a list of floating-point numbers that can be returned in ASCII format or in binary format.
+		- For ASCII format, the list numbers are decoded as comma-separated values.
+		- For Binary Format, the numbers are decoded based on the property BinFloatFormat, usually float 32-bit (FORM REAL,32).
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			stream = StreamWriter.as_bin_var()
+			self._session.query_bin_block_with_opc(query, stream, False, timeout)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
+			else:
+				result = Conv.str_to_float_list(stream.content)
+			self._session.query_and_clear_esr()
+			self.check_status()
+			return result
+
+	def query_bin_or_ascii_float_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[float]:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
+		The current implementation allows for the rest of the string to be only ASCII format."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			response = self._linker.cut_from_response_string(suppressed, string, query)
+			return Conv.str_to_float_list(response)
+
+	def query_bin_or_ascii_float_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[float]:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of floats.
+		If you do not provide timeout, the method uses current opc_timeout.
+		The current implementation allows for the rest of the string to be only ASCII format."""
+		with self._lock:
+			string = self.query_str_with_opc(query, timeout)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
+			response = self._linker.cut_from_response_string(suppressed, string, query)
+			return Conv.str_to_float_list(response)
+
+	def query_bin_or_ascii_int_list(self, query: str) -> List[int]:
+		"""Queries a list of integer numbers that can be returned in ASCII format or in binary format.
+		- For ASCII format, the list numbers are decoded as comma-separated values.
+		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32)."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, False)
+			stream = StreamWriter.as_bin_var()
+			self._session.query_bin_block(query, stream, False)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
+			else:
+				result = Conv.str_to_int_list(stream.content)
+			self.check_status()
+			return result
+
+	def query_bin_or_ascii_int_list_with_opc(self, query: str, timeout: int = None) -> List[int]:
+		"""Sends a OPC-synced query and reads a list of integer numbers that can be returned in ASCII format or in binary format.
+		- For ASCII format, the list numbers are decoded as comma-separated values.
+		- For Binary Format, the numbers are decoded based on the property BinIntFormat, usually int 32-bit (FORM REAL,32).
+		If you do not provide timeout, the method uses current opc_timeout."""
+		with self._lock:
+			query = self._replace_global_repcaps(query)
+			self.start_send_read_event(query, True)
+			stream = StreamWriter.as_bin_var()
+			self._session.query_bin_block_with_opc(query, stream, False, timeout)
+			self.end_send_read_event()
+			if self._simulating and not self._session.cached_to_stream:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			if stream.binary:
+				result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
+			else:
+				result = Conv.str_to_int_list(stream.content)
+			self._session.query_and_clear_esr()
+			self.check_status()
+			return result
+
+	def query_bin_or_ascii_int_list_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> List[int]:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
+		The current implementation allows for the rest of the string to be only ASCII format."""
+		with self._lock:
+			response = self.query_str(query)
+			if self._simulating:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			response = self._linker.cut_from_response_string(suppressed, response, query)
+			return Conv.str_to_int_list(response)
+
+	def query_bin_or_ascii_int_list_suppressed_with_opc(self, query: str, suppressed: ArgSingleSuppressed, timeout: int = None) -> List[int]:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument as list of integers.
+		If you do not provide timeout, the method uses current opc_timeout.
+		The current implementation allows for the rest of the string to be only ASCII format."""
+		with self._lock:
+			response = self.query_str_with_opc(query, timeout)
+			if self._simulating:
+				return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
+			response = self._linker.cut_from_response_string(suppressed, response, query)
+			return Conv.str_to_int_list(response)
+
+	def query_struct(self, query: str, struct: object) -> object:
+		"""Queries string of from instrument, and parses it based on the provided structure object.
+		THe method returns the copy of the entered object that it had modified."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return struct
+			struct_list = ArgStructList(struct)
+			struct_list.parse_from_cmd_response(string)
+			self._linker.invoke_struct_intern_links(struct, struct_list.args, query)
+			return struct
+
+	def query_str_suppressed(self, query: str, suppressed: ArgSingleSuppressed) -> str:
+		"""Queries string of unknown size from instrument, and returns the part without the suppressed argument."""
+		with self._lock:
+			string = self.query_str(query)
+			if self._simulating and self._sim_cached_value_not_found(string):
+				return string
+			response = self._linker.cut_from_response_string(suppressed, string, query)
+			return response
+
+	def self_test(self, timeout: int = None) -> Tuple[int, str]:
+		"""Performs instrument's selftest (*TST?).
+		Returns tuple (code:int, message: str). . Code 0 means the self-test passed.
+		You can define the custom timeout in milliseconds. If you do not define it, the default selftest timeout is used (usually 60 secs)."""
+		with self._lock:
+			if timeout is None or timeout == 0:
+				timeout = self.selftest_timeout
+			response = self.query_str_with_opc('*TST?', timeout)
+			m = re.search(r'^(-?[\d]+)(,(.*))?', response)
+			if not m:
+				raise InstrumentErrors.UnexpectedResponseException(self.resource_name, f"Unexpected response to a '*TST?' self-test query: '{response}'")
+			code = Conv.str_to_int(m.group(1))
+			msg = Utilities.trim_str_response(m.group(3))
+			self.check_status()
+			return code, msg
+
+	def get_session_handle(self) -> object:
+		"""Returns the underlying pyvisa session."""
+		return self._session.get_session_handle()
+
+	def close(self) -> None:
+		"""Closes the Instrument session."""
+		with self._lock:
+			self._session.close()
+			self._session = None
+
+	# Events part
+
+	@property
+	def io_events_include_data(self) -> bool:
+		"""If true, the read and write handlers also include read and written data."""
+		return self._io_events_include_data
+
+	@io_events_include_data.setter
+	def io_events_include_data(self, value: bool) -> None:
+		"""If true, the read and write handlers also include read and written data."""
+		self._io_events_include_data = value
+		self._session.io_events_include_data = value
+
+	def event_args_append_instr_info(self, args: IoTransferEventArgs) -> IoTransferEventArgs:
+		"""Appends instrument-related information to the read/write event argument"""
+		args.chunk_size = self.data_chunk_size
+		args.resource_name = self.resource_name
+		return args
+
+	def send_write_str_event(self, cmd: str, opc_sync: bool) -> None:
+		"""Creates and sends write string event. The transfer is marked as done (end_of_transfer = True)."""
+		args = IoTransferEventArgs.write_str(opc_sync, len(cmd), cmd)
+		args.transferred_size = args.total_size
+		args.chunk_ix = 0
+		args.end_of_transfer = True
+		args = self.event_args_append_instr_info(args)
+		if self._io_events_include_data:
+			args.data = cmd
+		self.on_write_handler(args)
+
+	def start_send_read_event(self, query: str, opc_sync: bool) -> None:
+		"""Registers VisaSession.on_read_chunk_handler() which then generates events with each chunk transfer.
+		Event handler for these events is the local function of this method, which sends IoTransferEventArgs further up to the Instrument.on_read_handler()"""
+		if not self.on_read_handler:
+			return
+
+		def _read_chunk_handler(visa_args: EventArgsChunk) -> None:
+			"""Receives events from VisaSession on read chunk transfers, and sends them as IoTransferEventArgs to the Instrument.on_read_handler()"""
+			args.end_of_transfer = visa_args.end_of_transfer
+			args.chunk_ix = visa_args.chunk_ix
+			args.total_chunks = visa_args.total_chunks
+			args.chunk_size = visa_args.chunk_size
+			args.transferred_size = visa_args.transferred_size
+			args.total_size = visa_args.total_size
+			args.data = visa_args.data
+			args.binary = visa_args.binary
+			self.on_read_handler(args)
+
+		args = IoTransferEventArgs.read_chunk(opc_sync, query)
+		args = self.event_args_append_instr_info(args)
+		self._session.on_read_chunk_handler = _read_chunk_handler
+
+	def end_send_read_event(self):
+		"""Unregisters VisaSession.on_read_chunk_handler()"""
+		self._session.on_read_chunk_handler = None
+
+	def start_send_write_bin_event(self, cmd: str) -> None:
+		"""Registers VisaSession.on_write_chunk_handler() which then generates events with each chunk transfer.
+		Event handler for these events is the local function of this method, which sends IoTransferEventArgs further up to the Instrument.on_write_handler()"""
+		if not self.on_write_handler:
+			return
+
+		def _write_chunk_handler(visa_args: EventArgsChunk) -> None:
+			"""Receives events from VisaSession on write chunk transfers, and sends them as IoTransferEventArgs to the Instrument.on_write_handler()"""
+			args.end_of_transfer = visa_args.end_of_transfer
+			args.chunk_ix = visa_args.chunk_ix
+			args.total_chunks = visa_args.total_chunks
+			args.chunk_size = visa_args.chunk_size
+			args.transferred_size = visa_args.transferred_size
+			args.total_size = visa_args.total_size
+			args.data = visa_args.data
+			args.binary = visa_args.binary
+			self.on_write_handler(args)
+
+		args = IoTransferEventArgs.write_bin(cmd)
+		args = self.event_args_append_instr_info(args)
+		self._session.on_write_chunk_handler = _write_chunk_handler
+
+	def end_send_write_bin_event(self):
+		"""Unregisters VisaSession.on_write_chunk_handler()"""
+		self._session.on_write_chunk_handler = None
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/InstrumentErrors.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/InstrumentErrors.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-class RsInstrException(Exception):
-	"""Exception base class for all the RsInstrument exceptions."""
-	def __init__(self, message: str):
-		super(RsInstrException, self).__init__(message)
-
-
-class TimeoutException(RsInstrException):
-	"""Exception for timeout errors."""
-	def __init__(self, message: str):
-		super(TimeoutException, self).__init__(message)
-
-
-class StatusException(RsInstrException):
-	"""Exception for instrument status errors."""
-	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
-		super(StatusException, self).__init__(message)
-
-
-class UnexpectedResponseException(RsInstrException):
-	"""Exception for instrument unexpected responses."""
-	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
-		super(UnexpectedResponseException, self).__init__(message)
-
-
-class ResourceError(RsInstrException):
-	"""Exception for resource name - e.g. resource not found."""
-	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
-		super(ResourceError, self).__init__(message)
-
-
-class DriverValueError(RsInstrException):
-	"""Exception for different driver value settings e.g. RepCap values or Enum values."""
-	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
-		super(DriverValueError, self).__init__(message)
-
-
-def assert_no_instrument_status_errors(rsrc_name: str, errors: list, context: str = '') -> None:
-	"""Checks the errors list and of it contains at least one element, it throws StatusException."""
-	if errors is None:
-		return
-	if len(errors) == 0:
-		return
-	if context:
-		message = f"'{rsrc_name}': {context} "
-	else:
-		message = f"'{rsrc_name}': "
-	if len(errors) == 1:
-		message += f'Instrument error detected: {errors[0]}'
-		raise StatusException(rsrc_name, message)
-	if len(errors) > 1:
-		message += '{} Instrument errors detected:\n{}'.format(len(errors), '\n'.join(errors))
-		raise StatusException(rsrc_name, message)
-
-
-def throw_opc_tout_exception(opc_tout: int, used_tout: int, context: str = '') -> None:
-	"""Throws TimeoutException - use it for any timeout error."""
-	if not context:
-		message = ''
-	else:
-		message = f'{context} '
-	if used_tout < 0 or used_tout == opc_tout:
-		message = message + f"Timeout expired before the operation completed. Current OPC timeout is set to {opc_tout} milliseconds. " \
-							"Change it with the property '_driver.UtilityFunctions.opc_timeout'. " \
-							"Optionally, if the method API contains an optional timeout parameter, set it there."
-	else:
-		message = message + f"Timeout expired before the operation completed. Used timeout: {used_tout} ms"
-	raise TimeoutException(message)
-
-
-def throw_bin_block_unexp_resp_exception(rsrc_name: str, received_data: str) -> None:
-	"""Throws InvalidDataException - use it in case an instrument response is not a binary block."""
-	if received_data.endswith('\n'):
-		raise UnexpectedResponseException(
-			rsrc_name, "Expected binary data header starting with #(hash), received data '{}'".format(received_data.replace('\n', '\\n')))
-	else:
-		raise UnexpectedResponseException(
-			rsrc_name, f"Expected binary data header starting with #(hash), received data starting with '{received_data}'...")
-
-
-def assert_query_has_qmark(query: str, context: str = '') -> None:
-	"""Throws Exception if the query does not contain any question marks."""
-	if '?' in query:
-		return
-	message = ''
-	if context:
-		message = ' ' + context
-	message = message + "Query commands must contain question-marks. Sent query: '{0}'".format(query.strip('\n'))
-	raise Exception(message)
-
-
-def assert_cmd_has_no_qmark(command: str, context: str = '') -> None:
-	"""Throws Exception if the query contains a question marks."""
-	if '?' not in command:
-		return
-	message = ''
-	if context:
-		message = ' ' + context
-	message = message + "Set commands must not contain question-marks. Sent command: '{0}'".format(command.strip('\n'))
-	raise Exception(message)
+class RsInstrException(Exception):
+	"""Exception base class for all the RsInstrument exceptions."""
+	def __init__(self, message: str):
+		super(RsInstrException, self).__init__(message)
+
+
+class TimeoutException(RsInstrException):
+	"""Exception for timeout errors."""
+	def __init__(self, message: str):
+		super(TimeoutException, self).__init__(message)
+
+
+class StatusException(RsInstrException):
+	"""Exception for instrument status errors."""
+	def __init__(self, rsrc_name: str, message: str):
+		self.rsrc_name = rsrc_name
+		super(StatusException, self).__init__(message)
+
+
+class UnexpectedResponseException(RsInstrException):
+	"""Exception for instrument unexpected responses."""
+	def __init__(self, rsrc_name: str, message: str):
+		self.rsrc_name = rsrc_name
+		super(UnexpectedResponseException, self).__init__(message)
+
+
+class ResourceError(RsInstrException):
+	"""Exception for resource name - e.g. resource not found."""
+	def __init__(self, rsrc_name: str, message: str):
+		self.rsrc_name = rsrc_name
+		super(ResourceError, self).__init__(message)
+
+
+class DriverValueError(RsInstrException):
+	"""Exception for different driver value settings e.g. RepCap values or Enum values."""
+	def __init__(self, rsrc_name: str, message: str):
+		self.rsrc_name = rsrc_name
+		super(DriverValueError, self).__init__(message)
+
+
+def assert_no_instrument_status_errors(rsrc_name: str, errors: list, context: str = '') -> None:
+	"""Checks the errors list and of it contains at least one element, it throws StatusException."""
+	if errors is None:
+		return
+	if len(errors) == 0:
+		return
+	if context:
+		message = f"'{rsrc_name}': {context} "
+	else:
+		message = f"'{rsrc_name}': "
+	if len(errors) == 1:
+		message += f'Instrument error detected: {errors[0]}'
+		raise StatusException(rsrc_name, message)
+	if len(errors) > 1:
+		message += '{} Instrument errors detected:\n{}'.format(len(errors), '\n'.join(errors))
+		raise StatusException(rsrc_name, message)
+
+
+def throw_opc_tout_exception(opc_tout: int, used_tout: int, context: str = '') -> None:
+	"""Throws TimeoutException - use it for any timeout error."""
+	if not context:
+		message = ''
+	else:
+		message = f'{context} '
+	if used_tout < 0 or used_tout == opc_tout:
+		message = message + f"Timeout expired before the operation completed. Current OPC timeout is set to {opc_tout} milliseconds. " \
+							"Change it with the property '_driver.UtilityFunctions.opc_timeout'. " \
+							"Optionally, if the method API contains an optional timeout parameter, set it there."
+	else:
+		message = message + f"Timeout expired before the operation completed. Used timeout: {used_tout} ms"
+	raise TimeoutException(message)
+
+
+def throw_bin_block_unexp_resp_exception(rsrc_name: str, received_data: str) -> None:
+	"""Throws InvalidDataException - use it in case an instrument response is not a binary block."""
+	if received_data.endswith('\n'):
+		raise UnexpectedResponseException(
+			rsrc_name, "Expected binary data header starting with #(hash), received data '{}'".format(received_data.replace('\n', '\\n')))
+	else:
+		raise UnexpectedResponseException(
+			rsrc_name, f"Expected binary data header starting with #(hash), received data starting with '{received_data}'...")
+
+
+def assert_query_has_qmark(query: str, context: str = '') -> None:
+	"""Throws Exception if the query does not contain any question marks."""
+	if '?' in query:
+		return
+	message = ''
+	if context:
+		message = ' ' + context
+	message = message + "Query commands must contain question-marks. Sent query: '{0}'".format(query.strip('\n'))
+	raise Exception(message)
+
+
+def assert_cmd_has_no_qmark(command: str, context: str = '') -> None:
+	"""Throws Exception if the query contains a question marks."""
+	if '?' not in command:
+		return
+	message = ''
+	if context:
+		message = ' ' + context
+	message = message + "Set commands must not contain question-marks. Sent command: '{0}'".format(command.strip('\n'))
+	raise Exception(message)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/InstrumentOptions.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/InstrumentOptions.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import re
-from enum import Enum
-
-from .Utilities import trim_str_response
-
-
-class ParseMode(Enum):
-	"""Options parse mode enum."""
-	Skip = 0
-	KeepOriginal = 1
-	KeepBeforeDash = 2
-	KeepAfterDash = 3
-	Auto = 4
-
-
-class Options(object):
-	_optionsList = []
-
-	def __init__(self, options_str: str, mode=ParseMode.Auto):
-		"""Initializes the options with the *OPT? return string."""
-		self._initialize_from_string(options_str, mode)
-
-	def __str__(self):
-		return ','.join(self._optionsList)
-
-	def _initialize_from_string(self, options_str: str, mode: ParseMode):
-		"""Fills the self._optionsList from the entered 'options_str'."""
-		if mode == ParseMode.Skip:
-			return
-
-		parse_patt = r'(.?)(K|B)(\d+)(.*)$'
-		options = trim_str_response(options_str).split(',')
-		new_opts = []
-		for x in options:
-			has_dash = '-' in x
-			if has_dash:
-				dash_ix = x.index('-')
-				before = x[0:dash_ix + 1].strip('-')
-				after = x[dash_ix:].strip('-')
-
-				if mode is ParseMode.KeepBeforeDash:
-					x = before
-
-				elif mode is ParseMode.KeepAfterDash:
-					x = after
-
-				elif mode is ParseMode.Auto:
-					found_before = re.match(parse_patt, before)
-					found_after = re.match(parse_patt, after)
-					if found_before is not None and found_after is not None:
-						x = after if len(found_after.group(0)) >= len(found_before.group(0)) else before
-					elif found_before is not None:
-						x = before
-					elif found_after is not None:
-						x = after
-
-			if len(x) > 0:
-				new_opts.append(x)
-
-		# Remove duplicates
-		new_opts = set(new_opts)
-
-		# Create a weighting number
-		result = []
-		for x in new_opts:
-			sort_value = x
-			m = re.match(parse_patt, x)
-			if m:
-				kb_weight = '02' if m.group(2) == 'B' else '01'
-				sort_value = '{0}{1}{2:09d}{3}'.format(m.group(1), kb_weight, int(m.group(3)), m.group(4))
-
-			result.append('{0} -> {1}'.format(sort_value, x))
-
-		# Sort keys in that dictionary and then reconstruct the original options
-		result.sort()
-		self._optionsList = [x.split(' -> ')[1] for x in result]
-
-	def get_all(self):
-		"""Returns all the options."""
-		return self._optionsList
+import re
+from enum import Enum
+
+from .Utilities import trim_str_response
+
+
+class ParseMode(Enum):
+	"""Options parse mode enum."""
+	Skip = 0
+	KeepOriginal = 1
+	KeepBeforeDash = 2
+	KeepAfterDash = 3
+	Auto = 4
+
+
+class Options(object):
+	_optionsList = []
+
+	def __init__(self, options_str: str, mode=ParseMode.Auto):
+		"""Initializes the options with the *OPT? return string."""
+		self._initialize_from_string(options_str, mode)
+
+	def __str__(self):
+		return ','.join(self._optionsList)
+
+	def _initialize_from_string(self, options_str: str, mode: ParseMode):
+		"""Fills the self._optionsList from the entered 'options_str'."""
+		if mode == ParseMode.Skip:
+			return
+
+		parse_patt = r'(.?)(K|B)(\d+)(.*)$'
+		options = trim_str_response(options_str).split(',')
+		new_opts = []
+		for x in options:
+			has_dash = '-' in x
+			if has_dash:
+				dash_ix = x.index('-')
+				before = x[0:dash_ix + 1].strip('-')
+				after = x[dash_ix:].strip('-')
+
+				if mode is ParseMode.KeepBeforeDash:
+					x = before
+
+				elif mode is ParseMode.KeepAfterDash:
+					x = after
+
+				elif mode is ParseMode.Auto:
+					found_before = re.match(parse_patt, before)
+					found_after = re.match(parse_patt, after)
+					if found_before is not None and found_after is not None:
+						x = after if len(found_after.group(0)) >= len(found_before.group(0)) else before
+					elif found_before is not None:
+						x = before
+					elif found_after is not None:
+						x = after
+
+			if len(x) > 0:
+				new_opts.append(x)
+
+		# Remove duplicates
+		new_opts = set(new_opts)
+
+		# Create a weighting number
+		result = []
+		for x in new_opts:
+			sort_value = x
+			m = re.match(parse_patt, x)
+			if m:
+				kb_weight = '02' if m.group(2) == 'B' else '01'
+				sort_value = '{0}{1}{2:09d}{3}'.format(m.group(1), kb_weight, int(m.group(3)), m.group(4))
+
+			result.append('{0} -> {1}'.format(sort_value, x))
+
+		# Sort keys in that dictionary and then reconstruct the original options
+		result.sort()
+		self._optionsList = [x.split(' -> ')[1] for x in result]
+
+	def get_all(self):
+		"""Returns all the options."""
+		return self._optionsList
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/InstrumentSettings.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/InstrumentSettings.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-from enum import Enum
-from enum import Flag
-
-from . import InstrumentOptions as Opts, Conversions as Conv
-
-
-class InstrViClearMode(Flag):
-	disabled = 0x00
-	ignore_error = 0x01
-	execute_on_all = 0x02
-	execute_on_socket = 0x04
-	execute_on_serial = 0x08
-	execute_on_usb = 0x10
-	execute_on_gpib = 0x20
-	execute_on_tcpvxi = 0x40
-
-
-class WaitForOpcMode(Enum):
-	"""Mode that is used for OPC-sync commands/queries"""
-	stb_poll = 1
-	stb_poll_slow = 2
-	stb_poll_superslow = 3
-	opc_query = 4
-
-
-class InstrumentSettings(object):
-	"""Defines settings of the instrument."""
-
-	def __init__(
-			self,
-			viclear_exe_mode: InstrViClearMode,
-			idn_model_full_name: bool,
-			write_delay: int,
-			read_delay: int,
-			io_segment_size: int,
-			opc_wait_mode: WaitForOpcMode,
-			opc_timeout: int,
-			visa_timeout: int,
-			self_test_timeout: int,
-			instr_options_parse_mode: Opts.ParseMode,
-			bin_float_numbers_format: Conv.BinFloatFormat,
-			bin_int_numbers_format: Conv.BinIntFormat,
-			opc_query_after_write: bool):
-
-		self.viclear_exe_mode = viclear_exe_mode
-		self.idn_model_full_name = idn_model_full_name
-		self.write_delay = write_delay
-		self.read_delay = read_delay
-		self.io_segment_size = io_segment_size
-		self.opc_wait_mode = opc_wait_mode
-		self.opc_timeout = opc_timeout
-		self.visa_timeout = visa_timeout
-		self.selftest_timeout = self_test_timeout
-		self.instr_options_parse_mode = instr_options_parse_mode
-		self.bin_float_numbers_format = bin_float_numbers_format
-		self.bin_int_numbers_format = bin_int_numbers_format
-		self.opc_query_after_write = opc_query_after_write
-
-		self.assure_write_with_tc = False
-		self.term_char = '\n'
-		self.add_term_char_to_write_bin_block = False
-
-		self.stb_in_error_check = True
-		self.disable_opc_query = False
-		self.visa_select = None
-
-	def apply_option_settings(self, settings: dict) -> None:
-
-		value = settings.get('SELECTVISA')
-		if value is not None:
-			self.visa_select = value
-
-		value = settings.get('DRIVERSETUP_WRITEDELAY')
-		if value is not None:
-			self.write_delay = Conv.str_to_int(value)
-
-		value = settings.get('DRIVERSETUP_READDELAY')
-		if value is not None:
-			self.read_delay = Conv.str_to_int(value)
-
-		value = settings.get('DRIVERSETUP_OPCWAITMODE')
-		if value is not None:
-			value = value.upper()
-			if value == 'STBPOLLING':
-				self.opc_wait_mode = WaitForOpcMode.stb_poll
-			elif value == 'STBPOLLINGSLOW':
-				self.opc_wait_mode = WaitForOpcMode.stb_poll_slow
-			elif value == 'STBPOLLINGSUPERSLOW':
-				self.opc_wait_mode = WaitForOpcMode.stb_poll_superslow
-			elif value == 'OPCQUERY':
-				self.opc_wait_mode = WaitForOpcMode.opc_query
-			else:
-				raise ValueError(
-					f"Unknown value in InitWithOptions string DriverSetup key 'WaitForOPC'. Value '{value}' is not recognized. "
-					"Valid values: 'StbPolling', 'StbPollingSlow', 'StbPollingSuperSlow', 'OpcQuery'")
-
-		value = settings.get('DRIVERSETUP_ADDTERMCHARTOWRITEBINBLOCK')
-		if value is not None:
-			self.add_term_char_to_write_bin_block = Conv.str_to_bool(value)
-
-		# Obsolete, use the DRIVERSETUP_ASSUREWRITEWITHTERMCHAR
-		value = settings.get('DRIVERSETUP_ASSUREWRITEWITHLF')
-		if value is not None:
-			self.assure_write_with_tc = Conv.str_to_bool(value)
-		value = settings.get('DRIVERSETUP_ASSUREWRITEWITHTERMCHAR')
-		if value is not None:
-			self.assure_write_with_tc = Conv.str_to_bool(value)
-
-		value = settings.get('DRIVERSETUP_TERMINATIONCHARACTER')
-		if value is not None:
-			self.term_char = value
-
-		value = settings.get('DRIVERSETUP_IOSEGMENTSIZE')
-		if value is not None:
-			self.io_segment_size = Conv.str_to_int(value)
-
-		value = settings.get('DRIVERSETUP_OPCTIMEOUT')
-		if value is not None:
-			self.opc_timeout = Conv.str_to_int(value)
-
-		value = settings.get('DRIVERSETUP_VISATIMEOUT')
-		if value is not None:
-			self.visa_timeout = Conv.str_to_int(value)
-
-		value = settings.get('DRIVERSETUP_VICLEAREXEMODE')
-		if value is not None:
-			self.viclear_exe_mode = value
-
-		value = settings.get('DRIVERSETUP_OPCQUERYAFTERWRITE')
-		if value is not None:
-			self.opc_query_after_write = Conv.str_to_bool(value)
-
-		value = settings.get('DRIVERSETUP_STBINERRORCHECK')
-		if value is not None:
-			self.stb_in_error_check = Conv.str_to_bool(value)
-
-		value = settings.get('DRIVERSETUP_DISABLEOPCQUERY')
-		if value is not None:
-			self.disable_opc_query = Conv.str_to_bool(value)
-
-		value = settings.get('DRIVERSETUP_QUERYOPT')
-		if value is not None:
-			value = value.upper()
-			if value == 'SKIP':
-				self.instr_options_parse_mode = Opts.ParseMode.Skip
-			elif value == 'AUTO':
-				self.instr_options_parse_mode = Opts.ParseMode.Auto
-			elif value == 'KEEPORIGINAL':
-				self.instr_options_parse_mode = Opts.ParseMode.KeepOriginal
-			elif value == 'KEEPBEFOREDASH':
-				self.instr_options_parse_mode = Opts.ParseMode.KeepBeforeDash
-			elif value == 'KEEPAFTERDASH':
-				self.instr_options_parse_mode = Opts.ParseMode.KeepAfterDash
-			else:
-				raise ValueError(
-					f"Unknown value in InitWithOptions string DriverSetup key 'QueryOpt'. Value '{value}' is not recognized. "
-					"Valid values: 'Skip', 'Auto', 'KeepOriginal', 'KeepBeforeDash', 'KeepAfterDash'")
+from enum import Enum
+from enum import Flag
+
+from . import InstrumentOptions as Opts, Conversions as Conv
+
+
+class InstrViClearMode(Flag):
+	disabled = 0x00
+	ignore_error = 0x01
+	execute_on_all = 0x02
+	execute_on_socket = 0x04
+	execute_on_serial = 0x08
+	execute_on_usb = 0x10
+	execute_on_gpib = 0x20
+	execute_on_tcpvxi = 0x40
+
+
+class WaitForOpcMode(Enum):
+	"""Mode that is used for OPC-sync commands/queries"""
+	stb_poll = 1
+	stb_poll_slow = 2
+	stb_poll_superslow = 3
+	opc_query = 4
+
+
+class InstrumentSettings(object):
+	"""Defines settings of the instrument."""
+
+	def __init__(
+			self,
+			viclear_exe_mode: InstrViClearMode,
+			idn_model_full_name: bool,
+			write_delay: int,
+			read_delay: int,
+			io_segment_size: int,
+			opc_wait_mode: WaitForOpcMode,
+			opc_timeout: int,
+			visa_timeout: int,
+			self_test_timeout: int,
+			instr_options_parse_mode: Opts.ParseMode,
+			bin_float_numbers_format: Conv.BinFloatFormat,
+			bin_int_numbers_format: Conv.BinIntFormat,
+			opc_query_after_write: bool):
+
+		self.viclear_exe_mode = viclear_exe_mode
+		self.idn_model_full_name = idn_model_full_name
+		self.write_delay = write_delay
+		self.read_delay = read_delay
+		self.io_segment_size = io_segment_size
+		self.opc_wait_mode = opc_wait_mode
+		self.opc_timeout = opc_timeout
+		self.visa_timeout = visa_timeout
+		self.selftest_timeout = self_test_timeout
+		self.instr_options_parse_mode = instr_options_parse_mode
+		self.bin_float_numbers_format = bin_float_numbers_format
+		self.bin_int_numbers_format = bin_int_numbers_format
+		self.opc_query_after_write = opc_query_after_write
+
+		self.assure_write_with_tc = False
+		self.term_char = '\n'
+		self.add_term_char_to_write_bin_block = False
+
+		self.stb_in_error_check = True
+		self.disable_opc_query = False
+		self.visa_select = None
+
+	def apply_option_settings(self, settings: dict) -> None:
+
+		value = settings.get('SELECTVISA')
+		if value is not None:
+			self.visa_select = value
+
+		value = settings.get('DRIVERSETUP_WRITEDELAY')
+		if value is not None:
+			self.write_delay = Conv.str_to_int(value)
+
+		value = settings.get('DRIVERSETUP_READDELAY')
+		if value is not None:
+			self.read_delay = Conv.str_to_int(value)
+
+		value = settings.get('DRIVERSETUP_OPCWAITMODE')
+		if value is not None:
+			value = value.upper()
+			if value == 'STBPOLLING':
+				self.opc_wait_mode = WaitForOpcMode.stb_poll
+			elif value == 'STBPOLLINGSLOW':
+				self.opc_wait_mode = WaitForOpcMode.stb_poll_slow
+			elif value == 'STBPOLLINGSUPERSLOW':
+				self.opc_wait_mode = WaitForOpcMode.stb_poll_superslow
+			elif value == 'OPCQUERY':
+				self.opc_wait_mode = WaitForOpcMode.opc_query
+			else:
+				raise ValueError(
+					f"Unknown value in InitWithOptions string DriverSetup key 'WaitForOPC'. Value '{value}' is not recognized. "
+					"Valid values: 'StbPolling', 'StbPollingSlow', 'StbPollingSuperSlow', 'OpcQuery'")
+
+		value = settings.get('DRIVERSETUP_ADDTERMCHARTOWRITEBINBLOCK')
+		if value is not None:
+			self.add_term_char_to_write_bin_block = Conv.str_to_bool(value)
+
+		# Obsolete, use the DRIVERSETUP_ASSUREWRITEWITHTERMCHAR
+		value = settings.get('DRIVERSETUP_ASSUREWRITEWITHLF')
+		if value is not None:
+			self.assure_write_with_tc = Conv.str_to_bool(value)
+		value = settings.get('DRIVERSETUP_ASSUREWRITEWITHTERMCHAR')
+		if value is not None:
+			self.assure_write_with_tc = Conv.str_to_bool(value)
+
+		value = settings.get('DRIVERSETUP_TERMINATIONCHARACTER')
+		if value is not None:
+			self.term_char = value
+
+		value = settings.get('DRIVERSETUP_IOSEGMENTSIZE')
+		if value is not None:
+			self.io_segment_size = Conv.str_to_int(value)
+
+		value = settings.get('DRIVERSETUP_OPCTIMEOUT')
+		if value is not None:
+			self.opc_timeout = Conv.str_to_int(value)
+
+		value = settings.get('DRIVERSETUP_VISATIMEOUT')
+		if value is not None:
+			self.visa_timeout = Conv.str_to_int(value)
+
+		value = settings.get('DRIVERSETUP_VICLEAREXEMODE')
+		if value is not None:
+			self.viclear_exe_mode = value
+
+		value = settings.get('DRIVERSETUP_OPCQUERYAFTERWRITE')
+		if value is not None:
+			self.opc_query_after_write = Conv.str_to_bool(value)
+
+		value = settings.get('DRIVERSETUP_STBINERRORCHECK')
+		if value is not None:
+			self.stb_in_error_check = Conv.str_to_bool(value)
+
+		value = settings.get('DRIVERSETUP_DISABLEOPCQUERY')
+		if value is not None:
+			self.disable_opc_query = Conv.str_to_bool(value)
+
+		value = settings.get('DRIVERSETUP_QUERYOPT')
+		if value is not None:
+			value = value.upper()
+			if value == 'SKIP':
+				self.instr_options_parse_mode = Opts.ParseMode.Skip
+			elif value == 'AUTO':
+				self.instr_options_parse_mode = Opts.ParseMode.Auto
+			elif value == 'KEEPORIGINAL':
+				self.instr_options_parse_mode = Opts.ParseMode.KeepOriginal
+			elif value == 'KEEPBEFOREDASH':
+				self.instr_options_parse_mode = Opts.ParseMode.KeepBeforeDash
+			elif value == 'KEEPAFTERDASH':
+				self.instr_options_parse_mode = Opts.ParseMode.KeepAfterDash
+			else:
+				raise ValueError(
+					f"Unknown value in InitWithOptions string DriverSetup key 'QueryOpt'. Value '{value}' is not recognized. "
+					"Valid values: 'Skip', 'Auto', 'KeepOriginal', 'KeepBeforeDash', 'KeepAfterDash'")
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/InternalLinker.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/InternalLinker.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from time import time
-from typing import Dict, Callable
-
-from . import ArgSingle, ArgSingleSuppressed
-from .ArgLinkedEventArgs import ArgLinkedEventArgs
-from .Utilities import get_plural_string
-
-
-class InternalLinker(object):
-	"""Class for:
-		- cutting out suppressed arguments from a device response.
-		- invoking a handler if the argument has InternalLinking defined.
-		- holds dictionary of handlers where the dict_key is the InternalLinking string.
-	Handlers registration/deleting is done with:
-		- set_handler()
-		- del_handler()
-		- del_all_handlers()"""
-
-	def __init__(self):
-		self._handlers = {}
-
-	def __str__(self):
-		if len(self._handlers) == 0:
-			return 'Linker, no handlers'
-		return f"Linker, {get_plural_string('handler', len(self._handlers))}: {','.join(self._handlers)}"
-
-	def set_handler(self, link_name: str, handler: Callable) -> Callable:
-		"""Adds / Updates handler for the link_name.
-		Returns the previous registered handler, or None if no handler was registered before."""
-		previous = None if link_name not in self._handlers else self._handlers[link_name]
-		self._handlers[link_name] = handler
-		return previous
-
-	def del_handler(self, link_name: str) -> Callable:
-		"""Deletes handler for the link_name.
-		Returns the deleted handler, or None if none existed."""
-		current = None if link_name not in self._handlers else self._handlers[link_name]
-		if current:
-			del self._handlers[link_name]
-		return current
-
-	def del_all_handlers(self) -> int:
-		"""Deletes all the handlers.
-		Returns number of deleted links."""
-		count = len(self._handlers)
-		self._handlers = {}
-		return count
-
-	def cut_from_response_string(self, arg: ArgSingleSuppressed, response: str, context: str) -> str:
-		"""Takes the string 'response', removes the suppressed argument value from it and returns the rest.
-		The cut out part is sent via handler if the internal linking exists for that argument exists."""
-		result = ''
-		if arg.argument_ix is None:
-			raise Exception(f'Argument has argument_ix attribute not assigned (equals None). Argument: {arg}')
-		if arg.argument_ix != 0:
-			raise Exception(f'Only arguments with index 0 can be suppressed. Argument: {arg}')
-		if arg.is_open_list:
-			raise Exception(f'Open List arguments can not be suppressed. Argument: {arg}')
-		repetition = 0
-		i = 0
-		for c in response:
-			if c == ',':
-				repetition += 1
-			if repetition == arg.repetition:
-				break
-			i += 1
-
-		suppressed_part = response[0:i]
-		i += 1
-		if i < len(response):
-			result = response[i:]
-
-		self.invoke_single_intern_link(arg, context, suppressed_part)
-		return result
-
-	def invoke_single_intern_link(self, arg: ArgSingleSuppressed or ArgSingle, context: str, value: str) -> None:
-		"""Invokes the registered handler for the internal linked argument."""
-		if arg.intern_link and arg.intern_link in self._handlers:
-			event_args = ArgLinkedEventArgs(arg.intern_link, arg.name, value, context, time())
-			self._handlers[arg.intern_link](event_args)
-
-	def invoke_struct_intern_links(self, struct, args: Dict, context: str) -> None:
-		"""Invokes handler for each of the Structure arguments that have internal linking."""
-		for arg in args.values():
-			if arg.intern_link and arg.intern_link in self._handlers:
-				event_args = ArgLinkedEventArgs(arg.intern_link, arg.name, getattr(struct, arg.name), context, time())
-				self._handlers[arg.intern_link](event_args)
+from time import time
+from typing import Dict, Callable
+
+from . import ArgSingle, ArgSingleSuppressed
+from .ArgLinkedEventArgs import ArgLinkedEventArgs
+from .Utilities import get_plural_string
+
+
+class InternalLinker(object):
+	"""Class for:
+		- cutting out suppressed arguments from a device response.
+		- invoking a handler if the argument has InternalLinking defined.
+		- holds dictionary of handlers where the dict_key is the InternalLinking string.
+	Handlers registration/deleting is done with:
+		- set_handler()
+		- del_handler()
+		- del_all_handlers()"""
+
+	def __init__(self):
+		self._handlers = {}
+
+	def __str__(self):
+		if len(self._handlers) == 0:
+			return 'Linker, no handlers'
+		return f"Linker, {get_plural_string('handler', len(self._handlers))}: {','.join(self._handlers)}"
+
+	def set_handler(self, link_name: str, handler: Callable) -> Callable:
+		"""Adds / Updates handler for the link_name.
+		Returns the previous registered handler, or None if no handler was registered before."""
+		previous = None if link_name not in self._handlers else self._handlers[link_name]
+		self._handlers[link_name] = handler
+		return previous
+
+	def del_handler(self, link_name: str) -> Callable:
+		"""Deletes handler for the link_name.
+		Returns the deleted handler, or None if none existed."""
+		current = None if link_name not in self._handlers else self._handlers[link_name]
+		if current:
+			del self._handlers[link_name]
+		return current
+
+	def del_all_handlers(self) -> int:
+		"""Deletes all the handlers.
+		Returns number of deleted links."""
+		count = len(self._handlers)
+		self._handlers = {}
+		return count
+
+	def cut_from_response_string(self, arg: ArgSingleSuppressed, response: str, context: str) -> str:
+		"""Takes the string 'response', removes the suppressed argument value from it and returns the rest.
+		The cut out part is sent via handler if the internal linking exists for that argument exists."""
+		result = ''
+		if arg.argument_ix is None:
+			raise Exception(f'Argument has argument_ix attribute not assigned (equals None). Argument: {arg}')
+		if arg.argument_ix != 0:
+			raise Exception(f'Only arguments with index 0 can be suppressed. Argument: {arg}')
+		if arg.is_open_list:
+			raise Exception(f'Open List arguments can not be suppressed. Argument: {arg}')
+		repetition = 0
+		i = 0
+		for c in response:
+			if c == ',':
+				repetition += 1
+			if repetition == arg.repetition:
+				break
+			i += 1
+
+		suppressed_part = response[0:i]
+		i += 1
+		if i < len(response):
+			result = response[i:]
+
+		self.invoke_single_intern_link(arg, context, suppressed_part)
+		return result
+
+	def invoke_single_intern_link(self, arg: ArgSingleSuppressed or ArgSingle, context: str, value: str) -> None:
+		"""Invokes the registered handler for the internal linked argument."""
+		if arg.intern_link and arg.intern_link in self._handlers:
+			event_args = ArgLinkedEventArgs(arg.intern_link, arg.name, value, context, time())
+			self._handlers[arg.intern_link](event_args)
+
+	def invoke_struct_intern_links(self, struct, args: Dict, context: str) -> None:
+		"""Invokes handler for each of the Structure arguments that have internal linking."""
+		for arg in args.values():
+			if arg.intern_link and arg.intern_link in self._handlers:
+				event_args = ArgLinkedEventArgs(arg.intern_link, arg.name, getattr(struct, arg.name), context, time())
+				self._handlers[arg.intern_link](event_args)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/RepeatedCapability.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/RepeatedCapability.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,92 @@
-from enum import Enum
-
-
-# Command integer value that signals Default value "DEFAULT"
-VALUE_DEFAULT = -1
-
-# Command integer value that signals "EMPTY"
-VALUE_EMPTY = -2
-
-
-class RepeatedCapability(object):
-	"""Represents Repeated Capability value and type"""
-
-	def __init__(self, header_name: str, method_get_name: str, method_set_name: str, start_value: Enum):
-		"""Constructor with header name, group property name and the start value"""
-
-		self._enum_value = None
-		self.enum_type = start_value.__class__
-		self.name = self.enum_type.__name__
-		self.header_name = header_name
-		self.method_get_name = method_get_name
-		self.method_set_name = method_set_name
-		self._start_value = start_value
-		self.set_to_start_value()
-
-	def __str__(self) -> str:
-		out = f'RepCap {self.name}'
-		if self._enum_value is not None:
-			out += f" = {self._enum_value}"
-		return out
-
-	@classmethod
-	def clsm_assert_type(cls, enum_value: Enum, enum_type) -> None:
-		"""Static assertion function to check if the entered value is a member of the defined repcap enum"""
-		if not isinstance(enum_value, enum_type):
-			raise TypeError(f"RepCap value must be of type '{enum_type}'. Entered value type: {type(enum_value)}, value '{enum_value}'")
-
-	@classmethod
-	def clsm_get_direct_cmd_value_int(cls, enum_value: Enum, enum_type) -> int:
-		"""Static function to get an integer interpretation of a direct enum value
-		Does not work with Empty or Default"""
-		RepeatedCapability.clsm_assert_type(enum_value, enum_type)
-		return enum_value.value
-
-	@classmethod
-	def clsm_is_default_value(cls, enum_value: Enum, enum_type) -> bool:
-		"""Returns True, if the entered value is enum.Default"""
-		return cls.clsm_get_direct_cmd_value_int(enum_value, enum_type) == VALUE_DEFAULT
-
-	def is_default_value(self) -> bool:
-		"""Returns True, if the repcap value is enum.Default"""
-		return RepeatedCapability.clsm_is_default_value(self._enum_value, self.enum_type)
-
-	def set_enum_value(self, enum_value: Enum) -> None:
-		"""Sets new enum value. Can not be Default"""
-		if RepeatedCapability.clsm_is_default_value(enum_value, self.enum_type):
-			raise ValueError(f"Setting RepCap enum value '{enum_value}' is not allowed. Please select a concrete value")
-		self._enum_value = enum_value
-
-	def get_enum_value(self) -> Enum:
-		"""Returns the actual enum value"""
-		return self._enum_value
-
-	def set_to_start_value(self) -> None:
-		"""Sets back to the value entered in the constructor"""
-		self.set_enum_value(self._start_value)
-
-	def matches_type(self, enum_type) -> bool:
-		"""Returns true, if the entered type matches the EnumType"""
-		return self.enum_type == enum_type
-
-	@classmethod
-	def clsm_get_cmd_string_value(cls, enum_value: Enum, enum_type) -> str:
-		"""Converts RepCap integer value to string
-		ValueEmpty is converted to "" (Not valid, but tolerated)
-		ValueDefault throws an exception
-		0 is converted to "" (Not valid, but tolerated)
-		Positive numbers are converted to integer strings e.g. 1 => '1' """
-		number = cls.clsm_get_direct_cmd_value_int(enum_value, enum_type)
-		if number == VALUE_EMPTY:
-			return ''
-		if number == 0:
-			# return empty string, if the enum definition does not contain a valid element with value 0
-			enum_values = [x.value for x in enum_type]
-			return '0' if 0 in enum_values else ''
-		if number == VALUE_DEFAULT:
-			raise ValueError(f"RepCap enum value Default can not be converted to the command string value. RepCap: {enum_type}")
-		return str(number)
-
-	def get_cmd_string_value(self) -> str:
-		"""Converts RepCap integer value to string
-		ValueEmpty is converted to "" (Not valid, but tolerated)
-		ValueDefault throws an exception
-		0 is converted to "" (Not valid, but tolerated)
-		Positive numbers are converted to integer strings e.g. 1 => '1' """
-		return RepeatedCapability.clsm_get_cmd_string_value(self._enum_value, self.enum_type)
+from enum import Enum
+
+
+# Command integer value that signals Default value "DEFAULT"
+VALUE_DEFAULT = -1
+
+# Command integer value that signals "EMPTY"
+VALUE_EMPTY = -2
+
+
+class RepeatedCapability(object):
+	"""Represents Repeated Capability value and type"""
+
+	def __init__(self, header_name: str, method_get_name: str, method_set_name: str, start_value: Enum):
+		"""Constructor with header name, group property name and the start value"""
+
+		self._enum_value = None
+		self.enum_type = start_value.__class__
+		self.name = self.enum_type.__name__
+		self.header_name = header_name
+		self.method_get_name = method_get_name
+		self.method_set_name = method_set_name
+		self._start_value = start_value
+		self.set_to_start_value()
+
+	def __str__(self) -> str:
+		out = f'RepCap {self.name}'
+		if self._enum_value is not None:
+			out += f" = {self._enum_value}"
+		return out
+
+	@classmethod
+	def clsm_assert_type(cls, enum_value: Enum, enum_type) -> None:
+		"""Static assertion function to check if the entered value is a member of the defined repcap enum"""
+		if not isinstance(enum_value, enum_type):
+			raise TypeError(f"RepCap value must be of type '{enum_type}'. Entered value type: {type(enum_value)}, value '{enum_value}'")
+
+	@classmethod
+	def clsm_get_direct_cmd_value_int(cls, enum_value: Enum, enum_type) -> int:
+		"""Static function to get an integer interpretation of a direct enum value
+		Does not work with Empty or Default"""
+		RepeatedCapability.clsm_assert_type(enum_value, enum_type)
+		return enum_value.value
+
+	@classmethod
+	def clsm_is_default_value(cls, enum_value: Enum, enum_type) -> bool:
+		"""Returns True, if the entered value is enum.Default"""
+		return cls.clsm_get_direct_cmd_value_int(enum_value, enum_type) == VALUE_DEFAULT
+
+	def is_default_value(self) -> bool:
+		"""Returns True, if the repcap value is enum.Default"""
+		return RepeatedCapability.clsm_is_default_value(self._enum_value, self.enum_type)
+
+	def set_enum_value(self, enum_value: Enum) -> None:
+		"""Sets new enum value. Can not be Default"""
+		if RepeatedCapability.clsm_is_default_value(enum_value, self.enum_type):
+			raise ValueError(f"Setting RepCap enum value '{enum_value}' is not allowed. Please select a concrete value")
+		self._enum_value = enum_value
+
+	def get_enum_value(self) -> Enum:
+		"""Returns the actual enum value"""
+		return self._enum_value
+
+	def set_to_start_value(self) -> None:
+		"""Sets back to the value entered in the constructor"""
+		self.set_enum_value(self._start_value)
+
+	def matches_type(self, enum_type) -> bool:
+		"""Returns true, if the entered type matches the EnumType"""
+		return self.enum_type == enum_type
+
+	@classmethod
+	def clsm_get_cmd_string_value(cls, enum_value: Enum, enum_type) -> str:
+		"""Converts RepCap integer value to string
+		ValueEmpty is converted to "" (Not valid, but tolerated)
+		ValueDefault throws an exception
+		0 is converted to "" (Not valid, but tolerated)
+		Positive numbers are converted to integer strings e.g. 1 => '1' """
+		number = cls.clsm_get_direct_cmd_value_int(enum_value, enum_type)
+		if number == VALUE_EMPTY or number == 0:
+			return ''
+		if number == VALUE_DEFAULT:
+			raise ValueError(f"RepCap enum value Default can not be converted to the command string value. RepCap: {enum_type}")
+		return str(number)
+
+	def get_cmd_string_value(self) -> str:
+		"""Converts RepCap integer value to string
+		ValueEmpty is converted to "" (Not valid, but tolerated)
+		ValueDefault throws an exception
+		0 is converted to "" (Not valid, but tolerated)
+		Positive numbers are converted to integer strings e.g. 1 => '1' """
+		return RepeatedCapability.clsm_get_cmd_string_value(self._enum_value, self.enum_type)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/StreamReader.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/StreamReader.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-from enum import Enum
-from os import path
-from typing import AnyStr
-
-from .Utilities import size_to_kb_mb_string
-
-
-class Type(Enum):
-	Variable = 1
-	File = 2
-
-
-class StreamReader:
-	"""Lightweight stream reader implementation. Data source can be: \n
-	- variable
-	- file"""
-
-	def __init__(self, binary: bool, source: Type, data: AnyStr):
-		"""Initializes StreamReader instance.\n
-		:param binary: True: Binary data, False: ASCII data
-		:param source: Source type for the stream. Variable / File
-		:param data: Depending on the 'binary' and 'source':
-		For source type Variable the data must be either bytes() or str
-		For source type File data must be string with existing file path."""
-		self._source = source
-		self._binary = binary
-		self._start_ptr = 0
-
-		if self._source == Type.Variable:
-			if self._binary:
-				assert isinstance(data, bytes), f'Data must be of bytes type. Actual type: {type(data)}'
-			else:
-				assert isinstance(data, str), f'Data must be of string type. Actual type: {type(data)}'
-			self._data = data
-			self._full_len = len(self._data)
-		elif self._source == Type.File:
-			assert isinstance(data, str), f'Data must be of string type (file path). Actual type: {type(data)}'
-			if not path.isfile(data):
-				raise Exception(f'File does not exist. File path: {data}')
-			self.file_path = data
-			self._data = open(self.file_path, 'rb' if self._binary else 'r')
-			self._full_len = path.getsize(self.file_path)
-		else:
-			raise Exception(f'StreamReader unknown type {source}')
-
-	@classmethod
-	def as_bin_var(cls, data: bytes) -> 'StreamReader':
-		"""Creates new StreamReader from bytes.
-		:param data: [bytes] data for the stream."""
-		return cls(True, Type.Variable, data)
-
-	@classmethod
-	def as_string_var(cls, data: str) -> 'StreamReader':
-		"""Creates new StreamReader from string.
-		:param data: [str] data for the stream."""
-		return cls(False, Type.Variable, data)
-
-	@classmethod
-	def as_bin_file(cls, file_path: str) -> 'StreamReader':
-		"""Creates new StreamReader from binary file. The file must exist at this time.
-		:param file_path: [str] Path to the file."""
-		return cls(True, Type.File, file_path)
-
-	@classmethod
-	def as_text_file(cls, file_path: str) -> 'StreamReader':
-		"""Creates new StreamReader from text file. The file must exist at this time.
-		:param file_path: [str] Path to the file."""
-		return cls(False, Type.File, file_path)
-
-	def __str__(self):
-		if self._source == Type.Variable:
-			mode = 'binary' if self._binary else 'string'
-			return f'StreamReader {mode} data, full size {size_to_kb_mb_string(self._full_len, True)}, remaining size {size_to_kb_mb_string(len(self), True)}'
-		if self._source == Type.File:
-			mode = 'binary' if self._binary else 'text'
-			return f'StreamReader {mode}, full size {size_to_kb_mb_string(self._full_len, True)}, remaining size {size_to_kb_mb_string(len(self), True)}'
-
-	def __len__(self):
-		"""Returns remaining length."""
-		return self._full_len - self._start_ptr
-
-	def __enter__(self):
-		return self
-
-	def __exit__(self, exception_type, exception_value, traceback):
-		self.close()
-
-	@property
-	def full_len(self) -> int:
-		"""Returns original full length."""
-		return self._full_len
-
-	@property
-	def binary(self) -> bool:
-		"""Returns true, if the data provided is binary."""
-		return self._binary
-
-	def read(self, chunk_size: int = None) -> AnyStr:
-		"""Read chunk from the data and moves the data pointer behind it.
-		If the remaining length is smaller than the chunk_size, the method returns the remaining length only.
-		:param chunk_size: chunk to read. If not set, the method reads the entire data."""
-		assert self._data is not None, 'StreamReader buffer is invalid. You have probably closed it already.'
-		chunk_size = len(self) if chunk_size is None else chunk_size
-		chunk_size = min(chunk_size, len(self))
-		if chunk_size < 0:
-			raise ValueError(f'Chunk size can not be negative number: {chunk_size}')
-
-		if self._source == Type.Variable:
-			self._start_ptr += chunk_size
-			return self._data[self._start_ptr - chunk_size: self._start_ptr]
-		elif self._source == Type.File:
-			self._start_ptr += chunk_size
-			return self._data.read(chunk_size)
-
-	def read_as_binary(self, chunk_size: int = None) -> bytes:
-		"""Same as read(), but always returns the data in binary format.
-		Practically works exactly as read() for binary streams.
-		For string streams, the method converts the returned data using utf-8 encoding to bytes()."""
-		if self._binary:
-			return self.read(chunk_size)
-		else:
-			return self.read(chunk_size).encode('utf-8')
-
-	def close(self):
-		"""Closes the StreamReader. You can not use its instance afterwards."""
-		if self._source == Type.File and self._data:
-			self._data.close()
-		self._data = None
+from enum import Enum
+from os import path
+from typing import AnyStr
+
+from .Utilities import size_to_kb_mb_string
+
+
+class Type(Enum):
+	Variable = 1
+	File = 2
+
+
+class StreamReader:
+	"""Lightweight stream reader implementation. Data source can be: \n
+	- variable
+	- file"""
+
+	def __init__(self, binary: bool, source: Type, data: AnyStr):
+		"""Initializes StreamReader instance.\n
+		:param binary: True: Binary data, False: ASCII data
+		:param source: Source type for the stream. Variable / File
+		:param data: Depending on the 'binary' and 'source':
+		For source type Variable the data must be either bytes() or str
+		For source type File data must be string with existing file path."""
+		self._source = source
+		self._binary = binary
+		self._start_ptr = 0
+
+		if self._source == Type.Variable:
+			if self._binary:
+				assert isinstance(data, bytes), f'Data must be of bytes type. Actual type: {type(data)}'
+			else:
+				assert isinstance(data, str), f'Data must be of string type. Actual type: {type(data)}'
+			self._data = data
+			self._full_len = len(self._data)
+		elif self._source == Type.File:
+			assert isinstance(data, str), f'Data must be of string type (file path). Actual type: {type(data)}'
+			if not path.isfile(data):
+				raise Exception(f'File does not exist. File path: {data}')
+			self.file_path = data
+			self._data = open(self.file_path, 'rb' if self._binary else 'r')
+			self._full_len = path.getsize(self.file_path)
+		else:
+			raise Exception(f'StreamReader unknown type {source}')
+
+	@classmethod
+	def as_bin_var(cls, data: bytes) -> 'StreamReader':
+		"""Creates new StreamReader from bytes.
+		:param data: [bytes] data for the stream."""
+		return cls(True, Type.Variable, data)
+
+	@classmethod
+	def as_string_var(cls, data: str) -> 'StreamReader':
+		"""Creates new StreamReader from string.
+		:param data: [str] data for the stream."""
+		return cls(False, Type.Variable, data)
+
+	@classmethod
+	def as_bin_file(cls, file_path: str) -> 'StreamReader':
+		"""Creates new StreamReader from binary file. The file must exist at this time.
+		:param file_path: [str] Path to the file."""
+		return cls(True, Type.File, file_path)
+
+	@classmethod
+	def as_text_file(cls, file_path: str) -> 'StreamReader':
+		"""Creates new StreamReader from text file. The file must exist at this time.
+		:param file_path: [str] Path to the file."""
+		return cls(False, Type.File, file_path)
+
+	def __str__(self):
+		if self._source == Type.Variable:
+			mode = 'binary' if self._binary else 'string'
+			return f'StreamReader {mode} data, full size {size_to_kb_mb_string(self._full_len, True)}, remaining size {size_to_kb_mb_string(len(self), True)}'
+		if self._source == Type.File:
+			mode = 'binary' if self._binary else 'text'
+			return f'StreamReader {mode}, full size {size_to_kb_mb_string(self._full_len, True)}, remaining size {size_to_kb_mb_string(len(self), True)}'
+
+	def __len__(self):
+		"""Returns remaining length."""
+		return self._full_len - self._start_ptr
+
+	def __enter__(self):
+		return self
+
+	def __exit__(self, exception_type, exception_value, traceback):
+		self.close()
+
+	@property
+	def full_len(self) -> int:
+		"""Returns original full length."""
+		return self._full_len
+
+	@property
+	def binary(self) -> bool:
+		"""Returns true, if the data provided is binary."""
+		return self._binary
+
+	def read(self, chunk_size: int = None) -> AnyStr:
+		"""Read chunk from the data and moves the data pointer behind it.
+		If the remaining length is smaller than the chunk_size, the method returns the remaining length only.
+		:param chunk_size: chunk to read. If not set, the method reads the entire data."""
+		assert self._data is not None, 'StreamReader buffer is invalid. You have probably closed it already.'
+		chunk_size = len(self) if chunk_size is None else chunk_size
+		chunk_size = min(chunk_size, len(self))
+		if chunk_size < 0:
+			raise ValueError(f'Chunk size can not be negative number: {chunk_size}')
+
+		if self._source == Type.Variable:
+			self._start_ptr += chunk_size
+			return self._data[self._start_ptr - chunk_size: self._start_ptr]
+		elif self._source == Type.File:
+			self._start_ptr += chunk_size
+			return self._data.read(chunk_size)
+
+	def read_as_binary(self, chunk_size: int = None) -> bytes:
+		"""Same as read(), but always returns the data in binary format.
+		Practically works exactly as read() for binary streams.
+		For string streams, the method converts the returned data using utf-8 encoding to bytes()."""
+		if self._binary:
+			return self.read(chunk_size)
+		else:
+			return self.read(chunk_size).encode('utf-8')
+
+	def close(self):
+		"""Closes the StreamReader. You can not use its instance afterwards."""
+		if self._source == Type.File and self._data:
+			self._data.close()
+		self._data = None
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/StreamWriter.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/StreamWriter.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-from enum import Flag
-from typing import AnyStr
-
-from .Utilities import size_to_kb_mb_string
-
-
-class Type(Flag):
-	Variable = 1
-	File = 2
-	FileAppend = 6
-
-
-class StreamWriter:
-	"""Lightweight stream writer implementation. Data target can be: \n
-	- bytes
-	- string
-	- file"""
-
-	def __init__(self, binary: bool, target: Type, meta_data=None):
-		"""Initializes StreamWriter instance.\n
-		:param binary: True: Binary data, False: ASCII data
-		:param target: Target for the stream. Variable / File (FileAppend)
-		:param meta_data: Only valid for File and FileAppend - define file path as string:
-		For Type.File, data must be string with file path. If the file exists, it will be overwritten.
-		For Type.FileAppend, data must be string with file path. If the file exists, it will be appended."""
-		self._binary = binary
-		self._written_len = 0
-		self._target = target
-
-		if Type.Variable in self._target:
-			assert meta_data is None, f'You can not define input meta_data for a Variable StreamWriter.'
-			self._data: AnyStr = bytes() if binary else ''
-		elif Type.File in self._target:
-			assert isinstance(meta_data, str), f'Additional data must be of string type (file path). Actual type: {type(meta_data)}'
-			self._file_path = meta_data
-			mode = 'w' if self._target == Type.File else 'a'
-			mode += 'b' if self._binary else ''
-			self._data = open(self._file_path, mode)
-		else:
-			raise Exception(f'StreamWriter unknown target {target}')
-
-	@classmethod
-	def as_bin_var(cls) -> 'StreamWriter':
-		"""Creates new StreamWriter with bytes variable."""
-		return cls(True, Type.Variable)
-
-	@classmethod
-	def as_string_var(cls) -> 'StreamWriter':
-		"""Creates new StreamWriter with string variable."""
-		return cls(False, Type.Variable)
-
-	@classmethod
-	def as_bin_file(cls, file_path: str, append: bool = False) -> 'StreamWriter':
-		"""Creates new StreamWriter to binary file.
-		:param file_path: [str] Path to the file.
-		:param append: Optional [bool] If True, the content is appended to the existing content."""
-		return cls(True, Type.FileAppend if append else Type.File, file_path)
-
-	@classmethod
-	def as_text_file(cls, file_path: str, append: bool = False) -> 'StreamWriter':
-		"""Creates new StreamWriter to text file.
-		:param file_path: [str] Path to the file.
-		:param append: Optional [bool] If True, the content is appended to the existing content."""
-		return cls(False, Type.FileAppend if append else Type.File, file_path)
-
-	def __str__(self):
-		if Type.Variable in self._target:
-			mode = 'binary' if self._binary else 'string'
-			return f'StreamWriter {mode} variable, current size {size_to_kb_mb_string(len(self), True)}'
-		if Type.File in self._target:
-			mode = 'binary' if self._binary else 'text'
-			append = ' appended' if Type.FileAppend in self._target else ''
-			return f'StreamWriter {mode} file{append}, current{append} size {size_to_kb_mb_string(len(self), True)}, file: {self._file_path}'
-
-	def __len__(self):
-		"""Returns remaining length."""
-		return self._written_len
-
-	def __enter__(self):
-		return self
-
-	def __exit__(self, exception_type, exception_value, traceback):
-		self.close()
-
-	@property
-	def binary(self) -> bool:
-		"""Returns true, if the data held is binary.
-		File streams are always binary."""
-		return self._binary
-
-	def write(self, data: AnyStr) -> None:
-		"""Writes chunk to the stream.
-			- For Type.Bytes data must be bytes.
-			- For Type.String, data must be string.
-			- For Type.File and Type.FileAppend, data must be bytes"""
-		assert self._data is not None, 'StreamWriter buffer is invalid. You have probably closed it already.'
-		if self._binary:
-			assert isinstance(data, bytes), f'Bytes data is required. Actual type: {type(data)}. {self}'
-		else:
-			assert isinstance(data, str), f'String data is required. Actual type: {type(data)}. {self}'
-
-		if Type.Variable in self._target:
-			self._data += data
-		elif Type.File in self._target:
-			self._data.write(data)
-		self._written_len += len(data)
-
-	def switch_to_string_data(self) -> None:
-		"""Switches from binary to string data.
-		For variables, the current content is converted.
-		For files, they are closed and reopened as for appended text writing."""
-		if self._binary is False:
-			return
-		self._binary = False
-		if Type.Variable in self._target:
-			if len(self) == 0:
-				self._data = ''
-			else:
-				# noinspection PyUnresolvedReferences
-				self._data = self._data.decode('utf-8')
-		elif Type.File in self._target:
-			self._data.close()
-			self._data = open(self._file_path, 'a')
-
-	@property
-	def content(self) -> AnyStr:
-		"""Returns content of the writer. Does only work with variable types."""
-		assert Type.Variable in self._target, f'Can not return content for the current {self}'
-		# noinspection PyTypeChecker
-		return self._data
-
-	def close(self) -> None:
-		"""Closes the StreamWriter. You can not use its instance afterwards."""
-		if Type.File in self._target and self._data:
-			self._data.close()
-		self._data = None
+from enum import Flag
+from typing import AnyStr
+
+from .Utilities import size_to_kb_mb_string
+
+
+class Type(Flag):
+	Variable = 1
+	File = 2
+	FileAppend = 6
+
+
+class StreamWriter:
+	"""Lightweight stream writer implementation. Data target can be: \n
+	- bytes
+	- string
+	- file"""
+
+	def __init__(self, binary: bool, target: Type, meta_data=None):
+		"""Initializes StreamWriter instance.\n
+		:param binary: True: Binary data, False: ASCII data
+		:param target: Target for the stream. Variable / File (FileAppend)
+		:param meta_data: Only valid for File and FileAppend - define file path as string:
+		For Type.File, data must be string with file path. If the file exists, it will be overwritten.
+		For Type.FileAppend, data must be string with file path. If the file exists, it will be appended."""
+		self._binary = binary
+		self._written_len = 0
+		self._target = target
+
+		if Type.Variable in self._target:
+			assert meta_data is None, f'You can not define input meta_data for a Variable StreamWriter.'
+			self._data: AnyStr = bytes() if binary else ''
+		elif Type.File in self._target:
+			assert isinstance(meta_data, str), f'Additional data must be of string type (file path). Actual type: {type(meta_data)}'
+			self._file_path = meta_data
+			mode = 'w' if self._target == Type.File else 'a'
+			mode += 'b' if self._binary else ''
+			self._data = open(self._file_path, mode)
+		else:
+			raise Exception(f'StreamWriter unknown target {target}')
+
+	@classmethod
+	def as_bin_var(cls) -> 'StreamWriter':
+		"""Creates new StreamWriter with bytes variable."""
+		return cls(True, Type.Variable)
+
+	@classmethod
+	def as_string_var(cls) -> 'StreamWriter':
+		"""Creates new StreamWriter with string variable."""
+		return cls(False, Type.Variable)
+
+	@classmethod
+	def as_bin_file(cls, file_path: str, append: bool = False) -> 'StreamWriter':
+		"""Creates new StreamWriter to binary file.
+		:param file_path: [str] Path to the file.
+		:param append: Optional [bool] If True, the content is appended to the existing content."""
+		return cls(True, Type.FileAppend if append else Type.File, file_path)
+
+	@classmethod
+	def as_text_file(cls, file_path: str, append: bool = False) -> 'StreamWriter':
+		"""Creates new StreamWriter to text file.
+		:param file_path: [str] Path to the file.
+		:param append: Optional [bool] If True, the content is appended to the existing content."""
+		return cls(False, Type.FileAppend if append else Type.File, file_path)
+
+	def __str__(self):
+		if Type.Variable in self._target:
+			mode = 'binary' if self._binary else 'string'
+			return f'StreamWriter {mode} variable, current size {size_to_kb_mb_string(len(self), True)}'
+		if Type.File in self._target:
+			mode = 'binary' if self._binary else 'text'
+			append = ' appended' if Type.FileAppend in self._target else ''
+			return f'StreamWriter {mode} file{append}, current{append} size {size_to_kb_mb_string(len(self), True)}, file: {self._file_path}'
+
+	def __len__(self):
+		"""Returns remaining length."""
+		return self._written_len
+
+	def __enter__(self):
+		return self
+
+	def __exit__(self, exception_type, exception_value, traceback):
+		self.close()
+
+	@property
+	def binary(self) -> bool:
+		"""Returns true, if the data held is binary.
+		File streams are always binary."""
+		return self._binary
+
+	def write(self, data: AnyStr) -> None:
+		"""Writes chunk to the stream.
+			- For Type.Bytes data must be bytes.
+			- For Type.String, data must be string.
+			- For Type.File and Type.FileAppend, data must be bytes"""
+		assert self._data is not None, 'StreamWriter buffer is invalid. You have probably closed it already.'
+		if self._binary:
+			assert isinstance(data, bytes), f'Bytes data is required. Actual type: {type(data)}. {self}'
+		else:
+			assert isinstance(data, str), f'String data is required. Actual type: {type(data)}. {self}'
+
+		if Type.Variable in self._target:
+			self._data += data
+		elif Type.File in self._target:
+			self._data.write(data)
+		self._written_len += len(data)
+
+	def switch_to_string_data(self) -> None:
+		"""Switches from binary to string data.
+		For variables, the current content is converted.
+		For files, they are closed and reopened as for appended text writing."""
+		if self._binary is False:
+			return
+		self._binary = False
+		if Type.Variable in self._target:
+			if len(self) == 0:
+				self._data = ''
+			else:
+				# noinspection PyUnresolvedReferences
+				self._data = self._data.decode('utf-8')
+		elif Type.File in self._target:
+			self._data.close()
+			self._data = open(self._file_path, 'a')
+
+	@property
+	def content(self) -> AnyStr:
+		"""Returns content of the writer. Does only work with variable types."""
+		assert Type.Variable in self._target, f'Can not return content for the current {self}'
+		# noinspection PyTypeChecker
+		return self._data
+
+	def close(self) -> None:
+		"""Closes the StreamWriter. You can not use its instance afterwards."""
+		if Type.File in self._target and self._data:
+			self._data.close()
+		self._data = None
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/StructBase.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/StructBase.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from .Types import DataType
-
-
-class StructBase:
-	"""Base class for all the driver's argument structures."""
-	def __init__(self, owner):
-		self.__meta_args_link = dict()
-		ix = 0
-		for arg in self.__get_meta_args_list(owner):
-			arg.argument_ix = ix
-			ix += 1
-
-			if arg.data_type == DataType.Enum or arg.data_type == DataType.EnumList:
-				assert arg.enum_type, f"Struct Argument '{arg.name}' is of enum type, you must define the parameter 'enum_type'"
-			else:
-				assert not arg.enum_type, f"Struct Argument '{arg.name}' data type is '{arg.data_type.name}'. You must set the parameter 'enum_type' to None"
-
-			if arg.is_optional:
-				# set all optional values to None
-				setattr(self, arg.name, None)
-			else:
-				# set all mandatory values to their default values
-				default = arg.data_type.get_default_value(arg.enum_type)
-				setattr(self, arg.name, default)
-
-	# noinspection PyMethodMayBeStatic
-	def __get_meta_args_list(self, owner):
-		args_list = getattr(owner, f'_{owner.__class__.__name__}__meta_args_list')
-		return args_list
+from .Types import DataType
+
+
+class StructBase:
+	"""Base class for all the driver's argument structures."""
+	def __init__(self, owner):
+		self.__meta_args_link = dict()
+		ix = 0
+		for arg in self.__get_meta_args_list(owner):
+			arg.argument_ix = ix
+			ix += 1
+
+			if arg.data_type == DataType.Enum or arg.data_type == DataType.EnumList:
+				assert arg.enum_type, f"Struct Argument '{arg.name}' is of enum type, you must define the parameter 'enum_type'"
+			else:
+				assert not arg.enum_type, f"Struct Argument '{arg.name}' data type is '{arg.data_type.name}'. You must set the parameter 'enum_type' to None"
+
+			if arg.is_optional:
+				# set all optional values to None
+				setattr(self, arg.name, None)
+			else:
+				# set all mandatory values to their default values
+				default = arg.data_type.get_default_value(arg.enum_type)
+				setattr(self, arg.name, default)
+
+	# noinspection PyMethodMayBeStatic
+	def __get_meta_args_list(self, owner):
+		args_list = getattr(owner, f'_{owner.__class__.__name__}__meta_args_list')
+		return args_list
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/Types.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/Types.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from enum import Enum, auto
-from typing import Any
-
-
-class DataType(Enum):
-	"""Data type of a variable in the driver."""
-	String = auto()
-	RawString = auto()
-	Integer = auto()
-	IntegerExt = auto()
-	Boolean = auto()
-	Float = auto()
-	FloatExt = auto()
-	Enum = auto()
-	StringList = auto()
-	RawStringList = auto()
-	IntegerList = auto()
-	IntegerExtList = auto()
-	BooleanList = auto()
-	FloatList = auto()
-	FloatExtList = auto()
-	EnumList = auto()
-
-	@property
-	def is_list(self) -> bool:
-		"""Returns True, if the data type is a list."""
-		return self in frozenset(
-			{
-				DataType.StringList,
-				DataType.RawStringList,
-				DataType.IntegerList,
-				DataType.IntegerExtList,
-				DataType.BooleanList,
-				DataType.FloatList,
-				DataType.FloatExtList,
-				DataType.EnumList
-			})
-
-	@property
-	def is_scalar(self) -> bool:
-		"""Returns True, if the data type is a scalar."""
-		return not self.is_list
-
-	@property
-	def is_enum(self) -> bool:
-		"""Returns True, if the data type is enum or enum array."""
-		return self == DataType.Enum or self == DataType.EnumList
-
-	@property
-	def is_raw_string(self) -> bool:
-		"""Returns True for raw string and raw string list."""
-		return self == DataType.RawString or self == DataType.RawStringList
-
-	@property
-	def is_boolean(self) -> bool:
-		"""Returns True for boolean and boolean list."""
-		return self == DataType.Boolean or self == DataType.BooleanList
-
-	@property
-	def is_string(self) -> bool:
-		"""Returns True for string and string list."""
-		return self == DataType.String or self == DataType.StringList
-
-	@property
-	def element_type(self):
-		"""For lists, the property returns type of the element.
-		For scalars, it returns the same type."""
-		if self.is_scalar:
-			return self
-		elif self == DataType.StringList:
-			return DataType.String
-		elif self == DataType.RawStringList:
-			return DataType.RawString
-		elif self == DataType.RawStringList:
-			return DataType.RawString
-		elif self == DataType.BooleanList:
-			return DataType.Boolean
-		elif self == DataType.IntegerList:
-			return DataType.Integer
-		elif self == DataType.IntegerExtList:
-			return DataType.IntegerExt
-		elif self == DataType.FloatList:
-			return DataType.Float
-		elif self == DataType.FloatExtList:
-			return DataType.FloatExt
-		elif self == DataType.EnumList:
-			return DataType.Enum
-
-	def get_default_value(self, enm: Enum = None) -> Any:
-		"""Returns default value for the current type.
-		If the data type is Enum or EnumString, you have to provide the enum class."""
-		if self.is_list:
-			return []
-		if self == DataType.RawString:
-			return ''
-		elif self == DataType.String:
-			return ''
-		elif self == DataType.Boolean:
-			return False
-		elif self == DataType.Integer:
-			return 0
-		elif self == DataType.IntegerExt:
-			return 0
-		elif self == DataType.Float:
-			return 0.0
-		elif self == DataType.FloatExt:
-			return 0.0
-		elif self == DataType.Enum:
-			return enm(0)
+from enum import Enum, auto
+from typing import Any
+
+
+class DataType(Enum):
+	"""Data type of a variable in the driver."""
+	String = auto()
+	RawString = auto()
+	Integer = auto()
+	IntegerExt = auto()
+	Boolean = auto()
+	Float = auto()
+	FloatExt = auto()
+	Enum = auto()
+	StringList = auto()
+	RawStringList = auto()
+	IntegerList = auto()
+	IntegerExtList = auto()
+	BooleanList = auto()
+	FloatList = auto()
+	FloatExtList = auto()
+	EnumList = auto()
+
+	@property
+	def is_list(self) -> bool:
+		"""Returns True, if the data type is a list."""
+		return self in frozenset(
+			{
+				DataType.StringList,
+				DataType.RawStringList,
+				DataType.IntegerList,
+				DataType.IntegerExtList,
+				DataType.BooleanList,
+				DataType.FloatList,
+				DataType.FloatExtList,
+				DataType.EnumList
+			})
+
+	@property
+	def is_scalar(self) -> bool:
+		"""Returns True, if the data type is a scalar."""
+		return not self.is_list
+
+	@property
+	def is_enum(self) -> bool:
+		"""Returns True, if the data type is enum or enum array."""
+		return self == DataType.Enum or self == DataType.EnumList
+
+	@property
+	def is_raw_string(self) -> bool:
+		"""Returns True for raw string and raw string list."""
+		return self == DataType.RawString or self == DataType.RawStringList
+
+	@property
+	def is_boolean(self) -> bool:
+		"""Returns True for boolean and boolean list."""
+		return self == DataType.Boolean or self == DataType.BooleanList
+
+	@property
+	def is_string(self) -> bool:
+		"""Returns True for string and string list."""
+		return self == DataType.String or self == DataType.StringList
+
+	@property
+	def element_type(self):
+		"""For lists, the property returns type of the element.
+		For scalars, it returns the same type."""
+		if self.is_scalar:
+			return self
+		elif self == DataType.StringList:
+			return DataType.String
+		elif self == DataType.RawStringList:
+			return DataType.RawString
+		elif self == DataType.RawStringList:
+			return DataType.RawString
+		elif self == DataType.BooleanList:
+			return DataType.Boolean
+		elif self == DataType.IntegerList:
+			return DataType.Integer
+		elif self == DataType.IntegerExtList:
+			return DataType.IntegerExt
+		elif self == DataType.FloatList:
+			return DataType.Float
+		elif self == DataType.FloatExtList:
+			return DataType.FloatExt
+		elif self == DataType.EnumList:
+			return DataType.Enum
+
+	def get_default_value(self, enm: Enum = None) -> Any:
+		"""Returns default value for the current type.
+		If the data type is Enum or EnumString, you have to provide the enum class."""
+		if self.is_list:
+			return []
+		if self == DataType.RawString:
+			return ''
+		elif self == DataType.String:
+			return ''
+		elif self == DataType.Boolean:
+			return False
+		elif self == DataType.Integer:
+			return 0
+		elif self == DataType.IntegerExt:
+			return 0
+		elif self == DataType.Float:
+			return 0.0
+		elif self == DataType.FloatExt:
+			return 0.0
+		elif self == DataType.Enum:
+			return enm(0)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/Utilities.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/Utilities.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-from enum import Flag
-from typing import Tuple
-
-
-class TrimStringMode(Flag):
-	"""Trimming mode for strings."""
-	white_chars_only = 1
-	white_chars_single_quotes = 2
-	white_chars_double_quotes = 3
-	white_chars_all_quotes = 4
-
-
-def trim_str_response(text: str, mode=TrimStringMode.white_chars_all_quotes) -> str:
-	"""Trims instrument string response.
-	In modes white_chars_all_quotes, white_chars_single_quotes, white_chars_double_quotes:
-	All the symmetrical leading and trailing quotation marks are trimmed,
-	but only if there are none in the remaining text."""
-	first_sq_ix = -1
-	first_dq_ix = -1
-	rem_sq = True if (mode == TrimStringMode.white_chars_all_quotes or mode == TrimStringMode.white_chars_single_quotes) else False
-	rem_dq = True if (mode == TrimStringMode.white_chars_all_quotes or mode == TrimStringMode.white_chars_double_quotes) else False
-
-	if not text:
-		return text
-	text = text.strip()
-	if rem_sq and text == "''":
-		return ''
-	if rem_dq and text == '""':
-		return ''
-	start_ix = 0
-	end_ix: int = len(text) - 1
-	if end_ix - 2 < start_ix:
-		return text
-	if mode is not TrimStringMode.white_chars_only:
-		# Loop to cut the outer paired quotation marks
-		trimmed = True
-		while trimmed:
-			trimmed = False
-			if rem_sq and text[start_ix] == "'" and text[end_ix] == "'":
-				if first_sq_ix < 0:
-					first_sq_ix = start_ix
-				start_ix += 1
-				end_ix -= 1
-				trimmed = True
-			if end_ix - 2 < start_ix:
-				break
-			if rem_dq and text[start_ix] == '"' and text[end_ix] == '"':
-				if first_dq_ix < 0:
-					first_dq_ix = start_ix
-				start_ix += 1
-				end_ix -= 1
-				trimmed = True
-			if end_ix - 2 < start_ix:
-				break
-		if start_ix == 0:
-			return text
-
-		final_cut_ix = start_ix
-		shortened_text = text[start_ix: -start_ix]
-		if first_sq_ix >= 0 and "'" in shortened_text:
-			# The cut quotes are also in the shortened string, do not removed the quotes, and set the cutting to start_ix
-			final_cut_ix = first_sq_ix
-		if first_dq_ix >= 0 and '"' in shortened_text:
-			if final_cut_ix > first_dq_ix:
-				final_cut_ix = first_dq_ix
-
-		if final_cut_ix == 0:
-			return text
-
-		text = text[final_cut_ix: -final_cut_ix]
-
-	return text
-
-
-def truncate_string_from_end(string: str, max_len: int) -> str:
-	"""If the string len is below the max_len, the function returns the same string.
-	If the string is above the max len, the function returns only the last max_len characters plus '...' at the beginning."""
-	if len(string) <= max_len:
-		return string
-	return f'Last {max_len} chars: "...{string[-max_len:]}"'
-
-
-def get_plural_string(word: str, amount: int) -> str:
-	"""Returns singular or plural of the word depending on the amount.
-	Example:
-		word = 'piece', amount = 0 -> '0 pieces'
-		word = 'piece', amount = 1 -> '1 piece'
-		word = 'piece', amount = 5 -> '5 pieces'"""
-	if amount == 1:
-		return f'1 {word}'
-	else:
-		return f'{amount} {word}s'
-
-
-def parse_token_to_key_and_value(token: str) -> Tuple[str, str]:
-	"""Parses entered string to name and value with the delimiter '='.
-	If the token is empty: name = None, value = None.
-	If the '=' is not found: name = token, value = None.
-	name is trimmed for white spaces.
-	value is trimmed with trim_str_response()."""
-	token = token.strip()
-	if not token:
-		# noinspection PyTypeChecker
-		return None, None
-	if '=' in token:
-		data = token.split('=')
-		name = data[0].strip()
-		value = trim_str_response(data[1])
-		return name, value
-
-	# noinspection PyTypeChecker
-	return token.strip(), None
-
-
-def size_to_kb_mb_string(data_size: int, as_additional_info: bool = False) -> str:
-	"""Returns human-readable string with kilobytes or megabytes depending on the data_size range. \n
-		:param data_size: data size in bytes to convert
-		:param as_additional_info:
-		if True, the dynamic data appear in round bracket after the number in bytes. e.g. '12345678 bytes (11.7 MB)'
-		if False, only the dynamic data is returned e.g. '11.7 MB' """
-	if data_size < 1024:
-		as_additional_info = False
-		dynamic = f'{data_size} bytes'
-	elif data_size < 1048576:
-		dynamic = f'{data_size / 1024:0.1f} kB'
-	else:
-		dynamic = f'{data_size / 1048576:0.1f} MB'
-
-	if as_additional_info:
-		return f'{data_size} bytes ({dynamic})'
-	else:
-		return dynamic
-
-
-def calculate_chunks_count(data_size: int, chunk_size: int) -> int:
-	"""Returns number of chunks needed to transfer the data_size split to maximum of chunk_size blocks. \n
-	:param data_size: total data size
-	:param chunk_size: maximum size of one block"""
-	return (data_size // chunk_size) + (1 if (data_size % chunk_size) > 0 else 0)
+from enum import Flag
+from typing import Tuple
+
+
+class TrimStringMode(Flag):
+	"""Trimming mode for strings."""
+	white_chars_only = 1
+	white_chars_single_quotes = 2
+	white_chars_double_quotes = 3
+	white_chars_all_quotes = 4
+
+
+def trim_str_response(text: str, mode=TrimStringMode.white_chars_all_quotes) -> str:
+	"""Trims instrument string response.
+	In modes white_chars_all_quotes, white_chars_single_quotes, white_chars_double_quotes:
+	All the symmetrical leading and trailing quotation marks are trimmed,
+	but only if there are none in the remaining text."""
+	first_sq_ix = -1
+	first_dq_ix = -1
+	rem_sq = True if (mode == TrimStringMode.white_chars_all_quotes or mode == TrimStringMode.white_chars_single_quotes) else False
+	rem_dq = True if (mode == TrimStringMode.white_chars_all_quotes or mode == TrimStringMode.white_chars_double_quotes) else False
+
+	if not text:
+		return text
+	text = text.strip()
+	if rem_sq and text == "''":
+		return ''
+	if rem_dq and text == '""':
+		return ''
+	start_ix = 0
+	end_ix: int = len(text) - 1
+	if end_ix - 2 < start_ix:
+		return text
+	if mode is not TrimStringMode.white_chars_only:
+		# Loop to cut the outer paired quotation marks
+		trimmed = True
+		while trimmed:
+			trimmed = False
+			if rem_sq and text[start_ix] == "'" and text[end_ix] == "'":
+				if first_sq_ix < 0:
+					first_sq_ix = start_ix
+				start_ix += 1
+				end_ix -= 1
+				trimmed = True
+			if end_ix - 2 < start_ix:
+				break
+			if rem_dq and text[start_ix] == '"' and text[end_ix] == '"':
+				if first_dq_ix < 0:
+					first_dq_ix = start_ix
+				start_ix += 1
+				end_ix -= 1
+				trimmed = True
+			if end_ix - 2 < start_ix:
+				break
+		if start_ix == 0:
+			return text
+
+		final_cut_ix = start_ix
+		shortened_text = text[start_ix: -start_ix]
+		if first_sq_ix >= 0 and "'" in shortened_text:
+			# The cut quotes are also in the shortened string, do not removed the quotes, and set the cutting to start_ix
+			final_cut_ix = first_sq_ix
+		if first_dq_ix >= 0 and '"' in shortened_text:
+			if final_cut_ix > first_dq_ix:
+				final_cut_ix = first_dq_ix
+
+		if final_cut_ix == 0:
+			return text
+
+		text = text[final_cut_ix: -final_cut_ix]
+
+	return text
+
+
+def truncate_string_from_end(string: str, max_len: int) -> str:
+	"""If the string len is below the max_len, the function returns the same string.
+	If the string is above the max len, the function returns only the last max_len characters plus '...' at the beginning."""
+	if len(string) <= max_len:
+		return string
+	return f'Last {max_len} chars: "...{string[-max_len:]}"'
+
+
+def get_plural_string(word: str, amount: int) -> str:
+	"""Returns singular or plural of the word depending on the amount.
+	Example:
+		word = 'piece', amount = 0 -> '0 pieces'
+		word = 'piece', amount = 1 -> '1 piece'
+		word = 'piece', amount = 5 -> '5 pieces'"""
+	if amount == 1:
+		return f'1 {word}'
+	else:
+		return f'{amount} {word}s'
+
+
+def parse_token_to_key_and_value(token: str) -> Tuple[str, str]:
+	"""Parses entered string to name and value with the delimiter '='.
+	If the token is empty: name = None, value = None.
+	If the '=' is not found: name = token, value = None.
+	name is trimmed for white spaces.
+	value is trimmed with trim_str_response()."""
+	token = token.strip()
+	if not token:
+		# noinspection PyTypeChecker
+		return None, None
+	if '=' in token:
+		data = token.split('=')
+		name = data[0].strip()
+		value = trim_str_response(data[1])
+		return name, value
+
+	# noinspection PyTypeChecker
+	return token.strip(), None
+
+
+def size_to_kb_mb_string(data_size: int, as_additional_info: bool = False) -> str:
+	"""Returns human-readable string with kilobytes or megabytes depending on the data_size range. \n
+		:param data_size: data size in bytes to convert
+		:param as_additional_info:
+		if True, the dynamic data appear in round bracket after the number in bytes. e.g. '12345678 bytes (11.7 MB)'
+		if False, only the dynamic data is returned e.g. '11.7 MB' """
+	if data_size < 1024:
+		as_additional_info = False
+		dynamic = f'{data_size} bytes'
+	elif data_size < 1048576:
+		dynamic = f'{data_size / 1024:0.1f} kB'
+	else:
+		dynamic = f'{data_size / 1048576:0.1f} MB'
+
+	if as_additional_info:
+		return f'{data_size} bytes ({dynamic})'
+	else:
+		return dynamic
+
+
+def calculate_chunks_count(data_size: int, chunk_size: int) -> int:
+	"""Returns number of chunks needed to transfer the data_size split to maximum of chunk_size blocks. \n
+	:param data_size: total data size
+	:param chunk_size: maximum size of one block"""
+	return (data_size // chunk_size) + (1 if (data_size % chunk_size) > 0 else 0)
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/VisaSession.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/VisaSession.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1131 +1,1111 @@
-import time
-from enum import Enum, Flag
-from typing import Tuple, Callable, AnyStr
-import os.path
-import re
-import threading
-
-# noinspection PyPackageRequirements
-import pyvisa
-
-from .VisaPluginSocketIo import ResourceManager, SocketIo
-from . import InstrumentSettings, InstrumentErrors, Conversions as Conv
-from .InstrumentSettings import WaitForOpcMode, InstrViClearMode as ViClearMode
-from .StreamReader import StreamReader
-from .StreamWriter import StreamWriter
-from .Utilities import size_to_kb_mb_string, calculate_chunks_count
-import platform
-import struct
-
-
-class SessionKind(Enum):
-	"""Visa instrument session type."""
-	unsupported = 0
-	gpib = 1
-	serial = 2
-	vxi11 = 3
-	socket = 5
-	usb = 6
-	rs_nrp = 7
-
-
-class ReadDataType(Enum):
-	"""Data type returned by the instrument."""
-	unknown = 0
-	ascii = 1
-	null = 2
-	bin_known_len = 3
-	bin_unknown_len = 4
-
-
-class StatusByte(Flag):
-	"""Status Byte flags."""
-	NONE = 0x00
-	error_queue_not_empty = 0x04
-	questionable_status_reg = 0x08
-	message_available = 0x10
-	event_status_byte = 0x20
-	request_service = 0x40
-	operation_status_reg = 0x80
-
-
-class EventStatusRegister(Flag):
-	"""Event Status Register flags."""
-	null = 0x00
-	operation_complete = 0x01
-
-
-# noinspection PyUnresolvedReferences
-class VisaSession(object):
-	"""Extended VISA class."""
-
-	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
-		self.reusing_session = direct_session is not None
-		# noinspection PyTypeChecker
-		self._data_chunk_size: int = None
-		self._std_bin_block_header_max_len: int = 999999999
-		self._lock = None
-		self.disable_opc_query: bool = settings.disable_opc_query
-		self.last_status = None
-		self.visa_library_name = None
-
-		# Implemented for interface compatibility with VisaSessionSim
-		self.cached_to_stream = False
-
-		# Event handlers
-		# noinspection PyTypeChecker
-		self.on_read_chunk_handler: Callable = None
-		"""If assigned a handler, the VisaSession sends it event on each read chunk transfer."""
-		# noinspection PyTypeChecker
-		self.on_write_chunk_handler: Callable = None
-		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
-		self.io_events_include_data: bool = False
-		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
-
-		if self.reusing_session:
-			# Reuse the session
-			assert isinstance(direct_session, pyvisa.Resource) or isinstance(direct_session, SocketIo), f"Direct_session must be a VISA resource object. Actual type: '{type(direct_session)}', value: '{direct_session}'"
-			self._session = direct_session
-			self._resource_name = self._session.resource_name
-		else:
-			# Create new session
-			# Check resource_name for the trailing (SelectVisa=..)
-			pure_resource_name, visa_select = self._get_pure_resource_name(resource_name)
-			if settings.visa_select is not None:
-				visa_select = settings.visa_select
-			self._rm = VisaSession.get_resource_manager(visa_select)
-			self.manufacturer = self._get_visa_manufacturer()
-
-			# Resource manager opening
-			try:
-				self._session = self._rm.open_resource(pure_resource_name)
-			except pyvisa.VisaIOError as e:
-				if e.error_code != pyvisa.constants.StatusCode.error_resource_not_found:
-					raise e
-				message = e.description
-				message += f"\nLibrary: {self._rm.visalib}\nManufacturer: {self.manufacturer}\nResource Name: '{resource_name}'"
-				raise InstrumentErrors.ResourceError(resource_name, message)
-			self._resource_name = resource_name
-
-		# Decide, whether to create a new thread lock or the existing one from the session
-		if hasattr(self._session, 'session_thread_rlock'):
-			rlock = self._session.session_thread_rlock
-			if isinstance(rlock, type(threading.RLock())):
-				self.assign_lock(rlock)
-		if self.get_lock() is None:
-			# The existing session did not have a thread lock, assign a new one
-			self.assign_lock(threading.RLock())
-
-		self._interface_type = SessionKind.unsupported
-		if self._session.interface_type == pyvisa.constants.InterfaceType.gpib or self._session.interface_type == pyvisa.constants.InterfaceType.gpib:
-			self._interface_type = SessionKind.gpib
-
-		elif self._session.interface_type == pyvisa.constants.InterfaceType.rsnrp:
-			self._interface_type = SessionKind.rs_nrp
-
-		elif self._session.interface_type == pyvisa.constants.InterfaceType.asrl:
-			self._interface_type = SessionKind.serial
-
-		elif self._session.interface_type == pyvisa.constants.InterfaceType.usb:
-			# Check whether it is not the NRP-Z
-			intf_type = self._session.get_visa_attribute(pyvisa.constants.VI_ATTR_INTF_TYPE)
-			if intf_type == pyvisa.constants.InterfaceType.rsnrp:
-				self._interface_type = SessionKind.rs_nrp
-
-		elif self._session.interface_type == pyvisa.constants.InterfaceType.tcpip:
-			self._interface_type = SessionKind.vxi11
-			if self._session.resource_class == 'SOCKET':
-				self._interface_type = SessionKind.socket
-
-		# Specifics for different interfaces
-		self._assure_write_with_tc = settings.assure_write_with_tc
-		self._term_char = settings.term_char
-		self._term_char_bin = self._term_char.encode('utf-8')
-		self._session.write_termination = ''
-		self.vxi_capable = True
-
-		if self._interface_type == SessionKind.serial:
-			self._session.read_termination = self._term_char
-			self.vxi_capable = False
-			self._assure_write_with_tc = True
-		elif self._interface_type == SessionKind.socket:
-			self._session.read_termination = self._term_char
-			self.vxi_capable = False
-			self._assure_write_with_tc = True
-		else:
-			self._session.read_termination = ''
-
-		# NRP-Z specific settings
-		if self.is_rsnrp_session():
-			self.disable_opc_query = True
-			# NRP-Z does not support chunk reading, therefore the segment must be in one piece
-			settings.io_segment_size = 1000000
-			self.vxi_capable = False
-
-		self.write_delay = settings.write_delay
-		self.read_delay = settings.read_delay
-		self._viclear_exe_mode = settings.viclear_exe_mode
-		self._opc_wait_mode = settings.opc_wait_mode
-
-		# Parameters that need to be coerced based on Vxi-capability
-		if self.vxi_capable:
-			self._add_term_char_to_write_bin_block = settings.add_term_char_to_write_bin_block
-		else:
-			self._add_term_char_to_write_bin_block = True
-
-		# Changeable settings
-		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
-		self.visa_timeout = settings.visa_timeout
-		self._session.chunk_size = settings.io_segment_size
-		self._data_chunk_size = settings.io_segment_size
-
-		# Must call the VISA viClear() before the any communication with the instrument
-		self.clear()
-
-		# Further steps are for NRP-Z session not valid
-		if self.is_rsnrp_session():
-			return
-
-		# Clear instrument status
-		self.write('*CLS')
-		if self.vxi_capable:
-			stb = self._read_stb()
-			if stb & StatusByte.message_available:
-				self._flush_junk_data()
-
-		# Apply settings for ESE and SRE, plus coerce the _opcWaitMode if necessary
-		self._opc_wait_mode = self._set_regs_ese_sre(self._opc_wait_mode)
-
-	@staticmethod
-	def _get_pure_resource_name(resource_name: str):
-		"""Returns pure resource name stripped of the (SelectVisa) part and the visa_select string"""
-		m = re.search(r'(.+)\(SelectVisa=([^),]+)\)', resource_name)
-		if not m:
-			return resource_name, None
-		resource_name = m.group(1).strip()
-		visa_select = m.group(2).strip()
-		return resource_name, visa_select
-
-	@classmethod
-	def get_resource_manager(cls, visa_select: str) -> pyvisa.ResourceManager:
-		"""Returns resource manager for the desired VISA implementation"""
-		operating_system = platform.system().lower()
-		bittness = struct.calcsize('P') * 8
-		if visa_select is None or visa_select in ['@default', '@standard', 'default', 'standard', 'defaultvisa', 'standardvisa', '@defaultvisa', '@standardvisa']:
-			return pyvisa.ResourceManager()
-		if visa_select.lower() in ['@ni', 'ni', 'visa-ni', 'nivisa', 'ni-visa', 'nationalinstruments', 'nationalinstrumentsvisa']:
-			return pyvisa.ResourceManager('@ni')
-		if visa_select.lower() in ['@py', 'pyvisa', 'visa-py', 'pyvisa-py']:
-			return pyvisa.ResourceManager('@py')
-		if 'rohde&schwarz' in visa_select.lower() or 'rohdeschwarz' in visa_select.lower() or visa_select.lower() == 'rsvisa' or visa_select.lower() == 'rs' or visa_select.lower() == 'r&s':
-			if operating_system == 'windows':
-				if bittness == 32:
-					visa_select = r'c:\Windows\SysWOW64\RsVisa32.dll'
-				else:
-					visa_select = r'c:\Windows\system32\RsVisa32.dll'
-				return pyvisa.ResourceManager(visa_select)
-			elif operating_system == 'linux':
-				# The default install location may be different
-				# for debian/red hat/opensuse derived distributions
-				check_visa = [f'/usr/lib{bittness}/librsvisa.so', r'/usr/lib/librsvisa.so']
-				for check in check_visa:
-					if os.path.isfile(check):
-						return pyvisa.ResourceManager(check)
-
-		if visa_select.lower() in ['socketio', 'socket', 'none']:
-			return ResourceManager()
-		return pyvisa.ResourceManager(visa_select)
-
-	def _get_visa_manufacturer(self) -> str:
-		"""Returns manufacturer of the current VISA"""
-		if hasattr(self._rm, 'VisaManufacturerName'):
-			return self._rm.VisaManufacturerName
-		try:
-			return self._rm.visalib.get_attribute(self._rm.session, pyvisa.constants.VI_ATTR_RSRC_MANF_NAME)[0]
-		except TypeError:
-			return self._rm.visalib.__class__.__name__
-
-	def is_rsnrp_session(self) -> bool:
-		"""Returns True, if the current session is a NRP-Z session"""
-		return self._interface_type == SessionKind.rs_nrp
-
-	def assign_lock(self, lock: threading.RLock) -> None:
-		"""Assigns the provided thread lock by setting the pyvisa runtime session attribute 'session_thread_rlock'
-		This is done, because if the session is to be entered as an existing session to another RsInstrument object,
-		the lock must be shared as well. The lock is only used by the parent class Instrument."""
-		setattr(self._session, 'session_thread_rlock', lock)
-		self._lock = lock
-
-	def get_lock(self) -> threading.RLock:
-		"""Returns the current RLock object."""
-		return self._lock
-
-	@property
-	def visa_timeout(self) -> int:
-		"""See the visa_timeout.setter."""
-		return int(self._session.timeout)
-
-	@visa_timeout.setter
-	def visa_timeout(self, value: int) -> None:
-		"""Sets / Gets visa IO timeout in milliseconds."""
-		self._session.timeout = int(value)
-
-	@property
-	def data_chunk_size(self) -> int:
-		"""Returns max chunk size of one data block."""
-		return self._data_chunk_size
-
-	@data_chunk_size.setter
-	def data_chunk_size(self, chunk_size: int) -> None:
-		"""Sets the maximum size of one block transferred during write/read operations."""
-		self._data_chunk_size = int(chunk_size)
-		self._session.chunk_size = int(chunk_size)
-
-	def _resolve_opc_timeout(self, timeout: int) -> int:
-		"""Resolves entered timeout value - if the input value is less than 1, it is replaces with opc_timeout."""
-		if timeout is None or timeout < 1:
-			return self.opc_timeout
-		else:
-			return timeout
-
-	def _set_regs_ese_sre(self, mode: WaitForOpcMode) -> WaitForOpcMode:
-		"""Based on the WaitForOpcMode, it sets the ESE and SRE register masks.
-		Returns coerced WaitForOpcMode."""
-		# Set the SRE and ESE registers accordingly
-		# No SRE is supported
-		self._set_ese_mask(EventStatusRegister.operation_complete)
-		self._set_sre_mask(StatusByte.NONE)
-		return mode
-
-	def _set_ese_mask(self, mask: EventStatusRegister, reset: bool = True) -> None:
-		"""Sends *ESE command with mask parameter."""
-		if reset is False:
-			current_value = int(self._query_str_no_events('*ESE?'))
-			mask = current_value | mask.value
-		self.write("*ESE %d" % mask.value)
-
-	def _set_sre_mask(self, mask: StatusByte, reset: bool = True) -> None:
-		"""Sends *SRE command with StatusByte mask parameter."""
-		if reset is False:
-			current_value = int(self._query_str_no_events('*SRE?'))
-			mask = current_value | mask.value
-		# Also affect the _opc_wait_mode:
-		# If the mask has event_status_byte == false, and the _opc_wait_mode is service_request, set it to stb_poll
-		# If the mask has event_status_byte == true, do not change anything
-		self.write(f'*SRE {mask.value}')
-
-	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int, end_mask: StatusByte) -> StatusByte:
-		"""Reads Status Byte Register and ends if the ESB bit (5) is set to 1.
-		Also works with the SOCKET and SERIAL interface by sending *STB? query.
-		In that case however, command cannot be a query.
-		Returns the last read Status Byte value."""
-		timeout_secs = timeout / 1000
-		self.clear_before_read()
-		if command.endswith(self._term_char):
-			command = command.rstrip(self._term_char)
-		self.write(command + ';*OPC')
-		# Use catch to return the VISA Timeout back
-		start = time.time()
-		# STB polling loop
-		while True:
-			stb = self._read_stb()
-			elapsed = self._polling_delay(start)
-			if elapsed > timeout_secs:
-				self._narrow_down_opc_tout_error(command, is_query, timeout)
-			if end_mask & stb:
-				break
-		return stb
-
-	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int, end_mask: StatusByte) -> StatusByte:
-		"""Queries Status Byte Register (*STB?) and ends if the ESB bit (5) is set to 1.
-			The command must not be a query. Also works with the SOCKET and SERIAL interface.
-			Returns the last read Status Byte value."""
-		timeout_secs = timeout / 1000
-		self.clear_before_read()
-		if command.endswith(self._term_char):
-			command = command.rstrip(self._term_char)
-		self.write(command + ';*OPC')
-		start = time.time()
-		# STB polling loop
-		while True:
-			stb = self._query_stb()
-			elapsed = self._polling_delay(start)
-			if elapsed > timeout_secs:
-				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout)
-			if stb & end_mask:
-				break
-		return stb
-
-	def _narrow_down_opc_tout_error(self, command: str, is_query: bool, timeout: int) -> None:
-		"""Called by the _write_and_poll_stb_vxi when the timeout expires.
-		The method tries to closer identify the cause of the timeout."""
-		stb = self._read_stb()
-		timeout = self._resolve_opc_timeout(timeout)
-		if is_query:
-			if stb & StatusByte.error_queue_not_empty:
-				self.clear()
-				context = f"Sending query '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
-				InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
-			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Sending query '{command.strip()}'.")
-		else:
-			if stb & StatusByte.error_queue_not_empty:
-				self.clear()
-				context = f"Sending command '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
-				InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
-			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Sending command '{command.strip()}'.")
-
-	def _narrow_down_io_tout_error(self, context: str, visa_timeout: int = 0) -> None:
-		"""Called internally after IOTimeoutException can narrow down the error to more specific exception.
-		You can define the visa_timeout value for the error message. Otherwise the current visa_timeout is reported."""
-		if self.vxi_capable:
-			stb = self._read_stb()
-		else:
-			# Non-Vxi session
-			old_tout = self.visa_timeout
-			try:
-				self.visa_timeout = 500
-				stb = self._query_stb()
-			finally:
-				self.visa_timeout = old_tout
-		if visa_timeout <= 0:
-			visa_timeout = self.visa_timeout
-		context = context + f'VISA Timeout error occurred ({visa_timeout} milliseconds)'
-		if stb & StatusByte.error_queue_not_empty:
-			InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context + ' and ...')
-		# In case the previous exception is not thrown
-		raise InstrumentErrors.TimeoutException(context)
-
-	def _polling_delay(self, start):
-		"""Generates progressive polling delay."""
-
-		elapsed = time.time() - start
-		if self._opc_wait_mode == WaitForOpcMode.stb_poll:
-			if elapsed < 0.01:
-				return elapsed
-			if elapsed < 0.1:
-				time.sleep(0.005)
-				return elapsed
-			if elapsed < 1:
-				time.sleep(0.02)
-				return elapsed
-			if elapsed < 5:
-				time.sleep(0.05)
-				return elapsed
-			if elapsed < 10:
-				time.sleep(0.1)
-				return elapsed
-			if elapsed < 50:
-				time.sleep(0.5)
-				return elapsed
-			time.sleep(1)
-		elif self._opc_wait_mode == WaitForOpcMode.stb_poll_slow:
-			if elapsed < 0.01:
-				time.sleep(0.001)
-				return elapsed
-			if elapsed < 1:
-				time.sleep(0.02)
-				return elapsed
-			if elapsed < 5:
-				time.sleep(0.1)
-				return elapsed
-			if elapsed < 10:
-				time.sleep(0.2)
-				return elapsed
-			if elapsed < 20:
-				time.sleep(0.5)
-				return elapsed
-			time.sleep(1)
-		elif self._opc_wait_mode == WaitForOpcMode.stb_poll_superslow:
-			if elapsed < 1:
-				time.sleep(0.1)
-				return elapsed
-			if elapsed < 10:
-				time.sleep(0.5)
-				return elapsed
-			if elapsed < 20:
-				time.sleep(1)
-				return elapsed
-			time.sleep(2)
-
-		return elapsed
-
-	def query_syst_error(self) -> str or None:
-		"""Returns one response to the SYSTEM:ERROR? query."""
-		error = self.query_str('SYST:ERR?')
-		if error.startswith('0,'):
-			return None
-		return error.strip()
-
-	def query_all_syst_errors(self) -> list or None:
-		"""Returns all errors in the instrument's error queue."""
-		errors = []
-		while True:
-			entry = self.query_syst_error()
-			if entry is None:
-				break
-			errors.append(entry)
-			if len(errors) > 50:
-				# Safety stop
-				errors.append('query_all_syst_errors - max limit 50 of SYST:ERR? sent.')
-				break
-
-		if len(errors) == 0:
-			return None
-		else:
-			return errors
-
-	def _query_stb(self) -> StatusByte:
-		"""Sends *STB? query and reads the result."""
-		return StatusByte(int(self._query_str_no_events('*STB?')))
-
-	def _read_stb(self) -> StatusByte:
-		"""Calls viReadStb and returns the result."""
-		return StatusByte(self._session.read_stb())
-
-	def clear_before_read(self) -> None:
-		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
-
-		# For NRP-Z sessions, skip this completely
-		if self.is_rsnrp_session():
-			return
-
-		if not self.vxi_capable:
-			# Non-Vxi session must use *CLS in any case
-			self.write('*CLS')
-			correct = False
-			opc = self._query_str_no_events('*OPC?')
-			repeat = 0
-			while not correct:
-				if len(opc) <= 2:
-					opc = opc.strip()
-					correct = opc == '0' or opc == '1'
-				if not correct:
-					# Read again with a small VISA timeout
-					opc = self._read_str_timed(5, True)
-				repeat += 1
-				if repeat > 10:
-					break
-
-		stb = self._query_stb()
-		condition = StatusByte.error_queue_not_empty | StatusByte.message_available | StatusByte.event_status_byte
-		if not stb & condition:
-			return
-		repeat = 0
-		# Loop more times to clear the status subsystem
-		while stb & condition:
-			if stb & StatusByte.error_queue_not_empty:
-				self.write('*CLS')
-				_ = self.query_all_syst_errors()
-			if stb & StatusByte.message_available:
-				# Clear output buffer
-				self._flush_junk_data()
-			if stb & StatusByte.event_status_byte:
-				# OPC or error bits in the ESR
-				self.write('*CLS')
-				self.query_and_clear_esr()
-			# Check if the status byte value changed
-			previous_stb = stb
-			stb = self._query_stb()
-			if stb == previous_stb:
-				repeat += 1
-				if repeat > 10:
-					raise Exception(f"Cannot clear the instrument's status subsystem. Status Byte: '{stb}'")
-
-	def _flush_junk_data(self) -> None:
-		"""Reads junk bytes to clear the instrument's output buffer."""
-		if self.read_delay > 0:
-			time.sleep(self.read_delay / 1000)
-		self._read_unknown_len(StreamWriter.as_bin_var(), False)
-
-	def clear(self) -> None:
-		"""Perform VISA viClear conditionally based on the instrument settings."""
-		perform_all = ViClearMode.execute_on_all in self._viclear_exe_mode
-		perform = False
-		if perform_all:
-			perform = True
-		else:
-			# Perform on all is blocked, use the SessionKind to decide
-			if self._interface_type == SessionKind.gpib:
-				perform = ViClearMode.execute_on_gpib in self._viclear_exe_mode
-
-			elif self._interface_type == SessionKind.serial:
-				perform = ViClearMode.execute_on_serial in self._viclear_exe_mode
-
-			elif self._interface_type == SessionKind.socket:
-				perform = ViClearMode.execute_on_socket in self._viclear_exe_mode
-
-			elif self._interface_type == SessionKind.usb:
-				perform = ViClearMode.execute_on_usb in self._viclear_exe_mode
-
-			elif self._interface_type == SessionKind.vxi11:
-				perform = ViClearMode.execute_on_tcpvxi in self._viclear_exe_mode
-
-		if not perform:
-			return
-
-		if ViClearMode.ignore_error in self._viclear_exe_mode:
-			# noinspection PyBroadException
-			try:
-				self._session.clear()
-			except Exception:
-				pass
-		else:
-			self._session.clear()
-
-	def _write_and_wait_for_opc(self, command: str, is_query: bool, timeout: int) -> StatusByte:
-		"""Internal method to synchronise a command with OPC timeout.
-		Timeout value 0 means the OPC timeout is used."""
-		timeout = self._resolve_opc_timeout(timeout)
-
-		if command.endswith(self._term_char):
-			command = command.rstrip(self._term_char)
-		if is_query:
-			InstrumentErrors.assert_query_has_qmark(command, 'Query with OPC')
-		else:
-			InstrumentErrors.assert_cmd_has_no_qmark(command, 'Write with OPC')
-
-		if self._opc_wait_mode == WaitForOpcMode.opc_query:
-			if is_query:
-				raise Exception('Sending a query with OpcQuery synchronization is not possible')
-			stb = self._write_and_query_opc(command, timeout)
-		else:
-			# STB polling
-			end_stb_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
-			if is_query:
-				end_stb_mask |= StatusByte.message_available
-			if self.vxi_capable:
-				stb = self._write_and_poll_stb_vxi(command, is_query, timeout, end_stb_mask)
-			else:
-				stb = self._write_and_poll_stb_non_vxi(command, timeout, end_stb_mask)
-
-		return stb
-
-	def _write_and_query_opc(self, cmd: str, timeout: int) -> StatusByte:
-		"""Internal method to write a command followed by query_opc().
-		Used for opc-synchronization if the mode is set to WaitForOpcMode.opc_query or the session is not-vxi.
-		Timeout value 0 means the OPC timeout is used."""
-		old_tout = self.visa_timeout
-
-		# Change VISA Timeout if necessary
-		if old_tout != timeout:
-			self.visa_timeout = timeout
-		try:
-			# try-catch to set the VISA timeout back
-			self.write(cmd)
-			self.query_opc()
-		finally:
-			if old_tout != timeout:
-				self.visa_timeout = old_tout
-		return self._query_stb()
-
-	def write(self, cmd: str) -> None:
-		"""Writes command to the instrument."""
-		if self.write_delay > 0:
-			time.sleep(self.write_delay / 1000)
-		add_tc = False
-		if self._assure_write_with_tc and not cmd.endswith(self._term_char):
-			add_tc = True
-		if add_tc:
-			self._session.write(cmd + self._term_char)
-		else:
-			self._session.write(cmd)
-
-	def _read_unknown_len(self, stream: StreamWriter, allow_chunk_events: bool, prepend_data: AnyStr = None) -> None:
-		"""Reads data of unknown length to the provided WriteStream.
-		The read is performed in an incremental chunk steps to optimize memory use (for NRP-Z session it is set to fixed self._data_chunk_size):
-			- The first read is performed with the fixed size of 1024 bytes
-			- The 2nd one reads 64 kBytes
-			- The 3rd one reads 128 kBytes
-			- The 4th one reads 256 kBytes and so on, with the max cap of self._data_chunk_size
-		:param stream: [StreamWriter] target for the read data
-		:param allow_chunk_events: [bool] if True, the method can send the chunk_events. If False, sending events is blocked.
-		:param prepend_data: Optional[bytes or string] You can prepend this data to the beginning. It will be considered part of the first chunk read
-		:return: read data [bytes or string], depending on the parameter binary."""
-		with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
-			if prepend_data and isinstance(prepend_data, str):
-				prepend_data = prepend_data.encode('utf-8')
-			chunk_ix = 0
-			eot = False
-			while not eot:
-				if self.is_rsnrp_session():
-					chunk_size = self._data_chunk_size
-				else:
-					if chunk_ix == 0:
-						# First read, set 1024 bytes read size
-						chunk_size = 1024
-					elif chunk_ix == 1:
-						chunk_size = 65536
-					else:
-						chunk_size *= 2
-				if chunk_size > self._data_chunk_size:
-					chunk_size = self._data_chunk_size
-				chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
-				if chunk_ix == 0 and prepend_data:
-					chunk = prepend_data + chunk
-				eot = not self._last_status_more_data_available()
-				if not stream.binary:
-					chunk = chunk.decode('utf-8')
-					if eot:
-						chunk = chunk.rstrip(self._term_char)
-				stream.write(chunk)
-				if self.on_read_chunk_handler and allow_chunk_events:
-					total_size = len(stream) if eot is True else None
-					event_args = EventArgsChunk(stream.binary, chunk_ix, len(chunk), total_size, len(stream), eot, None, chunk if self.io_events_include_data else None)
-					self.on_read_chunk_handler(event_args)
-				chunk_ix += 1
-
-	def _last_status_more_data_available(self):
-		"""Returns True, if the last status signalled that more data is available"""
-		return self.last_status == pyvisa.constants.StatusCode.success_max_count_read
-
-	def _read_str_no_events(self) -> str:
-		"""Reads response from the instrument. The response is then trimmed for trailing LF. \n
-		Sending of any read events is blocked."""
-		if self.read_delay > 0:
-			time.sleep(self.read_delay / 1000)
-		stream = StreamWriter.as_string_var()
-		self._read_unknown_len(stream, False)
-		return stream.content
-
-	def _query_str_no_events(self, query: str) -> str:
-		"""Queries the instrument and reads the response as string.
-		The length of the string is not limited. The response is then trimmed for trailing LF.
-		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
-		response = ''
-		self.write(query)
-		try:
-			response = self._read_str_no_events()
-		except pyvisa.VisaIOError:
-			self._narrow_down_io_tout_error(f"Querying '{query.rstrip(self._term_char)}' - ")
-		return response
-
-	def _query_str_no_events_timed(self, query: str, timeout: int, suppress_read_tout: bool = False) -> str:
-		"""Queries the instrument and reads the response as string.
-		The entered timeout sets the VISA timeout just for this call. You can suppress the timeout error.
-		The length of the string is not limited. The response is then trimmed for trailing LF.
-		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
-		response = ''
-		self.write(query)
-		try:
-			response = self._read_str_timed(timeout, suppress_read_tout)
-		except pyvisa.VisaIOError:
-			self._narrow_down_io_tout_error(f"Querying with timeout {timeout} ms '{query.rstrip(self._term_char)}' - ", timeout)
-		return response
-
-	def _read_str_timed(self, timeout: int, suppress_read_tout: bool = False) -> str:
-		"""Reads response from the instrument with a VISA timeout temporarily set for the read.
-		The VISA timeout is set back to the previous value before the method finishes even if an exception occurs.
-		Sending of any read events is blocked."""
-		old_visa_tout = self.visa_timeout
-		if suppress_read_tout:
-			try:
-				if timeout != old_visa_tout:
-					self.visa_timeout = timeout
-				data = self._read_str_no_events()
-				return data
-			except TimeoutError:
-				pass
-			finally:
-				self.visa_timeout = old_visa_tout
-		else:
-			try:
-				if timeout != old_visa_tout:
-					self.visa_timeout = timeout
-				data = self._read_str_no_events()
-				return data
-			finally:
-				self.visa_timeout = old_visa_tout
-
-	def _read_str(self) -> str:
-		"""Reads response from the instrument. The response is then trimmed for trailing LF."""
-		if self.read_delay > 0:
-			time.sleep(self.read_delay / 1000)
-		stream = StreamWriter.as_string_var()
-		self._read_unknown_len(stream, True)
-		return stream.content
-
-	def query_str(self, query: str) -> str:
-		"""Queries the instrument and reads the response as string.
-		The length of the string is not limited. The response is then trimmed for trailing LF."""
-		response = ''
-		self.write(query)
-		try:
-			response = self._read_str()
-		except pyvisa.VisaIOError:
-			self._narrow_down_io_tout_error(f"Querying '{query.rstrip(self._term_char)}' - ")
-		return response
-
-	def query_str_no_tout_err(self, query: str, tout: int) -> str:
-		"""Same as query_str, but you can set the timeout just for this one call.
-		If the timeout exception occurs, it is suppressed and the method returns Null"""
-		response = None
-		old_tout = self.visa_timeout
-		try:
-			self.visa_timeout = tout
-			response = self.query_str(query)
-		except (pyvisa.VisaIOError, InstrumentErrors.StatusException):
-			pass
-		finally:
-			self.visa_timeout = old_tout
-		return response
-
-	def write_with_opc(self, command: str, timeout: int = None) -> None:
-		"""Sends command with OPC-sync.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		self._write_and_wait_for_opc(command, False, timeout)
-
-	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
-		"""Query string with OPC synchronization.
-		The response is trimmed for any trailing LF.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		timeout = self._resolve_opc_timeout(timeout)
-		if self.vxi_capable and self._opc_wait_mode is not WaitForOpcMode.opc_query:
-			# For Vxi session, use the STB poll or SRQ wait and then read the response
-			stb = self._write_and_wait_for_opc(query, True, timeout)
-			self._check_msg_available_after_opc_wait(stb, query, timeout, 'Query String With OPC')
-			response = self._read_str()
-		else:
-			# For non-Vxi sessions, use the longer VISA Timeout without the *OPC?
-			# Same is valid for WaitForOpcMode.OpcQuery
-			InstrumentErrors.assert_query_has_qmark(query, 'Query with VISA timeout')
-			self.write(query)
-			old_tout = self.visa_timeout
-			# Change VISA Timeout if necessary
-			if old_tout != timeout:
-				self.visa_timeout = timeout
-			try:
-				# try-catch to set the VISA timeout back
-				response = self._read_str()
-				if self._opc_wait_mode is WaitForOpcMode.opc_query:
-					self.query_opc()
-			finally:
-				if old_tout != timeout:
-					self.visa_timeout = old_tout
-
-		return response
-
-	def query_opc(self, timeout: int = 0) -> bool:
-		"""Sends *OPC? query and reads the result.
-		If you define timeout > 0, the VISA timeout is set to that value just for this method call."""
-		if self.disable_opc_query:
-			return True
-		if timeout > 0:
-			response = self._query_str_no_events_timed('*OPC?', timeout)
-		else:
-			response = self._query_str_no_events('*OPC?')
-		return Conv.str_to_bool(response)
-
-	def query_and_clear_esr(self) -> int:
-		"""Sends *ESR? query and reads the result."""
-		response = self._query_str_no_events('*ESR?')
-		return int(response)
-
-	def _check_msg_available_after_opc_wait(self, stb: StatusByte, query: str, timeout: int, context: str) -> None:
-		"""Used internally after _StbPolling() to check if the message is available.
-		Throws an exception in case of MAV not available."""
-		if not self.vxi_capable:
-			return
-		if stb & StatusByte.message_available:
-			return
-		# Message not available
-		context = context + f" SCPI query '{query.rstrip(self._term_char)}'"
-		if stb & StatusByte.error_queue_not_empty:
-			# Instrument reports an error
-			InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
-		else:
-			# Sometimes even if the StatusByte.MessageAvailable is false, the message is available.
-			# Try to read the STB again
-			stb = self._read_stb()
-			if not stb & StatusByte.event_status_byte:
-				# Instrument did not respond within the defined time
-				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f'{context} No response from the instrument.')
-
-	def error_in_error_queue(self) -> bool:
-		"""Returns true, if error queue contains at least one error."""
-		stb = self._query_stb()
-		return (stb & StatusByte.error_queue_not_empty) != 0
-
-	def reset_ese_sre(self) -> None:
-		"""Resets the status of ESE and SRE registers to default values."""
-		self._set_regs_ese_sre(self._opc_wait_mode)
-
-	def write_bin_block(self, cmd: str, data_stream: StreamReader) -> None:
-		"""Writes all the payload as binary data block to the instrument.
-		The binary data header is added at the beginning of the transmission automatically.
-		:param cmd: [str] SCPI command with which to send the data
-		:param data_stream: [StreamReader] data provider for the payload"""
-		data_size = len(data_stream)
-		len_str = f'{data_size}'
-		cmd = cmd.rstrip(self._term_char)
-		if '#' in cmd:
-			raise Exception(
-				f"Command '{cmd}' must be provided without the binary data header. "
-				f"The method 'write_bin_block' composes and prepends the binary data header automatically.")
-		if data_size <= self._std_bin_block_header_max_len:
-			# Standard bin data header for sizes below 1E9 bytes, e.g.: '#512345'
-			cmd_plus_header = f'{cmd}#{len(len_str)}{len_str}'.encode('utf-8')
-		else:
-			# Big sizes bin data header: e.g.: '#(3000000000)'
-			cmd_plus_header = f'{cmd}#({len_str})'.encode('utf-8')
-
-		if data_size <= self._data_chunk_size:
-			# Write all in one step
-			full_chunk = data_stream.read_as_binary()
-			write_buf = cmd_plus_header + full_chunk
-			if self._add_term_char_to_write_bin_block:
-				write_buf += self._term_char_bin
-			self._session.write_raw(write_buf)
-			# Event sending
-			if self.on_write_chunk_handler:
-				event_args = EventArgsChunk(True, 0, data_size, data_size, data_size, True, 1, full_chunk if self.io_events_include_data else None)
-				self.on_write_chunk_handler(event_args)
-		else:
-			# Write in chunks
-			try:
-				# Use finally to set the session send_end back to True
-				self._session.send_end = False
-				total_chunks = calculate_chunks_count(data_size, self._data_chunk_size)
-				chunk_ix = 0
-				if self.write_delay > 0:
-					time.sleep(self.write_delay / 1000)
-				# Write bin header
-				self._session.write_raw(cmd_plus_header)
-				# Write chunks
-				while True:
-					if len(data_stream) > self._data_chunk_size:
-						#  Not the last segment
-						chunk = data_stream.read_as_binary(self._data_chunk_size)
-						self._session.write_raw(chunk)
-						# Event sending
-						if self.on_write_chunk_handler:
-							event_args = EventArgsChunk(
-								True, chunk_ix, self._data_chunk_size, data_size, data_size - len(data_stream), False, total_chunks, chunk if self.io_events_include_data else None)
-							self.on_write_chunk_handler(event_args)
-					else:
-						# Last segment, indicate end of message again
-						chunk = data_stream.read_as_binary()
-						if self._add_term_char_to_write_bin_block:
-							# Append LF
-							self._session.write_raw(chunk)
-							self._session.send_end = True
-							self._session.write_raw(self._term_char_bin)
-						else:
-							self._session.send_end = True
-							self._session.write_raw(chunk)
-
-						# Event sending
-						if self.on_write_chunk_handler:
-							event_args = EventArgsChunk(True, chunk_ix, len(chunk), data_size, data_size, True, total_chunks, chunk if self.io_events_include_data else None)
-							self.on_write_chunk_handler(event_args)
-						break
-					chunk_ix += 1
-			finally:
-				self._session.send_end = True
-
-	def _parse_bin_data_header(self, exc_if_not_bin: bool) -> Tuple[ReadDataType, str, int]:
-		"""Parses the binary data block and returns the expected length of the following data block. \n
-		:param exc_if_not_bin: [bool] if True, the method throws exception in case the data is not binary.
-		:return: read_data_type: [ReadDataType], parsed_header: [string], bin_data_len: [integer]"""
-		length = -1
-		if self.read_delay > 0:
-			time.sleep(self.read_delay / 1000)
-
-		char: AnyStr = self._session.read_bytes(1, break_on_termchar=True)
-		if char == b'#':
-			# binary transfer
-			char = self._session.read_bytes(1, break_on_termchar=True)
-			if char == b'0':
-				data_type = ReadDataType.bin_unknown_len
-				return data_type, '#0', -1
-			if char == b'(':
-				# format for big lengths i.e. > 1E9 bytes: '#(1234567890123)...'
-				data_type = ReadDataType.bin_known_len
-				len_str = (self.read_up_to_char(b')', 100)[:-1]).decode('utf-8')
-				whole_hdr = '#(' + len_str + ')'
-				length = int(len_str)
-				return data_type, whole_hdr, length
-
-			# classic format for < 1E9 bytes: '#9123456789...'
-			data_type = ReadDataType.bin_known_len
-			len_of_len = int(char)
-			len_str = self._session.read_bytes(len_of_len).decode('utf-8')
-			length = int(len_str)
-			whole_hdr = '#' + char.decode('utf-8') + len_str
-			return data_type, whole_hdr, length
-
-		data_type = ReadDataType.ascii
-		if char == self._term_char_bin:
-			data_type = ReadDataType.null
-		if self.vxi_capable:
-			# For Vxi session, to be sure, check whether there are more chars in the read buffer
-			stb = self._read_stb()
-			if stb & StatusByte.message_available:
-				data_type = ReadDataType.ascii
-		whole_hdr = char.decode('utf-8')
-		if exc_if_not_bin:
-			if data_type == ReadDataType.null:
-				InstrumentErrors.throw_bin_block_unexp_resp_exception(self._resource_name, self._term_char)
-			# Read 20 more characters to compose a better exception message
-			whole_hdr += self.read_up_to_char(self._term_char_bin, 20).decode('utf-8')
-			if self.last_status == pyvisa.constants.StatusCode.success_max_count_read:
-				self._flush_junk_data()
-			InstrumentErrors.throw_bin_block_unexp_resp_exception(self._resource_name, whole_hdr)
-		return data_type, whole_hdr, length
-
-	def read_bin_block(self, stream: StreamWriter, exc_if_not_bin: bool) -> None:
-		"""Reads binary data block to the provided stream. \n
-		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
-		:param exc_if_not_bin: if True, the method throws exception if the received data is not binary"""
-		data_type, header, length = self._parse_bin_data_header(exc_if_not_bin)
-		if data_type == ReadDataType.ascii:
-			stream.switch_to_string_data()
-			self._read_unknown_len(stream, True, header)
-		elif data_type == ReadDataType.null:
-			# No data, consider it ASCII, Return empty string, and False (signaling ASCII transfer)
-			stream.switch_to_string_data()
-		elif data_type == ReadDataType.bin_unknown_len:
-			if not self.vxi_capable:
-				raise Exception(f'Non-Vxi11 sessions can not read binary data block of unknown length.')
-			self._read_unknown_len(stream, True)
-		elif length == 0:
-			self._flush_junk_data()
-		else:
-			self._read_bin_block_known_len(stream, length)
-
-	def _read_bin_block_known_len(self, stream: StreamWriter, length: int) -> None:
-		"""Reads binary data of defined length. All remaining data above the length are disposed of. \n
-		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
-		:param length: [int] expected length of the data"""
-		# Use try-catch to switch the termination character back ON in case of an exception (for non-Vxi sessions)
-		try:
-			# Binary transmission, for non-Vxi session, set the termination character to OFF
-			if not self.vxi_capable:
-				self._session.read_termination = False
-			# Binary data of known length
-			left_to_read = length
-			self.last_status = pyvisa.constants.StatusCode.success
-			with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
-				chunk_ix = 0
-				total_chunks = calculate_chunks_count(length, self._data_chunk_size)
-				while len(stream) < length:
-					chunk_size = min(self._data_chunk_size, left_to_read)
-					chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
-					left_to_read -= len(chunk)
-					stream.write(chunk)
-					if self.on_read_chunk_handler:
-						event_args = EventArgsChunk(True, chunk_ix, chunk_size, length, len(stream), left_to_read == 0, total_chunks, chunk if self.io_events_include_data else None)
-						self.on_read_chunk_handler(event_args)
-					chunk_ix += 1
-			if self._last_status_more_data_available():
-				if not self.vxi_capable:
-					self._session.read_termination = self._term_char
-				self._flush_junk_data()
-		finally:
-			# Make sure that in any case the self._session.read_termination is ON again for non-Vxi sessions
-			if not self.vxi_capable:
-				self._session.read_termination = self._term_char
-
-	def query_bin_block(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True) -> None:
-		"""Query binary data block and returns it as byte data. \n
-		:param query: [str] query to send to the instrument
-		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
-		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary"""
-		self.write(query)
-		self.read_bin_block(stream, exc_if_not_bin)
-		return
-
-	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
-		"""Query binary data block with OPC and returns it as byte data.
-		:param query: [str] query to send to the instrument
-		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
-		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary
-		:param timeout: Optional[Integer] timeout for the operation. If you skip it, the method uses the current opc timeout."""
-		timeout = self._resolve_opc_timeout(timeout)
-		if self.vxi_capable and self._opc_wait_mode != WaitForOpcMode.opc_query:
-			# For Vxi session, use the STB poll and read the response
-			stb = self._write_and_wait_for_opc(query, True, timeout)
-			self._check_msg_available_after_opc_wait(stb, query, timeout, 'query_bin_block_with_opc')
-			self.read_bin_block(stream, exc_if_not_bin)
-		else:
-			# For non-Vxi session, use the longer VISA Timeout without the *OPC
-			InstrumentErrors.assert_query_has_qmark(query, 'query_bin_block_with_opc')
-			self.write(query)
-			old_visa_timeout = self.visa_timeout
-			# Change VISA Timeout if necessary
-			if old_visa_timeout != timeout:
-				self.visa_timeout = timeout
-			try:
-				# try-catch to set the VISA timeout back
-				self.read_bin_block(stream, exc_if_not_bin)
-				if self._opc_wait_mode == WaitForOpcMode.opc_query:
-					self.query_opc()
-			finally:
-				# Change VISA Timeout back if necessary
-				if old_visa_timeout != timeout:
-					self.visa_timeout = old_visa_timeout
-
-	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
-		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
-		Returns the read data including the stop character."""
-		response = b''
-		for i in range(max_cnt):
-			char, self.last_status = self._session.visalib.read(self._session.session, 1)
-			response += char
-			if char in stop_chars:
-				break
-			if self.last_status != pyvisa.constants.StatusCode.success_max_count_read:
-				break
-		return response
-
-	def get_session_handle(self) -> object:
-		"""Returns the underlying pyvisa session."""
-		return self._session
-
-	def close(self) -> None:
-		"""Closes the Visa session.
-		If the object was created with the direct session input, the session is not closed."""
-		if not self.reusing_session:
-			self._session.close()
-
-	# Events
-
-
-class EventArgsChunk:
-	"""Event arguments for chunk io event."""
-
-	def __init__(
-			self,
-			binary: bool,
-			chunk_ix: int,
-			chunk_size: int,
-			total_size: int,
-			transferred_size: int,
-			end_of_transfer: bool,
-			total_chunks: int or None,
-			data: AnyStr = None):
-
-		self.binary = binary
-		self.chunk_ix = chunk_ix
-		self.total_chunks = total_chunks
-		self.chunk_size = chunk_size
-		self.transferred_size = transferred_size
-		self.total_size = total_size
-		self.end_of_transfer = end_of_transfer
-		self.data = data
-
-	def __str__(self):
-		if self.binary:
-			type_info = 'binary'
-		else:
-			type_info = 'ascii'
-		if not self.total_chunks:
-			chunk_info = f' chunk nr. {self.chunk_ix + 1}'
-		elif self.total_chunks > 1:
-			chunk_info = f' chunk nr. {self.chunk_ix + 1}/{self.total_chunks}'
-		else:
-			chunk_info = ' chunk nr. 1/1'
-		eot = ' (EOT)' if self.end_of_transfer else ''
-		result = \
-			f'EventArgsChunk {type_info},{chunk_info}, {size_to_kb_mb_string(self.chunk_size, True)}, ' \
-			f'sum {size_to_kb_mb_string(self.transferred_size, True)} / {size_to_kb_mb_string(self.total_size, True) if self.total_size else "<N.A.>"}{eot}.'
-		return result
+import time
+from enum import Enum, Flag
+from typing import Tuple, Callable, AnyStr
+import os.path
+import re
+import threading
+
+# noinspection PyPackageRequirements
+import pyvisa
+
+from .VisaPluginSocketIo import ResourceManager, SocketIo
+from . import InstrumentSettings, InstrumentErrors, Conversions as Conv
+from .InstrumentSettings import WaitForOpcMode, InstrViClearMode as ViClearMode
+from .StreamReader import StreamReader
+from .StreamWriter import StreamWriter
+from .Utilities import size_to_kb_mb_string, calculate_chunks_count
+import platform
+import struct
+
+
+class SessionKind(Enum):
+	"""Visa instrument session type."""
+	unsupported = 0
+	gpib = 1
+	serial = 2
+	vxi11 = 3
+	socket = 5
+	usb = 6
+	rs_nrp = 7
+
+
+class ReadDataType(Enum):
+	"""Data type returned by the instrument."""
+	unknown = 0
+	ascii = 1
+	null = 2
+	bin_known_len = 3
+	bin_unknown_len = 4
+
+
+class StatusByte(Flag):
+	"""Status Byte flags."""
+	NONE = 0x00
+	error_queue_not_empty = 0x04
+	questionable_status_reg = 0x08
+	message_available = 0x10
+	event_status_byte = 0x20
+	request_service = 0x40
+	operation_status_reg = 0x80
+
+
+class EventStatusRegister(Flag):
+	"""Event Status Register flags."""
+	null = 0x00
+	operation_complete = 0x01
+
+
+# noinspection PyUnresolvedReferences
+class VisaSession(object):
+	"""Extended VISA class."""
+
+	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
+		self.reusing_session = direct_session is not None
+		# noinspection PyTypeChecker
+		self._data_chunk_size: int = None
+		self._std_bin_block_header_max_len: int = 999999999
+		self._lock = None
+		self.disable_opc_query: bool = settings.disable_opc_query
+		self.last_status = None
+		self.visa_library_name = None
+
+		# Implemented for interface compatibility with VisaSessionSim
+		self.cached_to_stream = False
+
+		# Event handlers
+		# noinspection PyTypeChecker
+		self.on_read_chunk_handler: Callable = None
+		"""If assigned a handler, the VisaSession sends it event on each read chunk transfer."""
+		# noinspection PyTypeChecker
+		self.on_write_chunk_handler: Callable = None
+		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
+		self.io_events_include_data: bool = False
+		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
+
+		if self.reusing_session:
+			# Reuse the session
+			assert isinstance(direct_session, pyvisa.Resource) or isinstance(direct_session, SocketIo), f"Direct_session must be a VISA resource object. Actual type: '{type(direct_session)}', value: '{direct_session}'"
+			self._session = direct_session
+			self._resource_name = self._session.resource_name
+		else:
+			# Create new session
+			# Check resource_name for the trailing (SelectVisa=..)
+			pure_resource_name, visa_select = self._get_pure_resource_name(resource_name)
+			if settings.visa_select is not None:
+				visa_select = settings.visa_select
+			self._rm = VisaSession.get_resource_manager(visa_select)
+			self.manufacturer = self._get_visa_manufacturer()
+
+			# Resource manager opening
+			try:
+				self._session = self._rm.open_resource(pure_resource_name)
+			except pyvisa.VisaIOError as e:
+				if e.error_code != pyvisa.constants.StatusCode.error_resource_not_found:
+					raise e
+				message = e.description
+				message += f"\nLibrary: {self._rm.visalib}\nManufacturer: {self.manufacturer}\nResource Name: '{resource_name}'"
+				raise InstrumentErrors.ResourceError(resource_name, message)
+			self._resource_name = resource_name
+
+		# Decide, whether to create a new thread lock or the existing one from the session
+		if hasattr(self._session, 'session_thread_rlock'):
+			rlock = self._session.session_thread_rlock
+			if isinstance(rlock, type(threading.RLock())):
+				self.assign_lock(rlock)
+		if self.get_lock() is None:
+			# The existing session did not have a thread lock, assign a new one
+			self.assign_lock(threading.RLock())
+
+		self._interface_type = SessionKind.unsupported
+		if self._session.interface_type == pyvisa.constants.InterfaceType.gpib or self._session.interface_type == pyvisa.constants.InterfaceType.gpib:
+			self._interface_type = SessionKind.gpib
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.rsnrp:
+			self._interface_type = SessionKind.rs_nrp
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.asrl:
+			self._interface_type = SessionKind.serial
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.usb:
+			# Check whether it is not the NRP-Z
+			intf_type = self._session.get_visa_attribute(pyvisa.constants.VI_ATTR_INTF_TYPE)
+			if intf_type == pyvisa.constants.InterfaceType.rsnrp:
+				self._interface_type = SessionKind.rs_nrp
+
+		elif self._session.interface_type == pyvisa.constants.InterfaceType.tcpip:
+			self._interface_type = SessionKind.vxi11
+			if self._session.resource_class == 'SOCKET':
+				self._interface_type = SessionKind.socket
+
+		# Specifics for different interfaces
+		self._assure_write_with_tc = settings.assure_write_with_tc
+		self._term_char = settings.term_char
+		self._term_char_bin = self._term_char.encode('utf-8')
+		self._session.write_termination = ''
+		self.vxi_capable = True
+
+		if self._interface_type == SessionKind.serial:
+			self._session.read_termination = self._term_char
+			self.vxi_capable = False
+			self._assure_write_with_tc = True
+		elif self._interface_type == SessionKind.socket:
+			self._session.read_termination = self._term_char
+			self.vxi_capable = False
+			self._assure_write_with_tc = True
+		else:
+			self._session.read_termination = ''
+
+		# NRP-Z specific settings
+		if self.is_rsnrp_session():
+			self.disable_opc_query = True
+			# NRP-Z does not support chunk reading, therefore the segment must be in one piece
+			settings.io_segment_size = 1000000
+			self.vxi_capable = False
+
+		self.write_delay = settings.write_delay
+		self.read_delay = settings.read_delay
+		self._viclear_exe_mode = settings.viclear_exe_mode
+		self._opc_wait_mode = settings.opc_wait_mode
+
+		# Parameters that need to be coerced based on Vxi-capability
+		if self.vxi_capable:
+			self._add_term_char_to_write_bin_block = settings.add_term_char_to_write_bin_block
+		else:
+			self._add_term_char_to_write_bin_block = True
+
+		# Changeable settings
+		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
+		self.visa_timeout = settings.visa_timeout
+		self._session.chunk_size = settings.io_segment_size
+		self._data_chunk_size = settings.io_segment_size
+
+		# Must call the VISA viClear() before the any communication with the instrument
+		self.clear()
+
+		# Further steps are for NRP-Z session not valid
+		if self.is_rsnrp_session():
+			return
+
+		# Clear instrument status
+		self.write("*CLS")
+		if self.vxi_capable:
+			stb = self._read_stb()
+			if stb & StatusByte.message_available:
+				self._flush_junk_data()
+
+		# Apply settings for ESE and SRE, plus coerce the _opcWaitMode if necessary
+		self._opc_wait_mode = self._set_regs_ese_sre(self._opc_wait_mode)
+
+	@staticmethod
+	def _get_pure_resource_name(resource_name: str):
+		"""Returns pure resource name stripped of the (SelectVisa) part and the visa_select string"""
+		m = re.search(r'(.+)\(SelectVisa=([^),]+)\)', resource_name)
+		if not m:
+			return resource_name, None
+		resource_name = m.group(1).strip()
+		visa_select = m.group(2).strip()
+		return resource_name, visa_select
+
+	@classmethod
+	def get_resource_manager(cls, visa_select: str) -> pyvisa.ResourceManager:
+		"""Returns resource manager for the desired VISA implementation"""
+		operating_system = platform.system().lower()
+		bittness = struct.calcsize("P") * 8
+		if visa_select is None or visa_select in ['@default', '@standard', 'default', 'standard', 'defaultvisa', 'standardvisa', '@defaultvisa', '@standardvisa']:
+			return pyvisa.ResourceManager()
+		if visa_select.lower() in ['@ni', 'ni', 'visa-ni', 'nivisa', 'ni-visa', 'nationalinstruments', 'nationalinstrumentsvisa']:
+			return pyvisa.ResourceManager('@ni')
+		if visa_select.lower() in ['@py', 'pyvisa', 'visa-py', 'pyvisa-py']:
+			return pyvisa.ResourceManager('@py')
+		if 'rohde&schwarz' in visa_select.lower() or 'rohdeschwarz' in visa_select.lower() or visa_select.lower() == 'rsvisa' or visa_select.lower() == 'rs' or visa_select.lower() == 'r&s':
+			if operating_system == 'windows':
+				if bittness == 32:
+					visa_select = r'c:\Windows\SysWOW64\RsVisa32.dll'
+				else:
+					visa_select = r'c:\Windows\system32\RsVisa32.dll'
+				return pyvisa.ResourceManager(visa_select)
+			elif operating_system == 'linux':
+				# The default install location may be different
+				# for debian/red hat/opensuse derived distributions
+				check_visa = [f'/usr/lib{bittness}/librsvisa.so', r'/usr/lib/librsvisa.so']
+				for check in check_visa:
+					if os.path.isfile(check):
+						return pyvisa.ResourceManager(check)
+
+		if visa_select.lower() in ['socketio', 'socket', 'none']:
+			return ResourceManager()
+		return pyvisa.ResourceManager(visa_select)
+
+	def _get_visa_manufacturer(self) -> str:
+		"""Returns manufacturer of the current VISA"""
+		if hasattr(self._rm, 'VisaManufacturerName'):
+			return self._rm.VisaManufacturerName
+		try:
+			return self._rm.visalib.get_attribute(self._rm.session, pyvisa.constants.VI_ATTR_RSRC_MANF_NAME)[0]
+		except TypeError:
+			return self._rm.visalib.__class__.__name__
+
+	def is_rsnrp_session(self) -> bool:
+		"""Returns True, if the current session is a NRP-Z session"""
+		return self._interface_type == SessionKind.rs_nrp
+
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the provided thread lock by setting the pyvisa runtime session attribute 'session_thread_rlock'
+		This is done, because if the session is to be entered as an existing session to another RsInstrument object,
+		the lock must be shared as well. The lock is only used by the parent class Instrument."""
+		setattr(self._session, 'session_thread_rlock', lock)
+		self._lock = lock
+
+	def get_lock(self) -> threading.RLock:
+		"""Returns the current RLock object."""
+		return self._lock
+
+	@property
+	def visa_timeout(self) -> int:
+		"""See the visa_timeout.setter."""
+		return int(self._session.timeout)
+
+	@visa_timeout.setter
+	def visa_timeout(self, value: int) -> None:
+		"""Sets / Gets visa IO timeout in milliseconds."""
+		self._session.timeout = int(value)
+
+	@property
+	def data_chunk_size(self) -> int:
+		"""Returns max chunk size of one data block."""
+		return self._data_chunk_size
+
+	@data_chunk_size.setter
+	def data_chunk_size(self, chunk_size: int) -> None:
+		"""Sets the maximum size of one block transferred during write/read operations."""
+		self._data_chunk_size = int(chunk_size)
+		self._session.chunk_size = int(chunk_size)
+
+	def _resolve_opc_timeout(self, timeout: int) -> int:
+		"""Resolves entered timeout value - if the input value is less than 1, it is replaces with opc_timeout."""
+		if timeout is None or timeout < 1:
+			return self.opc_timeout
+		else:
+			return timeout
+
+	def _set_regs_ese_sre(self, mode: WaitForOpcMode) -> WaitForOpcMode:
+		"""Based on the WaitForOpcMode, it sets the ESE and SRE register masks.
+		Returns coerced WaitForOpcMode."""
+		# Set the SRE and ESE registers accordingly
+		# No SRE is supported
+		self._set_ese_mask(EventStatusRegister.operation_complete)
+		self._set_sre_mask(StatusByte.NONE)
+		return mode
+
+	def _set_ese_mask(self, mask: EventStatusRegister, reset: bool = True) -> None:
+		"""Sends *ESE command with mask parameter."""
+		if reset is False:
+			current_value = int(self._query_str_no_events("*ESE?"))
+			mask = current_value | mask.value
+		self.write("*ESE %d" % mask.value)
+
+	def _set_sre_mask(self, mask: StatusByte, reset: bool = True) -> None:
+		"""Sends *SRE command with StatusByte mask parameter."""
+		if reset is False:
+			current_value = int(self._query_str_no_events("*SRE?"))
+			mask = current_value | mask.value
+		# Also affect the _opc_wait_mode:
+		# If the mask has event_status_byte == false, and the _opc_wait_mode is service_request, set it to stb_poll
+		# If the mask has event_status_byte == true, do not change anything
+		self.write("*SRE %d" % mask.value)
+
+	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int, end_mask: StatusByte) -> StatusByte:
+		"""Reads Status Byte Register and ends if the ESB bit (5) is set to 1.
+		Also works with the SOCKET and SERIAL interface by sending *STB? query.
+		In that case however, command cannot be a query.
+		Returns the last read Status Byte value."""
+		timeout_secs = timeout / 1000
+		self.clear_before_read()
+		if command.endswith(self._term_char):
+			command = command.rstrip(self._term_char)
+		self.write(command + ';*OPC')
+		# Use catch to return the VISA Timeout back
+		start = time.time()
+		# STB polling loop
+		while True:
+			stb = self._read_stb()
+			elapsed = self._polling_delay(start)
+			if elapsed > timeout_secs:
+				self._narrow_down_opc_tout_error(command, is_query, timeout)
+			if end_mask & stb:
+				break
+		return stb
+
+	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int, end_mask: StatusByte) -> StatusByte:
+		"""Queries Status Byte Register (*STB?) and ends if the ESB bit (5) is set to 1.
+			The command must not be a query. Also works with the SOCKET and SERIAL interface.
+			Returns the last read Status Byte value."""
+		timeout_secs = timeout / 1000
+		self.clear_before_read()
+		if command.endswith(self._term_char):
+			command = command.rstrip(self._term_char)
+		self.write(command + ';*OPC')
+		start = time.time()
+		# STB polling loop
+		while True:
+			stb = self._query_stb()
+			elapsed = self._polling_delay(start)
+			if elapsed > timeout_secs:
+				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout)
+			if stb & end_mask:
+				break
+		return stb
+
+	def _narrow_down_opc_tout_error(self, command: str, is_query: bool, timeout: int) -> None:
+		"""Called by the _write_and_poll_stb_vxi when the timeout expires.
+		The method tries to closer identify the cause of the timeout."""
+		stb = self._read_stb()
+		timeout = self._resolve_opc_timeout(timeout)
+		if is_query:
+			if stb & StatusByte.error_queue_not_empty:
+				self.clear()
+				context = f"Sending query '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
+				InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
+			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Sending query '{command.strip()}'.")
+		else:
+			if stb & StatusByte.error_queue_not_empty:
+				self.clear()
+				context = f"Sending command '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
+				InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
+			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Sending command '{command.strip()}'.")
+
+	def _narrow_down_io_tout_error(self, context: str) -> None:
+		"""Called internally after IOTimeoutException can narrow down the error to more specific exception."""
+		if self.vxi_capable:
+			stb = self._read_stb()
+		else:
+			# Non-Vxi session
+			old_tout = self.visa_timeout
+			try:
+				self.visa_timeout = 500
+				stb = self._query_stb()
+			finally:
+				self.visa_timeout = old_tout
+		context = context + f"VISA Timeout error occurred ({self.visa_timeout} milliseconds)"
+		if stb & StatusByte.error_queue_not_empty:
+			InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context + " and ...")
+		# In case the previous exception is not thrown
+		raise InstrumentErrors.TimeoutException(context)
+
+	def _polling_delay(self, start):
+		"""Generates progressive polling delay."""
+
+		elapsed = time.time() - start
+		if self._opc_wait_mode == WaitForOpcMode.stb_poll:
+			if elapsed < 0.01:
+				return elapsed
+			if elapsed < 0.1:
+				time.sleep(0.005)
+				return elapsed
+			if elapsed < 1:
+				time.sleep(0.02)
+				return elapsed
+			if elapsed < 5:
+				time.sleep(0.05)
+				return elapsed
+			if elapsed < 10:
+				time.sleep(0.1)
+				return elapsed
+			if elapsed < 50:
+				time.sleep(0.5)
+				return elapsed
+			time.sleep(1)
+		elif self._opc_wait_mode == WaitForOpcMode.stb_poll_slow:
+			if elapsed < 0.01:
+				time.sleep(0.001)
+				return elapsed
+			if elapsed < 1:
+				time.sleep(0.02)
+				return elapsed
+			if elapsed < 5:
+				time.sleep(0.1)
+				return elapsed
+			if elapsed < 10:
+				time.sleep(0.2)
+				return elapsed
+			if elapsed < 20:
+				time.sleep(0.5)
+				return elapsed
+			time.sleep(1)
+		elif self._opc_wait_mode == WaitForOpcMode.stb_poll_superslow:
+			if elapsed < 1:
+				time.sleep(0.1)
+				return elapsed
+			if elapsed < 10:
+				time.sleep(0.5)
+				return elapsed
+			if elapsed < 20:
+				time.sleep(1)
+				return elapsed
+			time.sleep(2)
+
+		return elapsed
+
+	def query_syst_error(self) -> str or None:
+		"""Returns one response to the SYSTEM:ERROR? query."""
+		error = self.query_str("SYST:ERR?")
+		if error.startswith('0,'):
+			return None
+		return error.strip()
+
+	def query_all_syst_errors(self) -> list or None:
+		"""Returns all errors in the instrument's error queue."""
+		errors = []
+		while True:
+			entry = self.query_syst_error()
+			if entry is None:
+				break
+			errors.append(entry)
+			if len(errors) > 50:
+				# Safety stop
+				errors.append('query_all_syst_errors - max limit 50 of SYST:ERR? sent.')
+				break
+
+		if len(errors) == 0:
+			return None
+		else:
+			return errors
+
+	def _query_stb(self) -> StatusByte:
+		"""Sends *STB? query and reads the result."""
+		return StatusByte(int(self._query_str_no_events('*STB?')))
+
+	def _read_stb(self) -> StatusByte:
+		"""Calls viReadStb and returns the result."""
+		return StatusByte(self._session.read_stb())
+
+	def clear_before_read(self) -> None:
+		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
+
+		# For NRP-Z sessions, skip this completely
+		if self.is_rsnrp_session():
+			return
+
+		if not self.vxi_capable:
+			# Non-Vxi session must use *CLS in any case
+			self.write("*CLS")
+			correct = False
+			opc = self._query_str_no_events('*OPC?')
+			repeat = 0
+			while not correct:
+				if len(opc) <= 2:
+					opc = opc.strip()
+					correct = opc == '0' or opc == '1'
+				if not correct:
+					# Read again with a small VISA timeout
+					opc = self._read_str_timed(5, True)
+				repeat += 1
+				if repeat > 10:
+					break
+
+		stb = self._query_stb()
+		condition = StatusByte.error_queue_not_empty | StatusByte.message_available | StatusByte.event_status_byte
+		if not stb & condition:
+			return
+		repeat = 0
+		# Loop more times to clear the status subsystem
+		while stb & condition:
+			if stb & StatusByte.error_queue_not_empty:
+				self.write("*CLS")
+				_ = self.query_all_syst_errors()
+			if stb & StatusByte.message_available:
+				# Clear output buffer
+				self._flush_junk_data()
+			if stb & StatusByte.event_status_byte:
+				# OPC or error bits in the ESR
+				self.write("*CLS")
+				self.query_and_clear_esr()
+			# Check if the status byte value changed
+			previous_stb = stb
+			stb = self._query_stb()
+			if stb == previous_stb:
+				repeat += 1
+				if repeat > 10:
+					raise Exception(f"Cannot clear the instrument's status subsystem. Status Byte: '{stb}'")
+
+	def _flush_junk_data(self) -> None:
+		"""Reads junk bytes to clear the instrument's output buffer."""
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+		self._read_unknown_len(StreamWriter.as_bin_var(), False)
+
+	def clear(self) -> None:
+		"""Perform VISA viClear conditionally based on the instrument settings."""
+		perform_all = ViClearMode.execute_on_all in self._viclear_exe_mode
+		perform = False
+		if perform_all:
+			perform = True
+		else:
+			# Perform on all is blocked, use the SessionKind to decide
+			if self._interface_type == SessionKind.gpib:
+				perform = ViClearMode.execute_on_gpib in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.serial:
+				perform = ViClearMode.execute_on_serial in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.socket:
+				perform = ViClearMode.execute_on_socket in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.usb:
+				perform = ViClearMode.execute_on_usb in self._viclear_exe_mode
+
+			elif self._interface_type == SessionKind.vxi11:
+				perform = ViClearMode.execute_on_tcpvxi in self._viclear_exe_mode
+
+		if not perform:
+			return
+
+		if ViClearMode.ignore_error in self._viclear_exe_mode:
+			# noinspection PyBroadException
+			try:
+				self._session.clear()
+			except Exception:
+				pass
+		else:
+			self._session.clear()
+
+	def _write_and_wait_for_opc(self, command: str, is_query: bool, timeout: int) -> StatusByte:
+		"""Internal method to synchronise a command with OPC timeout.
+		Timeout value 0 means the OPC timeout is used."""
+		timeout = self._resolve_opc_timeout(timeout)
+
+		if command.endswith(self._term_char):
+			command = command.rstrip(self._term_char)
+		if is_query:
+			InstrumentErrors.assert_query_has_qmark(command, "Query with OPC")
+		else:
+			InstrumentErrors.assert_cmd_has_no_qmark(command, "Write with OPC")
+
+		if self._opc_wait_mode == WaitForOpcMode.opc_query:
+			if is_query:
+				raise Exception("Sending a query with OpcQuery synchronization is not possible")
+			stb = self._write_and_query_opc(command, timeout)
+		else:
+			# STB polling
+			end_stb_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
+			if is_query:
+				end_stb_mask |= StatusByte.message_available
+			if self.vxi_capable:
+				stb = self._write_and_poll_stb_vxi(command, is_query, timeout, end_stb_mask)
+			else:
+				stb = self._write_and_poll_stb_non_vxi(command, timeout, end_stb_mask)
+
+		return stb
+
+	def _write_and_query_opc(self, cmd: str, timeout: int) -> StatusByte:
+		"""Internal method to write a command followed by query_opc().
+		Used for opc-synchronization if the mode is set to WaitForOpcMode.opc_query or the session is not-vxi.
+		Timeout value 0 means the OPC timeout is used."""
+		old_tout = self.visa_timeout
+
+		# Change VISA Timeout if necessary
+		if old_tout != timeout:
+			self.visa_timeout = timeout
+		try:
+			# try-catch to set the VISA timeout back
+			self.write(cmd)
+			self.query_opc()
+		finally:
+			if old_tout != timeout:
+				self.visa_timeout = old_tout
+		return self._query_stb()
+
+	def write(self, cmd: str) -> None:
+		"""Writes command to the instrument."""
+		if self.write_delay > 0:
+			time.sleep(self.write_delay / 1000)
+		add_tc = False
+		if self._assure_write_with_tc and not cmd.endswith(self._term_char):
+			add_tc = True
+		if add_tc:
+			self._session.write(cmd + self._term_char)
+		else:
+			self._session.write(cmd)
+
+	def _read_unknown_len(self, stream: StreamWriter, allow_chunk_events: bool, prepend_data: AnyStr = None) -> None:
+		"""Reads data of unknown length to the provided WriteStream.
+		The read is performed in an incremental chunk steps to optimize memory use (for NRP-Z session it is set to fixed self._data_chunk_size):
+			- The first read is performed with the fixed size of 1024 bytes
+			- The 2nd one reads 64 kBytes
+			- The 3rd one reads 128 kBytes
+			- The 4th one reads 256 kBytes and so on, with the max cap of self._data_chunk_size
+		:param stream: [StreamWriter] target for the read data
+		:param allow_chunk_events: [bool] if True, the method can send the chunk_events. If False, sending events is blocked.
+		:param prepend_data: Optional[bytes or string] You can prepend this data to the beginning. It will be considered part of the first chunk read
+		:return: read data [bytes or string], depending on the parameter binary."""
+		with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
+			if prepend_data and isinstance(prepend_data, str):
+				prepend_data = prepend_data.encode('utf-8')
+			chunk_ix = 0
+			eot = False
+			while not eot:
+				if self.is_rsnrp_session():
+					chunk_size = self._data_chunk_size
+				else:
+					if chunk_ix == 0:
+						# First read, set 1024 bytes read size
+						chunk_size = 1024
+					elif chunk_ix == 1:
+						chunk_size = 65536
+					else:
+						chunk_size *= 2
+				if chunk_size > self._data_chunk_size:
+					chunk_size = self._data_chunk_size
+				chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
+				if chunk_ix == 0 and prepend_data:
+					chunk = prepend_data + chunk
+				eot = not self._last_status_more_data_available()
+				if not stream.binary:
+					chunk = chunk.decode('utf-8')
+					if eot:
+						chunk = chunk.rstrip(self._term_char)
+				stream.write(chunk)
+				if self.on_read_chunk_handler and allow_chunk_events:
+					total_size = len(stream) if eot is True else None
+					event_args = EventArgsChunk(stream.binary, chunk_ix, len(chunk), total_size, len(stream), eot, None, chunk if self.io_events_include_data else None)
+					self.on_read_chunk_handler(event_args)
+				chunk_ix += 1
+
+	def _last_status_more_data_available(self):
+		"""Returns True, if the last status signalled that more data is available"""
+		return self.last_status == pyvisa.constants.StatusCode.success_max_count_read
+
+	def _read_str_no_events(self) -> str:
+		"""Reads response from the instrument. The response is then trimmed for trailing LF. \n
+		Sending of any read events is blocked."""
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+		stream = StreamWriter.as_string_var()
+		self._read_unknown_len(stream, False)
+		return stream.content
+
+	def _query_str_no_events(self, query: str) -> str:
+		"""Queries the instrument and reads the response as string.
+		The length of the string is not limited. The response is then trimmed for trailing LF.
+		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
+		response = ''
+		self.write(query)
+		try:
+			response = self._read_str_no_events()
+		except pyvisa.VisaIOError:
+			self._narrow_down_io_tout_error("Querying '{}' - ".format(query.rstrip(self._term_char)))
+		return response
+
+	def _read_str_timed(self, timeout: int, suppress_read_tout: bool = False) -> str:
+		"""Reads response from the instrument with a VISA timeout temporarily set for the read.
+		The VISA timeout is set back to the previous value before the method finishes even if an exception occurs.
+		Sending of any read events is blocked."""
+		old_visa_tout = self.visa_timeout
+		if suppress_read_tout:
+			try:
+				if timeout != old_visa_tout:
+					self.visa_timeout = timeout
+				data = self._read_str_no_events()
+				return data
+			except TimeoutError:
+				pass
+			finally:
+				self.visa_timeout = old_visa_tout
+		else:
+			try:
+				if timeout != old_visa_tout:
+					self.visa_timeout = timeout
+				data = self._read_str_no_events()
+				return data
+			finally:
+				self.visa_timeout = old_visa_tout
+
+	def _read_str(self) -> str:
+		"""Reads response from the instrument. The response is then trimmed for trailing LF."""
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+		stream = StreamWriter.as_string_var()
+		self._read_unknown_len(stream, True)
+		return stream.content
+
+	def query_str(self, query: str) -> str:
+		"""Queries the instrument and reads the response as string.
+		The length of the string is not limited. The response is then trimmed for trailing LF."""
+		response = ''
+		self.write(query)
+		try:
+			response = self._read_str()
+		except pyvisa.VisaIOError:
+			self._narrow_down_io_tout_error("Querying '{}' - ".format(query.rstrip(self._term_char)))
+		return response
+
+	def query_str_no_tout_err(self, query: str, tout: int) -> str:
+		"""Same as query_str, but you can set the timeout just for this one call.
+		If the timeout exception occurs, it is suppressed and the method returns Null"""
+		response = None
+		old_tout = self.visa_timeout
+		try:
+			self.visa_timeout = tout
+			response = self.query_str(query)
+		except (pyvisa.VisaIOError, InstrumentErrors.StatusException):
+			pass
+		finally:
+			self.visa_timeout = old_tout
+		return response
+
+	def write_with_opc(self, command: str, timeout: int = None) -> None:
+		"""Sends command with OPC-sync.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		self._write_and_wait_for_opc(command, False, timeout)
+
+	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
+		"""Query string with OPC synchronization.
+		The response is trimmed for any trailing LF.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		timeout = self._resolve_opc_timeout(timeout)
+		if self.vxi_capable and self._opc_wait_mode is not WaitForOpcMode.opc_query:
+			# For Vxi session, use the STB poll or SRQ wait and then read the response
+			stb = self._write_and_wait_for_opc(query, True, timeout)
+			self._check_msg_available_after_opc_wait(stb, query, timeout, "Query String With OPC")
+			response = self._read_str()
+		else:
+			# For non-Vxi sessions, use the longer VISA Timeout without the *OPC?
+			# Same is valid for WaitForOpcMode.OpcQuery
+			InstrumentErrors.assert_query_has_qmark(query, "Query with VISA timeout")
+			self.write(query)
+			old_tout = self.visa_timeout
+			# Change VISA Timeout if necessary
+			if old_tout != timeout:
+				self.visa_timeout = timeout
+			try:
+				# try-catch to set the VISA timeout back
+				response = self._read_str()
+				if self._opc_wait_mode is WaitForOpcMode.opc_query:
+					self.query_opc()
+			finally:
+				if old_tout != timeout:
+					self.visa_timeout = old_tout
+
+		return response
+
+	def query_opc(self) -> bool:
+		"""Sends *OPC? query and reads the result."""
+		if self.disable_opc_query:
+			return True
+		response = self._query_str_no_events("*OPC?")
+		return Conv.str_to_bool(response)
+
+	def query_and_clear_esr(self) -> int:
+		"""Sends *ESR? query and reads the result."""
+		response = self._query_str_no_events("*ESR?")
+		return int(response)
+
+	def _check_msg_available_after_opc_wait(self, stb: StatusByte, query: str, timeout: int, context: str) -> None:
+		"""Used internally after _StbPolling() to check if the message is available.
+		Throws an exception in case of MAV not available."""
+		if not self.vxi_capable:
+			return
+		if stb & StatusByte.message_available:
+			return
+		# Message not available
+		context = context + " SCPI query '{}'".format(query.rstrip(self._term_char))
+		if stb & StatusByte.error_queue_not_empty:
+			# Instrument reports an error
+			InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
+		else:
+			# Sometimes even if the StatusByte.MessageAvailable is false, the message is available.
+			# Try to read the STB again
+			stb = self._read_stb()
+			if not stb & StatusByte.event_status_byte:
+				# Instrument did not respond within the defined time
+				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, "{} No response from the instrument.".format(context))
+
+	def error_in_error_queue(self) -> bool:
+		"""Returns true, if error queue contains at least one error."""
+		stb = self._query_stb()
+		return stb & StatusByte.error_queue_not_empty
+
+	def reset_ese_sre(self) -> None:
+		"""Resets the status of ESE and SRE registers to default values."""
+		self._set_regs_ese_sre(self._opc_wait_mode)
+
+	def write_bin_block(self, cmd: str, data_stream: StreamReader) -> None:
+		"""Writes all the payload as binary data block to the instrument.
+		The binary data header is added at the beginning of the transmission automatically.
+		:param cmd: [str] SCPI command with which to send the data
+		:param data_stream: [StreamReader] data provider for the payload"""
+		data_size = len(data_stream)
+		len_str = f'{data_size}'
+		cmd = cmd.rstrip(self._term_char)
+		if '#' in cmd:
+			raise Exception(
+				f"Command '{cmd}' must be provided without the binary data header. "
+				f"The method 'write_bin_block' composes and prepends the binary data header automatically.")
+		if data_size <= self._std_bin_block_header_max_len:
+			# Standard bin data header for sizes below 1E9 bytes, e.g.: '#512345'
+			cmd_plus_header = f'{cmd}#{len(len_str)}{len_str}'.encode('utf-8')
+		else:
+			# Big sizes bin data header: e.g.: '#(3000000000)'
+			cmd_plus_header = f'{cmd}#({len_str})'.encode('utf-8')
+
+		if data_size <= self._data_chunk_size:
+			# Write all in one step
+			full_chunk = data_stream.read_as_binary()
+			write_buf = cmd_plus_header + full_chunk
+			if self._add_term_char_to_write_bin_block:
+				write_buf += self._term_char_bin
+			self._session.write_raw(write_buf)
+			# Event sending
+			if self.on_write_chunk_handler:
+				event_args = EventArgsChunk(True, 0, data_size, data_size, data_size, True, 1, full_chunk if self.io_events_include_data else None)
+				self.on_write_chunk_handler(event_args)
+		else:
+			# Write in chunks
+			try:
+				# Use finally to set the session send_end back to True
+				self._session.send_end = False
+				total_chunks = calculate_chunks_count(data_size, self._data_chunk_size)
+				chunk_ix = 0
+				if self.write_delay > 0:
+					time.sleep(self.write_delay / 1000)
+				# Write bin header
+				self._session.write_raw(cmd_plus_header)
+				# Write chunks
+				while True:
+					if len(data_stream) > self._data_chunk_size:
+						#  Not the last segment
+						chunk = data_stream.read_as_binary(self._data_chunk_size)
+						self._session.write_raw(chunk)
+						# Event sending
+						if self.on_write_chunk_handler:
+							event_args = EventArgsChunk(
+								True, chunk_ix, self._data_chunk_size, data_size, data_size - len(data_stream), False, total_chunks, chunk if self.io_events_include_data else None)
+							self.on_write_chunk_handler(event_args)
+					else:
+						# Last segment, indicate end of message again
+						chunk = data_stream.read_as_binary()
+						if self._add_term_char_to_write_bin_block:
+							# Append LF
+							self._session.write_raw(chunk)
+							self._session.send_end = True
+							self._session.write_raw(self._term_char_bin)
+						else:
+							self._session.send_end = True
+							self._session.write_raw(chunk)
+
+						# Event sending
+						if self.on_write_chunk_handler:
+							event_args = EventArgsChunk(True, chunk_ix, len(chunk), data_size, data_size, True, total_chunks, chunk if self.io_events_include_data else None)
+							self.on_write_chunk_handler(event_args)
+						break
+					chunk_ix += 1
+			finally:
+				self._session.send_end = True
+
+	def _parse_bin_data_header(self, exc_if_not_bin: bool) -> Tuple[ReadDataType, str, int]:
+		"""Parses the binary data block and returns the expected length of the following data block. \n
+		:param exc_if_not_bin: [bool] if True, the method throws exception in case the data is not binary.
+		:return: read_data_type: [ReadDataType], parsed_header: [string], bin_data_len: [integer]"""
+		length = -1
+		if self.read_delay > 0:
+			time.sleep(self.read_delay / 1000)
+
+		char: AnyStr = self._session.read_bytes(1, break_on_termchar=True)
+		if char == b'#':
+			# binary transfer
+			char = self._session.read_bytes(1, break_on_termchar=True)
+			if char == b'0':
+				data_type = ReadDataType.bin_unknown_len
+				return data_type, '#0', -1
+			if char == b'(':
+				# format for big lengths i.e. > 1E9 bytes: '#(1234567890123)...'
+				data_type = ReadDataType.bin_known_len
+				len_str = (self.read_up_to_char(b')', 100)[:-1]).decode("utf-8")
+				whole_hdr = '#(' + len_str + ')'
+				length = int(len_str)
+				return data_type, whole_hdr, length
+
+			# classic format for < 1E9 bytes: '#9123456789...'
+			data_type = ReadDataType.bin_known_len
+			len_of_len = int(char)
+			len_str = self._session.read_bytes(len_of_len).decode("utf-8")
+			length = int(len_str)
+			whole_hdr = '#' + char.decode("utf-8") + len_str
+			return data_type, whole_hdr, length
+
+		data_type = ReadDataType.ascii
+		if char == self._term_char_bin:
+			data_type = ReadDataType.null
+		if self.vxi_capable:
+			# For Vxi session, to be sure, check whether there are more chars in the read buffer
+			stb = self._read_stb()
+			if stb & StatusByte.message_available:
+				data_type = ReadDataType.ascii
+		whole_hdr = char.decode("utf-8")
+		if exc_if_not_bin:
+			if data_type == ReadDataType.null:
+				InstrumentErrors.throw_bin_block_unexp_resp_exception(self._resource_name, self._term_char)
+			# Read 20 more characters to compose a better exception message
+			whole_hdr += self.read_up_to_char(self._term_char_bin, 20).decode("utf-8")
+			if self.last_status == pyvisa.constants.StatusCode.success_max_count_read:
+				self._flush_junk_data()
+			InstrumentErrors.throw_bin_block_unexp_resp_exception(self._resource_name, whole_hdr)
+		return data_type, whole_hdr, length
+
+	def read_bin_block(self, stream: StreamWriter, exc_if_not_bin: bool) -> None:
+		"""Reads binary data block to the provided stream. \n
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param exc_if_not_bin: if True, the method throws exception if the received data is not binary"""
+		data_type, header, length = self._parse_bin_data_header(exc_if_not_bin)
+		if data_type == ReadDataType.ascii:
+			stream.switch_to_string_data()
+			self._read_unknown_len(stream, True, header)
+		elif data_type == ReadDataType.null:
+			# No data, consider it ASCII, Return empty string, and False (signaling ASCII transfer)
+			stream.switch_to_string_data()
+		elif data_type == ReadDataType.bin_unknown_len:
+			if not self.vxi_capable:
+				raise Exception(f'Non-Vxi11 sessions can not read binary data block of unknown length.')
+			self._read_unknown_len(stream, True)
+		elif length == 0:
+			self._flush_junk_data()
+		else:
+			self._read_bin_block_known_len(stream, length)
+
+	def _read_bin_block_known_len(self, stream: StreamWriter, length: int) -> None:
+		"""Reads binary data of defined length. All remaining data above the length are disposed of. \n
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param length: [int] expected length of the data"""
+		# Use try-catch to switch the termination character back ON in case of an exception (for non-Vxi sessions)
+		try:
+			# Binary transmission, for non-Vxi session, set the termination character to OFF
+			if not self.vxi_capable:
+				self._session.read_termination = False
+			# Binary data of known length
+			left_to_read = length
+			self.last_status = pyvisa.constants.StatusCode.success
+			with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
+				chunk_ix = 0
+				total_chunks = calculate_chunks_count(length, self._data_chunk_size)
+				while len(stream) < length:
+					chunk_size = min(self._data_chunk_size, left_to_read)
+					chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
+					left_to_read -= len(chunk)
+					stream.write(chunk)
+					if self.on_read_chunk_handler:
+						event_args = EventArgsChunk(True, chunk_ix, chunk_size, length, len(stream), left_to_read == 0, total_chunks, chunk if self.io_events_include_data else None)
+						self.on_read_chunk_handler(event_args)
+					chunk_ix += 1
+			if self._last_status_more_data_available():
+				if not self.vxi_capable:
+					self._session.read_termination = self._term_char
+				self._flush_junk_data()
+		finally:
+			# Make sure that in any case the self._session.read_termination is ON again for non-Vxi sessions
+			if not self.vxi_capable:
+				self._session.read_termination = self._term_char
+
+	def query_bin_block(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True) -> None:
+		"""Query binary data block and returns it as byte data. \n
+		:param query: [str] query to send to the instrument
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary"""
+		self.write(query)
+		self.read_bin_block(stream, exc_if_not_bin)
+		return
+
+	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
+		"""Query binary data block with OPC and returns it as byte data.
+		:param query: [str] query to send to the instrument
+		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
+		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary
+		:param timeout: Optional[Integer] timeout for the operation. If you skip it, the method uses the current opc timeout."""
+		timeout = self._resolve_opc_timeout(timeout)
+		if self.vxi_capable and self._opc_wait_mode != WaitForOpcMode.opc_query:
+			# For Vxi session, use the STB poll and read the response
+			stb = self._write_and_wait_for_opc(query, True, timeout)
+			self._check_msg_available_after_opc_wait(stb, query, timeout, 'query_bin_block_with_opc')
+			self.read_bin_block(stream, exc_if_not_bin)
+		else:
+			# For non-Vxi session, use the longer VISA Timeout without the *OPC
+			InstrumentErrors.assert_query_has_qmark(query, "query_bin_block_with_opc")
+			self.write(query)
+			old_visa_timeout = self.visa_timeout
+			# Change VISA Timeout if necessary
+			if old_visa_timeout != timeout:
+				self.visa_timeout = timeout
+			try:
+				# try-catch to set the VISA timeout back
+				self.read_bin_block(stream, exc_if_not_bin)
+				if self._opc_wait_mode == WaitForOpcMode.opc_query:
+					self.query_opc()
+			finally:
+				# Change VISA Timeout back if necessary
+				if old_visa_timeout != timeout:
+					self.visa_timeout = old_visa_timeout
+
+	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
+		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
+		Returns the read data including the stop character."""
+		response = b''
+		for i in range(max_cnt):
+			char, self.last_status = self._session.visalib.read(self._session.session, 1)
+			response += char
+			if char in stop_chars:
+				break
+			if self.last_status != pyvisa.constants.StatusCode.success_max_count_read:
+				break
+		return response
+
+	def get_session_handle(self) -> object:
+		"""Returns the underlying pyvisa session."""
+		return self._session
+
+	def close(self) -> None:
+		"""Closes the Visa session.
+		If the object was created with the direct session input, the session is not closed."""
+		if not self.reusing_session:
+			self._session.close()
+
+	# Events
+
+
+class EventArgsChunk:
+	"""Event arguments for chunk io event."""
+
+	def __init__(
+			self,
+			binary: bool,
+			chunk_ix: int,
+			chunk_size: int,
+			total_size: int,
+			transferred_size: int,
+			end_of_transfer: bool,
+			total_chunks: int or None,
+			data: AnyStr = None):
+
+		self.binary = binary
+		self.chunk_ix = chunk_ix
+		self.total_chunks = total_chunks
+		self.chunk_size = chunk_size
+		self.transferred_size = transferred_size
+		self.total_size = total_size
+		self.end_of_transfer = end_of_transfer
+		self.data = data
+
+	def __str__(self):
+		if self.binary:
+			type_info = 'binary'
+		else:
+			type_info = 'ascii'
+		if not self.total_chunks:
+			chunk_info = f' chunk nr. {self.chunk_ix + 1}'
+		elif self.total_chunks > 1:
+			chunk_info = f' chunk nr. {self.chunk_ix + 1}/{self.total_chunks}'
+		else:
+			chunk_info = ' chunk nr. 1/1'
+		eot = ' (EOT)' if self.end_of_transfer else ''
+		result = \
+			f'EventArgsChunk {type_info},{chunk_info}, {size_to_kb_mb_string(self.chunk_size, True)}, ' \
+			f'sum {size_to_kb_mb_string(self.transferred_size, True)} / {size_to_kb_mb_string(self.total_size, True) if self.total_size else "<N.A.>"}{eot}.'
+		return result
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/Internal/VisaSessionSim.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/Internal/VisaSessionSim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-import threading
-from typing import Callable, Dict, AnyStr
-
-from . import InstrumentSettings
-from .StreamReader import StreamReader
-from .StreamWriter import StreamWriter
-
-
-# noinspection PyMethodMayBeStatic,PyUnusedLocal
-class VisaSessionSim(object):
-	"""Visa session in simulation mode.
-	Provides the properties for the simulation mode.
-	Also serves as a cache for the SCPI command values: If you query a SCPI command value, it returns the last set value by that SCPI command."""
-
-	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
-		# noinspection PyTypeChecker
-		self._data_chunk_size: int = None
-		# noinspection PyTypeChecker
-		self._lock: threading.RLock = None
-
-		# Event handlers
-		# noinspection PyTypeChecker
-		self.on_read_chunk_handler: Callable = None
-		"""If assigned a handler, the VisaSession sends it event on each read chunk transfer."""
-		# noinspection PyTypeChecker
-		self.on_write_chunk_handler: Callable = None
-		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
-		self.io_events_include_data: bool = False
-		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
-
-		self.manufacturer: str = 'Rohde&Schwarz'
-		self._resource_name = resource_name
-		self.vxi_capable = True
-
-		# Changeable settings
-		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
-		self.visa_timeout = settings.visa_timeout
-		self.data_chunk_size = settings.io_segment_size
-
-		self._last_cmd = None
-
-		# If the return value is written to a cache, this flag signals if it was a cached value
-		self.cached_to_stream = False
-
-		# cache command values dictionary
-		self._cmd_vals_cache: Dict[str, AnyStr] = {}
-
-		# Decide, whether to create a new thread lock or the existing one from the direct_session
-		if direct_session and hasattr(direct_session, 'session_thread_rlock'):
-			rlock = direct_session.session_thread_rlock
-			if isinstance(rlock, type(threading.RLock())):
-				self.assign_lock(rlock)
-		if self.get_lock() is None:
-			# The existing session did not have a thread lock, assign a new one
-			self.assign_lock(threading.RLock())
-
-	def assign_lock(self, lock: threading.RLock) -> None:
-		"""Assigns the provided thread lock. The lock is only used by the parent class Instrument."""
-		self._lock = lock
-
-	def get_lock(self) -> threading.RLock:
-		"""Returns the current RLock object."""
-		return self._lock
-
-	def _update_cmd_vals_cache(self, cmd: str, param: AnyStr = None) -> None:
-		"""Parses out the parameter from the command and stores/updates them in the cache"""
-		aux = cmd.split(' ', 1)
-		if len(aux) < 2:
-			return
-		headers = aux[0].strip().lower()
-		param = aux[1].strip()
-		self._cmd_vals_cache[headers] = param
-
-	def _update_cmd_vals_cache_split(self, cmd: str, param: AnyStr) -> None:
-		"""Stores/updates cmd and param in the cache"""
-		headers = cmd.strip().lower()
-		self._cmd_vals_cache[headers] = param
-
-	def _get_cmd_cached_value(self, cmd: str) -> str or None:
-		"""Returns cached parameter to the corresponding command
-		Returns None of the command is not found in the cache"""
-		aux = cmd.split('?', 1)
-		headers = aux[0].strip().lower()
-		return self._cmd_vals_cache.get(headers, None)
-
-	def get_last_sent_cmd(self) -> str:
-		"""Returns the last commands sent to the instrument"""
-		return self._last_cmd
-
-	def is_rsnrp_session(self) -> bool:
-		"""Returns True, if the current session is a NRP-Z session"""
-		return False
-
-	def query_syst_error(self) -> str or None:
-		"""Returns one response to the SYSTEM:ERROR? query."""
-		return None
-
-	def query_all_syst_errors(self) -> list or None:
-		"""Returns all errors in the instrument's error queue."""
-		return []
-
-	def clear_before_read(self) -> None:
-		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
-		return
-
-	def clear(self) -> None:
-		"""Perform VISA viClear conditionally based on the instrument settings."""
-		return
-
-	def write(self, cmd: str) -> None:
-		"""Writes command to the instrument."""
-		self._last_cmd = cmd
-		self._update_cmd_vals_cache(cmd)
-		return
-
-	def query_str(self, query: str) -> str:
-		"""Queries the instrument and reads the response as string.
-		The length of the string is not limited. The response is then trimmed for trailing LF."""
-		self._last_cmd = query
-		cached = self._get_cmd_cached_value(query)
-		return 'Simulating' if cached is None else cached
-
-	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
-		"""Sends command with OPC-sync.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		self.write(cmd)
-
-	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
-		"""Query string with OPC synchronization.
-		The response is trimmed for any trailing LF.
-		If you do not provide timeout, the method uses current opc_timeout."""
-		return self.query_str(query)
-
-	def query_opc(self, timeout: int = 0) -> bool:
-		"""Sends *OPC? query and reads the result."""
-		return True
-
-	def query_and_clear_esr(self) -> int:
-		"""Sends *ESR? query and reads the result."""
-		return 0
-
-	def error_in_error_queue(self) -> bool:
-		"""Returns true, if error queue contains at least one error."""
-		return False
-
-	def reset_ese_sre(self) -> None:
-		"""Resets the status of ESE and SRE registers to default values."""
-		return
-
-	def write_bin_block(self, cmd: str, data_stream: StreamReader) -> None:
-		"""Writes all the payload as binary data block to the instrument.
-		The binary data header is added at the beginning of the transmission automatically."""
-		self._last_cmd = cmd
-		param = data_stream.read()
-		self._update_cmd_vals_cache_split(cmd, param)
-
-	def query_bin_block(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True) -> None:
-		"""Query binary data block and returns it as byte data."""
-		self._last_cmd = query
-		cached = self._get_cmd_cached_value(query)
-
-		if cached is None:
-			stream.write(bytes([0, 1, 2, 3, 4, 5, 6, 7, 8, 65, 66]))
-			self.cached_to_stream = False
-		else:
-			if isinstance(cached, str):
-				stream.switch_to_string_data()
-			stream.write(cached)
-			self.cached_to_stream = True
-
-	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
-		"""Query binary data block with OPC and returns it as byte data."""
-		self.query_bin_block(query, stream)
-
-	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
-		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
-		Returns the read data including the stop character."""
-		return b'Simulating'
-
-	def get_session_handle(self) -> object:
-		"""Returns the underlying pyvisa session."""
-		return f"Simulating session, resource name '{self._resource_name}'"
-
-	def close(self) -> None:
-		"""Closes the Visa session.
-		If the object was created with the direct session input, the session is not closed."""
-		return
+import threading
+from typing import Callable, Dict, AnyStr
+
+from . import InstrumentSettings
+from .StreamReader import StreamReader
+from .StreamWriter import StreamWriter
+
+
+# noinspection PyMethodMayBeStatic,PyUnusedLocal
+class VisaSessionSim(object):
+	"""Visa session in simulation mode.
+	Provides the properties for the simulation mode.
+	Also serves as a cache for the SCPI command values: If you query a SCPI command value, it returns the last set value by that SCPI command."""
+
+	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
+		# noinspection PyTypeChecker
+		self._data_chunk_size: int = None
+		# noinspection PyTypeChecker
+		self._lock: threading.RLock = None
+
+		# Event handlers
+		# noinspection PyTypeChecker
+		self.on_read_chunk_handler: Callable = None
+		"""If assigned a handler, the VisaSession sends it event on each read chunk transfer."""
+		# noinspection PyTypeChecker
+		self.on_write_chunk_handler: Callable = None
+		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
+		self.io_events_include_data: bool = False
+		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
+
+		self.manufacturer: str = 'Rohde&Schwarz'
+		self._resource_name = resource_name
+		self.vxi_capable = True
+
+		# Changeable settings
+		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
+		self.visa_timeout = settings.visa_timeout
+		self.data_chunk_size = settings.io_segment_size
+
+		self._last_cmd = None
+
+		# If the return value is written to a cache, this flag signals if it was a cached value
+		self.cached_to_stream = False
+
+		# cache command values dictionary
+		self._cmd_vals_cache: Dict[str, AnyStr] = {}
+
+		# Decide, whether to create a new thread lock or the existing one from the direct_session
+		if direct_session and hasattr(direct_session, 'session_thread_rlock'):
+			rlock = direct_session.session_thread_rlock
+			if isinstance(rlock, type(threading.RLock())):
+				self.assign_lock(rlock)
+		if self.get_lock() is None:
+			# The existing session did not have a thread lock, assign a new one
+			self.assign_lock(threading.RLock())
+
+	def assign_lock(self, lock: threading.RLock) -> None:
+		"""Assigns the provided thread lock. The lock is only used by the parent class Instrument."""
+		self._lock = lock
+
+	def get_lock(self) -> threading.RLock:
+		"""Returns the current RLock object."""
+		return self._lock
+
+	def _update_cmd_vals_cache(self, cmd: str, param: AnyStr = None) -> None:
+		"""Parses out the parameter from the command and stores/updates them in the cache"""
+		aux = cmd.split(' ', 1)
+		if len(aux) < 2:
+			return
+		headers = aux[0].strip().lower()
+		param = aux[1].strip()
+		self._cmd_vals_cache[headers] = param
+
+	def _update_cmd_vals_cache_split(self, cmd: str, param: AnyStr) -> None:
+		"""Stores/updates cmd and param in the cache"""
+		headers = cmd.strip().lower()
+		self._cmd_vals_cache[headers] = param
+
+	def _get_cmd_cached_value(self, cmd: str) -> str or None:
+		"""Returns cached parameter to the corresponding command
+		Returns None of the command is not found in the cache"""
+		aux = cmd.split('?', 1)
+		headers = aux[0].strip().lower()
+		return self._cmd_vals_cache.get(headers, None)
+
+	def get_last_sent_cmd(self) -> str:
+		"""Returns the last commands sent to the instrument"""
+		return self._last_cmd
+
+	def is_rsnrp_session(self) -> bool:
+		"""Returns True, if the current session is a NRP-Z session"""
+		return False
+
+	def query_syst_error(self) -> str or None:
+		"""Returns one response to the SYSTEM:ERROR? query."""
+		return None
+
+	def query_all_syst_errors(self) -> list or None:
+		"""Returns all errors in the instrument's error queue."""
+		return []
+
+	def clear_before_read(self) -> None:
+		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
+		return
+
+	def clear(self) -> None:
+		"""Perform VISA viClear conditionally based on the instrument settings."""
+		return
+
+	def write(self, cmd: str) -> None:
+		"""Writes command to the instrument."""
+		self._last_cmd = cmd
+		self._update_cmd_vals_cache(cmd)
+		return
+
+	def query_str(self, query: str) -> str:
+		"""Queries the instrument and reads the response as string.
+		The length of the string is not limited. The response is then trimmed for trailing LF."""
+		self._last_cmd = query
+		cached = self._get_cmd_cached_value(query)
+		return 'Simulating' if cached is None else cached
+
+	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
+		"""Sends command with OPC-sync.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		self.write(cmd)
+
+	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
+		"""Query string with OPC synchronization.
+		The response is trimmed for any trailing LF.
+		If you do not provide timeout, the method uses current opc_timeout."""
+		return self.query_str(query)
+
+	def query_opc(self) -> bool:
+		"""Sends *OPC? query and reads the result."""
+		return True
+
+	def query_and_clear_esr(self) -> int:
+		"""Sends *ESR? query and reads the result."""
+		return 0
+
+	def error_in_error_queue(self) -> bool:
+		"""Returns true, if error queue contains at least one error."""
+		return False
+
+	def reset_ese_sre(self) -> None:
+		"""Resets the status of ESE and SRE registers to default values."""
+		return
+
+	def write_bin_block(self, cmd: str, data_stream: StreamReader) -> None:
+		"""Writes all the payload as binary data block to the instrument.
+		The binary data header is added at the beginning of the transmission automatically."""
+		self._last_cmd = cmd
+		param = data_stream.read()
+		self._update_cmd_vals_cache_split(cmd, param)
+
+	def query_bin_block(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True) -> None:
+		"""Query binary data block and returns it as byte data."""
+		self._last_cmd = query
+		cached = self._get_cmd_cached_value(query)
+
+		if cached is None:
+			stream.write(bytes([0, 1, 2, 3, 4, 5, 6, 7, 8, 65, 66]))
+			self.cached_to_stream = False
+		else:
+			if isinstance(cached, str):
+				stream.switch_to_string_data()
+			stream.write(cached)
+			self.cached_to_stream = True
+
+	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
+		"""Query binary data block with OPC and returns it as byte data."""
+		self.query_bin_block(query, stream)
+
+	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
+		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
+		Returns the read data including the stop character."""
+		return b'Simulating'
+
+	def get_session_handle(self) -> object:
+		"""Returns the underlying pyvisa session."""
+		return f"Simulating session, resource name '{self._resource_name}'"
+
+	def close(self) -> None:
+		"""Closes the Visa session.
+		If the object was created with the direct session input, the session is not closed."""
+		return
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/RsCMPX_Gprf.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/RsCMPX_Gprf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from . import repcap
 from .Internal.RepeatedCapability import RepeatedCapability
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class RsCMPX_Gprf:
 	"""666 total commands, 16 Sub-groups, 0 group commands"""
-	_driver_options = "SupportedInstrModels = CMX500/CMP/CMW, SupportedIdnPatterns = CMX/CMP/CMW, SimulationIdnString = 'Rohde&Schwarz,CMX,100001,4.0.7.0010'"
+	driver_options = "SupportedInstrModels = CMX500/CMP/CMW, SupportedIdnPatterns = CMX/CMP/CMW, SimulationIdnString = 'Rohde&Schwarz,CMX,100001,4.0.7.0009'"
 
 	def __init__(self, resource_name: str, id_query: bool = True, reset: bool = False, options: str = None, direct_session: object = None):
 		"""Initializes new RsCMPX_Gprf session. \n
 		Parameter options tokens examples:
 			- 'Simulate=True' - starts the session in simulation mode. Default: False
 			- 'SelectVisa=socket' - uses no VISA implementation for socket connections - you do not need any VISA-C installation
 			- 'SelectVisa=rs' - forces usage of RohdeSchwarz Visa
@@ -32,25 +32,25 @@
 			- 'DriverSetup=(ViClearExeMode = 255)' - Binary combination where 1 means performing viClear() on a certain interface as the very first command in init
 			- 'DriverSetup=(OpcQueryAfterWrite = True)' - same as driver.utilities.opc_query_after_write = True
 		:param resource_name: VISA resource name, e.g. 'TCPIP::192.168.2.1::INSTR'
 		:param id_query: if True: the instrument's model name is verified against the models supported by the driver and eventually throws an exception.
 		:param reset: Resets the instrument (sends *RST command) and clears its status sybsystem
 		:param options: string tokens alternating the driver settings.
 		:param direct_session: Another driver object or pyVisa object to reuse the session instead of opening a new session."""
-		self._core = Core(resource_name, id_query, reset, RsCMPX_Gprf._driver_options, options, direct_session)
-		self._core.driver_version = '4.0.7.0010'
+		self._core = Core(resource_name, id_query, reset, RsCMPX_Gprf.driver_options, options, direct_session)
+		self._core.driver_version = '4.0.7.0009'
 		self._options = options
 		self._add_all_global_repcaps()
 		self._custom_properties_init()
 		# noinspection PyTypeChecker
 		self._base = CommandsGroup("ROOT", self._core, None)
 
 	@classmethod
 	def from_existing_session(cls, session: object, options: str = None) -> 'RsCMPX_Gprf':
-		"""Creates a new RsCMPX_Gprf object with the entered 'session' reused. \n
+		"""Creates a new RsCmwBluetoothSig object with the entered 'session' reused. \n
 		:param session: can be an another driver or a direct pyvisa session.
 		:param options: string tokens alternating the driver settings."""
 		# noinspection PyTypeChecker
 		return cls(None, False, False, options, session)
 
 	def __str__(self) -> str:
 		if self._core.io:
@@ -59,25 +59,25 @@
 			return f"RsCMPX_Gprf with session closed"
 
 	@staticmethod
 	def assert_minimum_version(min_version: str) -> None:
 		"""Asserts that the driver version fulfills the minimum required version you have entered.
 		This way you make sure your installed driver is of the entered version or newer."""
 		min_version_list = min_version.split('.')
-		curr_version_list = '4.0.7.0010'.split('.')
+		curr_version_list = '4.0.7.0009'.split('.')
 		count_min = len(min_version_list)
 		count_curr = len(curr_version_list)
 		count = count_min if count_min < count_curr else count_curr
 		for i in range(count):
 			minimum = int(min_version_list[i])
 			curr = int(curr_version_list[i])
 			if curr > minimum:
 				break
 			if curr < minimum:
-				raise RsInstrException(f"Assertion for minimum RsCMPX_Gprf version failed. Current version: '4.0.7.0010', minimum required version: '{min_version}'")
+				raise RsInstrException(f"Assertion for minimum RsCMPX_Gprf version failed. Current version: '4.0.7.0009', minimum required version: '{min_version}'")
 				
 	@staticmethod
 	def list_resources(expression: str = '?*::INSTR', visa_select: str = None) -> List[str]:
 		"""Finds all the resources defined by the expression
 			- '?*' - matches all the available instruments
 			- 'USB::?*' - matches all the USB instruments
 			- "TCPIP::192?*' - matches all the LAN instruments with the IP address starting with 192
@@ -250,15 +250,14 @@
 			self._system = System(self._core, self._base)
 		return self._system
 
 	def clone(self) -> 'RsCMPX_Gprf':
 		"""Creates a deep copy of the RsCMPX_Gprf object. Also copies:
 			- All the existing Global repeated capability values
 			- All the default group repeated capabilities setting \n
-		Does not check the *IDN? response, and does not perform Reset.
 		After cloning, you can set all the repeated capabilities settings independentely from the original group.
 		Calling close() on the new object does not close the original VISA session"""
 		cloned = RsCMPX_Gprf.from_existing_session(self.get_session_handle(), self._options)
 		self._base.synchronize_repcaps(cloned)
 		cloned.repcap_instance_set(self.repcap_instance_get())
 		return cloned
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/__init__.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""RsCMPX_Gprf instrument driver
-	:version: 4.0.7.10
-	:copyright: 2021 by Rohde & Schwarz GMBH & Co. KG
-	:license: MIT, see LICENSE for more details.
-"""
-
-__version__ = '4.0.7.10'
-
-# Main class
-from RsCMPX_Gprf.RsCMPX_Gprf import RsCMPX_Gprf
-
-# Bin data format
-from RsCMPX_Gprf.Internal.Conversions import BinIntFormat, BinFloatFormat
-
-# Exceptions
-from RsCMPX_Gprf.Internal.InstrumentErrors import RsInstrException, TimeoutException, StatusException, UnexpectedResponseException, ResourceError, DriverValueError
-
-# Callback Event Argument prototypes
-from RsCMPX_Gprf.Internal.IoTransferEventArgs import IoTransferEventArgs
-
-# enums
-from RsCMPX_Gprf import enums
-
-# repcaps
+"""RsCMPX_Gprf instrument driver
+	:version: 4.0.7.9
+	:copyright: 2020 by Rohde & Schwarz GMBH & Co. KG
+	:license: MIT, see LICENSE for more details.
+"""
+
+__version__ = '4.0.7.9'
+
+# Main class
+from RsCMPX_Gprf.RsCMPX_Gprf import RsCMPX_Gprf
+
+# Bin data format
+from RsCMPX_Gprf.Internal.Conversions import BinIntFormat, BinFloatFormat
+
+# Exceptions
+from RsCMPX_Gprf.Internal.InstrumentErrors import RsInstrException, TimeoutException, StatusException, UnexpectedResponseException, ResourceError, DriverValueError
+
+# Callback Event Argument prototypes
+from RsCMPX_Gprf.Internal.IoTransferEventArgs import IoTransferEventArgs
+
+# enums
+from RsCMPX_Gprf import enums
+
+# repcaps
 from RsCMPX_Gprf import repcap
 
-# Reliability interface
+# Reliability interface
 from RsCMPX_Gprf.CustomFiles.reliability import Reliability, ReliabilityEventArgs, codes_table
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/enums.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/enums.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf/repcap.py` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf/repcap.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf.egg-info/PKG-INFO` & `RsCMPX_Gprf-4.0.7.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 Metadata-Version: 2.1
-Name: RsCMPX-Gprf
-Version: 4.0.7.10
+Name: RsCMPX_Gprf
+Version: 4.0.7.9
 Summary: CMX/CMP Global Purpose RF Remote-control Module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 Author-email: Customer.Support@rohde-schwarz.com
 License: MIT
-Description: Rohde & Schwarz CMX/CMP Global Purpose RF RsCMPX_Gprf instrument driver.
+Description: Rohde & Schwarz CMX/CMP Global Purpose RF RsCMPX_Gprf instrument driver Version 4.0.7.9
         
-        Supported instruments: CMX500, CMP200
-        
-        The package is hosted here: https://pypi.org/project/RsCMPX_Gprf/
-        
-        Documentation: https://RsCMPX_Gprf.readthedocs.io/
-        
-        Examples: https://github.com/Rohde-Schwarz/Examples/
+        Check out the module documentation on https://RsCMPX_Gprf.readthedocs.io/
         
         --------------------------------------------------------------------------------
         
         Currently supported CMX/CMP subsystems:
         
         - Base: `RsCmpx_Base <https://RsCmpx_Base.readthedocs.io/>`_
         - GPRF: `RsCmpx_Gprf <https://RsCmpx_Gprf.readthedocs.io/>`_
@@ -31,19 +25,19 @@
         In case you require support for more subsystems, please contact our customer support on customersupport@rohde-schwarz.com
         with the topic "Auto-generated Python drivers" in the email subject. This will speed up the response process
         
         --------------------------------------------------------------------------------
         
         Release Notes: for the whole RsCmpx_xxx group:
         
-        Latest release notes summary: Added documentation on ReadTheDocs
+        Latest release notes summary: Added documentation on ReadTheDocs.io
         
         Version 4.0.7.4
         
-        - Added documentation on ReadTheDocs
+        - Added documentation on ReadTheDocs.io
         
         Version 4.0.7.3
         
         - Added new subsystems NrFr2Meas, UwbMeas, Signaling
         
         Version 4.0.7.2
```

### Comparing `RsCMPX_Gprf-4.0.7.10/RsCMPX_Gprf.egg-info/SOURCES.txt` & `RsCMPX_Gprf-4.0.7.9/RsCMPX_Gprf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 RsCMPX_Gprf/Implementations/Trigger.py
 RsCMPX_Gprf/Implementations/__init__.py
 RsCMPX_Gprf/Implementations/Add_/System.py
 RsCMPX_Gprf/Implementations/Add_/Tenvironment.py
 RsCMPX_Gprf/Implementations/Add_/__init__.py
 RsCMPX_Gprf/Implementations/Add_/System_/Attenuation.py
 RsCMPX_Gprf/Implementations/Add_/System_/__init__.py
+RsCMPX_Gprf/Implementations/Add_/System_/Attenuation_/CorrectionTable.py
+RsCMPX_Gprf/Implementations/Add_/System_/Attenuation_/__init__.py
 RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath.py
 RsCMPX_Gprf/Implementations/Add_/Tenvironment_/__init__.py
 RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable.py
 RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/__init__.py
 RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/Rx.py
 RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/Tx.py
 RsCMPX_Gprf/Implementations/Add_/Tenvironment_/Spath_/CorrectionTable_/__init__.py
@@ -126,15 +128,15 @@
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/Frequency.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqRecorder_/ListPy_/__init__.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/Trigger.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/__init__.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/EnvelopePower.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/Frequency.py
-RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/Retrigger.py
+RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/ReTrigger.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/IqVsSlot_/ListPy_/__init__.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/__init__.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor_/Frequency.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Nrpm_/Sensor_/__init__.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/ListPy.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Ploss_/Mpath.py
@@ -156,15 +158,15 @@
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/Gauss.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/FilterPy_/__init__.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/EnvelopePower.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Frequency.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/IqData.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Irepetition.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/ParameterSetList.py
-RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/Retrigger.py
+RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/ReTrigger.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ListPy_/__init__.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Catalog.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/FilterPy.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Mlength.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/PdefSet.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/Slength.py
 RsCMPX_Gprf/Implementations/Configure_/Gprf_/Measurement_/Power_/ParameterSetList_/__init__.py
@@ -206,14 +208,16 @@
 RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/Tx.py
 RsCMPX_Gprf/Implementations/Configure_/Tenvironment_/Spath_/CorrectionTable_/__init__.py
 RsCMPX_Gprf/Implementations/Create_/System.py
 RsCMPX_Gprf/Implementations/Create_/Tenvironment.py
 RsCMPX_Gprf/Implementations/Create_/__init__.py
 RsCMPX_Gprf/Implementations/Create_/System_/Attenuation.py
 RsCMPX_Gprf/Implementations/Create_/System_/__init__.py
+RsCMPX_Gprf/Implementations/Create_/System_/Attenuation_/CorrectionTable.py
+RsCMPX_Gprf/Implementations/Create_/System_/Attenuation_/__init__.py
 RsCMPX_Gprf/Implementations/Create_/Tenvironment_/Spath.py
 RsCMPX_Gprf/Implementations/Create_/Tenvironment_/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic_/Catalog.py
 RsCMPX_Gprf/Implementations/Diagnostic_/Generic.py
 RsCMPX_Gprf/Implementations/Diagnostic_/Gprf.py
 RsCMPX_Gprf/Implementations/Diagnostic_/Meas.py
 RsCMPX_Gprf/Implementations/Diagnostic_/Route.py
@@ -441,14 +445,17 @@
 RsCMPX_Gprf/Implementations/Remove_/System_/__init__.py
 RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation_/CorrectionTable.py
 RsCMPX_Gprf/Implementations/Remove_/System_/Attenuation_/__init__.py
 RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath.py
 RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/__init__.py
 RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/CorrectionTable.py
 RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/__init__.py
+RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/CorrectionTable_/Rx.py
+RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/CorrectionTable_/Tx.py
+RsCMPX_Gprf/Implementations/Remove_/Tenvironment_/Spath_/CorrectionTable_/__init__.py
 RsCMPX_Gprf/Implementations/Results_/Gprf.py
 RsCMPX_Gprf/Implementations/Results_/__init__.py
 RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement.py
 RsCMPX_Gprf/Implementations/Results_/Gprf_/__init__.py
 RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power.py
 RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/__init__.py
 RsCMPX_Gprf/Implementations/Results_/Gprf_/Measurement_/Power_/Current.py
```

