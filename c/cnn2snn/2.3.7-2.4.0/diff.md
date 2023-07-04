# Comparing `tmp/cnn2snn-2.3.7.tar.gz` & `tmp/cnn2snn-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnn2snn-2.3.7.tar", last modified: Fri Jun  9 15:01:59 2023, max compression
+gzip compressed data, was "cnn2snn-2.4.0.tar", last modified: Tue Jul  4 09:05:43 2023, max compression
```

## Comparing `cnn2snn-2.3.7.tar` & `cnn2snn-2.4.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.623969 cnn2snn-2.3.7/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      520 2023-06-09 15:01:59.623969 cnn2snn-2.3.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      252 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.619969 cnn2snn-2.3.7/cnn2snn/
--rw-r--r--   0 root         (0) root         (0)     1483 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/akida_versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.619969 cnn2snn-2.3.7/cnn2snn/calibration/
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/calibration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16847 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/calibration/adaround.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/calibration/bias_correction.py
--rw-r--r--   0 root         (0) root         (0)    12381 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/calibration/calibration.py
--rw-r--r--   0 root         (0) root         (0)    10739 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/cli.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/cnn2snn_objects.py
--rw-r--r--   0 root         (0) root         (0)    12382 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)    13936 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/converter.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/min_value_constraint.py
--rw-r--r--   0 root         (0) root         (0)    14077 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/model_generator.py
--rw-r--r--   0 root         (0) root         (0)    13749 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantization.py
--rw-r--r--   0 root         (0) root         (0)    26028 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantization_layers.py
--rw-r--r--   0 root         (0) root         (0)    12977 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantization_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.623969 cnn2snn-2.3.7/cnn2snn/quantizeml/
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3962 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/activations.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/add.py
--rw-r--r--   0 root         (0) root         (0)     4489 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/attention.py
--rw-r--r--   0 root         (0) root         (0)     5283 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/batchnorm.py
--rw-r--r--   0 root         (0) root         (0)     2924 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/block_converter.py
--rw-r--r--   0 root         (0) root         (0)     9312 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/blocks.py
--rw-r--r--   0 root         (0) root         (0)    14915 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/concatenate.py
--rw-r--r--   0 root         (0) root         (0)     6579 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/convolution.py
--rw-r--r--   0 root         (0) root         (0)    11957 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/dense.py
--rw-r--r--   0 root         (0) root         (0)     6272 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/depthwise_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     6348 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/dequantizer.py
--rw-r--r--   0 root         (0) root         (0)     2872 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/extract_token.py
--rw-r--r--   0 root         (0) root         (0)     3442 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/input_data.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/layer_utils.py
--rw-r--r--   0 root         (0) root         (0)     4981 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/madnorm.py
--rw-r--r--   0 root         (0) root         (0)     6214 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/model_generator.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/outputs.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/padding.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/pooling.py
--rw-r--r--   0 root         (0) root         (0)     5555 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/separable_convolution.py
--rw-r--r--   0 root         (0) root         (0)     3083 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/shiftmax.py
--rw-r--r--   0 root         (0) root         (0)     8660 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/stem.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/quantizeml/weights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.623969 cnn2snn-2.3.7/cnn2snn/transforms/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/batch_normalization.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/clone.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/equalization.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/reshape.py
--rw-r--r--   0 root         (0) root         (0)    14261 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/transforms/sequential.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/utils.py
--rw-r--r--   0 root         (0) root         (0)    11223 2023-06-09 15:01:57.000000 cnn2snn-2.3.7/cnn2snn/weights_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:59.619969 cnn2snn-2.3.7/cnn2snn.egg-info/
--rw-r--r--   0 root         (0) root         (0)      520 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1798 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 15:01:59.000000 cnn2snn-2.3.7/cnn2snn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 15:01:59.623969 cnn2snn-2.3.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2023-06-09 15:01:53.000000 cnn2snn-2.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:05:43.074613 cnn2snn-2.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      520 2023-07-04 09:05:43.074613 cnn2snn-2.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      252 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:05:43.070613 cnn2snn-2.4.0/cnn2snn/
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/akida_versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:05:43.070613 cnn2snn-2.4.0/cnn2snn/calibration/
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/calibration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17761 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/calibration/adaround.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/calibration/bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)    12381 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/calibration/calibration.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/cnn2snn_objects.py
+-rw-r--r--   0 root         (0) root         (0)    11297 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)    12731 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/converter.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/min_value_constraint.py
+-rw-r--r--   0 root         (0) root         (0)    14054 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)    13749 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    26014 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantization_layers.py
+-rw-r--r--   0 root         (0) root         (0)    12977 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantization_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:05:43.070613 cnn2snn-2.4.0/cnn2snn/quantizeml/
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/activations.py
+-rw-r--r--   0 root         (0) root         (0)     4085 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/add.py
+-rw-r--r--   0 root         (0) root         (0)     5200 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/attention.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/batchnorm.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/block_converter.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/blocks.py
+-rw-r--r--   0 root         (0) root         (0)     7708 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/concatenate.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)    14765 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/conv_common.py
+-rw-r--r--   0 root         (0) root         (0)     7628 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/convolution.py
+-rw-r--r--   0 root         (0) root         (0)    11871 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/dense.py
+-rw-r--r--   0 root         (0) root         (0)     6342 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/depthwise_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     5502 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/dequantizer.py
+-rw-r--r--   0 root         (0) root         (0)     4175 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/extract_token.py
+-rw-r--r--   0 root         (0) root         (0)     7207 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/input_conv.py
+-rw-r--r--   0 root         (0) root         (0)     3207 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/input_data.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/layer_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5662 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/madnorm.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/outputs.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/padding.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/pooling.py
+-rw-r--r--   0 root         (0) root         (0)     6312 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/separable_convolution.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/shiftmax.py
+-rw-r--r--   0 root         (0) root         (0)     8571 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/stem.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/quantizeml/weights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:05:43.074613 cnn2snn-2.4.0/cnn2snn/transforms/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/transforms/batch_normalization.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/transforms/clone.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/transforms/equalization.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/transforms/reshape.py
+-rw-r--r--   0 root         (0) root         (0)    14261 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/transforms/sequential.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11223 2023-07-04 09:05:40.000000 cnn2snn-2.4.0/cnn2snn/weights_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:05:43.070613 cnn2snn-2.4.0/cnn2snn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-07-04 09:05:43.000000 cnn2snn-2.4.0/cnn2snn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-07-04 09:05:43.000000 cnn2snn-2.4.0/cnn2snn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 09:05:43.000000 cnn2snn-2.4.0/cnn2snn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-04 09:05:43.000000 cnn2snn-2.4.0/cnn2snn.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-04 09:05:43.000000 cnn2snn-2.4.0/cnn2snn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-04 09:05:43.000000 cnn2snn-2.4.0/cnn2snn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 09:05:43.074613 cnn2snn-2.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-07-04 09:05:38.000000 cnn2snn-2.4.0/setup.py
```

### Comparing `cnn2snn-2.3.7/LICENSE` & `cnn2snn-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/PKG-INFO` & `cnn2snn-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.3.7
+Version: 2.4.0
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Alvaro Moran
 Author-email: amoran@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnn2snn-2.3.7/cnn2snn/__init__.py` & `cnn2snn-2.4.0/cnn2snn/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/akida_versions.py` & `cnn2snn-2.4.0/cnn2snn/akida_versions.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/calibration/__init__.py` & `cnn2snn-2.4.0/cnn2snn/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/calibration/adaround.py` & `cnn2snn-2.4.0/cnn2snn/calibration/adaround.py`

 * *Files 7% similar despite different names*

```diff
@@ -174,46 +174,57 @@
             :obj:`tensorflow.Tensor`: a Tensor of quantized weights.
         """
         if self.training:
             return self.recons_weights()
         return self.quantizer.quantize(self.recons_weights())
 
 
-def initialize_training(layer):
-    """Prepare target layer for Adaround optimization
+def initialize_training(optimizer, model):
+    """Prepare target model for Adaround optimization
 
     The original quantizers are replaced by AdaRound quantizers
 
     Args:
-        layer (:obj:`keras.layers.Layer`): the layer to optimize
+        optimizer (:obj:`tensorflow.keras.optimizers.Optimizer`): an optimizer
+        model (:obj:`keras.models.Model`): a quantized Keras Model
 
     Returns:
-        [`AdaRoundQuantizer`], [`tf.Variable`]: a list of AdaRound quantizers and a list of
-        trainable variables
+        dict of [`AdaRoundQuantizer`], dict of [`tf.Variable`]: a list of AdaRound quantizers and
+        a list of trainable variables, grouped by layer
 
     """
-    # Replace standard quantizers by Adaround quantizers
-    adarounds = []
-    trainable_variables = []
-    if isinstance(layer, QuantizedSeparableConv2D):
-        w_list = layer.get_weights()
-        dw = w_list[0]
-        layer.quantizer_dw = AdaRoundQuantizer(layer.quantizer_dw, dw)
-        adarounds.append(layer.quantizer_dw)
-        trainable_variables.append(layer.quantizer_dw.alpha)
-        pw = w_list[1]
-        layer.quantizer = AdaRoundQuantizer(layer.quantizer, pw)
-        adarounds.append(layer.quantizer)
-        trainable_variables.append(layer.quantizer.alpha)
-    elif isinstance(layer, (QuantizedDense, QuantizedConv2D)):
-        w_list = layer.get_weights()
-        w = w_list[0]
-        layer.quantizer = AdaRoundQuantizer(layer.quantizer, w)
-        adarounds.append(layer.quantizer)
-        trainable_variables.append(layer.quantizer.alpha)
+    adarounds = {}
+    trainable_variables = {}
+    for layer in model.layers:
+        if not is_quantized_neural(layer):
+            continue
+        # Replace standard quantizers by Adaround quantizers
+        adarounds[layer] = []
+        trainable_variables[layer] = []
+        if isinstance(layer, QuantizedSeparableConv2D):
+            w_list = layer.get_weights()
+            dw = w_list[0]
+            layer.quantizer_dw = AdaRoundQuantizer(layer.quantizer_dw, dw)
+            adarounds[layer].append(layer.quantizer_dw)
+            trainable_variables[layer].append(layer.quantizer_dw.alpha)
+            pw = w_list[1]
+            layer.quantizer = AdaRoundQuantizer(layer.quantizer, pw)
+            adarounds[layer].append(layer.quantizer)
+            trainable_variables[layer].append(layer.quantizer.alpha)
+        elif isinstance(layer, (QuantizedDense, QuantizedConv2D)):
+            w_list = layer.get_weights()
+            w = w_list[0]
+            layer.quantizer = AdaRoundQuantizer(layer.quantizer, w)
+            adarounds[layer].append(layer.quantizer)
+            trainable_variables[layer].append(layer.quantizer.alpha)
+    # Create all optimizer variables
+    all_trainable_variables = sum(trainable_variables.values(), [])
+    # Since TensorFlow 2.12, the optimizer must build the variables before use them.
+    if hasattr(optimizer, 'build'):
+        optimizer.build(all_trainable_variables)
     return adarounds, trainable_variables
 
 
 def finalize_training(layer):
     """Restore target layer after Adaround optimization
 
     The original quantizers are restored and the rounded weights are frozen.
@@ -299,15 +310,15 @@
         print(message)
     else:
         col, _ = shutil.get_terminal_size()
         print(f"{message:<{col}}", sep='', end='\r', flush=True)
 
 
 def optimize_rounding(model, samples, layer, optimizer, epochs, loss,
-                      batch_size, include_activation):
+                      batch_size, include_activation, adarounds, trainable_variables):
     """AdaRound main optimization method
 
     Optimize the AdaRound alpha variables using gradient descent to minimize
     the quantization error.
 
     Args:
         model (:obj:`keras.models.Model`): a quantized Keras Model
@@ -322,16 +333,14 @@
     """
     # Instantiate a sampler and select the target layer
     sampler = QuantizationSampler(model, samples, batch_size)
     sampler.select_layer(layer, include_activation)
     m = keras.metrics.MeanSquaredError()
     # Evaluate quantization error
     err_before = sampler.quantization_error(m)
-    # Prepare layer for training
-    adarounds, trainable_variables = initialize_training(layer)
     float_outputs = None
     # Training loop
     print_console("Optimizing {}:".format(layer.name))
     for e in range(epochs):
         # Evaluate rounding loss parameter
         beta = compute_beta(e, epochs)
         for i in range(sampler.n_batches):
@@ -426,13 +435,25 @@
           activation.
 
     Returns:
         :obj:`tf.Model`: a quantized Keras model whose weights have been
         optimized
     """
     adaround_model = clone_model_with_weights(model)
+    # Initialize all trainable variables
+    adarounds, trainable_variables = initialize_training(optimizer, adaround_model)
+
     for layer in adaround_model.layers:
         if is_quantized_neural(layer):
             # Optimize rounding
-            optimize_rounding(adaround_model, samples, layer, optimizer, epochs,
-                              loss, batch_size, include_activation)
+            optimize_rounding(
+                adaround_model,
+                samples,
+                layer,
+                optimizer,
+                epochs,
+                loss,
+                batch_size,
+                include_activation,
+                adarounds[layer],
+                trainable_variables[layer])
     return adaround_model
```

### Comparing `cnn2snn-2.3.7/cnn2snn/calibration/bias_correction.py` & `cnn2snn-2.4.0/cnn2snn/calibration/bias_correction.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/calibration/calibration.py` & `cnn2snn-2.4.0/cnn2snn/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/cli.py` & `cnn2snn-2.4.0/cnn2snn/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,21 +48,20 @@
         # Only keep the actual base name (group(2) contains the suffix)
         base_name = m.group(1)
     out_path = f"{base_name}_iq{iq}_wq{wq}_aq{aq}.h5"
     model_q.save(out_path, include_optimizer=False)
     print(f"Model successfully quantized and saved as {out_path}.")
 
 
-def convert_model(model_path, input_scaling, is_image):
+def convert_model(model_path, input_scaling):
     """Wrapper to convert model"""
     base_name = os.path.splitext(model_path)[0]
     q_model = load_quantized_model(model_path)
     ak_model = convert(q_model,
-                       input_scaling=input_scaling,
-                       input_is_image=is_image)
+                       input_scaling=input_scaling)
     out_path = f"{base_name}.fbz"
     ak_model.save(out_path)
     print(f"Model successfully converted and saved as {out_path}.")
 
 
 def reshape_model(model_path, input_height, input_width):
     """Wrapper to reshape model"""
@@ -158,18 +157,14 @@
                           default=None,
                           help="The scale factor applied on uint8 inputs.")
     c_parser.add_argument("-sh",
                           "--shift",
                           type=int,
                           default=None,
                           help="The shift applied on uint8 inputs.")
-    c_parser.add_argument("--no-image-input",
-                          action='store_true',
-                          default=False,
-                          help="If inputs are not 8-bit images")
     r_parser = sp.add_parser(
         "reshape",
         parents=[parent_parser],
         help="Reshape a (quantized) Keras model Input layer to a given size.")
     r_parser.add_argument("-ih",
                           "--input_height",
                           type=int,
@@ -231,15 +226,15 @@
                        args.activ_quantization, args.input_weight_quantization,
                        args.fold_BN)
     if args.action == "convert":
         if args.scale is None or args.shift is None:
             input_scaling = None
         else:
             input_scaling = (args.scale, args.shift)
-        convert_model(args.model, input_scaling, not args.no_image_input)
+        convert_model(args.model, input_scaling)
     if args.action == "reshape":
         reshape_model(args.model, args.input_height, args.input_width)
     if args.action == "calibrate":
         data = np.load(args.samples)
         lst = data.files
         samples_arr = data[lst[0]]
         for item in lst[1:]:
```

### Comparing `cnn2snn-2.3.7/cnn2snn/cnn2snn_objects.py` & `cnn2snn-2.4.0/cnn2snn/cnn2snn_objects.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/compatibility_checks.py` & `cnn2snn-2.4.0/cnn2snn/compatibility_checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,34 +21,29 @@
 from . import quantization_layers as qlayers
 
 neural_layers = (layers.Conv2D, layers.SeparableConv2D, layers.Dense,
                  qlayers.QuantizedConv2D, qlayers.QuantizedSeparableConv2D,
                  qlayers.QuantizedDense)
 
 
-def check_sequential_compatibility(model, input_is_image):
+def check_sequential_compatibility(model):
     """Checks compatibility of a Sequential Keras model.
 
     If an incompatibility is detected, an error is raised. This function can be
     applied on native Keras models and does not check quantization parameters.
 
     Args:
         model (:obj:`tf.keras.Model`): a Sequential Keras model.
-        input_is_image (bool): True if input is an image.
     """
 
     assert isinstance(model, Sequential)
 
     if len(model.layers) == 0:
         return
 
-    # Check if the first layer is a (Quantized)Conv2D if input_is_image=True
-    if input_is_image:
-        _check_first_layer_with_image_input(model)
-
     # The two following variables are used to know if there is an alternation
     # between a neural layer and an activation layer. For example, when we go
     # through a neural layer in the model, 'last_visited_neural_layer' must be
     # None. If not, it means that there is no activation layer between this
     # neural layer and the previous one. 'last_visited_neural_layer' is then set
     # to the current neural layer and 'last_visited_activation' is set to None.
     # A (sub)model must start with a neural layer.
@@ -82,36 +77,14 @@
             _check_unsupported_activation(model, i)
         else:
             raise RuntimeError(
                 f"Layer {layer.name} of type {layer.__class__.__name__} is not "
                 f"supported for Akida conversion")
 
 
