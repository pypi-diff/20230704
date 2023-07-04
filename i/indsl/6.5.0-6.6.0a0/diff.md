# Comparing `tmp/indsl-6.5.0.tar.gz` & `tmp/indsl-6.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indsl-6.5.0.tar", max compression
+gzip compressed data, was "indsl-6.6.0a0.tar", max compression
```

## Comparing `indsl-6.5.0.tar` & `indsl-6.6.0a0.tar`

### file list

```diff
@@ -1,120 +1,121 @@
--rw-r--r--   0        0        0    11357 2023-03-31 12:57:38.194630 indsl-6.5.0/LICENSE
--rw-r--r--   0        0        0     9485 2023-03-31 12:57:38.194630 indsl-6.5.0/README.md
--rw-r--r--   0        0        0      286 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/__init__.py
--rw-r--r--   0        0        0       22 2023-03-31 12:58:27.590128 indsl-6.5.0/indsl/_version.py
--rw-r--r--   0        0        0     1011 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/__init__.py
--rw-r--r--   0        0        0     5161 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/completeness.py
--rw-r--r--   0        0        0     6636 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/gaps_identification.py
--rw-r--r--   0        0        0     7256 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/low_density_identification.py
--rw-r--r--   0        0        0    13200 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/outliers.py
--rw-r--r--   0        0        0     1696 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/rolling_stddev.py
--rw-r--r--   0        0        0      159 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/score/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/score/accuracy/__init__.py
--rw-r--r--   0        0        0     7972 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/score/base.py
--rw-r--r--   0        0        0       45 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/score/completeness/__init__.py
--rw-r--r--   0        0        0     3843 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/score/completeness/density.py
--rw-r--r--   0        0        0     4984 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/score/completeness/gap.py
--rw-r--r--   0        0        0     3911 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/value_decrease_indication.py
--rw-r--r--   0        0        0     3875 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/data_quality/value_decrease_indication_v1.py
--rw-r--r--   0        0        0      370 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/detect/__init__.py
--rw-r--r--   0        0        0    11955 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/detect/change_point_detector.py
--rw-r--r--   0        0        0    18818 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/detect/cusum.py
--rw-r--r--   0        0        0     2426 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/detect/drift_detector.py
--rw-r--r--   0        0        0     2249 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/detect/drift_detector_v1.py
--rw-r--r--   0        0        0    14877 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/detect/oscillation_detector.py
--rw-r--r--   0        0        0    10636 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/detect/steady_state.py
--rw-r--r--   0        0        0     3414 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/detect/unchanged_signal_detector.py
--rw-r--r--   0        0        0     2578 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/detect/utils.py
--rw-r--r--   0        0        0      265 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/drilling/__init__.py
--rw-r--r--   0        0        0     4295 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/drilling/flag_detection.py
--rw-r--r--   0        0        0      725 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/equipment/__init__.py
--rw-r--r--   0        0        0     7830 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/equipment/pump_parameters.py
--rw-r--r--   0        0        0     3492 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/equipment/valve_parameters.py
--rw-r--r--   0        0        0     3483 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/equipment/valve_parameters_.py
--rw-r--r--   0        0        0     9409 2023-03-31 12:57:38.454651 indsl-6.5.0/indsl/equipment/volume_vessel.py
--rw-r--r--   0        0        0      506 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/exceptions.py
--rw-r--r--   0        0        0      196 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/filter/__init__.py
--rw-r--r--   0        0        0     2102 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/filter/simple_filters.py
--rw-r--r--   0        0        0     2704 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/filter/wavelet_filter.py
--rw-r--r--   0        0        0     2779 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/filter/wavelet_filter_v1.py
--rw-r--r--   0        0        0      151 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/fluid_dynamics/__init__.py
--rw-r--r--   0        0        0      973 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/fluid_dynamics/dimensionless.py
--rw-r--r--   0        0        0      906 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/fluid_dynamics/friction.py
--rw-r--r--   0        0        0      214 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/forecast/__init__.py
--rw-r--r--   0        0        0     4619 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/forecast/arma_predictor.py
--rw-r--r--   0        0        0     5074 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/forecast/holt_winters_predictor.py
--rw-r--r--   0        0        0      315 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/not_listed_operations/__init__.py
--rw-r--r--   0        0        0     3453 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/not_listed_operations/deprecated_functions.py
--rw-r--r--   0        0        0      398 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/not_listed_operations/utils.py
--rw-r--r--   0        0        0      510 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/not_listed_operations/versioning_test.py
--rw-r--r--   0        0        0      388 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/not_listed_operations/versioning_test_v1.py
--rw-r--r--   0        0        0      502 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/oil_and_gas/__init__.py
--rw-r--r--   0        0        0     1378 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/oil_and_gas/engineering_calcs.py
--rw-r--r--   0        0        0     6663 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/oil_and_gas/gas_density_calcs.py
--rw-r--r--   0        0        0     4310 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/oil_and_gas/live_fluid_properties.py
--rw-r--r--   0        0        0     5741 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/oil_and_gas/shut_in_detector.py
--rw-r--r--   0        0        0     3134 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/oil_and_gas/shut_in_variables.py
--rw-r--r--   0        0        0     3087 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/oil_and_gas/tab_fp_identifier.json
--rw-r--r--   0        0        0     3346 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/oil_and_gas/well_prod_status.py
--rw-r--r--   0        0        0      129 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/regression/__init__.py
--rw-r--r--   0        0        0     2293 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/regression/polynomial.py
--rw-r--r--   0        0        0     4144 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/resample/README.md
--rw-r--r--   0        0        0      313 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/resample/__init__.py
--rw-r--r--   0        0        0     1113 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/resample/auto_align.py
--rw-r--r--   0        0        0     3521 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/resample/group_by.py
--rw-r--r--   0        0        0     4580 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/resample/interpolate.py
--rw-r--r--   0        0        0     5179 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/resample/interpolate_v1.py
--rw-r--r--   0        0        0     6328 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/resample/reindex.py
--rw-r--r--   0        0        0     7381 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/resample/reindex_v1.py
--rw-r--r--   0        0        0     8361 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/resample/resample.py
--rw-r--r--   0        0        0     8449 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/resample/resample_v1.py
--rw-r--r--   0        0        0      362 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/signals/__init__.py
--rw-r--r--   0        0        0    23811 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/signals/generator.py
--rw-r--r--   0        0        0     1349 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/signals/noise.py
--rw-r--r--   0        0        0      935 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/signals/polynomial.py
--rw-r--r--   0        0        0     8149 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/smooth/README.md
--rw-r--r--   0        0        0      474 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/smooth/__init__.py
--rw-r--r--   0        0        0     2679 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/smooth/alma.py
--rw-r--r--   0        0        0     1178 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/smooth/arma_smoother.py
--rw-r--r--   0        0        0     1724 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/smooth/butterworth.py
--rw-r--r--   0        0        0     2227 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/smooth/butterworth_v1.py
--rw-r--r--   0        0        0     2105 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/smooth/chebyshev.py
--rw-r--r--   0        0        0     5730 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/smooth/eweight_ma.py
--rw-r--r--   0        0        0     5886 2023-03-31 12:57:38.458651 indsl-6.5.0/indsl/smooth/eweight_ma_v1.py
--rw-r--r--   0        0        0    73573 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/smooth/img/ma_min_periods1.png
--rw-r--r--   0        0        0    63892 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/smooth/img/ma_min_periods5.png
--rw-r--r--   0        0        0    52202 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/smooth/img/zoom_min_periods5.png
--rw-r--r--   0        0        0     3007 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/smooth/lweight_ma.py
--rw-r--r--   0        0        0     3049 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/smooth/lweight_ma_v1.py
--rw-r--r--   0        0        0      730 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/smooth/moving_averages.md
--rw-r--r--   0        0        0     2848 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/smooth/savitzky_golay.py
--rw-r--r--   0        0        0     1275 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/smooth/simple_ma.py
--rw-r--r--   0        0        0     1418 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/smooth/simple_ma_v1.py
--rw-r--r--   0        0        0      494 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/statistics/README.md
--rw-r--r--   0        0        0      231 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/statistics/__init__.py
--rw-r--r--   0        0        0     2313 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/statistics/confidence.py
--rw-r--r--   0        0        0     1948 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/statistics/correlation.py
--rw-r--r--   0        0        0    26141 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/statistics/img/csaps_vs_scipy.png
--rw-r--r--   0        0        0    26153 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/statistics/img/dbscan_principle.png
--rw-r--r--   0        0        0    69055 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/statistics/img/input_timeseries.png
--rw-r--r--   0        0        0    69329 2023-03-31 12:57:38.462651 indsl-6.5.0/indsl/statistics/img/output_function.png
--rw-r--r--   0        0        0   102644 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/statistics/img/process_function.png
--rw-r--r--   0        0        0     4926 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/statistics/outliers.md
--rw-r--r--   0        0        0    13787 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/statistics/outliers.py
--rw-r--r--   0        0        0    13227 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/statistics/outliers_v1.py
--rw-r--r--   0        0        0       78 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/sustainability/__init__.py
--rw-r--r--   0        0        0     5008 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/sustainability/co2_emissions_calculations.py
--rw-r--r--   0        0        0     1558 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/ts_utils/__init__.py
--rw-r--r--   0        0        0     1453 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/ts_utils/logarithmic_functions.py
--rw-r--r--   0        0        0     2791 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/ts_utils/logical_operations.py
--rw-r--r--   0        0        0     7912 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/ts_utils/numerical_calculus.py
--rw-r--r--   0        0        0     2573 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/ts_utils/numerical_calculus_v1.py
--rw-r--r--   0        0        0     5476 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/ts_utils/operators.py
--rw-r--r--   0        0        0     3610 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/ts_utils/trigonometric_functions.py
--rw-r--r--   0        0        0    14723 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/ts_utils/ts_utils.py
--rw-r--r--   0        0        0    18290 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/ts_utils/utility_functions.py
--rw-r--r--   0        0        0      752 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/type_check.py
--rw-r--r--   0        0        0     1653 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/validations.py
--rw-r--r--   0        0        0     5041 2023-03-31 12:57:38.466652 indsl-6.5.0/indsl/versioning.py
--rw-r--r--   0        0        0     2035 2023-03-31 12:58:27.534124 indsl-6.5.0/pyproject.toml
--rw-r--r--   0        0        0    10818 1970-01-01 00:00:00.000000 indsl-6.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-04 12:11:41.133681 indsl-6.6.0a0/LICENSE
+-rw-r--r--   0        0        0     9485 2023-07-04 12:11:41.133681 indsl-6.6.0a0/README.md
+-rw-r--r--   0        0        0      568 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-04 12:12:16.314440 indsl-6.6.0a0/indsl/_version.py
+-rw-r--r--   0        0        0     1110 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/__init__.py
+-rw-r--r--   0        0        0     5161 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/completeness.py
+-rw-r--r--   0        0        0     3881 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/datapoint_diff.py
+-rw-r--r--   0        0        0     6648 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/gaps_identification.py
+-rw-r--r--   0        0        0     7263 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/low_density_identification.py
+-rw-r--r--   0        0        0    13211 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/outliers.py
+-rw-r--r--   0        0        0     1739 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/rolling_stddev.py
+-rw-r--r--   0        0        0      258 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/score/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/score/accuracy/__init__.py
+-rw-r--r--   0        0        0     7964 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/score/base.py
+-rw-r--r--   0        0        0       89 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/score/completeness/__init__.py
+-rw-r--r--   0        0        0     4032 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/score/completeness/density.py
+-rw-r--r--   0        0        0     5173 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/score/completeness/gap.py
+-rw-r--r--   0        0        0     3911 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/value_decrease_indication.py
+-rw-r--r--   0        0        0     3875 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/data_quality/value_decrease_indication_v1.py
+-rw-r--r--   0        0        0      484 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/detect/__init__.py
+-rw-r--r--   0        0        0    12000 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/detect/change_point_detector.py
+-rw-r--r--   0        0        0    19019 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/detect/cusum.py
+-rw-r--r--   0        0        0     2595 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/detect/drift_detector.py
+-rw-r--r--   0        0        0     2249 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/detect/drift_detector_v1.py
+-rw-r--r--   0        0        0    22015 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/detect/oscillation_detector.py
+-rw-r--r--   0        0        0    10677 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/detect/steady_state.py
+-rw-r--r--   0        0        0     3414 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/detect/unchanged_signal_detector.py
+-rw-r--r--   0        0        0     2590 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/detect/utils.py
+-rw-r--r--   0        0        0      265 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/drilling/__init__.py
+-rw-r--r--   0        0        0     4302 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/drilling/flag_detection.py
+-rw-r--r--   0        0        0      725 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/equipment/__init__.py
+-rw-r--r--   0        0        0     7828 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/equipment/pump_parameters.py
+-rw-r--r--   0        0        0     5837 2023-07-04 12:11:41.333685 indsl-6.6.0a0/indsl/equipment/valve_parameters.py
+-rw-r--r--   0        0        0     6865 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/equipment/valve_parameters_.py
+-rw-r--r--   0        0        0     9598 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/equipment/volume_vessel.py
+-rw-r--r--   0        0        0      506 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/exceptions.py
+-rw-r--r--   0        0        0      196 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/filter/__init__.py
+-rw-r--r--   0        0        0     2102 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/filter/simple_filters.py
+-rw-r--r--   0        0        0     2881 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/filter/wavelet_filter.py
+-rw-r--r--   0        0        0     2786 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/filter/wavelet_filter_v1.py
+-rw-r--r--   0        0        0      151 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/fluid_dynamics/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/fluid_dynamics/dimensionless.py
+-rw-r--r--   0        0        0      906 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/fluid_dynamics/friction.py
+-rw-r--r--   0        0        0      214 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/forecast/__init__.py
+-rw-r--r--   0        0        0     4624 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/forecast/arma_predictor.py
+-rw-r--r--   0        0        0     5254 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/forecast/holt_winters_predictor.py
+-rw-r--r--   0        0        0      315 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/not_listed_operations/__init__.py
+-rw-r--r--   0        0        0     3482 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/not_listed_operations/deprecated_functions.py
+-rw-r--r--   0        0        0      398 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/not_listed_operations/utils.py
+-rw-r--r--   0        0        0      510 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/not_listed_operations/versioning_test.py
+-rw-r--r--   0        0        0      388 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/not_listed_operations/versioning_test_v1.py
+-rw-r--r--   0        0        0      502 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/oil_and_gas/__init__.py
+-rw-r--r--   0        0        0     1378 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/oil_and_gas/engineering_calcs.py
+-rw-r--r--   0        0        0     6667 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/oil_and_gas/gas_density_calcs.py
+-rw-r--r--   0        0        0     4479 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/oil_and_gas/live_fluid_properties.py
+-rw-r--r--   0        0        0     5783 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/oil_and_gas/shut_in_detector.py
+-rw-r--r--   0        0        0     3142 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/oil_and_gas/shut_in_variables.py
+-rw-r--r--   0        0        0     3087 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/oil_and_gas/tab_fp_identifier.json
+-rw-r--r--   0        0        0     3353 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/oil_and_gas/well_prod_status.py
+-rw-r--r--   0        0        0      129 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/regression/__init__.py
+-rw-r--r--   0        0        0     2470 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/regression/polynomial.py
+-rw-r--r--   0        0        0     4144 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/resample/README.md
+-rw-r--r--   0        0        0      313 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/resample/__init__.py
+-rw-r--r--   0        0        0     1113 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/resample/auto_align.py
+-rw-r--r--   0        0        0     3693 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/resample/group_by.py
+-rw-r--r--   0        0        0     4763 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/resample/interpolate.py
+-rw-r--r--   0        0        0     5381 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/resample/interpolate_v1.py
+-rw-r--r--   0        0        0     6525 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/resample/reindex.py
+-rw-r--r--   0        0        0     7911 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/resample/reindex_v1.py
+-rw-r--r--   0        0        0     8543 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/resample/resample.py
+-rw-r--r--   0        0        0     8670 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/resample/resample_v1.py
+-rw-r--r--   0        0        0      420 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/signals/__init__.py
+-rw-r--r--   0        0        0    26910 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/signals/generator.py
+-rw-r--r--   0        0        0    12149 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/signals/noise.py
+-rw-r--r--   0        0        0      955 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/signals/polynomial.py
+-rw-r--r--   0        0        0     8149 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/README.md
+-rw-r--r--   0        0        0      474 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/__init__.py
+-rw-r--r--   0        0        0     2691 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/alma.py
+-rw-r--r--   0        0        0     1186 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/arma_smoother.py
+-rw-r--r--   0        0        0     1892 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/butterworth.py
+-rw-r--r--   0        0        0     2227 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/butterworth_v1.py
+-rw-r--r--   0        0        0     2102 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/chebyshev.py
+-rw-r--r--   0        0        0     5736 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/eweight_ma.py
+-rw-r--r--   0        0        0     5899 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/eweight_ma_v1.py
+-rw-r--r--   0        0        0    73573 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/img/ma_min_periods1.png
+-rw-r--r--   0        0        0    63892 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/img/ma_min_periods5.png
+-rw-r--r--   0        0        0    52202 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/img/zoom_min_periods5.png
+-rw-r--r--   0        0        0     3007 2023-07-04 12:11:41.337685 indsl-6.6.0a0/indsl/smooth/lweight_ma.py
+-rw-r--r--   0        0        0     3053 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/smooth/lweight_ma_v1.py
+-rw-r--r--   0        0        0      730 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/smooth/moving_averages.md
+-rw-r--r--   0        0        0     2856 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/smooth/savitzky_golay.py
+-rw-r--r--   0        0        0     1275 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/smooth/simple_ma.py
+-rw-r--r--   0        0        0     1420 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/smooth/simple_ma_v1.py
+-rw-r--r--   0        0        0      494 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/README.md
+-rw-r--r--   0        0        0      231 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/__init__.py
+-rw-r--r--   0        0        0     2313 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/confidence.py
+-rw-r--r--   0        0        0     1948 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/correlation.py
+-rw-r--r--   0        0        0    26141 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/img/csaps_vs_scipy.png
+-rw-r--r--   0        0        0    26153 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/img/dbscan_principle.png
+-rw-r--r--   0        0        0    69055 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/img/input_timeseries.png
+-rw-r--r--   0        0        0    69329 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/img/output_function.png
+-rw-r--r--   0        0        0   102644 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/img/process_function.png
+-rw-r--r--   0        0        0     4926 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/outliers.md
+-rw-r--r--   0        0        0    13787 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/outliers.py
+-rw-r--r--   0        0        0    13229 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/statistics/outliers_v1.py
+-rw-r--r--   0        0        0       78 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/sustainability/__init__.py
+-rw-r--r--   0        0        0     5009 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/sustainability/co2_emissions_calculations.py
+-rw-r--r--   0        0        0     1558 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/ts_utils/__init__.py
+-rw-r--r--   0        0        0     1453 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/ts_utils/logarithmic_functions.py
+-rw-r--r--   0        0        0     3000 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/ts_utils/logical_operations.py
+-rw-r--r--   0        0        0     7912 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/ts_utils/numerical_calculus.py
+-rw-r--r--   0        0        0     2573 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/ts_utils/numerical_calculus_v1.py
+-rw-r--r--   0        0        0     5479 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/ts_utils/operators.py
+-rw-r--r--   0        0        0     3610 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/ts_utils/trigonometric_functions.py
+-rw-r--r--   0        0        0    14958 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/ts_utils/ts_utils.py
+-rw-r--r--   0        0        0    18839 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/ts_utils/utility_functions.py
+-rw-r--r--   0        0        0      773 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/type_check.py
+-rw-r--r--   0        0        0     1653 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/validations.py
+-rw-r--r--   0        0        0     4843 2023-07-04 12:11:41.341685 indsl-6.6.0a0/indsl/versioning.py
+-rw-r--r--   0        0        0     3120 2023-07-04 12:12:16.230438 indsl-6.6.0a0/pyproject.toml
+-rw-r--r--   0        0        0    10839 1970-01-01 00:00:00.000000 indsl-6.6.0a0/PKG-INFO
```

### Comparing `indsl-6.5.0/LICENSE` & `indsl-6.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/README.md` & `indsl-6.6.0a0/README.md`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/data_quality/__init__.py` & `indsl-6.6.0a0/indsl/data_quality/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright 2022 Cognite AS
 
+from .datapoint_diff import datapoint_diff_over_time_period
 from .gaps_identification import (
     gaps_identification_iqr,
     gaps_identification_modified_z_scores,
     gaps_identification_threshold,
     gaps_identification_z_scores,
 )
 from .low_density_identification import (
@@ -27,8 +28,9 @@
     "low_density_identification_iqr",
     "low_density_identification_modified_z_scores",
     "low_density_identification_threshold",
     "low_density_identification_z_scores",
     "extreme",
     "value_decrease_check",
     "rolling_stddev_timedelta",
+    "datapoint_diff_over_time_period",
 ]
```