-def _check_first_layer_with_image_input(model):
-    """Checks that the first neural layer of a model with input_is_image=True
-    is a Conv2D or QuantizedConv2D layer.
-
-    Args:
-        model (:obj:`tf.keras.Model`): a Sequential Keras (sub)model.
-    """
-
-    next_layer = 0
-    if isinstance(model.layers[next_layer], layers.Rescaling):
-        next_layer += 1
-
-    if (type(model.layers[next_layer]) not in (layers.Conv2D, qlayers.QuantizedConv2D)
-            or model.layers[next_layer].input_shape[-1] not in (1, 3)):
-        layer = model.layers[next_layer]
-        raise RuntimeError(
-            f"With input_is_image=True, first layer '{layer.name}' must be "
-            f"Conv2D and input shape must have 1 or 3 channels. Receives layer "
-            f"of type {layer.__class__.__name__} with {layer.input_shape[-1]} "
-            f"channels.")
-
-
 def _check_dense_shape(layer):
     """Asserts Dense layer is compatible for conversion.
     One check is performed here:
     - input shape must be (bs, N) or (bs, 1, 1, N) (bs is the batch size).
 
     Args:
         layer(:obj:`tf.keras.Layer`): the Dense or QuantizedDense layer to
```

### Comparing `cnn2snn-2.3.7/cnn2snn/converter.py` & `cnn2snn-2.4.0/cnn2snn/converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,67 +22,63 @@
 from .model_generator import generate_model as cnn2snn_generate_model
 from .quantizeml import generate_model as qml_generate_model
 
 from .transforms import sequentialize, syncretize
 from .compatibility_checks import check_sequential_compatibility
 
 
-def _sync_and_check_model(model, input_is_image):
+def _sync_and_check_model(model):
     # Make sure the model is sequential
     seq_model = sequentialize(model)
 
     # For now, we support only models with a single branch
     if not isinstance(seq_model, Sequential):
         raise RuntimeError(
             "The model contains more than one sequential branch.")
 
     # Transform model to prepare conversion: change the order of layers,
     # fold BN, freeze quantizers, remove useless layers.
     sync_model = syncretize(seq_model)
 
     # Check model compatibility
-    check_sequential_compatibility(sync_model, input_is_image)
+    check_sequential_compatibility(sync_model)
 
     return sync_model
 
 
-def convert(model, file_path=None, input_scaling=None, input_is_image=True):
+def convert(model, file_path=None, input_scaling=None):
     """Converts a Keras quantized model to an Akida one.
 
     This method is compatible with model quantized with :func:`cnn2snn.quantize`
     and :func:`quantizeml.quantize`. To check the difference between the two
     conversion processes check the methods _convert_cnn2snn and _convert_quantizeml
     below.
 
     Args:
         model (:obj:`tf.keras.Model`): a tf.keras model
         file_path (str, optional): destination for the akida model.
             (Default value = None)
         input_scaling (2 elements tuple, optional): value of the input scaling.
             (Default value = None)
-        input_is_image (bool, optional): True if input is an image (3-D 8-bit
-            input with 1 or 3 channels) followed by QuantizedConv2D. Akida model
-            input will be InputConvolutional. If False, Akida model input will
-            be InputData. (Default value = True)
 
     Returns:
         :obj:`akida.Model`: an Akida model.
     """
     if not tf.executing_eagerly():
         raise SystemError("Tensorflow eager execution is disabled. "
                           "It is required to convert Keras weights to Akida.")
 
     # Check if the model has been quantized with quantizeml by checking quantized layers type
     cnn2snn_model = not any("quantizeml" in str(type(layer)) for layer in model.layers)
 
     # Convert the model
     if cnn2snn_model:
-        ak_model = _convert_cnn2snn(model, input_scaling, input_is_image)
+        ak_model = _convert_cnn2snn(model, input_scaling)
     else:
-        ak_model = _convert_quantizeml(model, input_is_image)
+        ak_model = _convert_quantizeml(model)
 
     # Save model if file_path is given
     if file_path:
         # Create directories
         dir_name, base_name = os.path.split(file_path)
         if base_name:
             file_root, file_ext = os.path.splitext(base_name)
@@ -97,45 +93,44 @@
 
         save_path = os.path.join(dir_name, file_root + file_ext)
         ak_model.save(save_path)
 
     return ak_model
 
 
-def _convert_quantizeml(model, input_is_image):
+def _convert_quantizeml(model):
     """Converts a Keras quantized model with quantizeml to an Akida one.
 
     After quantizing a Keras model with :func:`quantizeml.quantize`, it can be
     converted to an Akida model.
 
     Args:
         model (:obj:`tf.keras.Model`): a tf.keras model
-        input_is_image (bool): True if input is an 8-bit unsigned tensors (like images).
 
     Returns:
         :obj:`akida.Model`: an Akida model.
 
     """
 
     # Generate Akida model with empty weights/thresholds for now
-    ak_model = qml_generate_model(model, input_is_image)
+    ak_model = qml_generate_model(model)
 
     return ak_model
 
 
-def _convert_cnn2snn(model, input_scaling=None, input_is_image=True):
+def _convert_cnn2snn(model, input_scaling=None):
     """Converts a Keras quantized model to an Akida one.
 
     After quantizing a Keras model with :func:`cnn2snn.quantize`, it can be
     converted to an Akida model. By default, the conversion expects that the
     Akida model takes 8-bit images as inputs. ``input_scaling`` defines how the
     images have been rescaled to be fed into the Keras model (see note below).
 
-    If inputs are spikes, you can set ``input_is_image=False``. In this case,
-    Akida inputs are then expected to be integers between 0 and 15.
+    If inputs are spikes, Akida inputs are then expected to be integers between
+    0 and 15.
 
     Note:
         The relationship between Keras and Akida inputs is defined as::
 
             input_akida = input_scaling[0] * input_keras + input_scaling[1].
 
         If a :class:`tf.keras.layers.Rescaling`
@@ -163,18 +158,14 @@
         >>> # Convert and directly save the Akida model to fbz file.
         >>> cnn2snn.convert(model_keras, 'model_akida.fbz')
 
     Args:
         model (:obj:`tf.keras.Model`): a tf.keras model
         input_scaling (2 elements tuple, optional): value of the input scaling.
             (Default value = None)
-        input_is_image (bool, optional): True if input is an image (3-D 8-bit
-            input with 1 or 3 channels) followed by QuantizedConv2D. Akida model
-            input will be InputConvolutional. If False, Akida model input will
-            be InputData. (Default value = True)
 
     Returns:
         :obj:`akida.Model`: an Akida model.
 
     Raises:
         ValueError: If ``input_scaling[0]`` is null or negative.
         ValueError: If a :class:`Rescaling` layer is present and
@@ -192,18 +183,18 @@
     input_scaling = rescaling_input_scaling or input_scaling or (1, 0)
 
     if input_scaling[0] <= 0:
         raise ValueError("The scale factor 'input_scaling[0]' must be strictly"
                          f" positive. Receives: input_scaling={input_scaling}")
 
     # Prepare model for conversion and check its compatibility
-    sync_model = _sync_and_check_model(model, input_is_image)
+    sync_model = _sync_and_check_model(model)
 
     # Generate Akida model with converted weights/thresholds
-    ak_model = cnn2snn_generate_model(sync_model, input_scaling, input_is_image)
+    ak_model = cnn2snn_generate_model(sync_model, input_scaling)
 
     return ak_model
 
 
 def _get_rescaling_layer_params(model):
     """Computes the new input scaling retrieved from the Keras
     `Rescaling` layer.
@@ -232,15 +223,15 @@
     Rescaling = tf.keras.layers.Rescaling
     for layer in model.layers[:2]:
         if isinstance(layer, Rescaling):
             return (1 / layer.scale, -layer.offset / layer.scale)
     return None
 
 
-def check_model_compatibility(model, input_is_image=True):
+def check_model_compatibility(model):
     r"""Checks if a Keras model is compatible for cnn2snn conversion.
 
     This function doesn't convert the Keras model to an Akida model
     but only checks if the model design is compatible.
 
     Note that this function doesn't check if the model is compatible with
     Akida hardware.
@@ -356,20 +347,16 @@
       before the activation
     - a Flatten layer can only be used before a Dense layer
     - an Activation layer other than ReLU can only be used in the last layer
 
 
     Args:
         model (:obj:`tf.keras.Model`): the model to check.
-        input_is_image (bool, optional): True if input is an image (8-bit input
-            with 1 or 3 channels) followed by QuantizedConv2D. Akida model
-            input will be InputConvolutional. If False, Akida model input will
-            be InputData. (Default value = True)
     """
     try:
-        _sync_and_check_model(model, input_is_image)
+        _sync_and_check_model(model)
         return True
     except RuntimeError as e:
         print(
             "The Keras quantized model is not compatible for a conversion "
             "to an Akida model:\n", str(e))
         return False
```

### Comparing `cnn2snn-2.3.7/cnn2snn/min_value_constraint.py` & `cnn2snn-2.4.0/cnn2snn/min_value_constraint.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/model_generator.py` & `cnn2snn-2.4.0/cnn2snn/model_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                                  int(layer.input_shape[3]))
     params['name'] = layer.name + "_input"
 
 
 def _parse_input_conv(layer, params, input_shift):
     if not isinstance(layer, qlayers.QuantizedConv2D):
         raise TypeError(f"First layer {layer.name} must be QuantizedConv2D "
-                        "when input_is_image=True. Received layer of type "
+                        "when model input shape is equal to 1 or 3. Received layer of type "
                         f"{layer.__class__.__name__}")
     params["input_shape"] = (int(layer.input_shape[1]),
                              int(layer.input_shape[2]),
                              int(layer.input_shape[3]))
     params["padding"] = _get_padding(layer.padding)
     params["kernel_size"] = (layer.kernel_size[0], layer.kernel_size[1])
     params["filters"] = int(layer.kernel.shape[3])
@@ -126,35 +126,34 @@
         layer_ak = SeparableConvolutional(**params)
     elif layer_type == LayerType.FullyConnected:
         layer_ak = FullyConnected(**params)
 
     return layer_ak
 
 
-def generate_model(model, input_scaling, input_is_image):
+def generate_model(model, input_scaling):
     """Generates an Akida model.
 
     This function creates an Akida model by parsing every Sequential branch of
     the input model: for each submodel, Akida layers are created sequentially
     and added to the Akida model.
 
     Args:
         model (:obj:`tf.keras.Model`): a Keras model to convert.
         input_scaling (2-element tuple): the input factor and shift.
-        input_is_image (bool): True if input is an image.
 
     Returns:
         :obj:`akida.Model`: the generated Akida model.
 
     """
 
     model_ak = Model()
     previous_layer_ak = None
 
-    if not input_is_image:
+    if model.input_shape[-1] not in (1, 3):
         # Handle first akida layer as InputData and add it to the model
         params = {}
         _parse_input_data(model, params)
         layer_ak = InputData(**params)
         model_ak.add(layer_ak)
         previous_layer_ak = layer_ak
 
@@ -285,16 +284,16 @@
 
 def _handle_input_conv_layer(model, input_scaling):
     """Parses the first conv layer to create the future InputConvolutional Akida
     layer.
 
     This function also returns the layer after the first conv layer, which is
     the starting point for parsing the rest of the model. Note that a Sequential
-    model with input_is_image=True (i.e. InputConvolutional) must start with a
-    QuantizedConv2D layer with an optional Rescaling layer before.
+    model with model input_shape last dim in (1, 3) (i.e. InputConvolutional) must
+    start with a QuantizedConv2D layer with an optional Rescaling layer before.
 
     Args:
         model (:obj:`tf.keras.Model`): the Sequential model to parse.
 
     Returns:
         :obj:`tf.keras.Layer`: the first QuantizedConv2D layer.
         dict: the parameters to create the future Akida layer.
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantization.py` & `cnn2snn-2.4.0/cnn2snn/quantization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/quantization_layers.py` & `cnn2snn-2.4.0/cnn2snn/quantization_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # ******************************************************************************
 """Quantized layers API: neural quantized layers and quantized activations"""
 
 # Tensorflow imports
 import tensorflow as tf
 from keras import backend as K
 from keras import layers
-from keras.utils.generic_utils import serialize_keras_object
+from keras.utils import serialize_keras_object
 from keras.utils import conv_utils
 from tensorflow.python.ops import nn
 from .quantization_ops import get as get_quantizer
 from .quantization_ops import ceil_through
 
 
 def _check_unsupported_args(kwargs, unsupported_args):
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantization_ops.py` & `cnn2snn-2.4.0/cnn2snn/quantization_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/activations.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/activations.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # limitations under the License.
 # ******************************************************************************
 """Functions to convert keras activation layers parameters and variables to akida.
 """
 import numpy as np
 from quantizeml.layers import QuantizedReLU, AlignedWeightQuantizer, OutputQuantizer
 from .weights import broadcast_and_set_variable
-from ..akida_versions import AkidaVersion, get_akida_version
 
 
 def v1_relu_checks(layer):
     """Additionnal checks on QuantizedReLU layers of akida v1 models.
 
     Args:
         layer (:obj:`tf.keras.Layer`): the QuantizedReLU layer to check.
@@ -59,43 +58,31 @@
 
     Args:
         layer_k (:obj:`tf.keras.Layer`): the QuantizedReLU layer to parse.
 
     Returns:
         dict: the corresponding akida parameters.
     """
-    assert isinstance(layer_k.max_value_quantizer, AlignedWeightQuantizer)
 
-    # Check if there is an output_quantizer
-    out_quantizer = getattr(layer_k, "out_quantizer", None)
-
-    if not out_quantizer:
-        return {'activation': True}
-
-    assert isinstance(out_quantizer, OutputQuantizer)
-    return {'activation': True, 'output_bits': out_quantizer.bitwidth}
+    return {'activation': True}
 
 
 def set_relu_variables(layer_ak, layer_k):
-    """Computes and sets the activation variables in an akida layer.
+    """Computes and sets the activation variables in an akida v2 layer.
 
     Args:
         layer_ak (:obj:`akida.Layer`): the targeted akida layer.
         layer_k (:obj:`quantizeml.QuantizedRelu`): the source QuantizedReLU layer.
     """
-    # Nothing to do in AkidaVersion.v1 : the values will be modified by
-    # :func:`set_output_v1_variables`.
-    # TODO: remove this checks once the conversion pipeline uses only BlockConverter
-    if get_akida_version() == AkidaVersion.v1:
-        return
 
     assert isinstance(layer_k, QuantizedReLU)
 
     variables_ak = layer_ak.variables
 
-    max_value_quantizer = layer_k.max_value_quantizer
-    assert isinstance(max_value_quantizer, AlignedWeightQuantizer)
-    max_value = max_value_quantizer.qweights.value.values.numpy().astype(np.int32)
-    max_value_shift = max_value_quantizer.shift.value.numpy().astype(np.uint8)
-    max_value_ak = (max_value >> max_value_shift).astype(np.uint8)
-    broadcast_and_set_variable(variables_ak, "max_value", max_value_ak)
-    broadcast_and_set_variable(variables_ak, "max_value_shift", max_value_shift)
+    if layer_k.max_value is not None:
+        max_value_quantizer = layer_k.max_value_quantizer
+        assert isinstance(max_value_quantizer, AlignedWeightQuantizer)
+        max_value = max_value_quantizer.qweights.value.values.numpy().astype(np.int32)
+        max_value_shift = max_value_quantizer.shift.value.numpy().astype(np.uint8)
+        max_value_ak = (max_value >> max_value_shift).astype(np.uint8)
+        broadcast_and_set_variable(variables_ak, "max_value", max_value_ak)
+        broadcast_and_set_variable(variables_ak, "max_value_shift", max_value_shift)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/add.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/add.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,83 +12,104 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """Functions to convert QuantizedAdd to Akida.
 """
-from akida import LayerType, Add
+from akida import Add
 import quantizeml.layers as qlayers
 import numpy as np
 
+from ..akida_versions import AkidaVersion
 from .layer_utils import get_inbound_layers
 from .weights import broadcast_and_set_variable
+from .block_converter import BlockConverter, register_conversion_patterns
+from .blocks import get_block_out_quantizer
+from .outputs import set_output_v2_variables, parse_output_bits
 
 
-def _set_add_variables(ak_layer, k_layer):
+__all__ = ["AddBlockConverter"]
+
+_PATTERNS = [(qlayers.QuantizedAdd,)]
+
+
+def _set_add_variables(ak_layer, block):
     """Computes and sets the variables for an Akida Add layer.
 
     This function converts the variables of a Keras layer and sets them into
     the corresponding variables of the equivalent Akida layer.
 
     Args:
         ak_layer (:obj:`akida.Layer`): the targeted akida layer.
-        k_layer (:obj:`tf.keras.Layer`): the source quantized layer.
+        block (list(:obj:`tf.keras.Layer`)): the block of keras layers.
     """
-    assert isinstance(k_layer, qlayers.QuantizedAdd)
-    assert ak_layer.parameters.layer_type == LayerType.Add
+    add_layer = block[0]
 
     variables_ak = ak_layer.variables
-
-    a_shift = k_layer.a_shift.value.numpy().astype(np.uint8)
+    a_shift = add_layer.a_shift.value.numpy().astype(np.uint8)
     broadcast_and_set_variable(variables_ak, "a_shift", a_shift)
-    b_shift = k_layer.b_shift.value.numpy().astype(np.uint8)
+    b_shift = add_layer.b_shift.value.numpy().astype(np.uint8)
     broadcast_and_set_variable(variables_ak, "b_shift", b_shift)
 
-    out_quantizer = getattr(k_layer, "out_quantizer", False)
+    out_quantizer = get_block_out_quantizer(block)
     if out_quantizer:
-        assert isinstance(out_quantizer, qlayers.OutputQuantizer)
-        out_shift = out_quantizer.shift.value.numpy().astype(np.int8)
-        variables_ak["output_shift"] = out_shift
+        set_output_v2_variables(ak_layer, out_quantizer)
 
 
-def _create_add(layer):
+def _create_add(block):
     """Parses a quantizeml QuantizedAdd layer and returns the corresponding
-    Akida Add layer.
+    Akida v2 Add layer.
 
     Args:
-        layer (:obj:`tf.keras.Layer`): the quantizeml QuantizedAdd layer to convert.
+        block (list(:obj:`tf.keras.Layer`)): list of quantizeml quantized layers.
 
     Returns:
         :obj:`akida.Add`: The created akida layer.
     """
-    assert isinstance(layer, qlayers.QuantizedAdd)
+    add_layer = block[0]
     # In quantizeml one reserves automaticaly one bit for the sign, but in akida
     # this is rather checked during the clipping operations.
-    buffer_bits = layer.buffer_bitwidth + 1
-    if getattr(layer, 'out_quantizer', False):
-        output_bits = layer.out_quantizer.bitwidth
-    else:
-        output_bits = buffer_bits
-    return Add(output_bits=output_bits,
-               buffer_bits=buffer_bits,
-               name=layer.name)
+    add_params = {"buffer_bits": add_layer.buffer_bitwidth + 1}
+    # parse the block output bits
+    parse_output_bits(block, add_params)
 
+    return Add(**add_params,
+               name=add_layer.name)
 
-def convert_quantized_add(model_ak, layer_k):
-    """Converts QuantizedAdd layer and its variables and adds it to the
-    Akida's model.
+
+def convert_quantized_add_block(model_ak, block):
+    """Converts QuantizedAdd layer block and its variables and adds it to the
+    Akida's v2 model.
 
     Args:
         model_ak (:obj:`akida.Model`): the Akida model where the model will be added.
-        layer_k (:obj:`tf.keras.Layer`): the quantizeml QuantizedAdd layer to convert.
+        block (list(:obj:`tf.keras.Layer`)): list of quantizeml quantized layers.
+
+    Returns:
+        bool: Returns True for a successful conversion.
     """
-    if not isinstance(layer_k, qlayers.QuantizedAdd):
-        raise TypeError(f"Layer {layer_k.name} was expected to be "
-                        "QuantizedAdd")
     # Retrieve the akida inbound layers
-    inbound_layers_ak = get_inbound_layers(model_ak, layer_k)
+    inbound_layers_ak = get_inbound_layers(model_ak, block[0])
     # Create and add layer to the akida model
-    layer_ak = _create_add(layer_k)
+    layer_ak = _create_add(block)
     model_ak.add(layer_ak, inbound_layers_ak)
     # Set the akida layer converted variables
-    _set_add_variables(layer_ak, layer_k)
+    _set_add_variables(layer_ak, block)
+    return True
+
+
+class AddBlockConverter(BlockConverter):
+    """Main class that should be used to check if the Add layer block is compatible to an
+    Akida v2 conversion and provides a method to convert it in an equivalent Akida
+    Add layer.
+
+    Args:
+        block (list): list of quantizeml quantized layers.
+    """
+
+    def convert(self, model_ak):
+        return convert_quantized_add_block(model_ak, self._block)
+
+
+# Register the valid add block pattern for Akida v2
+register_conversion_patterns(AkidaVersion.v2, _PATTERNS, AddBlockConverter)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/attention.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/batchnorm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,144 @@
 #!/usr/bin/env python
 # ******************************************************************************
-# Copyright 2022 Brainchip Holdings Ltd.
+# Copyright 2023 Brainchip Holdings Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
-"""Functions to convert QuantizedAttention to Akida.
+"""Functions to convert QuantizedBatchNormalization to Akida.
 """
-from akida import LayerType, Attention
-import quantizeml.layers as qlayers
+from akida import BatchNormalization
+from quantizeml.layers import (QuantizedBatchNormalization, QuantizedReLU,
+                               WeightQuantizer, AlignedWeightQuantizer)
 import numpy as np
 
 from .weights import broadcast_and_set_variable
+from .outputs import set_output_v2_variables, parse_output_bits
+from .activations import set_relu_variables
 from .layer_utils import get_inbound_layers
+from .block_converter import BlockConverter, register_conversion_patterns
+from ..akida_versions import AkidaVersion
+from .conv_common import get_layer_by_type
+from .blocks import get_block_out_quantizer
 
+__all__ = ["BatchNormBlockConverter"]
 
-def _set_attention_variables(ak_layer, k_layer):
-    """Computes and sets the variables for an Akida Attention layer.
+_PATTERNS = [(QuantizedBatchNormalization,),
+             (QuantizedBatchNormalization, QuantizedReLU)]
+
+
+def _set_batchnorm_variables(ak_layer, block):
+    """Computes and sets the variables for an Akida BatchNormalization layer.
 
     This function converts the variables of a Keras layer and sets them into
     the corresponding variables of the equivalent Akida layer.
 
     Args:
         ak_layer (:obj:`akida.Layer`): the targeted akida layer.
-        k_layer (:obj:`tf.keras.Layer`): the source quantized layer.
+        block (list(:obj:`tf.keras.Layer`)): the block of keras layers.
     """
-    assert isinstance(k_layer, qlayers.QuantizedAttention)
-    assert ak_layer.parameters.layer_type == LayerType.Attention
+    layer_bn = block[0]
+    assert isinstance(layer_bn.a_quantizer, WeightQuantizer)
+    assert isinstance(layer_bn.b_quantizer, AlignedWeightQuantizer)
+
+    # get the QuantizedBatchNormalization a, b and shift
+    a_ak = layer_bn.a_quantizer.qweights.value.values.numpy()
+    b_quantizer = layer_bn.b_quantizer
+    b = b_quantizer.qweights.value.values.numpy().astype(np.int32)
+    b_shift = b_quantizer.shift.value.numpy().astype(np.uint8)
+    b_ak = (b >> b_shift).astype(np.int8)
 
     variables_ak = ak_layer.variables
 
-    # Get the QuantizedAttention layer shifts
-    value_shift = k_layer.values_shift.value.numpy().astype(np.uint8)
-    broadcast_and_set_variable(variables_ak, "value_shift", value_shift)
-    shiftmax = k_layer.softmax_op
-    shiftmax_input_shift = shiftmax.input_shift.value.numpy()
-    if np.any(shiftmax_input_shift < 0):
-        raise RuntimeError(
-            f"Layer {k_layer.name} contains negative values for " +
-            "shiftmax_input_shift, that is not supported")
-    broadcast_and_set_variable(ak_layer.variables, "shiftmax_input_shift",
-                               shiftmax_input_shift.astype(np.uint8))
-    out_quantizer = getattr(k_layer, "out_quantizer", False)
+    input_shift = layer_bn.input_shift.value
+    if input_shift is not None:
+        broadcast_and_set_variable(variables_ak, "input_shift",
+                                   input_shift.numpy().astype(np.uint8))
+
+    variables_ak["a"] = a_ak.astype(np.int8)
+    variables_ak["b"] = b_ak
+    broadcast_and_set_variable(variables_ak, "b_shift", b_shift)
+
+    relu = get_layer_by_type(block, QuantizedReLU)
+    if relu:
+        set_relu_variables(ak_layer, relu)
+
+    out_quantizer = get_block_out_quantizer(block)
     if out_quantizer:
-        output_shift = out_quantizer.shift.value.numpy().astype(np.int8)
-        broadcast_and_set_variable(ak_layer.variables, "output_shift",
-                                   output_shift)
+        set_output_v2_variables(ak_layer, out_quantizer)
 
 
-def _create_attention(layer):
-    """Parses a quantizeml QuantizedAttention layer and returns the params to
-    create the corresponding Akida Attention layer.
+def _create_batchnorm(block):
+    """Parses a quantizeml QuantizedBatchNormalization layers block and returns the
+    corresponding Akida v2 BatchNormalization layer.
 
     Args:
-        layer (:obj:`tf.keras.Layer`): the quantizeml QuantizedAttention layer to convert.
+        block (list(:obj:`tf.keras.Layer`)): list of quantizeml quantized layers.
 
     Returns:
-        :obj:`akida.Attention`: The created akida layer.
+        :obj:`akida.BatchNormalization`: The created akida layer.
     """
-    assert isinstance(layer, qlayers.QuantizedAttention)
-
-    # Find out if there is a quantizer
-    out_quantizer = getattr(layer, "out_quantizer", False)
-    # In quantizeml one bit is reserved automatically for the sign, but in akida
-    # this is rather checked during the clipping operations.
-    buffer_bits = layer.buffer_bitwidth + 1
-    if out_quantizer:
-        output_bits = out_quantizer.bitwidth
-    else:
-        # Default to buffer bitwidth
-        output_bits = buffer_bits
-
-    # As with output_bits and buffer_bits, shiftmax_output_bits is set with one
-    # bit more.
-    shiftmax_output_bits = layer.softmax_op.exp_bitwidth + 1
-
-    return Attention(num_heads=layer.num_heads,
-                     output_bits=output_bits,
-                     buffer_bits=buffer_bits,
-                     shiftmax_output_bits=shiftmax_output_bits,
-                     name=layer.name)
-
-
-def convert_quantized_attention(model_ak, layer_k):
-    """Converts QuantizedAttention layer and its variables and adds it to the
-    Akida's model.
+    bn = block[0]
+    bn_params = {}
+    relu = get_layer_by_type(block, QuantizedReLU)
+    if relu:
+        bn_params['activation'] = True
+    # In quantizeml one bit is reserved for the sign in the buffer bitwidth
+    # variable, but in akida this value has to be added back to have the
+    # correct clipping.
+    bn_params['buffer_bits'] = bn.buffer_bitwidth + 1
+
+    # parse the block output bits
+    parse_output_bits(block, bn_params)
+
+    return BatchNormalization(**bn_params,
+                              name=bn.name)
+
+
+def convert_batchnorm_block(model_ak, block):
+    """Converts QuantizedBatchNormalization layer and its variables and adds
+    it to the Akida's model. If followed by QuantizedReLU, it will set its
+    variables too.
 
     Args:
-        model_ak (:obj:`akida.Model`): the Akida model where the model will be added.
-        layer_k (:obj:`tf.keras.Layer`): the quantizeml QuantizedAttention layer to convert.
+        model_ak (:obj:`akida.Model`): the Akida model where the model will be
+            added.
+        block (list(:obj:`tf.keras.Layer`)): list of quantizeml quantized layers.
+
+    Returns:
+        bool: Returns True for a successful conversion.
     """
+    layer_ak = _create_batchnorm(block)
     # Retrieve the akida inbound layers
-    inbound_layers_ak = get_inbound_layers(model_ak, layer_k)
-    if not isinstance(layer_k, qlayers.QuantizedAttention):
-        raise TypeError(f"Layer {layer_k.name} was expected to be "
-                        "QuantizedAttention")
-    layer_ak = _create_attention(layer_k)
+    inbound_layers_ak = get_inbound_layers(model_ak, block[0])
+    # Add the layer to the Akida model
     model_ak.add(layer_ak, inbound_layers_ak)
-    _set_attention_variables(layer_ak, layer_k)
+    # Set its variables
+    _set_batchnorm_variables(layer_ak, block)
+    return True
+
+
+class BatchNormBlockConverter(BlockConverter):
+    """Main class that should be used to check if the batch norm layer block is compatible to an
+    Akida v2 conversion and provides a method to convert it in an equivalent Akida
+    BatchNormalization layer.
+
+    Args:
+        block (list): list of quantizeml quantized layers.
+    """
+
+    def convert(self, model_ak):
+        return convert_batchnorm_block(model_ak, self._block)
+
+
+# Register the valid batch norm block pattern for Akida v2
+register_conversion_patterns(AkidaVersion.v2, _PATTERNS, BatchNormBlockConverter)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/batchnorm.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/attention.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,134 @@
 #!/usr/bin/env python
 # ******************************************************************************
-# Copyright 2023 Brainchip Holdings Ltd.
+# Copyright 2022 Brainchip Holdings Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
-"""Functions to convert QuantizedBatchNormalization to Akida.
+"""Functions to convert QuantizedAttention to Akida.
 """
-from akida import LayerType, BatchNormalization
-import quantizeml.layers as qlayers
+from akida import Attention
+from quantizeml.layers import QuantizedAttention
 import numpy as np
 
+from ..akida_versions import AkidaVersion
 from .weights import broadcast_and_set_variable
-from .outputs import set_output_v2_variables
-from .activations import parse_relu_v2, set_relu_variables
 from .layer_utils import get_inbound_layers
+from .block_converter import BlockConverter, register_conversion_patterns
+from .blocks import get_block_out_quantizer
+from .outputs import set_output_v2_variables, parse_output_bits
 
 
-def _set_batchnorm_variables(ak_layer, block):
-    """Computes and sets the variables for an Akida BatchNormalization layer.
+__all__ = ["AttentionBlockConverter"]
+
+_PATTERNS = [(QuantizedAttention,)]
+
+
+def _set_attention_variables(ak_layer, block):
+    """Computes and sets the variables for an Akida v2 Attention layer.
 
     This function converts the variables of a Keras layer and sets them into
     the corresponding variables of the equivalent Akida layer.
 
     Args:
         ak_layer (:obj:`akida.Layer`): the targeted akida layer.
         block (list(:obj:`tf.keras.Layer`)): the block of keras layers.
     """
-    layer_bn = block[0]
-    assert isinstance(layer_bn, qlayers.QuantizedBatchNormalization)
-    assert ak_layer.parameters.layer_type == LayerType.BatchNormalization
-    assert isinstance(layer_bn.a_quantizer, qlayers.WeightQuantizer)
-    assert isinstance(layer_bn.b_quantizer, qlayers.AlignedWeightQuantizer)
-
-    # get the QuantizedBatchNormalization a, b and shift
-    a_ak = layer_bn.a_quantizer.qweights.value.values.numpy()
-    b_quantizer = layer_bn.b_quantizer
-    b = b_quantizer.qweights.value.values.numpy().astype(np.int32)
-    b_shift = b_quantizer.shift.value.numpy().astype(np.uint8)
-    b_ak = (b >> b_shift).astype(np.int8)
-
+    attention_layer = block[0]
     variables_ak = ak_layer.variables
 
-    input_shift = layer_bn.input_shift.value
-    if input_shift is not None:
-        broadcast_and_set_variable(variables_ak, "input_shift",
-                                   input_shift.numpy().astype(np.uint8))
-
-    variables_ak["a"] = a_ak.astype(np.int8)
-    variables_ak["b"] = b_ak
-    broadcast_and_set_variable(variables_ak, "b_shift", b_shift)
-
-    out_quantizer = getattr(layer_bn, "out_quantizer", False)
-    if len(block) > 1:
-        relu_layer = block[1]
-        set_relu_variables(ak_layer, relu_layer)
-        # the effective output_quantizer should be the relu one
-        out_quantizer = getattr(relu_layer, "out_quantizer", False)
-
+    # Get the QuantizedAttention layer shifts
+    value_shift = attention_layer.values_shift.value.numpy().astype(np.uint8)
+    broadcast_and_set_variable(variables_ak, "value_shift", value_shift)
+    shiftmax = attention_layer.softmax_op
+    shiftmax_input_shift = shiftmax.input_shift.value.numpy()
+    broadcast_and_set_variable(ak_layer.variables, "shiftmax_input_shift",
+                               shiftmax_input_shift.astype(np.uint8))
+    out_quantizer = get_block_out_quantizer(block)
     if out_quantizer:
         set_output_v2_variables(ak_layer, out_quantizer)
 
 
-def _create_batchnorm(layer_block):
-    """Parses a quantizeml QuantizedBatchNormalization layer and returns the
-    params to create the corresponding Akida BatchNormalization layer.
+def _create_attention(block):
+    """Parses a quantizeml QuantizedAttention layer and returns the params to
+    create the corresponding Akida Attention layer.
 
     Args:
-        layer (:obj:`tf.keras.Layer`): the quantizeml
-            QuantizedBatchNormalization layer to convert.
+        block (list(:obj:`tf.keras.Layer`)): list of quantizeml quantized layers.
 
     Returns:
-        :obj:`akida.BatchNormalization`: The created akida layer.
+        :obj:`akida.Attention`: The created akida layer.
     """
-    layer = layer_block[0]
-    assert isinstance(layer, qlayers.QuantizedBatchNormalization)
-    act_params = {}
-    if len(layer_block) > 1:
-        act_params = parse_relu_v2(layer_block[1])
-    # In quantizeml one bit is reserved for the sign in the buffer bitwidth
-    # variable, but in akida this value has to be added back to have the
-    # correct clipping.
-    buffer_bits = layer.buffer_bitwidth + 1
-    # If there is no activation, find out output_bits
-    if not act_params:
-        out_quantizer = getattr(layer, "out_quantizer", False)
-        if out_quantizer:
-            act_params['output_bits'] = out_quantizer.bitwidth
-        else:
-            # Default to buffer bitwidth
-            act_params['output_bits'] = buffer_bits
-
-    return BatchNormalization(**act_params,
-                              buffer_bits=buffer_bits,
-                              name=layer.name)
-
-
-def convert_batchnorm_block(model_ak, layers):
-    """Converts QuantizedBatchNormalization layer and its variables and adds
-    it to the Akida's model. If followed by QuantizedReLU, it will set its
-    variables too.
+    attention_layer = block[0]
+    # In quantizeml one bit is reserved automatically for the sign, but in akida
+    # this is rather checked during the clipping operations.
+    block_params = {"buffer_bits": attention_layer.buffer_bitwidth + 1}
+
+    # parse the block output bits
+    parse_output_bits(block, block_params)
+
+    # As with output_bits and buffer_bits, shiftmax_output_bits is set with one
+    # bit more.
+    block_params['shiftmax_output_bits'] = attention_layer.softmax_op.exp_bitwidth + 1
+
+    block_params['num_heads'] = attention_layer.num_heads
+    return Attention(**block_params,
+                     name=attention_layer.name)
+
+
+def convert_quantized_attention(model_ak, block):
+    """Converts QuantizedAttention layer and its variables and adds it to the
+    Akida's model.
 
     Args:
-        model_ak (:obj:`akida.Model`): the Akida model where the model will be
-            added.
-        layers (list(:obj:`tf.keras.Layer`)): the remaining model layers to
-            convert.
+        model_ak (:obj:`akida.Model`): the Akida model where the model will be added.
+        block (list(:obj:`tf.keras.Layer`)): list of quantizeml quantized layers.
 
-    Return:
-        int: the number of converted layers.
+    Returns:
+        bool: Returns True for a successful conversion.
     """
-    if not layers or not isinstance(layers[0],
-                                    qlayers.QuantizedBatchNormalization):
-        return 0
-
-    block = [layers[0]]
-    if len(layers) > 1 and isinstance(layers[1], qlayers.QuantizedReLU):
-        block.append(layers[1])
-    layer_ak = _create_batchnorm(block)
-
+    layer_ak = _create_attention(block)
     # Retrieve the akida inbound layers
-    inbound_layers_ak = get_inbound_layers(model_ak, layers[0])
+    inbound_layers_ak = get_inbound_layers(model_ak, block[0])
     model_ak.add(layer_ak, inbound_layers_ak)
-    _set_batchnorm_variables(layer_ak, block)
-    return len(block)
+    _set_attention_variables(layer_ak, block)
+    return True
+
+
+class AttentionBlockConverter(BlockConverter):
+    """Main class that should be used to check if the attention layer block is compatible to an
+    Akida v2 conversion and provides a method to convert it in an equivalent Akida Attention layer.
+
+    Args:
+        block (list): list of quantizeml quantized layers.
+    """
+
+    def __init__(self, block):
+        super().__init__(block)
+        self._attention_additional_checks()
+
+    def _attention_additional_checks(self):
+        shiftmax = self._block[0].softmax_op
+        # if input_shift available, make sure it has no negative values
+        if shiftmax.input_shift.value:
+            shiftmax_input_shift = shiftmax.input_shift.value.numpy()
+            if np.any(shiftmax_input_shift < 0):
+                raise ValueError(
+                    f"Layer {self._block[0].name} contains negative values for " +
+                    "shiftmax_input_shift, that is not supported")
+
+    def convert(self, model_ak):
+        return convert_quantized_attention(model_ak, self._block)
+
+
+# Register the valid attention block pattern for Akida v2
+register_conversion_patterns(AkidaVersion.v2, _PATTERNS, AttentionBlockConverter)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/block_converter.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/block_converter.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/blocks.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/stem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,235 +1,209 @@
 #!/usr/bin/env python
 # ******************************************************************************