### Comparing `indsl-6.5.0/indsl/data_quality/completeness.py` & `indsl-6.6.0a0/indsl/data_quality/completeness.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/data_quality/gaps_identification.py` & `indsl-6.6.0a0/indsl/data_quality/gaps_identification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright 2021 Cognite AS
 import numpy as np
 import pandas as pd
 
-from ..ts_utils.utility_functions import (
+from indsl.ts_utils.utility_functions import (
     generate_step_series,
     modified_z_scores_test,
     normality_assumption_test,
     z_scores_test,
 )
-from ..type_check import check_types
-from ..validations import validate_series_has_time_index, validate_series_is_not_empty
+from indsl.type_check import check_types
+from indsl.validations import validate_series_has_time_index, validate_series_is_not_empty
 
 
 @check_types
 def gaps_identification_z_scores(
     data: pd.Series, cutoff: float = 3.0, test_normality_assumption: bool = False
 ) -> pd.Series:
     """Gaps detection, Z-scores.
```

### Comparing `indsl-6.5.0/indsl/data_quality/low_density_identification.py` & `indsl-6.6.0a0/indsl/data_quality/low_density_identification.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 
 from indsl.ts_utils.utility_functions import (
     generate_step_series,
     modified_z_scores_test,
     normality_assumption_test,
     z_scores_test,
 )
-
-from ..type_check import check_types
-from ..validations import validate_series_has_time_index, validate_series_is_not_empty
+from indsl.type_check import check_types
+from indsl.validations import validate_series_has_time_index, validate_series_is_not_empty
 
 
 # todo add as indsl function
 @check_types
 def get_densities(data: pd.Series, time_window: pd.Timedelta = pd.Timedelta("5m")) -> pd.Series:
     """Point density.
```

### Comparing `indsl-6.5.0/indsl/data_quality/outliers.py` & `indsl-6.6.0a0/indsl/data_quality/outliers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 
 import numpy as np
 import pandas as pd
 
 from numpy.polynomial import polynomial
 from scipy.stats import t as student_dist
 
+from indsl.exceptions import UserValueError
 from indsl.resample.reindex import reindex
 from indsl.smooth import sg
-
-from ..exceptions import UserValueError
-from ..type_check import check_types
-from ..validations import validate_series_has_minimum_length
+from indsl.type_check import check_types
+from indsl.validations import validate_series_has_minimum_length
 
 
 @check_types
 def extreme(data: pd.Series, alpha: float = 0.05, bc_relaxation: float = 0.167, poly_order: int = 3) -> pd.Series:
     r"""Extreme outliers removal.
 
     Outlier detector and removal based on the `paper from Gustavo A. Zarruk
```

### Comparing `indsl-6.5.0/indsl/data_quality/rolling_stddev.py` & `indsl-6.6.0a0/indsl/data_quality/rolling_stddev.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,16 +32,11 @@
         UserValueError: data is empty
         UserTypeError: time_window is not of type pandas.Timedelta
     """
     validate_series_has_time_index(data)
     validate_series_is_not_empty(data)
     validate_timedelta_unit(time_window)
 
-    return (
-        data.index.to_series()
-        .diff()
-        .astype("timedelta64[ms]")
-        .fillna(0)
-        .rolling(window=time_window, min_periods=min_periods)
-        .std()
-        .fillna(0)
-    )
+    timedelta_series = data.index.to_series().diff().astype("timedelta64[ms]")
+    timedelta_series_ms = timedelta_series.dt.total_seconds().fillna(0) * 1000
+
+    return timedelta_series_ms.rolling(window=time_window, min_periods=min_periods).std().fillna(0)
```

### Comparing `indsl-6.5.0/indsl/data_quality/score/base.py` & `indsl-6.6.0a0/indsl/data_quality/score/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2021 Cognite AS
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 
 from indsl.exceptions import UserValueError
 from indsl.type_check import check_types
 from indsl.validations import validate_series_has_time_index
@@ -33,15 +33,15 @@
 
         Args:
             analysis_start: Analysis start time
             analysis_end: Analysis end time
             events: List of event events
                 Represented as pairs of timestamps
         """
-        for (event_start, event_end) in events:
+        for event_start, event_end in events:
             if event_start > event_end:
                 raise UserValueError(
                     f"Expected start date of event to be before end date, got event_start='{event_start}' and event_end='{event_end}'"
                 )
             if event_start < analysis_start or event_end > analysis_end:
                 raise UserValueError(
                     f"Expected event to be in analysis window, got event='{event_start}-{event_end}' and analysis_window='{analysis_start}-{analysis_end}'"
@@ -122,15 +122,15 @@
             UserValueError: If series has no time index
         """
         validate_series_has_time_index(series)
 
         self.series = series
 
     @abstractmethod
-    def compute_score(self, analysis_start: pd.Timestamp, analysis_end: pd.Timestamp) -> DataQualityScore:
+    def compute_score(self, analysis_start: pd.Timestamp, analysis_end: pd.Timestamp) -> Optional[DataQualityScore]:
         """Compute data quality result.
 
         Args:
             analysis_start: analyis start time
             analysis_end: analyis end time
 
         Returns:
@@ -142,39 +142,39 @@
         """
         if analysis_start > analysis_end:
             raise UserValueError(
                 f"Expected analysis_start < analysis_end, got analysis_start '{analysis_start}' and analysis_end '{analysis_end}'"
             )
 
         if len(self.series) < 1:
-            return  # type: ignore
+            return None
 
         if analysis_start < self.series.index[0]:
             raise UserValueError(
                 f"Expected analysis_start to be equal or after the first timestamp in series, got analysis_start={analysis_start} and series.index[0]={self.series.index[0]}"
             )
         if analysis_end > self.series.index[-1]:
             raise UserValueError(
                 f"Expected analysis_end to be before or equal the last timestamp in series, got analysis_end={analysis_end} and series.index[-1]={self.series.index[-1]}"
             )
-        return  # type: ignore
+        return None
 
     def _convert_series_to_events(self, series) -> List[Tuple[pd.Timestamp, pd.Timestamp]]:
         # Each gap in the input series is represented as a consecutive (1, 1) pair.
         # Hence filtering the 1 values and re-arranging the associated index as pairs
         # yields a list of the (start, end) gap events.
         events_array = list(series[series == 1].index.values.reshape(-1, 2))
 
         # gaps are merged if the input series has consecutive gaps (see generate_step_series)
         # to split the gaps again we need to loop though the events and add the original timestamps:
         # todo: remove this code if generate_step_series handles consecutive gaps without merging
         timestamps = np.array(self.series.index)
         events_array_unmerged = []
 
-        for (start, end) in events_array:
+        for start, end in events_array:
             merged_timestamps = timestamps[(timestamps > start) & (timestamps < end)]
             if merged_timestamps.size > 0:
                 events_unmerged = np.concatenate(
                     (merged_timestamps, merged_timestamps, np.array([start, end])), axis=0
                 )  # duplicate timestamps to create events
                 events_unmerged_sorted = np.sort(events_unmerged)
                 events_array_unmerged.extend(events_unmerged_sorted.reshape(-1, 2))
@@ -183,22 +183,20 @@
 
         return [(pd.Timestamp(start), pd.Timestamp(end)) for start, end in events_array_unmerged]
 
     @staticmethod
     def _filter_events_outside_analysis_period(
         events: List[Tuple[pd.Timestamp, pd.Timestamp]], analysis_start: pd.Timestamp, analysis_end: pd.Timestamp
     ) -> List[Tuple[pd.Timestamp, pd.Timestamp]]:
-
         return [(start, end) for start, end in events if end > analysis_start and start < analysis_end]
 
     @staticmethod
     def _limit_first_and_last_events_to_analysis_period(
         gaps: List[Tuple[pd.Timestamp, pd.Timestamp]], analysis_start: pd.Timestamp, analysis_end: pd.Timestamp
     ) -> List[Tuple[pd.Timestamp, pd.Timestamp]]:
-
         if len(gaps) == 0:
             return gaps
 
         first_gap = gaps[0]
         gaps[0] = (max(first_gap[0], analysis_start), first_gap[1])
 
         last_gap = gaps[-1]
```

### Comparing `indsl-6.5.0/indsl/data_quality/score/completeness/density.py` & `indsl-6.6.0a0/indsl/data_quality/score/completeness/density.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Copyright 2021 Cognite AS
 from __future__ import annotations
 
-from typing import Literal, Optional, Union
+from typing import Optional, Union
 
 import pandas as pd
 
+
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
 from indsl.data_quality.low_density_identification import (
     low_density_identification_iqr,
     low_density_identification_modified_z_scores,
     low_density_identification_threshold,
     low_density_identification_z_scores,
 )
 from indsl.data_quality.score.base import DataQualityScore, DataQualityScoreAnalyser
```

### Comparing `indsl-6.5.0/indsl/data_quality/score/completeness/gap.py` & `indsl-6.6.0a0/indsl/data_quality/score/completeness/gap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Copyright 2021 Cognite AS
 from __future__ import annotations
 
-from typing import List, Literal, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import pandas as pd
 
+
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
 from indsl.data_quality.gaps_identification import (
     gaps_identification_iqr,
     gaps_identification_modified_z_scores,
     gaps_identification_threshold,
     gaps_identification_z_scores,
 )
 from indsl.data_quality.score.base import DataQualityScore, DataQualityScoreAnalyser
```

### Comparing `indsl-6.5.0/indsl/data_quality/value_decrease_indication.py` & `indsl-6.6.0a0/indsl/data_quality/value_decrease_indication.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/data_quality/value_decrease_indication_v1.py` & `indsl-6.6.0a0/indsl/data_quality/value_decrease_indication_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/detect/change_point_detector.py` & `indsl-6.6.0a0/indsl/detect/change_point_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Copyright 2022 Cognite AS
-from typing import Callable, List
+from typing import List
 
 import numpy as np
 import pandas as pd
 
 from numba import jit
 
 from indsl.detect.utils import resample_timeseries
-
-from ..exceptions import UserRuntimeError, UserTypeError, UserValueError
-from ..type_check import check_types
-from ..validations import validate_series_has_time_index
+from indsl.exceptions import UserRuntimeError, UserTypeError, UserValueError
+from indsl.type_check import check_types
+from indsl.validations import validate_series_has_time_index
 
 
 @check_types
 def cpd_ed_pelt(data: pd.Series, min_distance: int = 1) -> pd.Series:
     """Change Point Detection.
 
     This function detects change points in a time series. The time series is split into "statistically homogeneous" segments using the
@@ -30,15 +29,14 @@
     Returns:
         pandas.Series: Time series.
         Binary time series.
     """
     validate_series_has_time_index(data)
 
     data_resampled: pd.Series = resample_timeseries(data=data)
-
     # the maximum allowable distance is half the number of datapoints
     max_distance: int = int(np.floor(len(data_resampled) / 2))
     if min_distance > max_distance:
         raise UserRuntimeError(
             f"Minimum segment distance argument ({min_distance}) is larger than the maximum allowable segment distance ({max_distance})"
         )
 
@@ -189,15 +187,16 @@
 
     # we should precalculate sums for empirical CDF, it will allow fast evaluating of the segment cost
     partial_sums: np.ndarray = get_partial_sums(data, k)
 
     # since we use the same values of `partial_sums`, `k`, `n` all the time,
     # we introduce a shortcut `cost(tau1, tau2)` for segment cost evaluation.
     # hereinafter, we use `tau` to name variables that are changepoint candidates.
-    cost: Callable[[int, int], float] = lambda tau1, tau2: get_segment_cost(partial_sums, tau1, tau2, k, n)
+    def cost(tau1: int, tau2: int) -> float:
+        return get_segment_cost(partial_sums, tau1, tau2, k, n)
 
     # we will use dynamic programming to find the best solution; `best_cost` is the cost array.
     # `best_cost[i]` is the cost for subarray `data[0..i - 1]`.
     # it's a 1-based array (`data[0]`..`data[n-1]` correspond to `best_cost[1]`..`best_cost[n]`)
     best_cost: np.ndarray = np.zeros(n + 1)
     best_cost[0] = -penalty
     for current_tau in range(min_distance, 2 * min_distance):
@@ -222,15 +221,15 @@
         # segment. This cost equals the cost for the `previous_tau` plus cost of the new segment (from `previous_tau`
         # to `current_tau`) plus penalty for the new changepoint.
         cost_for_previous_tau: List[float] = [
             best_cost[previous_tau] + cost(previous_tau, current_tau) + penalty for previous_tau in previous_taus
         ]
 
         # Now we should choose the tau that provides the minimum possible cost.
-        best_previous_tau_index: int = np.argmin(cost_for_previous_tau)
+        best_previous_tau_index: np.int64 = np.argmin(cost_for_previous_tau)
         best_cost[current_tau] = cost_for_previous_tau[best_previous_tau_index]
         previous_change_point_index[current_tau] = previous_taus[best_previous_tau_index]
 
         # Prune phase: we remove "useless" tau values that will not help to achieve minimum cost in the future
         current_best_cost: float = best_cost[current_tau]
         new_previous_taus_size: int = 0
         for i in range(len(previous_taus)):
@@ -240,17 +239,19 @@
         previous_taus = previous_taus[:new_previous_taus_size]
 
         # We add a new tau value that is located on the `min_distance` distance from the next `current_tau` value
         previous_taus.append(current_tau - (min_distance - 1))
 
     # here we collect the result list of changepoint indexes `change_point_indexes` using `previous_change_point_index`
     change_point_indexes: List[int] = []
-    current_index: int = previous_change_point_index[n]  # The index of the end of the last segment is `n`
+    current_index: np.int64 = np.int64(
+        previous_change_point_index[n]
+    )  # The index of the end of the last segment is `n`
     while current_index != 0:
         change_point_indexes.append(current_index)
-        current_index = previous_change_point_index[current_index]
+        current_index = np.int64(previous_change_point_index[current_index])
 
     # sort the change_point_indexes and transform it to a numpy ndarray
     result: np.ndarray = np.asarray(change_point_indexes, dtype=int)
     result_sorted: np.ndarray = np.sort(result)
 
     return result_sorted
```

### Comparing `indsl-6.5.0/indsl/detect/cusum.py` & `indsl-6.6.0a0/indsl/detect/cusum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # Copyright 2022 Cognite AS
-from typing import Literal, Optional
+from typing import Optional
 
 import numpy as np
 import pandas as pd
 
-from ..exceptions import UserValueError
-from ..type_check import check_types
-from ..validations import validate_series_has_time_index, validate_series_is_not_empty
+
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
+from indsl.exceptions import UserValueError
+from indsl.type_check import check_types
+from indsl.validations import validate_series_has_time_index, validate_series_is_not_empty
 
 
 class Cusum:
     """Cumulative sum (CUSUM).
 
     This technique calculates the cumulative sum of positive and negative changes (g+t and g−t) in the data (x) and compares them to a threshold.
     When this threshold is exceeded, a change is detected (time_talarm), and the cumulative sum restarts from zero.
```

### Comparing `indsl-6.5.0/indsl/detect/drift_detector.py` & `indsl-6.6.0a0/indsl/detect/drift_detector_v1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 # Copyright 2021 Cognite AS
-from typing import Literal
-
 import numpy as np
 import pandas as pd
 
 from indsl import versioning
 from indsl.type_check import check_types
 
-from . import drift_detector_v1  # noqa
-
 
-@versioning.register(version="2.0", changelog="Updated input parameter types")
+@versioning.register(version="1.0", deprecated=True)
 @check_types
 def drift(
     data: pd.Series,
-    long_interval: pd.Timedelta = pd.Timedelta("3d"),
-    short_interval: pd.Timedelta = pd.Timedelta("4h"),
+    long_interval: str = "3d",
+    short_interval: str = "4h",
     std_threshold: float = 3,
-    detect: Literal["decrease", "increase", "both"] = "both",
+    detect: str = "both",
 ) -> pd.Series:
     """Drift.
 
     This function detects data drift (deviation) by comparing two rolling averages, short and long interval, of the signal. The
     deviation between the short and long term average is considered significant if it is above a given threshold
     multiplied by the rolling standard deviation of the long term average.
```

### Comparing `indsl-6.5.0/indsl/detect/drift_detector_v1.py` & `indsl-6.6.0a0/indsl/detect/drift_detector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # Copyright 2021 Cognite AS
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
 import numpy as np
 import pandas as pd
 
+from typing_extensions import Literal
+
 from indsl import versioning
 from indsl.type_check import check_types
 
+from . import drift_detector_v1  # noqa
+
 
-@versioning.register(version="1.0", deprecated=True)
+@versioning.register(version="2.0", changelog="Updated input parameter types")
 @check_types
 def drift(
     data: pd.Series,
-    long_interval: str = "3d",
-    short_interval: str = "4h",
+    long_interval: pd.Timedelta = pd.Timedelta("3d"),
+    short_interval: pd.Timedelta = pd.Timedelta("4h"),
     std_threshold: float = 3,
-    detect: str = "both",
+    detect: Literal["decrease", "increase", "both"] = "both",
 ) -> pd.Series:
     """Drift.
 
     This function detects data drift (deviation) by comparing two rolling averages, short and long interval, of the signal. The
     deviation between the short and long term average is considered significant if it is above a given threshold
     multiplied by the rolling standard deviation of the long term average.
```

### Comparing `indsl-6.5.0/indsl/detect/steady_state.py` & `indsl-6.6.0a0/indsl/detect/steady_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import numpy as np
 import pandas as pd
 
 from scipy import stats
 
 from indsl.detect.change_point_detector import ed_pelt
 from indsl.detect.utils import constrain, resample_timeseries
-
-from ..exceptions import UserValueError
+from indsl.exceptions import UserValueError
 
 # Detectors
-from ..type_check import check_types
-from ..validations import validate_series_has_time_index
+from indsl.type_check import check_types
+from indsl.validations import validate_series_has_time_index
 
 
 @check_types
 def ssd_cpd(
     data: pd.Series, min_distance: int = 15, var_threshold: float = 2.0, slope_threshold: float = -3.0
 ) -> pd.Series:
     """Steady State Detection (CPD).
@@ -74,16 +73,16 @@
     # this will prevent generating infinite values on the var calculation below
     divisor: float = constrain(value=avg, min=1.0e-4, max=1.0e6)
 
     # loop over all changepoint segments
     # we consider a region as transient (value = 0) unless it passes the subsequent logical tests
     ss_map: np.ndarray = np.zeros_like(y)
     for i in range(1, len(change_points)):
-        i0: int = change_points[i - 1]
-        i1: int = change_points[i]
+        i0: np.int64 = np.int64(change_points[i - 1])
+        i1: np.int64 = np.int64(change_points[i])
         xi: np.ndarray = x[i0:i1]
         yi: np.ndarray = y[i0:i1]
 
         # compute the segment standard deviation and normalize it by the segment length
         std: float = np.std(yi) / (i1 - i0)
         # calculate a normalized variance (this is an effort to make the var_threshold more generic between different
         # timeseries)
```

### Comparing `indsl-6.5.0/indsl/detect/unchanged_signal_detector.py` & `indsl-6.6.0a0/indsl/detect/unchanged_signal_detector.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/detect/utils.py` & `indsl-6.6.0a0/indsl/detect/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2021 Cognite AS
 import numpy as np
 import pandas as pd
 
-from ..exceptions import UserValueError
-from ..type_check import check_types
-from ..validations import validate_series_has_time_index
+from indsl.exceptions import UserValueError
+from indsl.type_check import check_types
+from indsl.validations import validate_series_has_time_index
 
 
 @check_types
 def resample_timeseries(data: pd.Series, is_step: bool = False) -> pd.Series:
     """Resample timeseries.
 
     Resamples a timeseries (provided as a pandas Series with datetime index)
```

### Comparing `indsl-6.5.0/indsl/drilling/flag_detection.py` & `indsl-6.6.0a0/indsl/drilling/flag_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Copyright 2022 Cognite AS
 
 import numpy as np
 import pandas as pd
 
+from indsl.exceptions import UserValueError
+from indsl.ts_utils.utility_functions import generate_step_series
 from indsl.type_check import check_types
 
-from ..exceptions import UserValueError
-from ..ts_utils.utility_functions import generate_step_series
-
 
 @check_types
 def rotation_detection(
     rot_vel: pd.Series,
     thresh: float = 0,
 ) -> pd.Series:
     """Rotation detection.
```

### Comparing `indsl-6.5.0/indsl/equipment/__init__.py` & `indsl-6.6.0a0/indsl/equipment/__init__.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/equipment/pump_parameters.py` & `indsl-6.6.0a0/indsl/equipment/pump_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,14 @@
     if the pump liquid flow rate :math:`Q_L\:[\frac{m^3}{s}]`, total head across the pump
     :math:`h` [m], and density of the fluid :math:`\rho_L\:[\frac{kg}{m^3}]`.
 
     .. math::
         Pump\:hydraulic\:power=9.81Q_L\rho_Lh
 
     Args:
-
         pump_liquid_flowrate: Pump liquid flow rate [:math:`\mathrm{\frac{m^3}{s}}`].
             The current flow rate of the pump.
         total_head: Total head across pump [m].
             Difference in pressure between discharge and suction of pump.
         den: Density of the fluid [:math:`\mathrm{\frac{kg}{m^3}}`].
         align_timesteps: Auto-align.
             Automatically align time stamp  of input time series. Default is False.
@@ -139,15 +138,14 @@
     Therefore the input parameters of the curve are coefficients
     to :math:`x^2` and :math:`x` and the :math:`y` intercept of the curve.
 
     .. math::
         Pump\:shaft\:power=\frac{Pump\:hydraulic\:power}{\eta(Q_L)}
 
     Args:
-
         pump_hydraulic_power: Pump hydraulic power [W].
         pump_liquid_flowrate: Pump liquid flowrate [:math:`\mathrm{\frac{m^3}{h}}`].
             The current flow rate of the pump.
         eff_parameter_1: :math:`x^2` coefficient [-].
             Coefficient of :math:`x^2`.
         eff_parameter_2: :math:`x` coefficient [-].
             Coefficient of :math:`x`.
```

### Comparing `indsl-6.5.0/indsl/equipment/volume_vessel.py` & `indsl-6.6.0a0/indsl/equipment/volume_vessel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright 2022 Cognite AS
 import os
 
-from typing import List, Literal, Union
+from typing import List, Union
 
 import numpy as np
 import pandas as pd
 
+
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
 from indsl.resample.auto_align import auto_align
 from indsl.type_check import check_types
 
 
 # InDSL runs some PR checks with numba disabled which does not work with the
 # numba vectorized implementation from fluids package
 NUMBA_DISABLED = os.environ.get("NUMBA_DISABLE_JIT") == "1"
```

### Comparing `indsl-6.5.0/indsl/filter/simple_filters.py` & `indsl-6.6.0a0/indsl/filter/simple_filters.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/filter/wavelet_filter.py` & `indsl-6.6.0a0/indsl/filter/wavelet_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright 2022 Cognite AS
-from typing import Literal
 
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
 import pandas as pd
 
 from skimage.restoration import denoise_wavelet
+from typing_extensions import Literal
 
 from indsl import versioning
+from indsl.exceptions import UserValueError
+from indsl.type_check import check_types
 
-from ..exceptions import UserValueError
-from ..type_check import check_types
 from . import wavelet_filter_v1  # noqa
 
 
 # TODO: Add more wavelet types from https://pywavelets.readthedocs.io/en/latest/ref/wavelets.html
 wavelet_options = Literal[
     "db1",
     "db2",
```

### Comparing `indsl-6.5.0/indsl/filter/wavelet_filter_v1.py` & `indsl-6.6.0a0/indsl/filter/wavelet_filter_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from enum import Enum
 
 import pandas as pd
 
 from skimage.restoration import denoise_wavelet
 
 from indsl import versioning
-
-from ..exceptions import UserValueError
-from ..type_check import check_types
+from indsl.exceptions import UserValueError
+from indsl.type_check import check_types
 
 
 class WaveletType(Enum):
     """Wavelet types."""
 
     DAUBECHIES_1 = "db1"
     DAUBECHIES_2 = "db2"
```

### Comparing `indsl-6.5.0/indsl/fluid_dynamics/dimensionless.py` & `indsl-6.6.0a0/indsl/fluid_dynamics/dimensionless.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/fluid_dynamics/friction.py` & `indsl-6.6.0a0/indsl/fluid_dynamics/friction.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/forecast/arma_predictor.py` & `indsl-6.6.0a0/indsl/forecast/arma_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
 import numpy as np
 import pandas as pd
 
 from statsmodels.tsa.arima.model import ARIMA
 
 from indsl import versioning
-
-from ..exceptions import UserRuntimeError, UserValueError
-from ..type_check import check_types
+from indsl.exceptions import UserRuntimeError, UserValueError
+from indsl.type_check import check_types
 
 
 class MethodType(Enum):
     """Method type."""
 
     ONESTEP = "onestep"
     MULTISTEP = "multistep"
@@ -71,23 +70,21 @@
     # If method is multistep, then simply forecast some steps ahead of training dataset
     if method == MethodType.MULTISTEP:
         train_data = data.iloc[:n_train]
         pred_data = _train_and_return_forecast(ar_order, ma_order, train_data, steps, dt_step_sec)
 
     # If method is onestep, then iterate through test dataset and perform a one step prediction
     elif method == MethodType.ONESTEP:
-
         # Storage array
         store_forecast = []
 
         # Limiting number of cycles to 100
         cycles = min(n_obs - n_train, 100)
 
         for it in range(cycles + 1):
-
             # Append new observation
             train_data = data.iloc[it : it + n_train]
             res = _train_and_return_forecast(ar_order, ma_order, train_data, steps, dt_step_sec)
             store_forecast.append(res.tail(1))
 
         # Concatenate prediction dataframe
         pred_data = pd.concat(store_forecast)
```

### Comparing `indsl-6.5.0/indsl/forecast/holt_winters_predictor.py` & `indsl-6.6.0a0/indsl/forecast/holt_winters_predictor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # Copyright 2022 Cognite AS
-import typing
 
 import numpy as np
 import pandas as pd
 
 from statsmodels.tsa.holtwinters import ExponentialSmoothing
 
-from indsl import versioning
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
 
-from ..exceptions import UserRuntimeError, UserValueError
-from ..type_check import check_types
-from ..validations import validate_series_has_time_index
+from indsl import versioning
+from indsl.exceptions import UserRuntimeError, UserValueError
+from indsl.type_check import check_types
+from indsl.validations import validate_series_has_time_index
 
 
 @versioning.register(version="1.0", deprecated=True)
 @check_types
 def holt_winters_predictor(
     data: pd.Series,
     seasonal_periods: int,
-    seasonality: typing.Literal["add", "mul"] = "add",
-    trend: typing.Literal["add", "mul"] = "add",
+    seasonality: Literal["add", "mul"] = "add",
+    trend: Literal["add", "mul"] = "add",
     dampen_trend: bool = False,
     steps: int = 1,
     train_fraction: float = 0.8,
 ) -> pd.Series:
     """Triple exponential smoothing.
 
     This technique (also known as Holt-Winters) can forecast time series data with a trend and
```

### Comparing `indsl-6.5.0/indsl/not_listed_operations/deprecated_functions.py` & `indsl-6.6.0a0/indsl/not_listed_operations/deprecated_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,25 +118,25 @@
     "LOG": log,
     "LOG2": log2,
     "LOG10": log10,
     "LOGN": logn,
 }
 
 for old_op_code, f in old_to_new.items():
-
     # If multiple versions exist, use version 1.0
     try:
         f = versioning.get(versioning.get_name(f), "1.0")
     except ValueError:
         pass
 
     # inDSLs versioning does not support giving a function two names
     # (here e.g. SIN and sin). We work around this by creating a
     # dummy-wrapper function
-    def make_cpy(f):  # noqa
+    def make_cpy(f):
+        """Dummy wrapper function."""
         return functools.wraps(f)(lambda *args, **kwargs: f(*args, **kwargs))
 
     f_cpy = make_cpy(f)
 
     # Register function as a deprecated function with the old op code
     versioning.register(
         "1.0", old_op_code, deprecated=True, changelog="Deprecated function. Re-create node to upgrade"
```

### Comparing `indsl-6.5.0/indsl/oil_and_gas/engineering_calcs.py` & `indsl-6.6.0a0/indsl/oil_and_gas/engineering_calcs.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/oil_and_gas/gas_density_calcs.py` & `indsl-6.6.0a0/indsl/oil_and_gas/gas_density_calcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,26 +45,26 @@
            Estimated gas density in pound-mass per cubic foot (pcf).
 
     Raises:
        UserValueError: When all values of the pressure and temperature are out of range for calculating compressibility.
     """
     # check specific gravity value
     validate_series_is_not_empty(sg)
-    sg = sg[0]
-    if sg == 0:
+    sg_ = sg[0]
+    if sg_ == 0:
         raise UserValueError("Specific gravity cannot be zero")
 
     # auto-align
     pressure, temperature = auto_align([pressure, temperature], align_timesteps)
 
-    M = M_AIR * sg  # Molar mass of gas
+    M = M_AIR * sg_  # Molar mass of gas
     R = R_U / M  # gas constant
 
     # calculate the pseudo - crtitical pressure and temperature
-    (Pc, Tc) = calculate_critical_prop(sg)
+    (Pc, Tc) = calculate_critical_prop(sg_)
 
     # convert pressure to kPa and temperature to K
     pressure_Kpa = CONVERT_PSI_TO_KPA * pressure
     temperature_K = 273 + ((temperature - 32) * (5 / 9))
 
     # calculate the pseudo - reduced pressure and temperature
     (Ppr, Tpr) = calculate_reduced_prop(pressure_Kpa, temperature_K, Pc, Tc)
```

### Comparing `indsl-6.5.0/indsl/oil_and_gas/live_fluid_properties.py` & `indsl-6.6.0a0/indsl/oil_and_gas/live_fluid_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 import os
 
-from typing import Literal
-
 import numpy as np
 import pandas as pd
 
 from scipy import interpolate as intp
 
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
 from indsl.type_check import check_types
 
 
 @check_types
 def _error_handling(pvt_table: np.ndarray, pressure: pd.Series, temperature: pd.Series) -> None:
     max_pressure, min_pressure = max(pvt_table[:, [0]])[0], min(pvt_table[:, [0]])[0]
     max_temperature, min_temperature = max(pvt_table[:, [1]])[0], min(pvt_table[:, [1]])[0]
```

### Comparing `indsl-6.5.0/indsl/oil_and_gas/shut_in_detector.py` & `indsl-6.6.0a0/indsl/oil_and_gas/shut_in_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Copyright 2022 Cognite AS
+from typing import Optional
+
 import numpy as np
 import pandas as pd
 
+from indsl.exceptions import UserValueError
 from indsl.type_check import check_types
 
-from ..exceptions import UserValueError
-
 
 @check_types
 def calculate_shutin_interval(
     shut_valve: pd.Series,
     min_shutin_len: int = 6,
     min_time_btw_shutins: int = 1,
     shutin_state_below_threshold: bool = True,
-    shutin_threshold: int = None,
+    shutin_threshold: Optional[int] = None,
 ) -> pd.Series:
     """Shut-in interval.
 
     The shut-in interval is defined as the period when the valve is in closed state. The close state is determined based
     on the calculated manually-given threshold. The threshold is calculated based on the analysis of the valve signal
     histogram.
 
@@ -58,24 +59,24 @@
     # get shut-in starts and ends
     sh_start = list(wvalve[wvalve["valve_diff"] == -1]["timestamp"])
     sh_end = list(wvalve[wvalve["valve_diff"] == 1]["timestamp"])
     # create time pairs
     if sh_start and sh_end:
         # case 1: several shut-ins exist - the shut-in comes from the past - make a pseudo-start of the shut-in
         if sh_end[0] < sh_start[0]:
-            sh_start = [wvalve.iloc[0, :]["timestamp"]] + sh_start
+            sh_start = [wvalve.iloc[0, :]["timestamp"], *sh_start]
         # case 2: several shut-ins exist - the shut-in goes to the future - make a pseudo-end of shut-in
         if sh_end[-1] < sh_start[-1]:
-            sh_end = sh_end + [wvalve.iloc[-1, :]["timestamp"]]
+            sh_end = [*sh_end, wvalve.iloc[-1, :]["timestamp"]]
     elif not sh_start:
         # case 3: only one shut-in exist - the shut-in comes from the past - make a pseudo-start of the shut-in
-        sh_start = [wvalve.iloc[0, :]["timestamp"]] + sh_start
+        sh_start = [wvalve.iloc[0, :]["timestamp"], *sh_start]
     else:
         # case 4: only one shut-in exist - the shut-in comes from the past - make a pseudo-start of the shut-in
-        sh_end = sh_end + [wvalve.iloc[-1, :]["timestamp"]]
+        sh_end = [*sh_end, wvalve.iloc[-1, :]["timestamp"]]
     time_pairs = list(zip(sh_start, sh_end))
 
     # merge the shut-ins based on the minimum distance between consecutive shut-ins
     time_pairs_upd = []
     time_pairs.append(time_pairs[-1])
     i = 0
     new_pair = time_pairs[i]
```

### Comparing `indsl-6.5.0/indsl/oil_and_gas/shut_in_variables.py` & `indsl-6.6.0a0/indsl/oil_and_gas/shut_in_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import timedelta
 
 import numpy as np
 import pandas as pd
 
-from ..exceptions import UserValueError
-from ..type_check import check_types
+from indsl.exceptions import UserValueError
+from indsl.type_check import check_types
 
 
 @check_types
 def calculate_shutin_variable(
     variable_signal: pd.Series, shutin_signal: pd.Series, hrs_after_shutin: float
 ) -> pd.Series:
     """Shut-in variable calculator.
```

### Comparing `indsl-6.5.0/indsl/oil_and_gas/tab_fp_identifier.json` & `indsl-6.6.0a0/indsl/oil_and_gas/tab_fp_identifier.json`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/oil_and_gas/well_prod_status.py` & `indsl-6.6.0a0/indsl/oil_and_gas/well_prod_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Union
 
 import numpy as np
 import pandas as pd
 
+from indsl.exceptions import UserValueError
 from indsl.resample.auto_align import auto_align
-
-from ..exceptions import UserValueError
-from ..type_check import check_types
+from indsl.type_check import check_types
 
 
 @check_types
 def _pct_to_fraction(pct_value: Union[float, int]):
     return pct_value / 100.0
```

### Comparing `indsl-6.5.0/indsl/regression/polynomial.py` & `indsl-6.6.0a0/indsl/regression/polynomial.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright 2022 Cognite AS
-from typing import Literal
 
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
 import numpy as np
 import pandas as pd
 
 from sklearn.linear_model import Lasso, LinearRegression, Ridge
 from sklearn.pipeline import make_pipeline
 from sklearn.preprocessing import PolynomialFeatures
+from typing_extensions import Literal
 
-from ..exceptions import UserValueError
-from ..type_check import check_types
+from indsl.exceptions import UserValueError
+from indsl.type_check import check_types
 
 
 @check_types
 def poly_regression(
     data: pd.Series,
     order: int = 2,
     method: Literal["Lasso", "Ridge", "No regularisation"] = "No regularisation",
```

### Comparing `indsl-6.5.0/indsl/resample/README.md` & `indsl-6.6.0a0/indsl/resample/README.md`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/resample/auto_align.py` & `indsl-6.6.0a0/indsl/resample/auto_align.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/resample/group_by.py` & `indsl-6.6.0a0/indsl/resample/group_by.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright 2023 Cognite AS
 
-from typing import Literal
-
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
 import numpy as np
 import pandas as pd
 
+from typing_extensions import Literal
+
+from indsl.exceptions import UserValueError
 from indsl.resample.auto_align import auto_align
 from indsl.type_check import check_types
 
-from ..exceptions import UserValueError
-
 
 @check_types
 def group_by_region(
     data: pd.Series,
     filter_by: pd.Series,
     int_to_keep: int = 1,
     aggregate: Literal["Mean", "Median", "Standard deviation", "Count", "Min", "Max"] = "Mean",
```

### Comparing `indsl-6.5.0/indsl/resample/interpolate.py` & `indsl-6.6.0a0/indsl/resample/interpolate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Copyright 2022 Cognite AS
 import warnings
 
 from contextlib import suppress
-from typing import Literal, Union
+from typing import Union
 
 import numpy as np
 import pandas as pd
 import scipy.interpolate
 
+
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
 from indsl import versioning
+from indsl.exceptions import UserValueError
 from indsl.ts_utils.ts_utils import functional_mean, is_na_all
+from indsl.type_check import check_types
 
-from ..exceptions import UserValueError
-from ..type_check import check_types
 from . import interpolate_v1  # noqa
 
 
 @versioning.register(version="1.1", changelog="Removed outside_fill parameter")
 @check_types
 def interpolate(
     data: pd.Series,
@@ -65,15 +69,15 @@
     """
     # Check if all values are NaN
     if is_na_all(data):
         warnings.warn("All values in the time series are NaN.", UserWarning)
         return data
 
     # Allow for other ways of defining forward filling for stepwise functions
-    method = "previous" if method in ("ffill", "stepwise") else method  # type: ignore
+    method_ = "previous" if method in ("ffill", "stepwise") else method
 
     # Get outside fill value
     if bounded:
         fill_value = np.nan
     else:
         fill_value = "extrapolate"
 
@@ -97,15 +101,15 @@
 
     # x and y datapoints used to construct linear piecewise function
     x_observed = np.array([index.timestamp() for index in observations.index])
     y_observed = observations.values.squeeze()
 
     # interpolator function
     interper = scipy.interpolate.interp1d(
-        x_observed, y_observed, kind=method, bounds_error=False, fill_value=fill_value
+        x_observed, y_observed, kind=method_, bounds_error=False, fill_value=fill_value
     )
 
     # If pointwise, sample directly from interpolated (or original) points
     if kind == "pointwise":
         y_uniform = interper(x_uniform)
     elif kind == "average":
         y_uniform = functional_mean(interper, x_uniform)
```

### Comparing `indsl-6.5.0/indsl/resample/interpolate_v1.py` & `indsl-6.6.0a0/indsl/resample/interpolate_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # Copyright 2022 Cognite AS
 import warnings
 
 from contextlib import suppress
-from typing import Literal, Union
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import scipy.interpolate
 
+
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
 from indsl import versioning
+from indsl.exceptions import UserTypeError, UserValueError
 from indsl.ts_utils.ts_utils import functional_mean, is_na_all
-
-from ..exceptions import UserTypeError, UserValueError
-from ..type_check import check_types
+from indsl.type_check import check_types
 
 
 @versioning.register(version="1.0", deprecated=True)
 @check_types
 def interpolate(
     data: pd.Series,
     method: Literal["linear", "ffill", "stepwise", "zero", "slinear", "quadratic", "cubic"] = "linear",
     kind: Literal["pointwise", "average"] = "pointwise",
     granularity: str = "1s",
     bounded: int = 1,
-    outside_fill: str = None,
+    outside_fill: Optional[str] = None,
 ) -> Union[pd.DataFrame, pd.Series]:
     """Interpolation.
 
     Interpolates and resamples data with a uniform sampling frequency.
 
     Args:
         data: Time series.
@@ -76,15 +79,15 @@
 
     # Check if all values are NaN
     if is_na_all(data):
         warnings.warn("All values in the time series are NaN.", RuntimeWarning)
         return data
 
     # Allow for other ways of defining forward filling for stepwise functions
-    method = "previous" if method in ("ffill", "stepwise") else method  # type: ignore
+    method_ = "previous" if method in ("ffill", "stepwise") else method
 
     # check that bounded is correctly specified
     if bounded not in (0, 1):
         raise UserTypeError("If specified, bounded must be either 1 or 0.")
     else:
         bounds_error = bool(bounded)
 
@@ -109,15 +112,15 @@
 
     # x and y datapoints used to construct linear piecewise function
     x_observed = np.array([index.timestamp() for index in observations.index])
     y_observed = observations.values.squeeze()
 
     # interpolator function
     interper = scipy.interpolate.interp1d(
-        x_observed, y_observed, kind=method, bounds_error=bounds_error, fill_value=outside_fill
+        x_observed, y_observed, kind=method_, bounds_error=bounds_error, fill_value=outside_fill
     )
 
     # If pointwise, sample directly from interpolated (or original) points
     if kind == "pointwise":
         y_uniform = interper(x_uniform)
     elif kind == "average":
         y_uniform = functional_mean(interper, x_uniform)
```

### Comparing `indsl-6.5.0/indsl/resample/reindex.py` & `indsl-6.6.0a0/indsl/resample/reindex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # Copyright 2022 Cognite AS
-from typing import List, Literal
+from typing import List
 
 import numpy as np
 import pandas as pd
 import pandas.core.indexes.datetimes
 import scipy
 
+
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
 from indsl import versioning
+from indsl.exceptions import UserTypeError, UserValueError
 from indsl.ts_utils.ts_utils import functional_mean
+from indsl.type_check import check_types
 
-from ..exceptions import UserTypeError, UserValueError
-from ..type_check import check_types
 from . import reindex_v1  # noqa
 
 
 kind_options = Literal["pointwise", "average"]
 method_options = Literal["zero", "next", "slinear", "quadratic", "cubic"]
```

### Comparing `indsl-6.5.0/indsl/resample/reindex_v1.py` & `indsl-6.6.0a0/indsl/resample/reindex_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 
 import numpy as np
 import pandas as pd
 import pandas.core.indexes.datetimes
 import scipy
 
 from indsl import versioning
+from indsl.exceptions import UserTypeError, UserValueError
 from indsl.ts_utils.ts_utils import functional_mean
 
-from ..exceptions import UserTypeError, UserValueError
-from ..type_check import check_types
-
 
 class Kind(Enum):  # noqa: D101
     POINTWISE = "pointwise"
     AVERAGE = "average"
 
 
 class Method(Enum):  # noqa: D101
@@ -41,15 +39,16 @@
         if self is Method.QUADRATIC:
             return "quadratic"
         if self is Method.CUBIC:
             return "cubic"
 
 
 @versioning.register(version="1.0", deprecated=True)
-@check_types
+# @check_types # typeguard expects str, not class Methor or Kind as a data tyepe
+# it is commented out to avoid changing the signature of this deprecated function, so that it is compatible with Charts
 def reindex(
     data1: pd.Series,
     data2: pd.Series,
     method: Method = Method.LINEAR,
     kind: Kind = Kind.POINTWISE,
     bounded: bool = False,
 ) -> List[pd.Series]:
@@ -99,15 +98,16 @@
         UserTypeError: Bounded has to be of type bool
         UserValueError: All time series must have at least two values
     """
     return reindex_many([data1, data2], method, kind, bounded)
 
 
 @versioning.register(version="1.0", deprecated=True)
-@check_types
+# @check_types # typeguard expects str, not class Methor or Kind as a data tyepe
+# it is commented out to avoid changing the signature of this deprecated function, so that it is compatible with Charts
 def reindex_many(
     data: List[pd.Series],
     method: Method = Method.LINEAR,
     kind: Kind = Kind.POINTWISE,
     bounded: bool = False,
 ) -> List[pd.Series]:
     """Re-indexes list.
@@ -171,15 +171,16 @@
 
     # Reindex data to common index
     out = [_reindex(d, idx_common, method, kind, bounded) for d in data]
 
     return out
 
 
-@check_types
+# @check_types # typeguard expects str, not class Methor or Kind as a data tyepe
+# it is commented out to avoid changing the signature of this deprecated function, so that it is compatible with Charts
 def _reindex(
     data: pd.Series,
     new_index: pandas.core.indexes.datetimes.DatetimeIndex,
     method: Method,
     kind: Kind,
     bounds_error: bool,
 ) -> pd.Series:
```

### Comparing `indsl-6.5.0/indsl/resample/resample.py` & `indsl-6.6.0a0/indsl/resample/resample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Copyright 2022 Cognite AS
 import operator as op
 import warnings
 
-from typing import Literal, Optional
+from typing import Optional
 
 import pandas as pd
 
 from scipy import signal
 
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
 from indsl import versioning
 from indsl.exceptions import UserTypeError
 from indsl.ts_utils.ts_utils import fill_gaps, get_fixed_freq, is_na_all
 from indsl.type_check import check_types
 from indsl.validations import validate_series_has_time_index, validate_series_is_not_empty
 
 from . import resample_v1  # noqa
@@ -93,15 +96,15 @@
     validate_series_is_not_empty(data)
     if is_na_all(data):
         raise UserTypeError("All values in the time series are NaN.")
 
     # To resample data to uniform distribution
     if not granularity_current:
         # it returns none if it isn't able to infer the resolution
-        granularity_current = pd.infer_freq(data.index, True)
+        granularity_current = pd.infer_freq(data.index)
 
         if not granularity_current:
             # TODO: pick max resolution and apply to the rest of the timeseries?
             warnings.warn(
                 "Can't infer time series resolution with missing data. Please provide resolution", UserWarning
             )
             return data
```

### Comparing `indsl-6.5.0/indsl/resample/resample_v1.py` & `indsl-6.6.0a0/indsl/resample/resample_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Copyright 2022 Cognite AS
 import operator as op
 import warnings
 
 from enum import Enum
-from typing import Literal, Optional
+from typing import Optional
 
 import pandas as pd
 
 from scipy import signal
 
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
 from indsl import versioning
 from indsl.exceptions import UserTypeError, UserValueError
 from indsl.ts_utils.ts_utils import fill_gaps, get_fixed_freq, is_na_all
 from indsl.type_check import check_types
 from indsl.validations import validate_series_has_time_index
 
 
@@ -93,15 +96,15 @@
         raise UserValueError(f"Expected data to be of length > 0, got length {len(data)}")
     elif is_na_all(data):
         raise UserTypeError("All values in the time series are NaN.")
 
     # To resample data to uniform distribution
     if not granularity_current:
         # it returns none if it isn't able to infer the resolution
-        granularity_current = pd.infer_freq(data.index, True)
+        granularity_current = pd.infer_freq(data.index)
 
         if not granularity_current:
             # TODO: pick max resolution and apply to the rest of the timeseries?
             warnings.warn(
                 "Can't infer time series resolution with missing data. Please provide resolution", UserWarning
             )
             return data
@@ -187,22 +190,22 @@
 
     # Translates from cdf aggregates to pandas method names:
     # TODO: 'mean' (point-weighted) does not equal CDF average (time-weighted).
     # Read more in the docs: https://docs.cognite.com/dev/concepts/aggregation/
     start_time = series.index[0]
     end_time = series.index[-1]
     if aggregate in (AggregateEnum.MIN, AggregateEnum.MAX, AggregateEnum.SUM, AggregateEnum.COUNT, AggregateEnum.MEAN):
-        series = series.resample(granularity.replace("m", "T"), origin="epoch")
-        series = op.methodcaller(aggregate.value)(series)
+        resampled_series = series.resample(granularity.replace("m", "T"), origin="epoch")
+        agg_series = op.methodcaller(aggregate.value)(resampled_series)
         if aggregate is AggregateEnum.MEAN:
             # We only fill inner holes with lin.interp for average:
-            series = series.interpolate("slinear")
-        return series.dropna()
+            agg_series = agg_series.interpolate("slinear")
+        return agg_series.dropna()
 
     elif aggregate in (AggregateEnum.INTERPOLATION, AggregateEnum.STEP_INTERPOLATION):
         # We adhere to the CDF definition of interp. and step interp:
         fixed_freq = get_fixed_freq(start_time, end_time, granularity)
-        series = series.reindex(series.index.union(fixed_freq))  # Note: reindex, not resample
+        series_ = series.reindex(series.index.union(fixed_freq))  # Note: reindex, not resample
         if aggregate is AggregateEnum.INTERPOLATION:
-            return series.interpolate("slinear")[fixed_freq].dropna()
+            return series_.interpolate("slinear")[fixed_freq].dropna()
         else:
-            return series.ffill().bfill()[fixed_freq]
+            return series_.ffill().bfill()[fixed_freq]
```

### Comparing `indsl-6.5.0/indsl/signals/generator.py` & `indsl-6.6.0a0/indsl/signals/generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+# Copyright 2023 Cognite AS
 import warnings
 
-from typing import Any, List, Literal, Optional, Union
+from typing import Any, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 
-from ..exceptions import UserValueError
-from ..type_check import check_types
-from ..validations import validate_series_has_time_index
+
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
+from indsl.exceptions import UserValueError
+from indsl.signals.noise import RedNoise, Sinusoidal, TimeSampler, TimeSeries
+from indsl.ts_utils.utility_functions import TimeUnits
+from indsl.type_check import check_types
+from indsl.validations import validate_series_has_time_index
 
 
 @check_types
 def line(
     start_date: Optional[pd.Timestamp] = None,
     end_date: Optional[pd.Timestamp] = None,
     sample_freq: pd.Timedelta = pd.Timedelta("1 m"),
@@ -160,23 +167,110 @@
             f"The sampling frequency must be a value higher than zero. " f"Value provided was {sample_freq}"
         )
     if wave_period.total_seconds() == 0:
         raise UserValueError("The wave period can not be zero")
 
     idx = _make_index(start=start_date, end=end_date, freq=sample_freq)
 
-    wave_period = wave_period / pd.Timedelta(1, unit="s")
+    wave_period_ = wave_period / pd.Timedelta(1, unit="s")
 
-    angular_freq = 2 * np.pi * (1 / wave_period)
+    angular_freq = 2 * np.pi * (1 / wave_period_)
     wave_data = wave_amplitude * np.sin(angular_freq * _time_array(idx) + wave_phase) + wave_mean
 
     return pd.Series(data=wave_data, index=idx, name="Sine wave")
 
 
 @check_types
+def wave_with_brownian_noise(
+    duration: int = 14400,
+    resolution: float = 0.5,
+    percentage: float = 100,
+    amplitude: float = 10,
+    mean: float = 200,
+    frequency: float = 0.04,
+    noise: List[int] = [1, 1],
+):
+    """Wave with brownian noise.
+
+    Sinusoidal signal with brownian noise. The signal has a
+    given duration of 4 hours as a default, a resolution of 0.5,
+    an amplitude of 10, a mean of 200 and a frequency of 0.04 Hz.
+
+
+    Args:
+        duration: Duration.
+            Duration of the time series in seconds. Defaults to 14400.
+        resolution: Resolution.
+            Frequency resolution. Defaults to 0.5.
+        percentage: Percentage.
+            Percentage of the time series to keep. Defaults to 100.
+        amplitude: Amplitude.
+            Amplitude of the wave. Defaults to 10.
+        mean: Mean.
+            Mean of the wave. Defaults to 200.
+        frequency: Frequency.
+            Frequency of the wave. Defaults to 0.04 Hz.
+        noise: Noise.
+            Noise of the wave. Defaults to [1, 1].
+
+    Returns:
+        pd.Series:
+            Sine wave with brownian noise.
+    """
+    # Initializing TimeSampler
+    time_sampler = TimeSampler(stop_time=duration)
+    # Sampling irregular time samples
+    time_vector = time_sampler.sample_irregular_time(resolution=resolution, keep_percentage=percentage)
+
+    # Initializing Sinusoidal signal
+    sinusoid = Sinusoidal(amplitude=amplitude, frequency=frequency)
+
+    # Initializing Red (Brownian) noise
+    red_noise = RedNoise(std=noise[0], tau=noise[1])
+
+    # Initializing TimeSeries class with the signal and noise objects
+    timeseries_corr = TimeSeries(sinusoid, noise_generator=red_noise)
+
+    # Sampling using the irregular time samples
+    data_points, signals_corr, errors_corr = timeseries_corr.sample(time_vector)
+    data_points = data_points + mean
+
+    time_vector = pd.to_datetime(time_vector, unit="s")
+    return pd.Series(data=data_points, index=time_vector)
+
+
+@check_types
+def _get_sample_frequency(sample_freq: float, unit: TimeUnits):
+    """Get sample frequency.
+
+    Helper method to convert the frequency magnitude and units into a string
+    that is then used by other function to generate DatetimeIndex data.
+
+    Args:
+        sample_freq: Frequency magnitude
+        unit: Time unit
+            Valid values "ns|us|ms|s|m|h|D|W". Default is "m" (minutes)
+
+    Returns:
+        str: Frequency string
+
+    """
+    if unit == "m":
+        use_unit = "min"
+    elif unit == "s":
+        use_unit = "S"
+    elif unit == "W":
+        use_unit = "D"
+        sample_freq = sample_freq * 7
+    else:
+        use_unit = unit
+    return pd.Timedelta(sample_freq, use_unit)
+
+
+@check_types
 def perturb_timestamp(data: pd.Series, magnitude: float = 1) -> pd.Series:
     """Perturb timestamp.
 
     Perturb the date-time index (timestamp) of the original time series using a normal (Gaussian) distribution
     with a mean of zero and a given standard deviation (magnitude) in seconds.
 
     Args:
@@ -294,28 +388,28 @@
                 "The amount of data to remove exceeds the amount of data point available for creating gaps. Please "
                 "reduce the fraction of data to remove or use a time series with more data points"
             )
 
         # Generate random gap location, sizes and loc ranges that amount to the fraction of data to be removed
         gap_loc = np.sort(rng.integers(low=buffer1, high=buffer2, size=num_gaps))
         gap_size = _random_list_of_integers_that_gives_exact_sum(list_length=num_gaps, sum_output=points_to_remove)
-        gap_ranges = list(
-            zip(gap_loc, gap_loc + gap_size - 1)
+        gap_ranges = np.array(
+            list(zip(gap_loc, gap_loc + gap_size - 1))
         )  # BE CAREFUL WITH EDGE RANGE INCLUDING/EXCLUDING LAST DATA POINT
 
-        gap_ranges = _handle_overlapping_gaps(gap_ranges=gap_ranges, data_length=len(data))
-        idx_loc: List[np.array] = []
-        for ii in range(len(gap_ranges)):
-            idx_loc = np.append(idx_loc, np.arange(gap_ranges[ii][0], gap_ranges[ii][1] + 1, dtype=int)).astype(int)
+        gap_ranges_ = _handle_overlapping_gaps(gap_ranges=gap_ranges, data_length=len(data))
+        idx_loc: np.ndarray = np.array([])
+        for ii in range(len(gap_ranges_)):
+            idx_loc = np.append(idx_loc, np.arange(gap_ranges_[ii][0], gap_ranges_[ii][1] + 1, dtype=int)).astype(int)
         idx = data.index[idx_loc]
         return data.drop(labels=idx)
 
 
 @check_types
-def _handle_overlapping_gaps(gap_ranges: np.array, data_length: int, buffer: int = 5) -> np.ndarray:
+def _handle_overlapping_gaps(gap_ranges: np.ndarray, data_length: int, buffer: int = 5) -> np.ndarray:
     """Handle overlapping gaps.
 
     Internal method to handle overlapping gaps. The method calculates the
     number of available space to rearrange gaps in such a way that they do not
     overlap. Then traverses the ranges according to their location from left to
     right (time 0 to end) and estimates how many steps ranges to the left or
     right must be moved to comply with gap generation conditions:
```

### Comparing `indsl-6.5.0/indsl/signals/polynomial.py` & `indsl-6.6.0a0/indsl/signals/polynomial.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import List
 
 import pandas as pd
 
-from ..type_check import check_types
+from indsl.type_check import check_types
 
 
 @check_types
 def univariate_polynomial(signal: pd.Series, coefficients: List[float] = [0.0, 1.0]) -> pd.Series:
     """Univariate polynomial.
 
     Creates a univariate polynomial :math:`y`, of degree :math:`n`, from the time series :math:`x`, and a list of
     coefficients :math:`a_{n}`:
 
     .. math::
 
         y = a_0 + a_1x + a_2x^2 + a_3x^3 + ... + a_nx^n
 
     Args:
-        signal: Time series
-        coefficients: Coefficients.
-            List of coefficients separated by semicolons. The numbers must be entered, separated by semicolons (e.g., 0; 1).
-            The default is :math:`0.0; 1.0`, which returns the original time series.
+        signal (pandas.Series): Time series
+        coefficients (List[float]): Coefficients
+            List of coefficients separated by commas. The numbers must be entered separated by commas (e.g., 0, 1).
+            The default is :math:`0.0, 1.0`, which returns the original time series.
 
     Returns:
-        pandas.Series: Output
+        pd.Series: Output
     """
     poly = pd.Series(0, index=signal.index)
     n = 0
     for a in coefficients:
         poly = poly + a * signal**n
         n = n + 1
```

### Comparing `indsl-6.5.0/indsl/smooth/README.md` & `indsl-6.6.0a0/indsl/smooth/README.md`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/smooth/alma.py` & `indsl-6.6.0a0/indsl/smooth/alma.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright 2022 Cognite AS
 from typing import List, Union
 
 import numpy as np
 import pandas as pd
 
-from ..exceptions import UserValueError
-from ..type_check import check_types
-from ..validations import validate_series_has_time_index, validate_series_is_not_empty
+from indsl.exceptions import UserValueError
+from indsl.type_check import check_types
+from indsl.validations import validate_series_has_time_index, validate_series_is_not_empty
 
 
 @check_types
 def alma(data: pd.Series, window: int = 10, sigma: float = 6, offset_factor: float = 0.75) -> pd.Series:
     """Arnaud Legoux moving average.
 
     Moving average typically used in the financial industry, which aims to strike a good balance between smoothness
```

### Comparing `indsl-6.5.0/indsl/smooth/arma_smoother.py` & `indsl-6.6.0a0/indsl/smooth/arma_smoother.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022 Cognite AS
 import pandas as pd
 
 from statsmodels.tsa.arima.model import ARIMA
 
-from ..type_check import check_types
-from ..validations import validate_series_is_not_empty
+from indsl.type_check import check_types
+from indsl.validations import validate_series_is_not_empty
 
 
 @check_types
 def arma(data: pd.Series, ar_order: int = 2, ma_order: int = 2) -> pd.Series:
     """Autoregressive moving average.
 
     The autoregressive moving average (ARMA) is a popular model used in forecasting. It uses an autoregression (AR)
```

### Comparing `indsl-6.5.0/indsl/smooth/butterworth.py` & `indsl-6.6.0a0/indsl/smooth/butterworth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 Cognite AS
-from typing import Literal
-
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
 import pandas as pd
 
 from scipy.signal import butter, sosfilt
+from typing_extensions import Literal
 
 from indsl import versioning
 from indsl.type_check import check_types
 
 from . import butterworth_v1  # noqa
```

### Comparing `indsl-6.5.0/indsl/smooth/butterworth_v1.py` & `indsl-6.6.0a0/indsl/smooth/butterworth_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/smooth/chebyshev.py` & `indsl-6.6.0a0/indsl/smooth/chebyshev.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022 Cognite AS
 import pandas as pd
 
 from scipy.signal import cheby1, cheby2, sosfilt
 
-from ..exceptions import UserValueError
-from ..type_check import check_types
+from indsl.exceptions import UserValueError
+from indsl.type_check import check_types
 
 
 # noinspection SpellCheckingInspection
 
 
 @check_types
 def chebyshev(
@@ -43,15 +43,14 @@
             Defaults to "lowpass".
 
     Returns:
         pandas.Series: Filtered signal
     """
     # TODO: Move function to filter toolbox
     # TODO: Implement band and stop pass types
-    # noqa
     # Only type 1 and 2 chebyshev filter exist
     if filter_type not in {1, 2}:
         raise UserValueError("Filter type must be either 1 or 2.")
 
     if len(data) < 1:
         return data
```

### Comparing `indsl-6.5.0/indsl/smooth/eweight_ma.py` & `indsl-6.6.0a0/indsl/smooth/eweight_ma.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import numpy as np
 import pandas as pd
 
 from numba import jit
 
 from indsl import versioning
+from indsl.type_check import check_types
+from indsl.validations import validate_series_is_not_empty
 
-from ..type_check import check_types
-from ..validations import validate_series_is_not_empty
 from . import eweight_ma_v1  # noqa
 
 
 @versioning.register(version="2.0", changelog="Update parameter type")
 @check_types
 def ewma(
     data: pd.Series,
@@ -117,12 +117,12 @@
     Returns:
         None: Index of the current value is smaller than minimum number of observations in window required to have a value.
         float: Calculated ewma for the current datapoint.
     """
     if i < min_periods - 1:
         return None
     elif i == min_periods - 1:  # first value is the simple moving average
-        start_sma = data[:min_periods].sum() / len((data[:min_periods]))
+        start_sma = data[:min_periods].sum() / len(data[:min_periods])
         return start_sma
     else:
         ewma_val = (a[i] * value) + ((1 - a[i]) * ewma_vals[i - 1])
         return ewma_val
```

### Comparing `indsl-6.5.0/indsl/smooth/eweight_ma_v1.py` & `indsl-6.6.0a0/indsl/smooth/eweight_ma_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 import numpy as np
 import pandas as pd
 
 from numba import jit
 
 from indsl import versioning
-
-from ..ts_utils.ts_utils import time_parse
-from ..type_check import check_types
-from ..validations import validate_series_is_not_empty
+from indsl.ts_utils.ts_utils import time_parse
+from indsl.type_check import check_types
+from indsl.validations import validate_series_is_not_empty
 
 
 @versioning.register(version="1.0", deprecated=True)
 @check_types
 def ewma(
     data: pd.Series,
     time_window: str = "60min",
@@ -54,16 +53,16 @@
             Time window used to resample the calculated exponential moving average series. Defaults to '60min'.
 
     Returns:
         pandas.Series: Smoothed time series.
     """
     validate_series_is_not_empty(data)
 
-    time_window = time_parse(time_window)
-    win_pts_lst = np.array(data.rolling(time_window).count().values)
+    time_window_ = time_parse(time_window)
+    win_pts_lst = np.array(data.rolling(time_window_).count().values)
     ewma_vals = np.zeros_like(data)
     a = 2.0 / (win_pts_lst + 1)
     if not adjust:
         for i, value in enumerate(data):
             ewma_vals[i] = ewma_pt_not_adjust(data.values, value, min_periods, ewma_vals, i, a)
     else:
         ewma_vals[0] = data[0]
@@ -71,16 +70,16 @@
             if i == 0:
                 continue
             ewma_vals[i] = ewma_pt_adjust(data.values, value, i, a, max_pt)
     bool_mask = win_pts_lst < min_periods
     ewma_vals[bool_mask] = None
     ewma_series = pd.Series(ewma_vals, index=data.index)
     if resample:
-        resample_window = time_parse(resample_window)
-        ewma_series = ewma_series.resample(resample_window).mean()
+        resample_window_ = time_parse(resample_window)
+        ewma_series = ewma_series.resample(resample_window_).mean()
     return ewma_series
 
 
 @jit(nopython=True)  # @njit
 def ewma_pt_adjust(data: np.ndarray, value: float, i: int, a: np.ndarray, max_pt: int = 200) -> float:
     """Calculates ewma value using weights wi=(1−a)^i.
 
@@ -120,12 +119,12 @@
     Returns:
         None: Index of the current value is smaller than minimum number of observations in window required to have a value.
         float: Calculated ewma for the current datapoint.
     """
     if i < min_periods - 1:
         return None
     elif i == min_periods - 1:  # first value is the simple moving average
-        start_sma = data[:min_periods].sum() / len((data[:min_periods]))
+        start_sma = data[:min_periods].sum() / len(data[:min_periods])
         return start_sma
     else:
         ewma_val = (a[i] * value) + ((1 - a[i]) * ewma_vals[i - 1])
         return ewma_val
```

### Comparing `indsl-6.5.0/indsl/smooth/img/ma_min_periods1.png` & `indsl-6.6.0a0/indsl/smooth/img/ma_min_periods1.png`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/smooth/img/ma_min_periods5.png` & `indsl-6.6.0a0/indsl/smooth/img/ma_min_periods5.png`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/smooth/img/zoom_min_periods5.png` & `indsl-6.6.0a0/indsl/smooth/img/zoom_min_periods5.png`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/smooth/lweight_ma.py` & `indsl-6.6.0a0/indsl/smooth/lweight_ma.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/smooth/lweight_ma_v1.py` & `indsl-6.6.0a0/indsl/smooth/lweight_ma_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,24 @@
             Resamples the calculated linear weighted moving average series. Defaults to False
         resample_window: Resampling window.
             Time window used to resample the calculated linear weighted moving average series. Defaults to '60min'.
 
     Returns:
         pandas.Series: Smoothed time series.
     """
-    time_window = time_parse(time_window)
+    time_window_ = time_parse(time_window)
     lwma = np.zeros_like(data)
-    win_pts_lst = np.array(data.rolling(time_window).count().values.astype(int))
+    win_pts_lst = np.array(data.rolling(time_window_).count().values.astype(int))
 
     for i in range(len(data)):
         lwma[i] = get_lwma_val(data.values, win_pts_lst, i, min_periods=min_periods)
     lwma_series = pd.Series(lwma, index=data.index)
     if resample:
-        resample_window = time_parse(resample_window)
-        lwma_series = lwma_series.resample(resample_window).mean()
+        resample_window_ = time_parse(resample_window)
+        lwma_series = lwma_series.resample(resample_window_).mean()
     return lwma_series
 
 
 @jit(nopython=True)
 def get_lwma_val(data: np.ndarray, win_pts_lst: np.ndarray, i: int, min_periods: int) -> Optional[float]:
     """Calculates the Linear Weighted Moving Average for the current datapoint.
```

### Comparing `indsl-6.5.0/indsl/smooth/moving_averages.md` & `indsl-6.6.0a0/indsl/smooth/moving_averages.md`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/smooth/savitzky_golay.py` & `indsl-6.6.0a0/indsl/smooth/savitzky_golay.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright 2022 Cognite AS
 import pandas as pd
 
 from scipy.signal import savgol_filter
 
-from ..exceptions import UserValueError
+from indsl.exceptions import UserValueError
 
 # noinspection SpellCheckingInspection
-from ..type_check import check_types
+from indsl.type_check import check_types
 
 
 @check_types
 def sg(data: pd.Series, window_length: int = None, polyorder: int = 1) -> pd.Series:
     """Saviztky-Golay.
 
     Use this filter for smoothing data without distorting the data tendency. The method is independent of
```

### Comparing `indsl-6.5.0/indsl/smooth/simple_ma.py` & `indsl-6.6.0a0/indsl/smooth/simple_ma.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/smooth/simple_ma_v1.py` & `indsl-6.6.0a0/indsl/smooth/simple_ma_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,10 +22,10 @@
             If the user gives a number without unit (such as '60'), it will be considered as the number of minutes.
         min_periods: Minimum samples.
             Minimum number of observations in window required to have a value (otherwise result is NA). Defaults  to 1.
 
     Returns:
         pandas.Series: Smoothed time series
     """
-    time_window = time_parse(time_window, sma.__name__)
+    time_window_ = time_parse(time_window, sma.__name__)
 
-    return data.rolling(time_window, min_periods=min_periods).mean()
+    return data.rolling(time_window_, min_periods=min_periods).mean()
```

### Comparing `indsl-6.5.0/indsl/statistics/confidence.py` & `indsl-6.6.0a0/indsl/statistics/confidence.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/statistics/correlation.py` & `indsl-6.6.0a0/indsl/statistics/correlation.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/statistics/img/csaps_vs_scipy.png` & `indsl-6.6.0a0/indsl/statistics/img/csaps_vs_scipy.png`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/statistics/img/dbscan_principle.png` & `indsl-6.6.0a0/indsl/statistics/img/dbscan_principle.png`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/statistics/img/input_timeseries.png` & `indsl-6.6.0a0/indsl/statistics/img/input_timeseries.png`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/statistics/img/output_function.png` & `indsl-6.6.0a0/indsl/statistics/img/output_function.png`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/statistics/img/process_function.png` & `indsl-6.6.0a0/indsl/statistics/img/process_function.png`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/statistics/outliers.md` & `indsl-6.6.0a0/indsl/statistics/outliers.md`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/statistics/outliers.py` & `indsl-6.6.0a0/indsl/statistics/outliers.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/statistics/outliers_v1.py` & `indsl-6.6.0a0/indsl/statistics/outliers_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,21 +210,21 @@
         warnings.warn(
             f"Missing time unit in argument 'time_window' in remove_outliers function, assuming {time_window}min.",
             UserWarning,
         )
         time_window = str(time_window) + "min"
 
     try:
-        time_window = pd.Timedelta(time_window)
+        time_window_ = pd.Timedelta(time_window)
     except ValueError:
         raise UserValueError(
             f"Time window should be a string in weeks, days, hours or minutes format:'3w', '10d', '5h', '30min', '10s' not {time_window}."
         ) from None
 
-    df["rolling_mean"] = df["val"].rolling(time_window, min_periods=1).mean()  # calculate features
+    df["rolling_mean"] = df["val"].rolling(time_window_, min_periods=1).mean()  # calculate features
 
     if del_zero_val:  # delete 0 values if user requests it
         df = df[df["val"] != 0.0]
 
     df_dbscan = df[["val"]].copy()
 
     validate_series_is_not_empty(df_dbscan)
```

### Comparing `indsl-6.5.0/indsl/sustainability/co2_emissions_calculations.py` & `indsl-6.6.0a0/indsl/sustainability/co2_emissions_calculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     r"""Cumulative CO2 production.
 
     This function calculates the total CO2 production according to the rate of emissions. The total is calculated by performing trapezoidal integration
     over time (granularity of 1 hour). The rate of emissions is resampled to 1-hour granularity accordingly. If no start time is specified,
     it will default to the start of the current year.
 
     Args:
-        rate_of_emission: Rate of CO2 released over time [mass/time].
+        rate_of_emissions: Rate of CO2 released over time [mass/time].
         start_date: Start date to begin cumulative calculation.
 
     Returns:
         pandas.Series: Cumulative CO2 emissions
 
     """
     # Assign start_date to be start of year if not defined
```

### Comparing `indsl-6.5.0/indsl/ts_utils/__init__.py` & `indsl-6.6.0a0/indsl/ts_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/ts_utils/logarithmic_functions.py` & `indsl-6.6.0a0/indsl/ts_utils/logarithmic_functions.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/ts_utils/logical_operations.py` & `indsl-6.6.0a0/indsl/ts_utils/logical_operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Copyright 2022 Cognite AS
-from typing import Literal, Union
+from typing import Union
 
 import pandas as pd
 
-from ..resample.auto_align import auto_align
-from ..type_check import check_types
+
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
+from indsl.resample.auto_align import auto_align
+from indsl.type_check import check_types
 
 
 @check_types
 def logical_check(
     value_1: Union[pd.Series, float],
     value_2: Union[pd.Series, float],
     value_true: Union[pd.Series, float],
@@ -30,16 +34,18 @@
         value_true: True - time series/number.
         value_false: False - time series/number.
         operation: Logical operation.
 
     Returns:
         Union[pd.Series, Number]: Time series/number.
     """
-    # Select operation
-    def check_function(a: Union[pd.Series, float, int], b: Union[pd.Series, float, int]) -> Union[pd.Series, bool]:
+
+    def check_function(
+        a: Union[pd.Series, float, int], b: Union[pd.Series, float, int]
+    ) -> Union[pd.Series, bool]:  # Select operation
         if operation == "Equality":
             return a == b
         elif operation == "Inequality":
             return a != b
         elif operation == "Greater than":
             return a > b
         elif operation == "Greater or equal than":
```

### Comparing `indsl-6.5.0/indsl/ts_utils/numerical_calculus.py` & `indsl-6.6.0a0/indsl/ts_utils/numerical_calculus.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/ts_utils/numerical_calculus_v1.py` & `indsl-6.6.0a0/indsl/ts_utils/numerical_calculus_v1.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/ts_utils/operators.py` & `indsl-6.6.0a0/indsl/ts_utils/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from typing import List, Union
 
 import numpy as np
 
 # Simple operations
 import pandas as pd
 
+from indsl.exceptions import UserValueError
 from indsl.resample.auto_align import auto_align
 from indsl.type_check import check_types
 
-from ..exceptions import UserValueError
-
 
 @check_types
 def add(a, b, align_timesteps: bool = False):
     """Add.
 
     Add any two time series or numbers.
```

### Comparing `indsl-6.5.0/indsl/ts_utils/trigonometric_functions.py` & `indsl-6.6.0a0/indsl/ts_utils/trigonometric_functions.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/ts_utils/ts_utils.py` & `indsl-6.6.0a0/indsl/ts_utils/ts_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # Copyright 2022 Cognite AS
 import re
 import warnings
 
 from datetime import datetime
-from typing import Callable, List, Literal, Optional, Union
+from typing import Callable, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 import scipy.integrate
 
-from indsl.type_check import check_types
 
-from ..exceptions import UserRuntimeError, UserValueError
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
+
+from indsl.exceptions import UserRuntimeError, UserValueError
+from indsl.type_check import check_types
 
 
 _unit_in_ms_without_week = {"s": 1000, "m": 60000, "h": 3600000, "d": 86400000}
 _unit_in_ms = {**_unit_in_ms_without_week, "w": 604800000}
 
 
 def datetime_to_ms(dt):
@@ -255,14 +258,15 @@
 def make_uniform(data: pd.DataFrame, resolution: str = "1s", interpolation: str = None) -> pd.DataFrame:
     """Make time series uniform.
 
     Convenience method to make an input time series dataframe uniform per specified temporal resolution.
     Object must have a datetime-like index.
 
     Args:
+        data: Input time series dataframe.
         resolution: Temporal resolution of uniform time series. Follows Pandas DateTime convention. Defaults to "1s".
         interpolation: Method for optional interpolation. Follows pandas Resampler.interpolate. Defaults to None.
 
     Returns:
         pandas.DataFrame: Uniform Timeseries DataFrame.
     """
     # If no interpolation specified, do not perform interpolation
```

### Comparing `indsl-6.5.0/indsl/ts_utils/utility_functions.py` & `indsl-6.6.0a0/indsl/ts_utils/utility_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright 2022 Cognite AS
 
 from datetime import datetime, timedelta
-from typing import List, Literal, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from scipy.stats import shapiro
 
-from indsl.resample.auto_align import auto_align
+# todo: use Literal from typing instead of typing_extensions when the fix for this issue has been released: https://github.com/agronholm/typeguard/issues/363
+from typing_extensions import Literal
 
-from ..exceptions import UserValueError
-from ..type_check import check_types
+from indsl.exceptions import UserTypeError, UserValueError
+from indsl.resample.auto_align import auto_align
+from indsl.type_check import check_types
 
 
 TimeUnits = Literal["ns", "us", "ms", "s", "m", "h", "D", "W"]
 
 
 # Rounding and utility functions
 @check_types
@@ -275,28 +277,32 @@
     by using nan, inf and -inf (e.g. 1.0, 5, inf, -inf, 20, nan).
 
     Args:
         series: Time series
         to_replace: Replace
             List of values to replace. The values must be seperated by semicolons. Infinity and undefined values can be
             replaced by using the keywords inf, -inf and nan. The default is to replace no values.
-        value: By
-            Value used as replacement. Default is 0.0
+        value: Value used as replacement.
+            Default is 0.0
 
     Returns:
         pd.Series: time series
 
     Raises:
         UserTypeError: series is not a time series
         UserTypeError: to_replace is not a list
         UserTypeError: value is not a number
 
     """
     if to_replace is None:
         return series
+    elif not isinstance(to_replace, list):
+        raise UserTypeError("to_replace must be a list")
+    if value is not None and not isinstance(value, (float, int)):
+        raise UserTypeError("value must be a number")
     return series.replace(to_replace, value)
 
 
 @check_types
 def remove(
     series: pd.Series,
     to_remove: Optional[List[float]] = None,
@@ -320,14 +326,16 @@
     Returns:
         pd.Series: time series
 
     Raises:
         UserTypeError: series is not a time series
         UserTypeError: to_remove is not a list
     """
+    if to_remove is not None and not isinstance(to_remove, list):
+        raise UserTypeError("to_replace must be a list")
     if to_remove is not None:
         series = series[~series.isin(to_remove)]
     if range_from is not None:
         series = series[series >= range_from]
     if range_to is not None:
         series = series[series <= range_to]
     return series
@@ -448,15 +456,15 @@
         timestamps.append(timestamps[-1] + step)
     timestamps = pd.Series(timestamps)
     return pd.Series(np.zeros(len(timestamps)), index=timestamps)
 
 
 def normality_assumption_test(
     series: Union[pd.Series, np.array], max_data_points: int = 5000, min_p_value: float = 0.05, min_W: float = 0.5
-) -> Tuple[float, float]:
+) -> Optional[Tuple[float, float]]:
     """Test for normality assumption.
 
     This function performs a Shapiro-Wilk test to check if the data is normally distributed.
 
     Args:
         series: Time series
         max_data_points: Maximum number of data points.
@@ -481,15 +489,15 @@
     W, p_value = shapiro(series)
 
     if p_value == 1.0 and W == 1.0:
         raise UserValueError("This time series is uniform and not normally distributed")
     if p_value < min_p_value or W < min_W:
         raise UserValueError("This time series is not normally distributed")
 
-    return  # type: ignore
+    return None
 
 
 def z_scores_test(x: np.array, cutoff: float = 3.0, direction: Literal["greater", "less"] = "greater") -> np.array:
     """Z-scores test.
 
     This functions performs a z-scores test given a cut-off value and returns a binary time series.
```

### Comparing `indsl-6.5.0/indsl/type_check.py` & `indsl-6.6.0a0/indsl/type_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from functools import wraps
 
-from typeguard import typechecked
+from typeguard import TypeCheckError, typechecked
 
 from indsl.exceptions import UserTypeError
 
 
 def error_handling(operation):
     """Decorator that catches TypeError and wraps to inDSL specific error."""
 
     @wraps(operation)
     def wrapper(*args, **kwargs):
         try:
             return operation(*args, **kwargs)
-        except TypeError as e:
+        except TypeCheckError as e:
             raise UserTypeError(str(e)) from e
 
     return wrapper
 
 
 def check_types(operation):
     """Decorator to check types of inputs and outputs of a function.
```

### Comparing `indsl-6.5.0/indsl/validations.py` & `indsl-6.6.0a0/indsl/validations.py`

 * *Files identical despite different names*

### Comparing `indsl-6.5.0/indsl/versioning.py` & `indsl-6.6.0a0/indsl/versioning.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,18 +56,18 @@
         key = name or func.__name__
 
         if version in _registered_funcs[key]:
             raise ValueError(f"Function {key} with version {version} is already registered")
 
         _registered_funcs[key][version] = func
 
-        func.__versioning_version__ = version  # type: ignore
-        func.__versioning_name__ = key  # type: ignore
-        func.__versioning_deprecated__ = deprecated  # type: ignore
-        func.__versioning_changelog__ = changelog  # type: ignore
+        setattr(func, "__versioning_version__", version)
+        setattr(func, "__versioning_name__", key)
+        setattr(func, "__versioning_deprecated__", deprecated)
+        setattr(func, "__versioning_changelog__", changelog)
 
         return func
 
     return register_decorator
 
 
 def get_registered_functions() -> List[str]:
@@ -85,59 +85,50 @@
     return sorted(versions, key=Version)
 
 
 @check_types
 def get_name(func: Callable[..., Any]) -> str:
     """Return the name with which the function was registered."""
     try:
-        return func.__versioning_name__  # type: ignore
+        return getattr(func, "__versioning_name__")
     except AttributeError:
         raise ValueError("Cannot get name of an un-registerd function")
 
 
 @check_types
 def get_version(func: Callable[..., Any]) -> Optional[str]:
     """Return the version of a function.
 
     If the function is not registered, None is returned
     """
-    try:
-        return func.__versioning_version__  # type: ignore
-    except AttributeError:
-        return None
+    return getattr(func, "__versioning_version__", None)
 
 
 @check_types
 def is_versioned(func: Callable[..., Any]) -> bool:
     """Return true if the version is versioned."""
     return hasattr(func, "__versioning_version__")
 
 
 @check_types
 def is_deprecated(func: Callable[..., Any]) -> Optional[bool]:
     """Return true if the version is deprecated.
 
     If the function is not registered, None is returned
     """
-    try:
-        return func.__versioning_deprecated__  # type: ignore
-    except AttributeError:
-        return None
+    return getattr(func, "__versioning_deprecated__", None)
 
 
 @check_types
 def get_changelog(func: Callable[..., Any]) -> Optional[str]:
     """Return changelog of this version.
 
     If the function is not registered, None is returned
     """
-    try:
-        return func.__versioning_changelog__  # type: ignore
-    except AttributeError:
-        return None
+    return getattr(func, "__versioning_changelog__", None)
 
 
 @check_types
 def get(name: str, version: Optional[str] = None) -> Callable[..., Any]:
     """Return one of the versions of a function.
 
     If version is None, the latest version is returned
```

### Comparing `indsl-6.5.0/PKG-INFO` & `indsl-6.6.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: indsl
-Version: 6.5.0
+Version: 6.6.0a0
 Summary: Industrial Data Science Library by Cognite
 Home-page: https://indsl.docs.cognite.com
 License: Apache-2.0
 Author: Cognite
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: PyWavelets (>=1.2.0,<2.0.0)
 Requires-Dist: csaps (>=1.1.0,<2.0.0)
-Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0)
 Requires-Dist: fluids (>=1.0.22,<2.0.0)
 Requires-Dist: kneed (>=0.8.0,<0.9.0)
-Requires-Dist: numba (>=0.56.0,<0.57.0)
-Requires-Dist: numpy (<1.23.0)
+Requires-Dist: numba (>=0.57.0,<0.58.0)
+Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
-Requires-Dist: pandas (>=1.3.5,<2.0.0)
-Requires-Dist: pytest (>=6.2.2,<8.0.0)
-Requires-Dist: scikit-image (>=0.19.0,<0.20.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
 Requires-Dist: scikit-learn (>=1.1.3,<2.0.0)
 Requires-Dist: scipy (>=1.7.3,<2.0.0)
-Requires-Dist: statsmodels (>=0.13.1,<0.14.0)
+Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typeguard (>=2.13.3,<3.0.0)
+Requires-Dist: typeguard (>=4.0.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Project-URL: Documentation, https://indsl.docs.cognite.com
 Project-URL: Repository, https://github.com/cognitedata/indsl
 Description-Content-Type: text/markdown
 
 [![Downloads](https://static.pepy.tech/personalized-badge/indsl?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=PyPi%20Downloads)](https://pepy.tech/project/indsl) [![Code Quality](https://github.com/cognitedata/indsl/actions/workflows/code-quality.yaml/badge.svg)](https://github.com/cognitedata/indsl/actions/workflows/code-quality.yaml) [![CodeQL](https://github.com/cognitedata/indsl/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/cognitedata/indsl/actions/workflows/codeql-analysis.yml) [![codecov](https://codecov.io/gh/cognitedata/indsl/branch/master/graph/badge.svg?token=N63jUovh1o)](https://codecov.io/gh/cognitedata/indsl)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: indsl Version: 6.5.0 Summary: Industrial Data
+Metadata-Version: 2.1 Name: indsl Version: 6.6.0a0 Summary: Industrial Data
 Science Library by Cognite Home-page: https://indsl.docs.cognite.com License:
-Apache-2.0 Author: Cognite Requires-Python: >=3.8,<3.11 Classifier: License ::
+Apache-2.0 Author: Cognite Requires-Python: >=3.8,<3.12 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Scientific/Engineering Requires-Dist:
-PyWavelets (>=1.2.0,<2.0.0) Requires-Dist: csaps (>=1.1.0,<2.0.0) Requires-
-Dist: flake8-docstrings (>=1.6.0,<2.0.0) Requires-Dist: fluids
-(>=1.0.22,<2.0.0) Requires-Dist: kneed (>=0.8.0,<0.9.0) Requires-Dist: numba
-(>=0.56.0,<0.57.0) Requires-Dist: numpy (<1.23.0) Requires-Dist: packaging
-(>=23.0,<24.0) Requires-Dist: pandas (>=1.3.5,<2.0.0) Requires-Dist: pytest
-(>=6.2.2,<8.0.0) Requires-Dist: scikit-image (>=0.19.0,<0.20.0) Requires-Dist:
-scikit-learn (>=1.1.3,<2.0.0) Requires-Dist: scipy (>=1.7.3,<2.0.0) Requires-
-Dist: statsmodels (>=0.13.1,<0.14.0) Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typeguard (>=2.13.3,<3.0.0) Project-URL: Documentation, https://
-indsl.docs.cognite.com Project-URL: Repository, https://github.com/cognitedata/
-indsl Description-Content-Type: text/markdown [![Downloads](https://
-static.pepy.tech/personalized-badge/
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Scientific/Engineering Requires-Dist: PyWavelets (>=1.2.0,<2.0.0)
+Requires-Dist: csaps (>=1.1.0,<2.0.0) Requires-Dist: fluids (>=1.0.22,<2.0.0)
+Requires-Dist: kneed (>=0.8.0,<0.9.0) Requires-Dist: numba (>=0.57.0,<0.58.0)
+Requires-Dist: numpy (>=1.24.0,<2.0.0) Requires-Dist: packaging (>=23.0,<24.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0) Requires-Dist: scikit-image
+(>=0.21.0,<0.22.0) Requires-Dist: scikit-learn (>=1.1.3,<2.0.0) Requires-Dist:
+scipy (>=1.7.3,<2.0.0) Requires-Dist: statsmodels (>=0.14.0,<0.15.0) Requires-
+Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: typeguard (>=4.0.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.6.3,<5.0.0) Project-URL: Documentation,
+https://indsl.docs.cognite.com Project-URL: Repository, https://github.com/
+cognitedata/indsl Description-Content-Type: text/markdown [![Downloads](https:/
+/static.pepy.tech/personalized-badge/
 indsl?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=PyPi%20Downloads)]
 (https://pepy.tech/project/indsl) [![Code Quality](https://github.com/
 cognitedata/indsl/actions/workflows/code-quality.yaml/badge.svg)](https://
 github.com/cognitedata/indsl/actions/workflows/code-quality.yaml) [![CodeQL]
 (https://github.com/cognitedata/indsl/actions/workflows/codeql-analysis.yml/
 badge.svg)](https://github.com/cognitedata/indsl/actions/workflows/codeql-
 analysis.yml) [![codecov](https://codecov.io/gh/cognitedata/indsl/branch/
```