-# Copyright 2023 Brainchip Holdings Ltd.
+# Copyright 2022 Brainchip Holdings Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
-"""Utility function to convert block layers to akida.
+"""Functions to convert Stem block quantized layers to Akida.
+Those layers are:
+    - The Embedding layer
+    - The Reshape layer
+    - The ClassToken (+ the DistToken for distilled models) layer(s)
+    - The AddPosEmbedding layer
 """
-from quantizeml.layers import (QuantizedMaxPool2D,
-                               QuantizedGlobalAveragePooling2D,
-                               QuantizedReLU,
-                               QuantizedExtractToken,
-                               Dequantizer)
+from akida import LayerType, Stem
+from quantizeml.layers import (QuantizedConv2D, QuantizedReshape,
+                               QuantizedClassToken, QuantizedAddPositionEmbs, OutputQuantizer)
+import numpy as np
+from .blocks import get_block_out_quantizer
+from .outputs import set_output_v2_variables
+from .weights import broadcast_and_set_variables
+from .block_converter import BlockConverter, register_conversion_patterns
+from ..akida_versions import AkidaVersion
+
+_PATTERNS = [(QuantizedConv2D, QuantizedReshape, QuantizedClassToken, QuantizedAddPositionEmbs),
+             (QuantizedConv2D, QuantizedReshape, QuantizedAddPositionEmbs),
+             (QuantizedConv2D, QuantizedReshape, QuantizedClassToken, QuantizedClassToken,
+              QuantizedAddPositionEmbs)]
 
-from .pooling import parse_max_pooling, parse_global_average_pooling
-from .activations import parse_relu_v1, parse_relu_v2
-from ..akida_versions import AkidaVersion, get_akida_version
 
+def _get_cls_layers(block):
+    """Helper that returns the QuantizedClassToken layers of a stem block.
 
-def parse_block_additional_layers(layers, block_params):
-    """Parse block additional layers into the parameters of one.
+    Args:
+        block (list): the quantizeml quantized layers of the Stem to convert.
+
+    Returns:
+        list: Returns a list of the QuantizedClassToken layers of a stem block.
+    """
 
-    In Akida v1, we are able to manage this sequence of layers:
+    return [layer for layer in block if isinstance(layer, QuantizedClassToken)]
 
-    - QuantizedMaxPooling2D or QuantizedGlobalAveragePooling2D
-    - QuantizedReLU.
 
-    In v2, the possible sequences are:
+def _set_stem_variables(ak_layer, block):
+    """Computes and sets the variables for an Akida Stem layer.
 
-    - QuantizedMaxPooling2D
-    - QuantizedReLU
+    This function converts the variables of a Keras layers and sets them into
+    the corresponding variables of the equivalent Akida layer.
+
+    Args:
+        ak_layer (:obj:`akida.Layer`): the targeted akida layer.
+        block (list): list of the source quantized layers block.
+    """
+    assert ak_layer.parameters.layer_type == LayerType.Stem
 
-    or:
+    embedding_layer = block[0]
 
-    - QuantizedReLU
-    - QuantizedGlobalAveragePooling2D
+    # Get the optional QuantizedClassToken layer(s) and the QuantizedAddPositionEmbs layer
+    cls_layers = _get_cls_layers(block)
+    add_pos_emb_layer = block[-1]
+
+    # Prepare a dict for akida variables
+    variables_ak = {}
+
+    # get the Embedding weights
+    weights_ak = embedding_layer.weight_quantizer.qweights.value.fp.values.numpy()
+
+    # get the Embedding bias
+    bias_quantizer = embedding_layer.bias_quantizer
+    bias = bias_quantizer.qweights.value.values.numpy().astype(np.int32)
+    bias_shift = bias_quantizer.shift.value.numpy().astype(np.uint8)
+    bias_ak = (bias >> bias_shift).astype(np.int8)
+
+    if len(cls_layers) > 0:
+        tokens_ak = []
+        shifts_tokens_ak = []
+        for cls_layer in cls_layers:
+            # get the ClassToken layer token variable (aka cls member)
+            cls_quantizer = cls_layer.cls_quantizer
+            token = cls_quantizer.qweights.value.values.numpy().astype(np.int32)
+            token_shift = cls_quantizer.shift.value.numpy().astype(np.uint8)
+            token_ak = token >> token_shift
+            # Insert the token value at the first position. This allows us to match
+            # the model concatenation order.
+            tokens_ak.insert(0, np.squeeze(token_ak))
+            shifts_tokens_ak.insert(0, token_shift)
+        variables_ak["tokens"] = np.stack(tokens_ak)
+        variables_ak["tokens_shift"] = np.concatenate(shifts_tokens_ak)
+
+    # get the positional embedding matrix
+    pos_emb_quantizer = add_pos_emb_layer.pe_quantizer
+    pos_emb = pos_emb_quantizer.qweights.value.values.numpy().astype(np.int32)
+    pos_emb_shift = pos_emb_quantizer.shift.value.numpy().astype(np.uint8)
+    pos_emb_ak = pos_emb >> pos_emb_shift
+    variables_ak["pos_embedding"] = pos_emb_ak
+    # Get the QuantizedAddPositionEmbs layer shifts
+    variables_ak["pos_embs_shift"] = pos_emb_shift
+
+    variables_ak["weights"] = weights_ak.astype(np.int8)
+    variables_ak["bias"] = bias_ak
+    # Get the Embedding layer shifts
+    variables_ak["bias_shift"] = bias_shift.astype(np.uint8)
+
+    broadcast_and_set_variables(ak_layer, variables_ak)
+
+
+def _parse_stem_block_layers(block):
+    """Parses the quantizeml quantized additional layers of the Stem block and returns the
+    params to create the corresponding Akida Stem layer.
 
     Args:
-        layers (list(:obj:`tf.keras.Layer`)): the layers block.
-        block_params (dict): the current block parameters.
+        layers (list): the quantizeml quantized layers of the Stem to convert.
 
     Returns:
-        dict: additional layers found in the process, with layer type as key
+        dict: the corresponding akida parameters.
     """
-    # Identify the next layers
-    next_layers = {}
-    akida_version = get_akida_version()
-    if akida_version == AkidaVersion.v1:
-        layer_types = [QuantizedMaxPool2D, QuantizedGlobalAveragePooling2D, QuantizedReLU]
-    else:
-        layer_types = [QuantizedMaxPool2D, QuantizedReLU, QuantizedGlobalAveragePooling2D]
-    index = 1
-    while index < len(layers) and layer_types:
-        layer_type = layer_types.pop(0)
-        layer = layers[index]
-        if isinstance(layer, layer_type):
-            next_layers[layer_type] = layer
-            index += 1
-
-    relu_layer = next_layers.get(QuantizedReLU, None)
-    max_pool_layer = next_layers.get(QuantizedMaxPool2D, None)
-    global_average_pool_layer = next_layers.get(QuantizedGlobalAveragePooling2D, None)
-
-    if len(next_layers) == 1 and max_pool_layer:
-        raise RuntimeError("Unsupported configuration: a maxpool requires an activation.")
-
-    # Evaluate the neural layer parameters
-    neural_name = layers[0].name
-    if getattr(layers[0], "out_quantizer", False) and len(next_layers) > 0:
-        raise RuntimeError(f"{neural_name} layer is followed by a pool/activation layer."
-                           "It should not have an output_quantizer.")
-
-    if max_pool_layer:
-        pool_params = parse_max_pooling(max_pool_layer)
-        # Padding checked on check_compatibility_model()
-        block_params.update(pool_params)
-    if global_average_pool_layer:
-        pool_params = parse_global_average_pooling(global_average_pool_layer)
-        block_params.update(pool_params)
-    if relu_layer:
-        # TODO: Remove the dependence to the akida_version when the conv block conversion
-        # will be done with it proper ConvBlockConverter
-        if akida_version == AkidaVersion.v1:
-            act_params = parse_relu_v1(relu_layer)
-        else:
-            act_params = parse_relu_v2(relu_layer)
-        block_params.update(act_params)
-
-    return next_layers
-
-
-def split_model_into_blocks(model):
-    """Search into the model the sets of possible blocks and return them.
-
-    A set of layers are considered as block if:
-        1. There is only one output quantizer (in the last layer of the block)
-        2. There are no multi-inbound layers
-        3. There are no QuantizedExtractToken layers
+    # Extract neural layer of the block
+    embedding = block[0]
 
-    Layers with more than one inbound layer will be handled separately.
+    # Get the QuantizedClassToken layer(s)
+    cls_layers = _get_cls_layers(block)
+
+    # A block of layers always end with an OutputQuantizer. Extract it.
+    out_quantizer = get_block_out_quantizer(block)
+    assert isinstance(out_quantizer, OutputQuantizer)
+
+    return dict(input_shape=embedding.input_shape[1:],
+                filters=embedding.filters,
+                kernel_size=embedding.kernel_size[0],
+                buffer_bits=embedding.buffer_bitwidth + 1,
+                output_bits=out_quantizer.bitwidth,
+                num_non_patch_tokens=len(cls_layers),
+                name=embedding.name)
+
+
+def convert_quantized_stem_layers(model_ak, block):
+    """Converts stem block layers and their variables and adds them to the
+    Akida's model.
 
     Args:
-        model (:obj:`tf.models.Model`): The model to split
+        model_ak (:obj:`akida.Model`): the Akida model where the model will be added.
+        block (list): the quantizeml quantized layers of the Stem to convert.
 
     Returns:
-        list: a list of sequences of layers ('blocks').
+        bool: Returns True for a successful conversion.
     """
-    def _get_inbound_layers(target_layer):
-        inbound = target_layer.inbound_nodes[0].inbound_layers
-        return inbound if isinstance(inbound, (list, tuple)) else [inbound]
-
-    def _check_single_layer_block(target_layer):
-        # Single blocks will be multi-inputs and QuantizedExtractToken
-        prev_layers = _get_inbound_layers(target_layer)
-        if len(prev_layers) > 1:
-            return True
-        if isinstance(target_layer, QuantizedExtractToken):
-            return True
-        return False
-
-    def _search_block_v1(target_layer):
-        # We consider the target is part of one block if there are previous
-        # layers. (Akida v1 doesn't support multi inbound layers)
-        prev_layers = _get_inbound_layers(target_layer)
-        # If it's the first layer return it
-        if len(prev_layers) == 0:
-            return [target_layer]
-
-        # If previous layer has an output quantizer, the blocks end here.
-        next_target = prev_layers[0]
-        out_quantizer = getattr(next_target, "out_quantizer", None)
-        if out_quantizer:
-            if not isinstance(next_target, QuantizedReLU):
-                raise RuntimeError("Model incompatible with akida v1 version. The layer"
-                                   f" {next_target.name} followed by {target_layer.name}"
-                                   " is not valid.")
-            return [target_layer]
-
-        # Otherwise, we continue searching...
-        return _search_block_v1(next_target) + [target_layer]
-
-    def _search_block_v2(target_layer):
-        # We consider the target is part of one block if there are previous
-        # layers (target is not the model's input), or it's multi-inbound.
-        prev_layers = _get_inbound_layers(target_layer)
-        if len(prev_layers) != 1:
-            return [target_layer]
-        # If previous layer has an output quantizer, the blocks end here.
-        next_target = prev_layers[0]
-        out_quantizer = getattr(next_target, "out_quantizer", None)
-        if out_quantizer or _check_single_layer_block(next_target):
-            return [target_layer]
-
-        # Otherwise, we continue searching...
-        return _search_block_v2(next_target) + [target_layer]
-
-    def _search_block(layer):
-        return _search_block_v1(layer) if get_akida_version() == AkidaVersion.v1 \
-            else _search_block_v2(layer)
-
-    def _get_layers_before_dequantizer(model):
-        # Return layers before the first dequantizer
-        layers = []
-        last_deq_layer = None
-        for layer in model.layers:
-            if isinstance(layer, Dequantizer):
-                last_deq_layer = layer
-                break
-            layers.append(layer)
-        return last_deq_layer, layers
-
-    def _is_end_of_block(layer, blocks):
-        # Return true if the layer is the end of a new block.
-        # The very last layer is the end of another block
-        if not blocks:
-            return True
-        outbounds = layer.outbound_nodes
-        # If there are many outbounds, this is an end of block
-        if len(outbounds) > 1:
-            return True
-        # Prepare a list of all first layers of all blocks
-        first_layers = [block[0] for block in blocks]
-        outbound = outbounds[0].outbound_layer
-        return outbound in first_layers
-
-    blocks = []
-    # If there is a Dequantizer, save the first one as single block layer and then
-    # remove all layers after it (not supported at conversion time)
-    deq_layer, model_layers = _get_layers_before_dequantizer(model)
-    if deq_layer:
-        blocks.append([deq_layer])
-
-    # We forward from head to bottom
-    for layer in model_layers[::-1]:
-        if _is_end_of_block(layer, blocks):
-            new_block = _search_block(layer)
-            blocks.append(new_block)
-        # The skip layers must be inside of one block
-        elif layer not in sum(blocks, []):
-            raise RuntimeError(f"Impossible to append {layer.name} into a block.")
-
-    # At the end, we sort blocks from bottom to head
-    return blocks[::-1]
-
-
-def get_block_out_quantizer(block):
-    """Extract the output_quantizer of the layers block.
-
-    Note that a block of layers is considered as block if:
-        1. There is only one output quantizer (in the last layer of the block)
-        2. There are no multi-inbound layers
-        3. There are no QuantizedExtractToken layers
+    # Parse the Stem block layers parameters
+    stem_params = _parse_stem_block_layers(block)
 
-    This method should ideally be called after "split_model_into_blocks" to make sure
-    that the layers block can be handled correctly.
+    layer_ak = Stem(**stem_params)
+    model_ak.add(layer_ak)
+    _set_stem_variables(layer_ak, block)
+    # Get out_quantizer of the block.
+    out_quantizer = get_block_out_quantizer(block)
+    set_output_v2_variables(layer_ak, out_quantizer)
+
+    return True
+
+
+class StemBlockConverter(BlockConverter):
+    """Main class that should be used to check if the stem block is compatible to an Akida v2
+    conversion and provides a method to convert it in an equivalent Akida stem layer.
 
     Args:
-        block (list(:obj:`tf.keras.Layer`)): the layers block.
-
-    Returns:
-        :obj:`quantizeml.layers.OutputQuantizer`: the layers block output quantizer (None if the
-            block has no output quantizer)
+        block (list): list of quantizeml quantized layers.
     """
-    # Output quantizer is on the last layer of the block
-    return getattr(block[-1], "out_quantizer", None)
+
+    def __init__(self, block):
+        super().__init__(block)
+        self._stem_additional_checks()
+
+    def convert(self, model_ak):
+        assert len(model_ak.layers) == 0, "Stem layer should be the first model layer."
+        return convert_quantized_stem_layers(model_ak, self._block)
+
+    def _stem_additional_checks(self):
+        embedding = self._block[0]
+        # Get embedding layer input shape without the batch size.
+        input_shape = embedding.input_shape[1:]
+        # Stem handles only square inputs
+        if (input_shape[0] != input_shape[1]):
+            raise ValueError("input should have square spatial dimensions. Receives: "
+                             f"x_size={input_shape[0]} and y_size={input_shape[1]}")
+        # Stem handles only image-like inputs (1-D or 3-D uint8 inputs)
+        if input_shape[-1] not in (1, 3):
+            raise ValueError("Stem layer can only handle image like inputs (i.e 3-D or 1-D input "
+                             f"shape). Received: {embedding.input_shape[1:]}.")
+        # Get the kernel size
+        kernel_size = embedding.kernel_size
+        # Stem handles only square kernels.
+        if (kernel_size[0] != kernel_size[1]):
+            raise ValueError("input should have square kernels. Receives: "
+                             f"k_x={kernel_size[0]} and k_y={kernel_size[1]}")
+        # Stem input size must be a multiple of kernel size.
+        if (input_shape[0] % kernel_size[0] != 0):
+            raise ValueError("Input spatial dimension size must be a multiple of kernel size")
+
+
+# Register the valid stem block pattern for Akida v2
+register_conversion_patterns(AkidaVersion.v2, _PATTERNS, StemBlockConverter, input_pattern=True)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/compatibility_checks.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/conv_common.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 # ******************************************************************************
 # Copyright 2023 Brainchip Holdings Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -9,377 +10,377 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
-"""Functions to check model compatibility for CNN2SNN conversion.
+"""Helper functions to convert QuantizedConv2D to its equivalent Akida layers.
 """
-from keras import layers
-from quantizeml import layers as qlayers
+import numpy as np
+from akida import PoolType
+from quantizeml.layers import (QuantizedGlobalAveragePooling2D, QuantizedMaxPool2D,
+                               QuantizedConv2DTranspose, QuantizedReLU, WeightQuantizer,
+                               AlignedWeightQuantizer)
+from .activations import parse_relu_v1, parse_relu_v2, set_relu_variables
+from .pooling import parse_max_pool_v1, parse_max_pool_v2
+from .padding import get_padding_info
+from .weights import broadcast_and_set_variable
+from .blocks import get_block_out_quantizer
+from .outputs import set_output_v2_variables, parse_output_bits
 
-from .blocks import split_model_into_blocks
-from .padding import check_same_valid_compatibility
-from ..transforms.sequential import _check_layers_data_format, _check_layer_inbounds
-from ..akida_versions import get_akida_version, AkidaVersion
-from .block_converter import (_V1_PATTERN_CONVERTERS, _V2_PATTERN_CONVERTERS,
-                              _V1_INPUT_PATTERN_CONVERTERS, _V2_INPUT_PATTERN_CONVERTERS)
 
-neural_layers = (qlayers.QuantizedConv2D, qlayers.QuantizedSeparableConv2D,
-                 qlayers.QuantizedDense, qlayers.QuantizedDepthwiseConv2D,
-                 qlayers.QuantizedConv2DTranspose, qlayers.QuantizedDepthwiseConv2DTranspose)
-skippable_layers = (layers.InputLayer, layers.Rescaling, layers.Activation, layers.Softmax,
-                    layers.Dropout)
-pooling_layers = (qlayers.QuantizedGlobalAveragePooling2D, qlayers.QuantizedMaxPool2D)
-norm_layers = (qlayers.LayerMadNormalization, qlayers.QuantizedBatchNormalization)
-activation_layers = (qlayers.QuantizedReLU,)
-stem_layers = (qlayers.ClassToken, qlayers.AddPositionEmbs)
-reshape_layers = (qlayers.QuantizedReshape, qlayers.QuantizedFlatten)
+def get_layer_by_type(block, type_list):
+    """Helper to get the first layer, if found, of a block that match one of the types
 
+    Args:
+        block (list(:obj:`tf.keras.Layer`)): list of quantizeml quantized layers.
+        type_list (tuple): list of quantizeml layers types.
+
+    Returns:
+        :obj:`tf.keras.Layer`: the first quantized layer that match of the types of the list
+        if found. None otherwise.
+    """
+    targeted_layer = None
+
+    for layer in block:
+        if isinstance(layer, type_list):
+            targeted_layer = layer
+            break
+
+    return targeted_layer
+
+
+def set_conv_variables_v1(layer_ak, layer_k, input_layer=False):
+    """Computes and sets the variables for an Akida v1 Convolutional layer.
 
-class CompatibilityMessage:
-    """Helper to represent an error message
+    This function converts the variables of a Keras layer and sets them into
+    the corresponding variables of the equivalent Akida layer.
 
     Args:
-        message (str): main error message.
-        layers (list or tf.keras.Layers): layer(s) that will raise(s) the exception.
-            Defaults to None.
+        layer_ak (:obj:`akida.Layer`): the targeted akida layer.
+        layer_k (:obj:`tf.keras.Layer`): the source quantized layer.
+        input_layer (bool, optional): Boolean to check if the targeted layer is a
+            V1 conv input layer (i.e InputConvolutional). Defaults to False.
+
     """
+    assert isinstance(layer_k.weight_quantizer, WeightQuantizer)
+    if layer_k.use_bias:
+        assert isinstance(layer_k.bias_quantizer, AlignedWeightQuantizer)
+
+    # Get the weights
+    weights = layer_k.weight_quantizer.qweights.value.fp.values.numpy()
+    # Flip W and H dimensions for conv. kernels (not input conv.)
+    if not input_layer:
+        weights = np.flip(weights, axis=[0, 1])
+    layer_ak.variables["weights"] = weights.astype(np.int8)
+
+    # Set the bias (if there is one)
+    if layer_k.use_bias:
+        bias_quantizer = layer_k.bias_quantizer
+        bias = bias_quantizer.qweights.value.values.numpy().astype(np.int32)
+        # Store bias into the threshold variable
+        layer_ak.variables["threshold"] = -bias
 
-    def __init__(self, message, layers=None):
-        if not message.endswith("."):
-            message += "."
-        self.message = message
-        # Replace empty list by None
-        self.layers = layers or None
 
-    def __str__(self):
-        if self.layers is None:
-            return self.message
+def set_conv_variables_v2(layer_ak, layer_k, input_layer=False):
+    """Computes and sets the variables for an Akida v2 Conv2D layer.
 
-        message = f"{self.message} Layer(s): "
-        if isinstance(self.layers, list):
-            message += str([x.name for x in self.layers])
-        else:
-            message += self.layers.name
-        return message
+    This function converts the variables of a Keras layer and sets them into
+    the corresponding variables of the equivalent Akida layer.
 
+    Args:
+        layer_ak (:obj:`akida.Layer`): the targeted akida layer.
+        layer_k (:obj:`tf.keras.Layer`): the source quantized layer.
+        input_layer (bool, optional): Boolean to check if the targeted layer is a
+            V2 conv input layer (i.e InputConv2D). Defaults to False.
+    """
+    assert isinstance(layer_k.weight_quantizer, WeightQuantizer)
+    if layer_k.use_bias:
+        assert isinstance(layer_k.bias_quantizer, AlignedWeightQuantizer)
+
+    # Get the weights
+    weights = layer_k.weight_quantizer.qweights.value.fp.values.numpy()
+    # Flip W and H dimensions for conv. kernels (not input conv.)
+    if not input_layer:
+        weights = np.flip(weights, axis=[0, 1])
+    layer_ak.variables["weights"] = weights.astype(np.int8)
+
+    # Set the bias (if there is one)
+    if layer_k.use_bias:
+        bias_quantizer = layer_k.bias_quantizer
+        bias = bias_quantizer.qweights.value.values.numpy().astype(np.int32)
+        bias_shift = bias_quantizer.shift.value.numpy().astype(np.uint8)
+        # Unshift the bias and store it
+        layer_ak.variables["bias"] = (bias >> bias_shift).astype(np.int8)
+        # Also store the bias shift
+        broadcast_and_set_variable(layer_ak.variables, "bias_shift", bias_shift)
+        input_shift = getattr(layer_k, 'input_shift', None)
+        if input_shift is not None:
+            broadcast_and_set_variable(layer_ak.variables, "input_shift",
+                                       input_shift.value.numpy().astype(np.uint8))
 
-class CompatibilityBlockError:
-    """Helper to raise a list of ``CompatibilityMessage`` errors"""
 
-    def __init__(self):
-        self._errors_msg = []
+def _parse_additional_layers_v1(block, block_params):
+    """Parse conv block additional layers into the parameters of one for Akida v1.
 
-    @property
-    def status(self):
-        return len(self._errors_msg) > 0
+    Args:
+        block (list(:obj:`tf.keras.Layer`)): the layers block.
+        block_params (dict): the current block parameters.
 
-    def push(self, message, layers=None):
-        self._errors_msg.append(CompatibilityMessage(message, layers))
+    """
+    # Identify the next layers
 
-    def __str__(self):
-        err_msg = "The following errors were found when the block was checked:"
-        for err in self._errors_msg:
-            err_msg += "\n\t- " + str(err)
-        return err_msg
+    relu_layer = get_layer_by_type(block, QuantizedReLU)
+    pool_layer = get_layer_by_type(block, (QuantizedGlobalAveragePooling2D, QuantizedMaxPool2D))
 
-    def __call__(self):
-        if self.status:
-            raise RuntimeError(str(self))
+    if isinstance(pool_layer, QuantizedMaxPool2D):
+        pool_params = parse_max_pool_v1(pool_layer)
+        block_params.update(pool_params)
+    elif isinstance(pool_layer, QuantizedGlobalAveragePooling2D):
+        pool_params = dict(pool_type=PoolType.Average)
+        block_params.update(pool_params)
+    if relu_layer:
+        act_params = parse_relu_v1(relu_layer)
+        block_params.update(act_params)
 
 
-def _block_pattern(block):
-    """Method that returns the pattern of a block of layers.
+def _parse_additional_layers_v2(block, block_params):
+    """Parse conv block additional layers into the parameters of one for Akida v2.
 
     Args:
-        block (list): list of quantized quantizeml layers.
+        block (list(:obj:`tf.keras.Layer`)): the layers block.
+        block_params (dict): the current block parameters.
 
-    Returns:
-        tuple: list of layer types representing the block pattern.
     """
-    return tuple([layer.__class__ for layer in block])
+    # Identify the next layers
+
+    relu_layer = get_layer_by_type(block, QuantizedReLU)
+    pool_layer = get_layer_by_type(block, (QuantizedGlobalAveragePooling2D, QuantizedMaxPool2D))
+
+    if isinstance(pool_layer, QuantizedMaxPool2D):
+        pool_params = parse_max_pool_v2(pool_layer)
+        block_params.update(pool_params)
+    elif isinstance(pool_layer, QuantizedGlobalAveragePooling2D):
+        block_params.update({"pool_type": PoolType.Average})
+    if relu_layer:
+        act_params = parse_relu_v2(relu_layer)
+        block_params.update(act_params)
+    # parse the block output bits
+    parse_output_bits(block, block_params)
 
 
-def _get_block_converter(block):
-    """Helper to get the BlockConverter of a block of layers.
+def parse_conv_block_v1(block, input_layer=False):
+    """Parses a conv block parameters for an Akida v1 layer.
 
     Args:
-        block (list): list of quantized quantizeml layers.
+        block (list(:obj:`tf.keras.Layer`)): the conv block layers.
+        input_layer (bool, optional): Boolean to check if the targeted layer is a
+            V1 conv input layer (i.e InputConvolutional). Defaults to False.
 
     Returns:
-        (:obj:`BlockConverter`): the BlockConverter corresponding to the block of layers or None.
+        dict: the corresponding akida parameters.
     """
-    pattern = _block_pattern(block)
+    conv = block[0]
+    padding, padding_value = get_padding_info(conv)
 
-    if get_akida_version() == AkidaVersion.v1:
-        block_converter = _V1_PATTERN_CONVERTERS.get(pattern, None)
-    else:
-        block_converter = _V2_PATTERN_CONVERTERS.get(pattern, None)
+    conv_params = dict(
+        padding=padding,
+        kernel_size=(conv.kernel_size[0], conv.kernel_size[1]),
+        filters=int(conv.kernel.shape[3]),
+        weights_bits=conv.weight_quantizer.bitwidth,
+        kernel_stride=(conv.strides[0], conv.strides[1]),
+        activation=False,
+        name=conv.name
+    )
+    # If the targeted layer is a InputConvolutional add two params.
+    if input_layer:
+        input_layer_params = dict(input_shape=tuple(int(x) for x in conv.input_shape[1:4]),
+                                  padding_value=padding_value)
+        conv_params.update(input_layer_params)
 
-    return block_converter
+    _parse_additional_layers_v1(block, conv_params)
+    return conv_params
 
 
-def _get_input_block_converter(block):
-    """Helper to get the BlockConverter of an input block of layers.
+def parse_conv_block_v2(block, input_layer=False):
+    """Parses a conv block parameters for akida v2.
 
     Args:
-        block (list): list of quantized quantizeml layers.
+        block (list(:obj:`tf.keras.Layer`)): the conv block layers.
+        input_layer (bool, optional): Boolean to check if the targeted layer is a
+            V2 conv input layer (i.e InputConv2D). Defaults to False.
 
     Returns:
-        (:obj:`BlockConverter`): the BlockConverter corresponding to the block of layers or None.
+        dict: the corresponding akida parameters.
     """
-    pattern = _block_pattern(block)
+    conv = block[0]
+    # Padding value must be built in constructor
+    padding, padding_value = get_padding_info(conv)
+
+    # In quantizeml one bit is reserved for the sign in the buffer bitwidth
+    # variable, but in akida this value has to be added back to have the
+    # correct clipping.
+    conv_params = dict(
+        padding=padding,
+        kernel_size=conv.kernel_size[0],
+        filters=int(conv.kernel.shape[3]),
+        kernel_stride=conv.strides[0],
+        activation=False,
+        buffer_bits=conv.buffer_bitwidth + 1,
+        name=conv.name
+    )
+    # If the targeted layer is a InputConv2D add two params.
+    if input_layer:
+        input_layer_params = dict(input_shape=tuple(int(x) for x in conv.input_shape[1:4]),
+                                  padding_value=padding_value)
+        conv_params.update(input_layer_params)
 
-    if get_akida_version() == AkidaVersion.v1:
-        return _V1_INPUT_PATTERN_CONVERTERS.get(pattern, None)
-    return _V2_INPUT_PATTERN_CONVERTERS.get(pattern, None)
+    _parse_additional_layers_v2(block, conv_params)
+    return conv_params
 
 
-def check_model_compatibility(model, input_is_image):
-    r"""Checks if a QuantizeML model is compatible for Akida conversion.
+def parse_sepconv_block(block):
+    """Parses a quantizeml sepconv block parameters for Akida v1.
 
-    This function does NOT:
+    Args:
+        block (list(:obj:`tf.keras.Layer`)): the sepconv block layers.
+
+    Returns:
+        dict: the corresponding akida parameters.
+    """
+    sepconv = block[0]
+    # Padding value must be built in constructor
+    padding, _ = get_padding_info(sepconv)
+
+    sepconv_params = dict(kernel_size=(sepconv.kernel_size[0], sepconv.kernel_size[1]),
+                          filters=int(sepconv.pointwise_kernel.shape[3]),
+                          padding=padding,
+                          kernel_stride=(sepconv.strides[0], sepconv.strides[1]),
+                          weights_bits=sepconv.dw_weight_quantizer.bitwidth,
+                          activation=False,
+                          name=sepconv.name)
 
-    - convert the QuantizeML model to an Akida model,
-    - check if the model is compatible with Akida hardware
+    _parse_additional_layers_v1(block, sepconv_params)
+    return sepconv_params
 
-    It ONLY checks if the model design is compatible with Akida.
+
+def parse_depthwise_conv_block(block):
+    """Parses a quantizeml depthwise conv block parameters for Akida v2.
 
     Args:
-        model (:obj:`tf.keras.Model`): the model to check.
-        input_is_image (bool): True if input is an 8-bit unsigned tensors (like images).
+        block (list(:obj:`tf.keras.Layer`)): the depthwise conv2d block layers.
 
     Returns:
-        list: a list of sequences of the non_skippable layers ('blocks').
+        dict: the corresponding akida parameters.
     """
-    # Check general rules about model in three steps:
-    # 1. Check if model has only one input and one output,
-    # 2. Check right data format and
-    # 3. Over Akida 1.0, check if model is sequential.
-    _check_model_input_output(model)
-    _check_layers_data_format(model)
-    if get_akida_version() == AkidaVersion.v1:
-        _check_layer_inbounds(model)
-
-    # Split model into theirs blocks:
-    blocks = split_model_into_blocks(model)
-
-    # This list will contains either a block converter instance,
-    # or a list of non-skippable layers.
-    straight_blocks = []
-    # Evaluate block-by-block integrity
-    for id, block in enumerate(blocks):
-        # Split blocks into skippable and none skippable blocks
-        _, non_skippable = _extract_skippable_layers(block)
-        # Get the corresponding BlockConverter of the layers block if available.
-        if id == 0 and input_is_image and not any(isinstance(layer, qlayers.QuantizedDense)
-                                                  for layer in block):
-            block_converter = _get_input_block_converter(non_skippable)
-        else:
-            block_converter = _get_block_converter(non_skippable)
-        if block_converter:
-            straight_blocks.append(block_converter(non_skippable))
-            continue
-        # TODO: remove this part once all conversion uses BlockConverter classes
-        # Check pooling layers
-        _check_pooling_compatibility(non_skippable)
-        # Check other rules
-        _check_block_integrity(non_skippable)
-        if len(non_skippable) > 0:
-            straight_blocks.append(non_skippable)
-    return straight_blocks
-
-
-def _split_block_into_layer_types(block):
-    """Split input block into the following categories:
-
-    - neural (processing) layers,
-    - activation layers,
-    - normalization layers and
-    - stem block layers.
+    depth_conv = block[0]
+
+    # Padding value must be built in constructor
+    padding, _ = get_padding_info(depth_conv)
+
+    # In quantizeml one bit is reserved for the sign in the buffer bitwidth
+    # variable, but in akida this value has to be added back to have the
+    # correct clipping.
+    block_params = dict(
+        kernel_size=depth_conv.kernel_size[0],
+        kernel_stride=depth_conv.strides[0],
+        padding=padding,
+        buffer_bits=depth_conv.buffer_bitwidth + 1,
+        activation=False,
+        name=depth_conv.name
+    )
+    _parse_additional_layers_v2(block, block_params)
+
+    return block_params
+
+
+def parse_conv2d_transpose_block(block, depthwise=False):
+    """Parses a quantizeml (depthwise)conv transpose block parameters for Akida v2.
 
     Args:
-        block (list): block layers to split.
+        block (list(:obj:`tf.keras.Layer`)): the (depthwise)conv2d_transpose block layers.
+        depthwise (bool, optional): boolean to declare the main layer as a depthwise layer.
 
     Returns:
-        list: block divided into categories.
+        dict: the corresponding akida parameters.
     """
-    neurals, acts, norms, stems = [], [], [], []
-    for layer in block:
-        if isinstance(layer, neural_layers):
-            neurals.append(layer)
-        elif isinstance(layer, activation_layers):
-            acts.append(layer)
-        elif isinstance(layer, norm_layers):
-            norms.append(layer)
-        elif isinstance(layer, stem_layers):
-            stems.append(layer)
-        elif isinstance(layer, reshape_layers):
-            continue
-        elif not isinstance(layer, pooling_layers):
-            raise RuntimeError(f"Unrecognizable layer in block: {layer.name}")
-    return neurals, acts, norms, stems
-
-
-def _check_block_integrity(block):
-    """Check integrity of one block.
-
-    Args:
-        block (list(tf.keras.Layer)): block to analysis.
-    """
-    if len(block) == 0 or isinstance(block[0], qlayers.Dequantizer):
-        return
-
-    def _islast(layer):
-        outbound = layer.outbound_nodes
-        if len(outbound) == 1:
-            outbound_layer = outbound[0].outbound_layer
-            if isinstance(outbound_layer, skippable_layers):
-                return _islast(outbound_layer)
-            # If outbound layer is a Dequantizer, target is the final quantized layer
-            if isinstance(outbound_layer, qlayers.Dequantizer):
-                return True
-        return len(outbound) == 0
-
-    def _isfirst(layer):
-        ly_inbounds = layer.inbound_nodes[0].inbound_layers
-        if not isinstance(ly_inbounds, (tuple, list)):
-            ly_inbounds = [ly_inbounds]
-        if len(ly_inbounds) == 1 and isinstance(ly_inbounds[0], skippable_layers):
-            return _isfirst(ly_inbounds[0])
-        return len(ly_inbounds) == 0
-
-    # Start with Akida 1.0 restrictions
-    errors = CompatibilityBlockError()
-    ak_version = get_akida_version()
-    if ak_version == AkidaVersion.v1:
-        islast = _islast(block[-1])
-        if len(block) == 1 and not islast:
-            errors.push("In Akida 1.0, every block must have at least "
-                        "one neural and activation layer")
-        if islast and not isinstance(block[0], neural_layers):
-            errors.push("The last block must start by a neural layer", block[0])
-        if not (islast or isinstance(block[-1], activation_layers)):
-            errors.push("A block must end by an activation layer", block[-1])
-
-    # General limitations
-    if len(block) > 1:
-        neurals, acts, norms, stems = _split_block_into_layer_types(block)
-        if len(neurals) != 1:
-            errors.push("A block must have one neural layer", neurals)
-        if len(neurals) > 0:
-            if block[0] != neurals[0]:
-                errors.push("A block must start by a neural layer", block[0])
-        if len(acts) > 1:
-            errors.push("A block could have up to only one activation layer", acts)
-        if len(norms) != 0:
-            errors.push("A block should not have normalization layers: "
-                        "these must be folded into previous neural layers", norms)
-        if len(stems) > 0:
-            if ak_version == AkidaVersion.v1:
-                errors.push("Stem-block is not supported on Akida 1.0.")
-            if not _isfirst(block[0]):
-                errors.push("Stem-block must be the first one in the model.")
-            if not all(isinstance(x, qlayers.ClassToken) for x in stems[1:-1]):
-                errors.push("'ClassToken' is the only intermediate layer allowed "
-                            "in a stem block.", stems[1:-1])
-            if not isinstance(block[0], qlayers.QuantizedConv2D):
-                errors.push("Stem-block must begin by one 'Conv2D'", block[0])
-            if not isinstance(stems[-1], qlayers.AddPositionEmbs):
-                errors.push("Stem-block must end by one 'AddPositionEmbs'.", stems[-1])
-
-    # Raise exception if there is at least one error message
-    errors()
-
-
-def _check_model_input_output(model):
-    """Asserts that model inputs/outputs are supported for conversion.
-
-    The Keras model must have only one input layer and one output layer.
-    On Akida 1.0, the input shape must 4-D (N, H, W, C).
-
-    Args:
-        model (tf.keras.model): the Keras model to check.
-    """
-
-    # Error if multiple inputs
-    if len(model.input_names) > 1:
-        raise RuntimeError("Model must have only one input layer. Receives "
-                           f"inputs {model.input_names}.")
-
-    # Error if multiple outputs
-    if len(model.output_names) != 1:
-        raise RuntimeError("Model must have only one output layer. Receives"
-                           f"outputs {model.output_names}.")
-
-    # Error if input shape is not 2D or 4D
-    if len(model.input_shape) not in (2, 4) and get_akida_version() == AkidaVersion.v1:
-        raise RuntimeError(
-            "Input shape of model must be 2-D or 4-D (batch size + 1-D or 3-D "
-            f"tensors). Receives input shape {model.input_shape}.")
 
+    conv_transpose = block[0]
 
-def _extract_skippable_layers(block):
-    """Split block into skippable and non skippable layers
+    # In quantizeml one bit is reserved for the sign in the buffer bitwidth
+    # variable, but in akida this value has to be added back to have the
+    # correct clipping.
+    buffer_bits = conv_transpose.buffer_bitwidth + 1
+
+    block_params = dict(
+        kernel_size=conv_transpose.kernel_size[0],
+        buffer_bits=buffer_bits,
+        activation=False,
+        name=conv_transpose.name
+    )
+    # Add filters parameters if not a Depthwise convolution
+    if not depthwise:
+        assert isinstance(conv_transpose, QuantizedConv2DTranspose)
+        block_params["filters"] = conv_transpose.filters
+
+    relu_layer = get_layer_by_type(block, QuantizedReLU)
+    if relu_layer:
+        act_params = parse_relu_v2(relu_layer)
+        block_params.update(act_params)
+
+    # parse the block output bits
+    parse_output_bits(block, block_params)
+
+    return block_params
+
+
+def set_conv2d_transpose_block_variables(layer_ak, block):
+    """Computes and sets the variables for an Akida v2 Conv2DTranspose or DepthwiseConv2DTranspose
+    layers.
 
-    Args:
-        block (tf.keras.Layer): block to split.
+    This function converts the variables of a Keras layers block and sets them into
+    the corresponding variables of the equivalent Akida layer.
 
-    Returns:
-        tuple: list of skippable and non skippable layers
+    Args:
+        layer_ak (:obj:`akida.Layer`): the targeted akida layer.
+        block (list(:obj:`tf.keras.Layer`)): the (depthwise)conv2d_transpose block layers.
     """
-    skippable, non_skippable = [], []
-    for layer in block:
-        if isinstance(layer, skippable_layers):
-            skippable.append(layer)
-        elif isinstance(layer, qlayers.QuantizedReshape):
-            in_shape = layer.input_shape
-            out_shape = layer.output_shape
-            in_dims = [x for x in in_shape if x != 1]
-            out_dims = [x for x in out_shape if x != 1]
-            if in_dims != out_dims:
-                non_skippable.append(layer)
-            else:
-                skippable.append(layer)
-        else:
-            non_skippable.append(layer)
-    return skippable, non_skippable
-
-
-def _check_pooling_compatibility(block):
-    """Asserts pooling layer is compatible for conversion.
-
-    Args:
-        block (list): the layers block.
-    """
-    errors = CompatibilityBlockError()
-    conv_neural_layers = (qlayers.QuantizedConv2D,
-                          qlayers.QuantizedSeparableConv2D, qlayers.QuantizedDepthwiseConv2D)
-    pool_layer = [ly for ly in block if isinstance(ly, pooling_layers)]
-    if len(pool_layer) == 0:
-        return
-    elif len(pool_layer) != 1:
-        errors.push("A block could have up to only one pooling layer", pool_layer)
-
-    # Raise error if pooling does not have a convolutional layer in the block
-    pool_layer = pool_layer[0]
-    conv_layer = [ly for ly in block if isinstance(ly, conv_neural_layers)]
-    if len(conv_layer) != 1:
-        errors.push("Pooling layer must be placed after a convolutional layer", conv_layer)
-
-    if isinstance(pool_layer, qlayers.QuantizedGlobalAveragePooling2D) and pool_layer != block[-1] \
-            and get_akida_version() == AkidaVersion.v2:
-        errors.push("In v2, GAP should occur after ReLU and placed at the end of the block",
-                    pool_layer)
-    # Raise the exceptions(if exist)
-    errors()
-
-    # Raises error if the padding of MaxPool2D is different from the padding
-    # of the neural processing layer.
-    conv_layer = conv_layer[0]
-    neur_pad = conv_layer.padding if not check_same_valid_compatibility(conv_layer) else "same"
-    pool_pad = getattr(pool_layer, "padding", "")
-    if isinstance(pool_layer, qlayers.QuantizedMaxPool2D) and neur_pad != pool_pad:
-        raise RuntimeError(f"Pooling layer {pool_layer.name} (padding: {pool_pad}) must have "
-                           f"the same padding as {conv_layer.name} (padding: {neur_pad}).")
+    conv_transpose = block[0]
+
+    assert isinstance(conv_transpose.weight_quantizer, WeightQuantizer)
+    if conv_transpose.use_bias:
+        assert isinstance(conv_transpose.bias_quantizer, AlignedWeightQuantizer)
+
+    # Get the weights (Note that in qweights the filter and channel dimensions are already
+    # transposed)
+    weights = conv_transpose.weight_quantizer.qweights.value.fp.values.numpy()
+
+    layer_ak.variables["weights"] = weights.astype(np.int8)
+
+    # Set the bias (if there is one)
+    if conv_transpose.use_bias:
+        bias_quantizer = conv_transpose.bias_quantizer
+        bias = bias_quantizer.qweights.value.values.numpy().astype(np.int32)
+        bias_shift = bias_quantizer.shift.value.numpy().astype(np.uint8)
+
+        # Unshift the bias and store it
+        layer_ak.variables["bias"] = (bias >> bias_shift).astype(np.int8)
+        # Also store the bias shift
+        broadcast_and_set_variable(layer_ak.variables, "bias_shift", bias_shift)
+
+    # Set input shift if available
+    if getattr(conv_transpose, 'input_shift', None):
+        broadcast_and_set_variable(layer_ak.variables, "input_shift",
+                                   conv_transpose.input_shift.value.numpy().astype(np.uint8))
+
+    # Check if we have ReLU
+    relu_layer = get_layer_by_type(block, QuantizedReLU)
+    # Set optional activation variables
+    if relu_layer:
+        set_relu_variables(layer_ak, relu_layer)
+
+    # Get the layer block output_quantizer
+    out_quantizer = get_block_out_quantizer(block)
+    # Set optional output_quantizer variables
+    if out_quantizer:
+        set_output_v2_variables(layer_ak, out_quantizer)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/concatenate.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/concatenate.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,29 +13,54 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """Functions to convert QuantizedConcatenate to Akida.
 """
 from akida import Concatenate
-import quantizeml.layers as qlayers
+from quantizeml.layers import QuantizedConcatenate
 
 from .layer_utils import get_inbound_layers
+from .block_converter import BlockConverter, register_conversion_patterns
+from ..akida_versions import AkidaVersion
 
+__all__ = ["ConcatenateBlockConverter"]
 
-def convert_quantized_concatenate(model_ak, layer_k):
+_PATTERNS = [(QuantizedConcatenate,)]
+
+
+def convert_quantized_concatenate(model_ak, block):
     """Converts QuantizedConcatenate layer and its variables and adds it to the
     Akida's model.
 
     Args:
         model_ak (:obj:`akida.Model`): the Akida model where the model will be added.
-        layer (:obj:`tf.keras.Layer`): the quantizeml QuantizedConcatenate layer to convert.
+        block (list(:obj:`tf.keras.Layer`)): the block of keras layers.
+
+    Returns:
+        bool: Returns True for a successful conversion.
     """
-    if not isinstance(layer_k, qlayers.QuantizedConcatenate):
-        raise TypeError(f"Layer {layer_k.name} was expected to be "
-                        "QuantizedConcatenate")
+
     # Retrieve the akida inbound layers
-    inbound_layers_ak = get_inbound_layers(model_ak, layer_k)
+    inbound_layers_ak = get_inbound_layers(model_ak, block[0])
     # Create and add layer to the akida model
     # It is quite simple because there are no variables or params to be set.
     layer_ak = Concatenate()
     model_ak.add(layer_ak, inbound_layers_ak)
+    return True
+
+
+class ConcatenateBlockConverter(BlockConverter):
+    """Main class that should be used to check if the concatenate layer block is compatible to an
+    Akida v2 conversion and provides a method to convert it in an equivalent Akida Concatenate
+    layer.
+
+    Args:
+        block (list): list of quantizeml quantized layers.
+    """
+
+    def convert(self, model_ak):
+        return convert_quantized_concatenate(model_ak, self._block)
+
+
+# Register the valid concatenate block pattern for Akida v2
+register_conversion_patterns(AkidaVersion.v2, _PATTERNS, ConcatenateBlockConverter)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/dense.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                                WeightQuantizer, AlignedWeightQuantizer)
 import numpy as np
 
 from .layer_utils import get_inbound_layers
 from .weights import broadcast_and_set_variable
 from ..akida_versions import AkidaVersion
 from .activations import parse_relu_v1, parse_relu_v2, set_relu_variables, v1_relu_checks
-from .outputs import set_output_v1_variables, set_output_v2_variables
+from .outputs import set_output_v1_variables, set_output_v2_variables, parse_output_bits
 from .blocks import get_block_out_quantizer
 from .block_converter import BlockConverter, register_conversion_patterns
 
 _PATTERNS = [(QuantizedDense,), (QuantizedDense, QuantizedReLU), (QuantizedFlatten, QuantizedDense),
              (QuantizedFlatten, QuantizedDense, QuantizedReLU), (QuantizedReshape, QuantizedDense),
              (QuantizedReshape, QuantizedDense, QuantizedReLU),
              (QuantizedReshape, QuantizedFlatten, QuantizedDense),
@@ -141,24 +141,19 @@
 
     """
     # In quantizeml one bit is reserved for the sign in the buffer bitwidth
     # variable, but in akida this value has to be added back to have the
     # correct clipping.
     buffer_bits = layer.buffer_bitwidth + 1
 
-    # Find out if there is a quantizer
-    out_quantizer = getattr(layer, "out_quantizer", None)
-
     # Set by default the activation to false. It will be updated when parsing the optional ReLU
     # layer.
     dense_params = dict(units=layer.units, activation=False, name=layer.name)
 
     dense_params["buffer_bits"] = buffer_bits
-    dense_params["output_bits"] = out_quantizer.bitwidth if out_quantizer else buffer_bits
-
     return dense_params
 
 
 def _get_dense_layer(block):
     """Helper to extract QuantizedDense layer of the block.
 
     Args:
@@ -195,14 +190,16 @@
     dense = _get_dense_layer(block)
 
     # Parse main dense params
     if akida_type == FullyConnected:
         dense_params = _parse_dense_v1(dense)
     else:
         dense_params = _parse_dense_v2(dense)
+        # parse the block output bits
+        parse_output_bits(block, dense_params)
 
     # Extract ReLU if present
     relu_layer = None
     if isinstance(block[-1], QuantizedReLU):
         relu_layer = block[-1]
         # parse ReLU layer parameters
         if akida_type == FullyConnected:
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/depthwise_conv2d.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/depthwise_conv2d.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,160 +15,147 @@
 # limitations under the License.
 # ******************************************************************************
 """Functions to convert QuantizedDepthwiseConv2D to Akida.
 """
 import numpy as np
 
 from quantizeml.layers import (QuantizedDepthwiseConv2D, QuantizedReLU,
-                               WeightQuantizer, AlignedWeightQuantizer)
+                               QuantizedMaxPool2D, WeightQuantizer, AlignedWeightQuantizer)
 from akida import DepthwiseConv2D
 
-from ..akida_versions import AkidaVersion, get_akida_version
+from ..akida_versions import AkidaVersion
 from .activations import set_relu_variables
 from .weights import broadcast_and_set_variable
-from .outputs import set_output_v2_variables
-from .padding import get_padding_info
-from .blocks import parse_block_additional_layers
+from .outputs import set_output_v2_variables, parse_output_bits
+from .padding import check_conv_and_max_pool_compatibility
+from .pooling import max_pool_param_checks
+from .blocks import get_block_out_quantizer
+from .conv_common import get_layer_by_type, parse_depthwise_conv_block
+from .block_converter import BlockConverter, register_conversion_patterns
 
+_PATTERNS = [(QuantizedDepthwiseConv2D,), (QuantizedDepthwiseConv2D, QuantizedReLU),
+             (QuantizedDepthwiseConv2D, QuantizedMaxPool2D, QuantizedReLU)]
 
-def _set_depthwise_conv2d_variables(layer_ak, layer_k):
-    """Computes and sets the variables for an Akida DepthwiseConv2D layer.
 
-    This function converts the variables of a Keras layer and sets them into
+def _set_depthwise_conv2d_block_variables(layer_ak, block):
+    """Computes and sets the variables for an Akida v2 DepthwiseConv2D layer.
+
+    This function converts the variables of a Keras layers block and sets them into
     the corresponding variables of the equivalent Akida layer.
 
     Args:
         layer_ak (:obj:`akida.Layer`): the targeted akida layer.
-        layer_k (:obj:`tf.keras.Layer`): the source quantized layer.
+        block (list(:obj:`tf.keras.Layer`)): the depthwise convolutional block layers.
     """
-    assert isinstance(layer_k, QuantizedDepthwiseConv2D)
-    assert isinstance(layer_k.weight_quantizer, WeightQuantizer)
-    if layer_k.use_bias:
-        assert isinstance(layer_k.bias_quantizer, AlignedWeightQuantizer)
+    depth_conv = block[0]
+    assert isinstance(depth_conv.weight_quantizer, WeightQuantizer)
+    if depth_conv.use_bias:
+        assert isinstance(depth_conv.bias_quantizer, AlignedWeightQuantizer)
 
     # Get the weights
-    weights = layer_k.weight_quantizer.qweights.value.fp.values.numpy()
+    weights = depth_conv.weight_quantizer.qweights.value.fp.values.numpy()
     # Flip W and H dimensions for depthwise
     weights = np.flip(weights, axis=[0, 1])
 
     layer_ak.variables["weights"] = weights.astype(np.int8)
 
     # Set the bias (if there is one)
-    if layer_k.use_bias:
-        bias_quantizer = layer_k.bias_quantizer
+    if depth_conv.use_bias:
+        bias_quantizer = depth_conv.bias_quantizer
         bias = bias_quantizer.qweights.value.values.numpy().astype(np.int32)
         bias_shift = bias_quantizer.shift.value.numpy().astype(np.uint8)
 
         # Unshift the bias and store it
         layer_ak.variables["bias"] = (bias >> bias_shift).astype(np.int8)
         # Also store the bias shift
         broadcast_and_set_variable(layer_ak.variables, "bias_shift", bias_shift)
 
     # Set input shift
-    input_shift = getattr(layer_k, 'input_shift', None)
+    input_shift = getattr(depth_conv, 'input_shift', None)
     if input_shift is not None:
         broadcast_and_set_variable(layer_ak.variables, "input_shift",
-                                   layer_k.input_shift.value.numpy().astype(np.uint8))
-
+                                   depth_conv.input_shift.value.numpy().astype(np.uint8))
 
-def _parse_depthwise_conv(layer):
-    """Parses a quantizeml.QuantizedDepthwiseConv2D parameters.
-
-    Args:
-        layer (:obj:`tf.keras.Layer`): the layer to parse.
-
-    Returns:
-        dict: the corresponding akida parameters.
-    """
-    assert isinstance(layer, QuantizedDepthwiseConv2D)
+    # Check if we have ReLU
+    relu_layer = get_layer_by_type(block, QuantizedReLU)
+    if relu_layer:
+        set_relu_variables(layer_ak, relu_layer)
 
-    # Make sure the DepthwiseConv2D kernel size and stride params are square
-    assert layer.kernel_size[0] == layer.kernel_size[1], (
-        "DepthwiseConv2D kernel_size should be square")
-    assert layer.strides[0] == layer.strides[1], (
-        "DepthwiseConv2D strides should be the same on both dimension")
-
-    # Padding value must be built in constructor
-    padding, _ = get_padding_info(layer)
-
-    # The only weight bitwidth supported is [4, 8]
-    weight_bits = layer.weight_quantizer.bitwidth
-    assert weight_bits in [4, 8]
-
-    # In quantizeml one bit is reserved for the sign in the buffer bitwidth
-    # variable, but in akida this value has to be added back to have the
-    # correct clipping.
-    buffer_bits = layer.buffer_bitwidth + 1
-
-    return dict(
-        kernel_size=layer.kernel_size[0],
-        kernel_stride=layer.strides[0],
-        padding=padding,
-        buffer_bits=buffer_bits,
-        activation=False,
-        name=layer.name
-    )
+    # Get the layer block output_quantizer
+    out_quantizer = get_block_out_quantizer(block)
+    # Set optional output_quantizer variables
+    if out_quantizer:
+        set_output_v2_variables(layer_ak, out_quantizer)
 
 
-def convert_depthwise_conv_block(model_ak, layers):
-    """Converts a depthwise convolutional block into an akida DepthwiseConv2D layer.
+def convert_depthwise_conv_block(model_ak, block):
+    """Converts a depthwise convolutional block into an akida v2 DepthwiseConv2D layer.
 
     The expected sequence is:
 
     - QuantizedDepthwiseConv2D,
     - QuantizedMaxPool2D (optional),
     - QuantizedReLU (optional).
 
     Args:
         model_ak (:obj:`akida.Model`): the target Akida model.
-        layers (list(:obj:`tf.keras.Layer`)): the block layers.
+        block (list(:obj:`tf.keras.Layer`)): the block layers.
 
-    Return:
-        int: the number of layers in the block or O if the first layer is not a
-        QuantizedDepthwiseConv2D.
-    """
-    if len(layers) == 0 or not isinstance(layers[0], QuantizedDepthwiseConv2D):
-        return 0
-
-    if get_akida_version() == AkidaVersion.v1:
-        return 0
+    Returns:
+        bool: Returns True for a successful conversion.
 
-    dw_conv = layers[0]
+    """
 
     # Evaluate the depthwise convolutional layer parameters
-    conv_params = _parse_depthwise_conv(dw_conv)
-
-    # Identify the next layers
-    next_layers = parse_block_additional_layers(layers, conv_params)
-    # Check if we have ReLU or MaxPool
-    relu_layer = next_layers.get(QuantizedReLU, None)
-
-    if relu_layer:
-        # Output quantizer should be in ReLU layer
-        out_quantizer = getattr(relu_layer, "out_quantizer", False)
-    else:
-        # otherwise, output quantize is in the conv layer
-        out_quantizer = getattr(dw_conv, "out_quantizer", False)
+    conv_params = parse_depthwise_conv_block(block)
 
     # add output quantizer bitwidth parameter
-    if out_quantizer:
-        conv_params["output_bits"] = out_quantizer.bitwidth
-    else:
-        conv_params["output_bits"] = conv_params["buffer_bits"]
+    parse_output_bits(block, conv_params)
 
     # Create Akida layer
     dw_conv_ak = DepthwiseConv2D(**conv_params)
     # Add layer to the model to build its internal variables
     model_ak.add(dw_conv_ak)
 
     # Set base variables
-    _set_depthwise_conv2d_variables(dw_conv_ak, dw_conv)
+    _set_depthwise_conv2d_block_variables(dw_conv_ak, block)
 
-    # Set optional activation variables
-    if relu_layer:
-        set_relu_variables(dw_conv_ak, relu_layer)
+    return True
+
+
+class DepthwiseConvBlockConverter(BlockConverter):
+    """Main class that should be used to check if the depthwise conv block is compatible to an
+    Akida v2 conversion and provides a method to convert it in an equivalent Akida DepthwiseConv2D
+    layer.
+
+    Args:
+        block (list): list of quantizeml quantized layers.
+    """
+
+    def __init__(self, block):
+        super().__init__(block)
+        self._depthwise_conv_additional_checks()
+
+    def _depthwise_conv_additional_checks(self):
+        depth_conv = self._block[0]
+        # Make sure the DepthwiseConv2D kernel size and stride params are square
+        assert depth_conv.kernel_size[0] == depth_conv.kernel_size[1], (
+            "DepthwiseConv2D kernel should be square")
+        assert depth_conv.strides[0] == depth_conv.strides[1], (
+            "DepthwiseConv2D strides should be the same on both dimensions")
+
+        # The only weight bitwidth supported is [4, 8]
+        weight_bits = depth_conv.weight_quantizer.bitwidth
+        assert weight_bits in [4, 8], ("DepthwiseConv2D layer can only handle weights"
+                                       f" with 4 or 8 bits. Received: {weight_bits}.")
+
+        # Check optional pooling compatibility
+        pool_layer = get_layer_by_type(self._block, QuantizedMaxPool2D)
+        if pool_layer:
+            check_conv_and_max_pool_compatibility(depth_conv, pool_layer)
+            max_pool_param_checks(pool_layer)
+
+    def convert(self, model_ak):
+        return convert_depthwise_conv_block(model_ak, self._block)
 
-    # Set optional output_quantizer variables
-    if out_quantizer:
-        set_output_v2_variables(dw_conv_ak, out_quantizer)
 
-    return 1 + len(next_layers)
+register_conversion_patterns(AkidaVersion.v2, _PATTERNS, DepthwiseConvBlockConverter)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/depthwise_conv2d_transpose.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/separable_convolution.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,158 +10,146 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
-"""Functions to convert QuantizedDepthwiseConv2DTranspose to Akida.
+"""Functions to convert QuantizedSeparableConv2D to Akida.
 """
 import numpy as np
 
-from quantizeml.layers import (QuantizedDepthwiseConv2DTranspose, QuantizedReLU,
-                               WeightQuantizer, AlignedWeightQuantizer)
-from akida import DepthwiseConv2DTranspose
-
-from ..akida_versions import AkidaVersion, get_akida_version
-from .activations import set_relu_variables
-from .weights import broadcast_and_set_variable
-from .outputs import set_output_v2_variables
-from .blocks import parse_block_additional_layers, get_block_out_quantizer
+from akida import SeparableConvolutional
+from quantizeml.layers import (QuantizedSeparableConv2D, QuantizedGlobalAveragePooling2D,
+                               QuantizedMaxPool2D, QuantizedReLU, WeightQuantizer,
+                               AlignedWeightQuantizer)
+
+from ..akida_versions import AkidaVersion
+from .pooling import set_gap_variables_v1, gap_params_checks
+from .outputs import set_output_v1_variables
+from .padding import check_conv_and_max_pool_compatibility
+from .blocks import get_block_out_quantizer
+from .block_converter import BlockConverter, register_conversion_patterns
+from .conv_common import parse_sepconv_block, get_layer_by_type
+
+__all__ = ["SeparableConvBlockConverter"]
+
+_PATTERNS = [(QuantizedSeparableConv2D,), (QuantizedSeparableConv2D, QuantizedReLU),
+             (QuantizedSeparableConv2D, QuantizedGlobalAveragePooling2D, QuantizedReLU),
+             (QuantizedSeparableConv2D, QuantizedGlobalAveragePooling2D),
+             (QuantizedSeparableConv2D, QuantizedMaxPool2D, QuantizedReLU)]
 
 
-def _set_depthwise_conv2d_transpose_variables(layer_ak, layer_k):
-    """Computes and sets the variables for an Akida DepthwiseConv2DTranspose layer.
+def _set_sepconv_variables(ak_layer, k_layer):
+    """Computes and sets the variables for an Akida SeparableConvolutional layer.
 
     This function converts the variables of a Keras layer and sets them into
     the corresponding variables of the equivalent Akida layer.
 
     Args:
-        layer_ak (:obj:`akida.Layer`): the targeted akida layer.
-        layer_k (:obj:`tf.keras.Layer`): the source quantized layer.
+        ak_layer (:obj:`akida.Layer`): the targeted akida layer.
+        k_layer (:obj:`tf.keras.Layer`): the source quantized layer.
     """
-    assert isinstance(layer_k, QuantizedDepthwiseConv2DTranspose)
-    assert isinstance(layer_k.weight_quantizer, WeightQuantizer)
-    if layer_k.use_bias:
-        assert isinstance(layer_k.bias_quantizer, AlignedWeightQuantizer)
-
-    # Get the weights
-    weights = layer_k.weight_quantizer.qweights.value.fp.values.numpy()
-    layer_ak.variables["weights"] = weights.astype(np.int8)
-
-    # Set the bias (if there is one)
-    if layer_k.use_bias:
-        bias_quantizer = layer_k.bias_quantizer
-        bias = bias_quantizer.qweights.value.values.numpy().astype(np.int32)
-        bias_shift = bias_quantizer.shift.value.numpy().astype(np.uint8)
-
-        # Unshift the bias and store it
-        layer_ak.variables["bias"] = (bias >> bias_shift).astype(np.int8)
-        # Also store the bias shift
-        broadcast_and_set_variable(layer_ak.variables, "bias_shift", bias_shift)
-
-    # Set input shift
-    input_shift = getattr(layer_k, 'input_shift', None)
-    if input_shift is not None:
-        broadcast_and_set_variable(layer_ak.variables, "input_shift",
-                                   layer_k.input_shift.value.numpy().astype(np.uint8))
-
+    assert isinstance(k_layer.dw_weight_quantizer, WeightQuantizer)
+    assert isinstance(k_layer.pw_weight_quantizer, WeightQuantizer)
 
-def _parse_depthwise_conv2d_transpose(layer):
-    """Parses a quantizeml.QuantizedDepthwiseConv2DTranspose parameters.
-
-    Args:
-        layer (:obj:`tf.keras.Layer`): the layer to parse.
+    variables_ak = ak_layer.variables
 
-    Returns:
-        dict: the corresponding akida parameters.
-    """
-    assert isinstance(layer, QuantizedDepthwiseConv2DTranspose)
+    # Get the QuantizedSeparableConv2D weights
+    weights_ak = k_layer.dw_weight_quantizer.qweights.value.fp.values.numpy()
+    weights_pw_ak = k_layer.pw_weight_quantizer.qweights.value.fp.values.numpy()
+    # We require flip depthwise weights
+    weights_ak = np.flip(weights_ak, axis=[0, 1])
+
+    # Get the QuantizedSeparableConv2D bias
+    if k_layer.use_bias:
+        bias_quantizer = k_layer.bias_quantizer
+        assert isinstance(bias_quantizer, AlignedWeightQuantizer)
+        bias = bias_quantizer.qweights.value.values.numpy().astype(np.int32)
+        # Store bias into the threshold variable
+        variables_ak["threshold"] = -bias
 
-    # Make sure the DepthwiseConv2D kernel size and stride params are square
-    assert layer.kernel_size[0] == layer.kernel_size[1], (
-        "DepthwiseConv2DTranspose kernel_size should be square")
-    assert layer.strides[0] == layer.strides[1], (
-        "DepthwiseConv2DTranspose strides should be the same on both dimension")
-    assert layer.kernel_size[0] in [3, 4], (
-        "DepthwiseConv2DTranspose supports kernel_size of 3 or 4 only")
-    assert layer.strides[0] == 2, "DepthwiseConv2DTranspose supports stride 2 only"
-
-    # Padding value must be same
-    assert layer.padding == "same", "DepthwiseConv2DTranspose handles only 'same' padding"
-
-    # The only weight bitwidth supported is [4, 8]
-    weight_bits = layer.weight_quantizer.bitwidth
-    assert weight_bits in [4, 8]
-
-    # In quantizeml one bit is reserved for the sign in the buffer bitwidth
-    # variable, but in akida this value has to be added back to have the
-    # correct clipping.
-    buffer_bits = layer.buffer_bitwidth + 1
-
-    return dict(
-        kernel_size=layer.kernel_size[0],
-        buffer_bits=buffer_bits,
-        activation=False,
-        name=layer.name
-    )
+    variables_ak["weights"] = weights_ak.astype(np.int8)
+    variables_ak["weights_pw"] = weights_pw_ak.astype(np.int8)
 
 
-def convert_depthwise_conv2d_transpose_block(model_ak, layers):
-    """Converts a depthwise convolutional block into an akida DepthwiseConv2DTranspose layer.
+def convert_sepconv_block(model_ak, block):
+    """Converts a separable convolutional block into an akida v1 SeparableConvolutional layer.
 
     The expected sequence is:
 
-    - QuantizedDepthwiseConv2DTranspose,
-    - QuantizedReLU (optional).
+        - QuantizedSeparableConv2D,
+        - QuantizedMaxPooling2D or QuantizedGlobalAveragePooling2D (optional),
+        - QuantizedReLU (optional).
 
     Args:
-        model_ak (:obj:`akida.Model`): the target Akida model.
-        layers (list(:obj:`tf.keras.Layer`)): the block layers.
+        model_ak (:obj:`akida.Model`): the Akida model where the model will be added.
+        block (list(:obj:`tf.keras.Layer`)): the remaining model layers to convert.
 
     Returns:
-        int: the number of layers in the block or 0 if the first layer is not a
-        QuantizedDepthwiseConv2DTranspose.
+        bool: Returns True for a successful conversion.
     """
-    if len(layers) == 0 or not isinstance(layers[0], QuantizedDepthwiseConv2DTranspose):
-        return 0
-
-    if get_akida_version() == AkidaVersion.v1:
-        return 0
 
-    dw_conv = layers[0]
+    sepconv = block[0]
 
-    # Evaluate the depthwise convolutional transpose layer parameters
-    conv_params = _parse_depthwise_conv2d_transpose(dw_conv)
+    # Evaluate the separable convolutional layer parameters
+    sepconv_params = parse_sepconv_block(block)
 
-    # Identify the next layers
-    next_layers = parse_block_additional_layers(layers, conv_params)
+    # Create the Akida SeparableConvolutional layer
+    sepconv_ak = SeparableConvolutional(**sepconv_params)
 
-    layer_block = [dw_conv] + list(next_layers.values())
+    # Add layer to the model to build its internal variables
+    model_ak.add(sepconv_ak)
 
-    # Get block output quantizer
-    out_quantizer = get_block_out_quantizer(layer_block)
+    # Set variables
+    _set_sepconv_variables(sepconv_ak, sepconv)
+    # Get the optional GAP layer
+    pool_layer = get_layer_by_type(block, QuantizedGlobalAveragePooling2D)
+    if pool_layer:
+        set_gap_variables_v1(sepconv_ak, pool_layer)
 
-    # add output quantizer bitwidth parameter
+    # Get out_quantizer of the block.
+    out_quantizer = get_block_out_quantizer(block)
     if out_quantizer:
-        conv_params["output_bits"] = out_quantizer.bitwidth
-    else:
-        conv_params["output_bits"] = conv_params["buffer_bits"]
+        set_output_v1_variables(sepconv_ak, out_quantizer)
 
-    # Create Akida layer
-    dw_conv_ak = DepthwiseConv2DTranspose(**conv_params)
-    # Add layer to the model to build its internal variables
-    model_ak.add(dw_conv_ak)
+    return True
 
-    # Set base variables
-    _set_depthwise_conv2d_transpose_variables(dw_conv_ak, dw_conv)
 
-    # Set optional activation variables if we have a ReLU
-    relu_layer = next_layers.get(QuantizedReLU, None)
-    if relu_layer:
-        set_relu_variables(dw_conv_ak, relu_layer)
+class SeparableConvBlockConverter(BlockConverter):
+    """Main class that should be used to check if the sepconv block is compatible to an Akida v1
+    conversion and provides a method to convert it in an equivalent Akida SeparableConvolutional
+    layer.
+
+    Args:
+        block (list): list of quantizeml quantized layers.
+    """
+
+    def __init__(self, block):
+        super().__init__(block)
+        self._sepconv_additional_checks()
+
+    def _sepconv_additional_checks(self):
+        sep_conv = self._block[0]
+
+        # The only weight bitwidth supported is 4
+        weight_bits = sep_conv.dw_weight_quantizer.bitwidth
+        if weight_bits != 4:
+            raise ValueError("SeparableConvolutional layer can only handle weights with 4 bits."
+                             f" Received: {weight_bits}.")
+        if weight_bits != sep_conv.pw_weight_quantizer.bitwidth:
+            raise ValueError("SeparableConvolutional layer pointwise weights should also be 4 bits."
+                             f" Received: {sep_conv.pw_weight_quantizer.bitwidth}.")
+
+        pool_layer = get_layer_by_type(self._block, (QuantizedGlobalAveragePooling2D,
+                                                     QuantizedMaxPool2D))
+        if isinstance(pool_layer, QuantizedMaxPool2D):
+            check_conv_and_max_pool_compatibility(sep_conv, pool_layer)
+        elif isinstance(pool_layer, QuantizedGlobalAveragePooling2D):
+            gap_params_checks(pool_layer)
+
+    def convert(self, model_ak):
+        return convert_sepconv_block(model_ak, self._block)
 
-    # Set optional output_quantizer variables
-    if out_quantizer:
-        set_output_v2_variables(dw_conv_ak, out_quantizer)
 
-    return len(layer_block)
+# Register the valid input conv block pattern for Akida v1
+register_conversion_patterns(AkidaVersion.v1, _PATTERNS, SeparableConvBlockConverter)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/dequantizer.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/outputs.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,78 +10,82 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
-"""Functions to convert Dequantizer to Akida.
+"""Functions to update akida layer output variables from a keras OutputQuantizer.
 """
 import numpy as np
-
-import akida
-from quantizeml.layers import Dequantizer
-
+from quantizeml.layers import OutputQuantizer
+from quantizeml.tensors import pow2
 from .weights import broadcast_and_set_variable
-from ..akida_versions import AkidaVersion, get_akida_version
+from .blocks import get_block_out_quantizer
 
 
-def _set_dequantizer_variables(layer_ak, dequantizer):
-    """Computes and sets the dequantizer recorded variables into the akida layer
+def parse_output_bits(block, block_params):
+    """ Helper to set the block output bits in its corresponding dict block_params.
+    Note that this helper should be called only once the buffer_bits is set. What is normally done
+    when the main block layer is parsed.
 
     Args:
-        layer_ak (:obj:`akida.Layer`): the targeted akida layer.
-        dequantizer (:obj:`quantizeml.Dequantizer`): the source quantizeml layer.
+        block (list(:obj:`tf.keras.Layer`)): the layers block.
+        block_params (dict): the current block parameters.
     """
-    assert isinstance(dequantizer, Dequantizer)
-
-    # Extract the Dequantizer variables
-    frac_bits = dequantizer.frac_bits
-    scales = dequantizer.scales
-    if isinstance(frac_bits, (list, tuple)):
-        if len(frac_bits) > 1:
-            raise RuntimeError(f"Multi-inbounds in {dequantizer.name} is not supported.")
-        frac_bits = frac_bits[0]
-        scales = scales[0] if scales else None
-
-    # We project the frac_bits into the scales as:
-    #   new_scales = scales / 2 ** frac_bits
-    scales = scales.value if scales else 1.0
-    scales /= 2**frac_bits.value
-    scales = scales.numpy().astype(np.float32)
-
-    # Depending on ak_version:
-    layer_variables = layer_ak.variables
-    if get_akida_version() == AkidaVersion.v1:
-        # We should not modify the activation step if the model ends with an activation
-        if layer_ak.parameters.activation == 1:
-            return
-        # Project scales in the final layer activation step
-        params = ("act_step", layer_variables["act_step"] / scales)
+    # Get the layer block output_quantizer
+    out_quantizer = get_block_out_quantizer(block)
+    if out_quantizer:
+        block_params.update({"output_bits": out_quantizer.bitwidth})
     else:
-        # Set scales in the independant layer
-        assert layer_ak.parameters.layer_type == akida.LayerType.Dequantizer
-        params = ("scales", scales)
-    broadcast_and_set_variable(layer_variables, *params)
+        # Default to buffer bitwidth
+        block_params.update({'output_bits': block_params["buffer_bits"]})
 
 
-def convert_dequantizer(model_ak, layer_k):
-    """Converts Dequantizer layer and set its variables into the Akida model.
+def set_output_v1_variables(layer_ak, out_quantizer):
+    """Computes and sets the output variables in an akida v1 layer.
 
     Args:
-        model_ak (:obj:`akida.Model`): the model where the layer will be added.
-        layer_k (:obj:`tf.keras.Layer`): the quantizeml layer to convert.
+        layer_ak (:obj:`akida.Layer`): the targeted akida v1 layer.
+        out_quantizer (:obj:`quantizeml.OutputQuantizer`): the source output quantizer.
     """
-    if not isinstance(layer_k, Dequantizer):
-        raise TypeError(f"Layer {layer_k.name} was expected to be Dequantizer")
+    assert isinstance(out_quantizer, OutputQuantizer)
 
-    # Depending on ak_version:
-    if get_akida_version() == AkidaVersion.v1:
-        # Take the last layer to set variables
-        layer_ak = model_ak.layers[-1]
-    else:
-        # Create and add one akida.Dequantizer to the model
-        layer_ak = akida.Dequantizer(name=layer_k.name)
-        model_ak.add(layer_ak)
+    # Extract the OutputQuantizer variables
+    scales = out_quantizer.qscales.value.values
+    shift = out_quantizer.shift.value
+
+    # Quantizeml evaluates the outputs as: y = x * scales * 2^shift
+    # Calculate the float activation step, as the reciprocal of (scales * 2^shift)
+    scales_rec = (pow2(-shift) / scales).numpy().astype(np.float32)
+    # In akida 1.0, the outputs are evaluated as: y = x / act_step
+    layer_ak.variables["act_step"] = scales_rec
+    if layer_ak.parameters.activation:
+        # For activations, x is decreased by half the activations step before division
+        # to increase the precision. This is obtained by increasing the threshold.
+        layer_ak.variables["threshold"] += np.round(0.5 * scales_rec).astype(np.int32)
+        # Adjust activation step to match activation formula
+        act_bits = layer_ak.parameters.act_bits
+        layer_ak.variables["act_step"] *= 2 ** (act_bits - 4)
+
+
+def set_output_v2_variables(layer_ak, out_quantizer):
+    """Computes and sets the output variables in an akida v2 layer.
+
+    Args:
+        layer_ak (:obj:`akida.Layer`): the targeted akida v2 layer.
+        out_quantizer (:obj:`quantizeml.OutputQuantizer`): the source output quantizer.
+    """
+    assert isinstance(out_quantizer, OutputQuantizer)
 
-    # Set variables into the akida layer
-    _set_dequantizer_variables(layer_ak, layer_k)
+    # Extract the OutputQuantizer variables.
+    # Note that qscales exist only if the out_quantizer was used on QFloat (not FixedPoint as in
+    # the QuantizedAdd layer)
+    if hasattr(out_quantizer, 'qscales'):
+        scales = out_quantizer.qscales.value.values
+        output_scales = scales.numpy().astype(np.uint8)
+        broadcast_and_set_variable(layer_ak.variables, "output_scales",
+                                   output_scales)
+
+    shift = out_quantizer.shift.value
+    broadcast_and_set_variable(layer_ak.variables, "output_shift",
+                               shift.numpy().astype(np.int8))
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/extract_token.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/extract_token.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,58 +16,104 @@
 # ******************************************************************************
 """Functions to convert QuantizedExtractToken to Akida.
 """
 from akida import ExtractToken
 import quantizeml.layers as qlayers
 
 from .layer_utils import get_inbound_layers
+from .block_converter import BlockConverter, register_conversion_patterns
+from ..akida_versions import AkidaVersion
 
 
-def _create_extract_token(layer):
-    """Parses a quantizeml QuantizedExtractToken layer and returns the
-    params to create the corresponding Akida ExtractToken layer.
+__all__ = ["ExtractTokenBlockConverter"]
+
+_PATTERNS = [(qlayers.QuantizedExtractToken,)]
+
+
+def _get_layer_token_range(layer):
+    """Helper to extract the layer token range.
 
     Args:
-        layer (:obj:`tf.keras.Layer`): the quantizeml QuantizedExtractToken
-            layer to convert.
+        layer (:obj:`tf.keras.Layer`): the quantizeml QuantizedExtractToken layer.
 
     Returns:
-        :obj:`akida.MadNorm`: The created akida layer.
+        tuple, list: token range of the layer in the following format ((begin, end), token_range).
     """
     assert isinstance(layer, qlayers.QuantizedExtractToken)
-
     # Akida is capable of supporting only a given combination of token
     if isinstance(layer.token, int):
         token_range = [layer.token]
     else:
         token_range = [*layer.token]
-    # Check range is continuous
     begin = min(token_range)
     end = max(token_range) + 1
-    continuous = sorted(token_range) == list(range(begin, end))
-    if not continuous:
-        raise ValueError(f"Argument token in {layer.name} should contain a "
-                         "continuous range")
+
+    return (begin, end), token_range
+
+
+def _create_extract_token(block):
+    """Parses a quantizeml QuantizedExtractToken layer and returns the
+    params to create the corresponding Akida v2 ExtractToken layer.
+
+    Args:
+        block (list(:obj:`tf.keras.Layer`)): the block of keras layers.
+
+    Returns:
+        :obj:`akida.ExtractToken`: The created akida layer.
+    """
+    (begin, end), _ = _get_layer_token_range(block[0])
+
     extract_token = ExtractToken(begin=begin,
                                  end=end,
-                                 name=layer.name)
+                                 name=block[0].name)
     return extract_token
 
 
-def convert_extract_token(model_ak, layer_k):
+def convert_extract_token(model_ak, block):
     """Converts QuantizedExtractToken layer and adds it to the Akida's model.
 
     Args:
         model_ak (:obj:`akida.Model`): the Akida model where the model will be
             added.
-        layer_k (:obj:`tf.keras.Layer`): the quantizeml QuantizedExtractToken
-            layer to convert.
+        block (list(:obj:`tf.keras.Layer`)): the block of keras layers.
+
+    Returns:
+        bool: Returns True for a successful conversion.
     """
-    if not isinstance(layer_k, qlayers.QuantizedExtractToken):
-        raise TypeError(f"Layer {layer_k.name} was expected to be "
-                        "QuantizedExtractToken")
+
     # Retrieve the akida inbound layers
-    inbound_layers_ak = get_inbound_layers(model_ak, layer_k)
+    inbound_layers_ak = get_inbound_layers(model_ak, block[0])
     # Create and add layer to the akida model
     # It is quite simple because there are no variables or params to be set.
-    layer_ak = _create_extract_token(layer_k)
+    layer_ak = _create_extract_token(block)
     model_ak.add(layer_ak, inbound_layers_ak)
+    return True
+
+
+class ExtractTokenBlockConverter(BlockConverter):
+    """Main class that should be used to check if the extract token layer block is compatible to an
+    Akida v2 conversion and provides a method to convert it in an equivalent Akida ExtractToken
+    layer.
+
+    Args:
+        block (list): list of quantizeml quantized layers.
+    """
+
+    def __init__(self, block):
+        super().__init__(block)
+        self._extract_token_additional_checks()
+
+    def _extract_token_additional_checks(self):
+        layer = self._block[0]
+        (begin, end), token_range = _get_layer_token_range(layer)
+        # Check range is continuous
+        continuous = sorted(token_range) == list(range(begin, end))
+        if not continuous:
+            raise ValueError(f"Argument token in {layer.name} should contain a "
+                             "continuous range")
+
+    def convert(self, model_ak):
+        return convert_extract_token(model_ak, self._block)
+
+
+# Register the valid extract token block pattern for Akida v2
+register_conversion_patterns(AkidaVersion.v2, _PATTERNS, ExtractTokenBlockConverter)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/input_data.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/input_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 """
 from keras.layers import InputLayer
 from akida import Model, InputData
 
 from ..akida_versions import AkidaVersion, get_akida_version
 
 
-def _create_input_data(layer, input_is_image):
+def _create_input_data(layer):
     """Parses a keras InputLayer layer and returns the corresponding Akida
     InputData layer.
 
     Args:
         layer (:obj:`tf.keras.Layer`): the InputLayer to convert.
-        input_is_image (bool): True if input is an 8-bit unsigned tensors (like images).
 
     Returns:
         akida.InputData: The parsed layer.
     """
     if not isinstance(layer, InputLayer):
         raise TypeError(f"Layer {layer.name} was expected to be "
                         "InputLayer")
@@ -50,34 +49,32 @@
 
     # Create a list with 1 for each dimension that we miss before having 3
     # dims, that is what akida expects
     missing_dimensions = [1] * (3 - len(input_shape))
     input_shape = [*missing_dimensions, *input_shape]
     # the akida version determines the input_bits
     input_bits = 4 if get_akida_version() == AkidaVersion.v1 else 8
-    # if input_is_image is set to True the input is unsigned.
-    input_signed = not input_is_image
+    # With the convert api of cnn2snn the model should handle only unsigned inputs.
     return InputData(input_shape=input_shape,
                      input_bits=input_bits,
-                     input_signed=input_signed,
+                     input_signed=False,
                      name=layer.name)
 
 
-def convert_input(model_ak, layer_k, input_is_image):
+def convert_input(model_ak, layer_k):
     """Converts a keras Input layer into ``akida.InputData`` and add it to the
     Akida's model.
 
     Args:
         model_ak (:obj:`akida.Model`): the Akida model where the model will be added.
         layer_k (:obj:`keras.Layer`): the InputLayer layer to convert.
-        input_is_image (bool): True if input is an 8-bit unsigned tensors.
     """
     if not isinstance(layer_k, InputLayer):
         raise TypeError(f"Layer {layer_k.name} was expected to be "
                         "InputLayer")
     if not isinstance(model_ak, Model):
         raise TypeError(f"Expecting an akida model, received {type(model_ak)}")
     if len(model_ak.layers) != 0:
         raise TypeError("Akida model should be empty")
 
-    input_data = _create_input_data(layer_k, input_is_image)
+    input_data = _create_input_data(layer_k)
     model_ak.add(input_data)
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/layer_utils.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/layer_utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/padding.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/padding.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,14 +53,31 @@
     return _get_padding(padding), padding_ak_value
 
 
 def check_same_valid_compatibility(layer):
     """Check if a layer produces the same output regardless of its padding ('same' or 'valid').
 
     Args:
-        layer (tf.keras.layers.Layer): Layer to verify
+        layer (:obj:`akida.Layer`): Layer to verify
 
     Returns:
         bool: same/valid compatibility result.
     """
     # Layer produces same output when kernel size == 1
     return layer.kernel_size == (1, 1)
+
+
+def check_conv_and_max_pool_compatibility(conv_layer, max_pool_layer):
+    """Check if a conv layer and the following max_pool_layer are compatible for a conversion.
+    Raise an error if not.
+
+    Args:
+        conv_layer (:obj:`akida.Layer`): QuantizedConv2D layer to verify.
+        max_pool_layer (:obj:`akida.Layer`): QuantizedMaxPool2D layer to verify.
+
+    """
+
+    neur_pad = conv_layer.padding if not check_same_valid_compatibility(conv_layer) else "same"
+    pool_pad = getattr(max_pool_layer, "padding", "")
+    if neur_pad != pool_pad:
+        raise ValueError(f"Pooling layer {max_pool_layer.name} (padding: {pool_pad}) must"
+                         f" have the same padding as {conv_layer.name} (padding: {neur_pad}).")
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/pooling.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/pooling.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """Functions to convert keras pooling layers parameters to akida.
 """
 
-from quantizeml.layers import QuantizedMaxPool2D, QuantizedGlobalAveragePooling2D, OutputQuantizer
+from quantizeml.layers import QuantizedMaxPool2D
 from akida import Padding, PoolType
-from ..akida_versions import AkidaVersion, get_akida_version
 
 
-def parse_max_pooling(layer):
-    """Parses a quantizeml.QuantizedMaxPool2D parameters.
+def parse_max_pool_v1(layer):
+    """Parses a quantizeml.QuantizedMaxPool2D parameters for Akida v1.
 
     Args:
         layer (:obj:`quantizeml.QuantizedMaxPool2D`): the layer to parse.
 
     Returns:
         dict: the corresponding akida parameters.
     """
@@ -40,62 +39,85 @@
     pool_params = dict(
         pool_type=PoolType.Max,
         padding=padding,
         pool_size=pool_size,
         pool_stride=pool_stride
     )
 
-    if get_akida_version() == AkidaVersion.v2:
-
-        # Make sure the Conv2D layers spatial params are square
-        assert pool_size[0] == pool_size[1], "Akida v2 layers only handle square pooling"
-        pool_params.update({"pool_size": pool_size[0]})
-        assert pool_stride[0] == pool_stride[1], (
-            "Akida v2 layers pooling stride should be the same for both dimensions")
-        pool_params.update({"pool_stride": pool_stride[0]})
-
     return pool_params
 
 
-def parse_global_average_pooling(layer):
-    """Parses a quantizeml.QuantizedGlobalAveragePooling2D parameters.
+def parse_max_pool_v2(layer):
+    """Parses a quantizeml.QuantizedMaxPool2D parameters for Akida v2.
 
     Args:
-        layer (:obj:`quantizeml.QuantizedGlobalAveragePooling2D`): the layer to parse.
+        layer (:obj:`quantizeml.QuantizedMaxPool2D`): the layer to parse.
 
     Returns:
         dict: the corresponding akida parameters.
     """
-    assert isinstance(layer, QuantizedGlobalAveragePooling2D)
-
-    if get_akida_version() == AkidaVersion.v1:
-        return dict(pool_type=PoolType.Average)
+    assert isinstance(layer, QuantizedMaxPool2D)
 
-    # Check if there is an output_quantizer
-    out_quantizer = getattr(layer, "out_quantizer", None)
+    padding = Padding.Same if layer.padding == "same" else Padding.Valid
+    pool_size = layer.pool_size
+    pool_stride = layer.strides if layer.strides else pool_size
 
-    assert isinstance(out_quantizer, OutputQuantizer)
+    pool_params = dict(
+        pool_type=PoolType.Max,
+        padding=padding,
+        pool_size=pool_size[0],
+        pool_stride=pool_stride[0]
+    )
 
-    return dict(pool_type=PoolType.Average, output_bits=out_quantizer.bitwidth)
+    return pool_params
 
 
-def set_pooling_variables(layer_ak, layer_k):
-    """Computes and sets the pooling variables in an akida layer.
+def set_gap_variables_v1(layer_ak, gap_layer):
+    """Computes and sets the pooling variables in an akida v1 layer.
 
     Args:
         layer_ak (:obj:`akida.Layer`): the targeted akida layer.
-        layer_k (:obj:`quantizeml.Layer`): the source layer.
+        gap_layer (:obj:`quantizeml.Layer`): the source layer.
     """
-    assert isinstance(layer_k, (QuantizedGlobalAveragePooling2D, QuantizedMaxPool2D))
-    # Nothing to do in AkidaVersion.v2 or for QuantizedMaxPool2D
-    if get_akida_version() == AkidaVersion.v2 or isinstance(layer_k, QuantizedMaxPool2D):
-        return
 
     # In AkidaVersion.v1, biases are only applied when evaluating activations, by
     # subtracting the threshold. Since this happens after pooling, the scaling factor
     # introduced by the GAP operation must be applied to the threshold.
-    spatial_size = layer_k.input_shape[1] * layer_k.input_shape[2]
+    spatial_size = gap_layer.input_shape[1] * gap_layer.input_shape[2]
+    layer_ak.variables["threshold"] *= spatial_size
+
+
+def max_pool_param_checks(max_pool_layer):
+    """Check if the max_pool_layer has valid parameters for an Akida v2 conversion.
+    Raise an error if not.
+
+    Args:
+        max_pool_layer (:obj:`akida.Layer`): QuantizedMaxPool2D layer to verify.
+
+    """
+    # if max_pool strides are None max_pool.strides == max_pool.pool_size => Valid assertion
+    if max_pool_layer.strides is None:
+        return
+
+    pool_size = max_pool_layer.pool_size
+    pool_stride = max_pool_layer.strides
+    if pool_size[0] != pool_size[1]:
+        raise ValueError(f"In Akida v2 {max_pool_layer.name} should have square pooling")
+    if pool_stride[0] != pool_stride[1]:
+        raise ValueError(f"In Akida v2 {max_pool_layer.name} pooling stride should be the same for"
+                         "both dimensions")
+
+
+def gap_params_checks(gap_layer):
+    """Check if the gap layer has valid parameters for an Akida v1 conversion.
+    Raise an error if not.
+
+    Args:
+        gap_layer (:obj:`akida.Layer`): QuantizedGlobalAveragePooling2D layer to verify.
+
+    """
+
+    spatial_size = gap_layer.input_shape[1] * gap_layer.input_shape[2]
     if spatial_size > 2**8:
         raise RuntimeError(f"Unsupported spatial size product ({spatial_size}). "
                            "We only accepts values smaller than 256. "
                            "Consider to replace GlobalAveragePooling2D by MaxPooling2D.")
-    layer_ak.variables["threshold"] *= spatial_size
```

### Comparing `cnn2snn-2.3.7/cnn2snn/quantizeml/weights.py` & `cnn2snn-2.4.0/cnn2snn/quantizeml/weights.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/transforms/__init__.py` & `cnn2snn-2.4.0/cnn2snn/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/transforms/batch_normalization.py` & `cnn2snn-2.4.0/cnn2snn/transforms/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/transforms/clone.py` & `cnn2snn-2.4.0/cnn2snn/transforms/clone.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/transforms/equalization.py` & `cnn2snn-2.4.0/cnn2snn/transforms/equalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/transforms/reshape.py` & `cnn2snn-2.4.0/cnn2snn/transforms/reshape.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/transforms/sequential.py` & `cnn2snn-2.4.0/cnn2snn/transforms/sequential.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/utils.py` & `cnn2snn-2.4.0/cnn2snn/utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn/weights_ops.py` & `cnn2snn-2.4.0/cnn2snn/weights_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.7/cnn2snn.egg-info/PKG-INFO` & `cnn2snn-2.4.0/cnn2snn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.3.7
+Version: 2.4.0
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Alvaro Moran
 Author-email: amoran@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnn2snn-2.3.7/cnn2snn.egg-info/SOURCES.txt` & `cnn2snn-2.4.0/cnn2snn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,22 @@
 cnn2snn/quantizeml/attention.py
 cnn2snn/quantizeml/batchnorm.py
 cnn2snn/quantizeml/block_converter.py
 cnn2snn/quantizeml/blocks.py
 cnn2snn/quantizeml/compatibility_checks.py
 cnn2snn/quantizeml/concatenate.py
 cnn2snn/quantizeml/conv2d_transpose.py
+cnn2snn/quantizeml/conv_common.py
 cnn2snn/quantizeml/convolution.py
 cnn2snn/quantizeml/dense.py
 cnn2snn/quantizeml/depthwise_conv2d.py
 cnn2snn/quantizeml/depthwise_conv2d_transpose.py
 cnn2snn/quantizeml/dequantizer.py
 cnn2snn/quantizeml/extract_token.py
+cnn2snn/quantizeml/input_conv.py
 cnn2snn/quantizeml/input_data.py
 cnn2snn/quantizeml/layer_utils.py
 cnn2snn/quantizeml/madnorm.py
 cnn2snn/quantizeml/model_generator.py
 cnn2snn/quantizeml/outputs.py
 cnn2snn/quantizeml/padding.py
 cnn2snn/quantizeml/pooling.py
```

### Comparing `cnn2snn-2.3.7/setup.py` & `cnn2snn-2.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 
 def get_tf_dep():
   platform_string = platform()
   if 'macOS' in platform_string and 'arm64' in platform_string:
     tf_name = 'tensorflow-macos'
   else:
     tf_name = 'tensorflow'
-  return tf_name + '~=2.10.0'
+  return tf_name + '>=2.10.0,<2.13.0'
 
 
 # Read the contents of the README file
 directory = path.abspath(path.dirname(__file__))
 with open(path.join(directory, 'README'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cnn2snn',
-    version='2.3.7',
+    version='2.4.0',
     description='Keras to Akida CNN Converter',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alvaro Moran',
     author_email='amoran@brainchip.com',
     url='https://doc.brainchipinc.com',
     license='Apache 2.0',
     packages=['cnn2snn', 'cnn2snn.transforms', 'cnn2snn.calibration', 'cnn2snn.quantizeml'],
     entry_points={
         'console_scripts': [ 'cnn2snn = cnn2snn.cli:main' ]
     },
-    install_requires=[get_tf_dep(), 'keras~=2.10.0',
-        'akida==2.3.7', 'quantizeml~=0.4.1'],
+    install_requires=[get_tf_dep(), 'keras>=2.10.0,<2.13.0',
+        'akida==2.4.0', 'quantizeml~=0.5.0'],
 )
```

