# Comparing `tmp/piq-0.7.1.tar.gz` & `tmp/piq-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piq-0.7.1.tar", last modified: Tue Apr 18 17:47:37 2023, max compression
+gzip compressed data, was "piq-0.8.0.tar", last modified: Tue Jul  4 21:28:02 2023, max compression
```

## Comparing `piq-0.7.1.tar` & `piq-0.8.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.079668 piq-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 17:47:25.000000 piq-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-04-18 17:47:37.079668 piq-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-04-18 17:47:25.000000 piq-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.075668 piq-0.7.1/piq/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-18 17:47:25.000000 piq-0.7.1/piq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-18 17:47:25.000000 piq-0.7.1/piq/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-04-18 17:47:25.000000 piq-0.7.1/piq/brisque.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-04-18 17:47:25.000000 piq-0.7.1/piq/dss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.075668 piq-0.7.1/piq/feature_extractors/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 17:47:25.000000 piq-0.7.1/piq/feature_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-04-18 17:47:25.000000 piq-0.7.1/piq/feature_extractors/fid_inception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-18 17:47:25.000000 piq-0.7.1/piq/fid.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-04-18 17:47:25.000000 piq-0.7.1/piq/fsim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.075668 piq-0.7.1/piq/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/colour_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-04-18 17:47:25.000000 piq-0.7.1/piq/gmsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-18 17:47:25.000000 piq-0.7.1/piq/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-18 17:47:25.000000 piq-0.7.1/piq/haarpsi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-18 17:47:25.000000 piq-0.7.1/piq/isc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-04-18 17:47:25.000000 piq-0.7.1/piq/iw_ssim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-18 17:47:25.000000 piq-0.7.1/piq/kid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-04-18 17:47:25.000000 piq-0.7.1/piq/mdsi.py
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-04-18 17:47:25.000000 piq-0.7.1/piq/ms_ssim.py
--rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-04-18 17:47:25.000000 piq-0.7.1/piq/msid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20112 2023-04-18 17:47:25.000000 piq-0.7.1/piq/perceptual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-18 17:47:25.000000 piq-0.7.1/piq/pieapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-18 17:47:25.000000 piq-0.7.1/piq/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-18 17:47:25.000000 piq-0.7.1/piq/psnr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-04-18 17:47:25.000000 piq-0.7.1/piq/srsim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-18 17:47:25.000000 piq-0.7.1/piq/ssim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-18 17:47:25.000000 piq-0.7.1/piq/tv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.075668 piq-0.7.1/piq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-18 17:47:25.000000 piq-0.7.1/piq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-18 17:47:25.000000 piq-0.7.1/piq/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-04-18 17:47:25.000000 piq-0.7.1/piq/vif.py
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-18 17:47:25.000000 piq-0.7.1/piq/vsi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.075668 piq-0.7.1/piq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-04-18 17:47:37.000000 piq-0.7.1/piq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-18 17:47:37.000000 piq-0.7.1/piq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:47:37.000000 piq-0.7.1/piq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 17:47:37.000000 piq-0.7.1/piq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 17:47:37.000000 piq-0.7.1/piq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 17:47:37.079668 piq-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-18 17:47:25.000000 piq-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:28:02.440847 piq-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 21:27:48.000000 piq-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-07-04 21:28:02.436846 piq-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-07-04 21:27:48.000000 piq-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:28:02.436846 piq-0.8.0/piq/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-04 21:27:48.000000 piq-0.8.0/piq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-04 21:27:48.000000 piq-0.8.0/piq/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-07-04 21:27:48.000000 piq-0.8.0/piq/brisque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-04 21:27:48.000000 piq-0.8.0/piq/clip_iqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-07-04 21:27:48.000000 piq-0.8.0/piq/dss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:28:02.436846 piq-0.8.0/piq/feature_extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-04 21:27:48.000000 piq-0.8.0/piq/feature_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22866 2023-07-04 21:27:48.000000 piq-0.8.0/piq/feature_extractors/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-07-04 21:27:48.000000 piq-0.8.0/piq/feature_extractors/fid_inception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-07-04 21:27:48.000000 piq-0.8.0/piq/fid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-07-04 21:27:48.000000 piq-0.8.0/piq/fsim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:28:02.436846 piq-0.8.0/piq/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-04 21:27:48.000000 piq-0.8.0/piq/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-04 21:27:48.000000 piq-0.8.0/piq/functional/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-04 21:27:48.000000 piq-0.8.0/piq/functional/colour_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-04 21:27:48.000000 piq-0.8.0/piq/functional/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 21:27:48.000000 piq-0.8.0/piq/functional/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-07-04 21:27:48.000000 piq-0.8.0/piq/functional/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-07-04 21:27:48.000000 piq-0.8.0/piq/gmsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-07-04 21:27:48.000000 piq-0.8.0/piq/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-04 21:27:48.000000 piq-0.8.0/piq/haarpsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-04 21:27:48.000000 piq-0.8.0/piq/isc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-07-04 21:27:48.000000 piq-0.8.0/piq/iw_ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-07-04 21:27:48.000000 piq-0.8.0/piq/kid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-04 21:27:48.000000 piq-0.8.0/piq/mdsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-07-04 21:27:48.000000 piq-0.8.0/piq/ms_ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-07-04 21:27:48.000000 piq-0.8.0/piq/msid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20112 2023-07-04 21:27:48.000000 piq-0.8.0/piq/perceptual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-04 21:27:48.000000 piq-0.8.0/piq/pieapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-04 21:27:48.000000 piq-0.8.0/piq/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-04 21:27:48.000000 piq-0.8.0/piq/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-04 21:27:48.000000 piq-0.8.0/piq/srsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-07-04 21:27:48.000000 piq-0.8.0/piq/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-04 21:27:48.000000 piq-0.8.0/piq/tv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:28:02.436846 piq-0.8.0/piq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 21:27:48.000000 piq-0.8.0/piq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-07-04 21:27:48.000000 piq-0.8.0/piq/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-04 21:27:48.000000 piq-0.8.0/piq/vif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-04 21:27:48.000000 piq-0.8.0/piq/vsi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:28:02.436846 piq-0.8.0/piq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-07-04 21:28:02.000000 piq-0.8.0/piq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-04 21:28:02.000000 piq-0.8.0/piq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:28:02.000000 piq-0.8.0/piq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 21:28:02.000000 piq-0.8.0/piq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-04 21:28:02.000000 piq-0.8.0/piq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 21:28:02.440847 piq-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-04 21:27:48.000000 piq-0.8.0/setup.py
```

### Comparing `piq-0.7.1/LICENSE` & `piq-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/PKG-INFO` & `piq-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piq
-Version: 0.7.1
+Version: 0.8.0
 Summary: Measures and metrics for image2image tasks. PyTorch.
 Home-page: https://github.com/photosynthesis-team/piq
 Author: Sergey Kastryulin
 Author-email: snk4tr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -184,34 +184,35 @@
 SSIM         2003    `Structural Similarity <https://en.wikipedia.org/wiki/Structural_similarity>`_
 MS-SSIM      2004    `Multi-Scale Structural Similarity <https://ieeexplore.ieee.org/abstract/document/1292216>`_
 IW-SSIM      2011    `Information Content Weighted Structural Similarity Index <https://ece.uwaterloo.ca/~z70wang/publications/IWSSIM.pdf>`_
 VIFp         2004    `Visual Information Fidelity <https://ieeexplore.ieee.org/document/1576816>`_
 FSIM         2011    `Feature Similarity Index Measure <https://ieeexplore.ieee.org/document/5705575>`_
 SR-SIM       2012    `Spectral Residual Based Similarity <https://sse.tongji.edu.cn/linzhang/ICIP12/ICIP-SR-SIM.pdf>`_
 GMSD         2013    `Gradient Magnitude Similarity Deviation <https://arxiv.org/abs/1308.3052>`_
+MS-GMSD      2017    `Multi-Scale Gradient Magnitude Similarity Deviation <https://ieeexplore.ieee.org/document/7952357>`_
 VSI          2014    `Visual Saliency-induced Index <https://ieeexplore.ieee.org/document/6873260>`_
 DSS          2015    `DCT Subband Similarity Index <https://ieeexplore.ieee.org/document/7351172>`_
 \-           2016    `Content Score <https://arxiv.org/abs/1508.06576>`_
 \-           2016    `Style Score <https://arxiv.org/abs/1508.06576>`_
 HaarPSI      2016    `Haar Perceptual Similarity Index <https://arxiv.org/abs/1607.06140>`_
 MDSI         2016    `Mean Deviation Similarity Index <https://arxiv.org/abs/1608.07433>`_
-MS-GMSD      2017    `Multi-Scale Gradient Magnitude Similarity Deviation <https://ieeexplore.ieee.org/document/7952357>`_
 LPIPS        2018    `Learned Perceptual Image Patch Similarity <https://arxiv.org/abs/1801.03924>`_
 PieAPP       2018    `Perceptual Image-Error Assessment through Pairwise Preference <https://arxiv.org/abs/1806.02067>`_
 DISTS        2020    `Deep Image Structure and Texture Similarity <https://arxiv.org/abs/2004.07728>`_
 ===========  ======  ==========
 
 No-Reference (NR)
 ^^^^^^^^^^^^^^^^^
 
 ===========  ======  ==========
 Acronym      Year    Metric
 ===========  ======  ==========
 TV           1937    `Total Variation <https://en.wikipedia.org/wiki/Total_variation>`_
 BRISQUE      2012    `Blind/Referenceless Image Spatial Quality Evaluator <https://ieeexplore.ieee.org/document/6272356>`_
+CLIP-IQA     2022    `CLIP-IQA <https://arxiv.org/pdf/2207.12396.pdf>`_
 ===========  ======  ==========
 
 Distribution-Based (DB)
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 ===========  ======  ==========
 Acronym      Year    Metric
@@ -228,32 +229,34 @@
 
 .. benchmark-section-start
 
 Benchmark
 ---------
 
 As part of our library we provide `code to benchmark <tests/results_benchmark.py>`_ all metrics on a set of common Mean Opinon Scores databases.
-Currently we support `TID2013`_,  `KADID10k`_ and `PIPAL`_.
+Currently we support several Full-Reference (`TID2013`_,  `KADID10k`_ and `PIPAL`_) and No-Reference (`KonIQ10k`_ and `LIVE-itW`_) datasets.
 You need to download them separately and provide path to images as an argument to the script.
 
 Here is an example how to evaluate SSIM and MS-SSIM metrics on TID2013 dataset:
 
 .. code-block:: bash
 
    python3 tests/results_benchmark.py --dataset tid2013 --metrics SSIM MS-SSIM --path ~/datasets/tid2013 --batch_size 16
 
-Below we provide a comparison between `Spearman's Rank Correlation cCoefficient <https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient>`_ (SRCC) values obtained with PIQ and reported in surveys.
+Below we provide a comparison between `Spearman's Rank Correlation Coefficient <https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient>`_ (SRCC) values obtained with PIQ and reported in surveys.
 Closer SRCC values indicate the higher degree of agreement between results of computations on given datasets.
 We do not report `Kendall rank correlation coefficient <https://en.wikipedia.org/wiki/Kendall_rank_correlation_coefficient>`_ (KRCC)
 as it is highly correlated with SRCC and provides limited additional information.
 We do not report `Pearson linear correlation coefficient <https://en.wikipedia.org/wiki/Pearson_correlation_coefficient>`_ (PLCC)
 as it's highly dependent on fitting method and is biased towards simple examples.
 
 For metrics that can take greyscale or colour images, ``c`` means chromatic version.
 
+Full-Reference (FR) Datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 ===========  ===========================  ===========================  ===========================
      \                  TID2013                    KADID10k                       PIPAL
 -----------  ---------------------------  ---------------------------  ---------------------------
   Source            PIQ / Reference            PIQ / Reference                PIQ / Reference
 ===========  ===========================  ===========================  ===========================
 PSNR         0.69 / 0.69 `TID2013`_       0.68 / -                     0.41 / 0.41 `PIPAL`_
 SSIM         0.72 / 0.64 `TID2013`_       0.72 / 0.72 `KADID10k`_      0.50 / 0.53 `PIPAL`_
@@ -273,30 +276,45 @@
 MDSI         0.89 / 0.89 `MDSI`_          0.89 / 0.89 `KADID10k`_      0.59 / -
 MS-GMSD      0.81 / 0.81 `MS-GMSD`_       0.85 / -                     0.59 / -
 MS-GMSDc     0.89 / 0.89 `MS-GMSD`_       0.87 / -                     0.59 / -
 LPIPS-VGG    0.67 / 0.67 `DISTS`_         0.72 / -                     0.57 / 0.58 `PIPAL`_
 PieAPP       0.84 / 0.88 `DISTS`_         0.87 / -                     0.70 / 0.71 `PIPAL`_
 DISTS        0.81 / 0.83 `DISTS`_         0.88 / -                     0.62 / 0.66 `PIPAL`_
 BRISQUE      0.37 / 0.84 `Eval2019`_      0.33 / 0.53 `KADID10k`_      0.21 / -
+CLIP-IQA     0.50 / -                     0.48 / -                     0.26 / -
 IS           0.26 / -                     0.25 / -                     0.09 / -
 FID          0.67 / -                     0.66 / -                     0.18 / -
 KID          0.42 / -                     0.66 / -                     0.12 / -
 MSID         0.21 / -                     0.32 / -                     0.01 / -
 GS           0.37 / -                     0.37 / -                     0.02 / -
 ===========  ===========================  ===========================  ===========================
 
+No-Reference (NR) Datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+===========  ===========================  ===========================
+     \                  KonIQ10k                    LIVE-itW
+-----------  ---------------------------  ---------------------------
+  Source            PIQ / Reference            PIQ / Reference
+===========  ===========================  ===========================
+BRISQUE      0.22 / -                     0.31 / -
+CLIP-IQA     0.68 / 0.68 `CLIP-IQA off`_  0.64 / 0.64 `CLIP-IQA off`_
+===========  ===========================  ===========================
+
 .. _TID2013: http://www.ponomarenko.info/tid2013.htm
 .. _KADID10k: http://database.mmsp-kn.de/kadid-10k-database.html
 .. _Eval2019: https://ieeexplore.ieee.org/abstract/document/8847307/
 .. _`MDSI`: https://arxiv.org/abs/1608.07433
 .. _MS-GMSD: https://ieeexplore.ieee.org/document/7952357
 .. _DISTS: https://arxiv.org/abs/2004.07728
 .. _HaarPSI: https://arxiv.org/abs/1607.06140
 .. _PIPAL: https://arxiv.org/pdf/2011.15002.pdf
 .. _IW-SSIM: https://ieeexplore.ieee.org/document/7442122
+.. _KonIQ10k: http://database.mmsp-kn.de/koniq-10k-database.html
+.. _LIVE-itW: https://live.ece.utexas.edu/research/ChallengeDB/index.html
+.. _CLIP-IQA off: https://github.com/IceClear/CLIP-IQA
 
 Unlike FR and NR IQMs, designed to compute an image-wise distance, the DB metrics compare distributions of *sets* of images.
 To address these problems, we adopt a different way of computing the DB IQMs proposed in `<https://arxiv.org/abs/2203.07809>`_.
 Instead of extracting features from the whole images, we crop them into overlapping tiles of size ``96 × 96`` with ``stride = 32``.
 This pre-processing allows us to treat each pair of images as a pair of distributions of tiles, enabling further comparison.
 The other stages of computing the DB IQMs are kept intact.
```

### Comparing `piq-0.7.1/README.rst` & `piq-0.8.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -171,34 +171,35 @@
 SSIM         2003    `Structural Similarity <https://en.wikipedia.org/wiki/Structural_similarity>`_
 MS-SSIM      2004    `Multi-Scale Structural Similarity <https://ieeexplore.ieee.org/abstract/document/1292216>`_
 IW-SSIM      2011    `Information Content Weighted Structural Similarity Index <https://ece.uwaterloo.ca/~z70wang/publications/IWSSIM.pdf>`_
 VIFp         2004    `Visual Information Fidelity <https://ieeexplore.ieee.org/document/1576816>`_
 FSIM         2011    `Feature Similarity Index Measure <https://ieeexplore.ieee.org/document/5705575>`_
 SR-SIM       2012    `Spectral Residual Based Similarity <https://sse.tongji.edu.cn/linzhang/ICIP12/ICIP-SR-SIM.pdf>`_
 GMSD         2013    `Gradient Magnitude Similarity Deviation <https://arxiv.org/abs/1308.3052>`_
+MS-GMSD      2017    `Multi-Scale Gradient Magnitude Similarity Deviation <https://ieeexplore.ieee.org/document/7952357>`_
 VSI          2014    `Visual Saliency-induced Index <https://ieeexplore.ieee.org/document/6873260>`_
 DSS          2015    `DCT Subband Similarity Index <https://ieeexplore.ieee.org/document/7351172>`_
 \-           2016    `Content Score <https://arxiv.org/abs/1508.06576>`_
 \-           2016    `Style Score <https://arxiv.org/abs/1508.06576>`_
 HaarPSI      2016    `Haar Perceptual Similarity Index <https://arxiv.org/abs/1607.06140>`_
 MDSI         2016    `Mean Deviation Similarity Index <https://arxiv.org/abs/1608.07433>`_
-MS-GMSD      2017    `Multi-Scale Gradient Magnitude Similarity Deviation <https://ieeexplore.ieee.org/document/7952357>`_
 LPIPS        2018    `Learned Perceptual Image Patch Similarity <https://arxiv.org/abs/1801.03924>`_
 PieAPP       2018    `Perceptual Image-Error Assessment through Pairwise Preference <https://arxiv.org/abs/1806.02067>`_
 DISTS        2020    `Deep Image Structure and Texture Similarity <https://arxiv.org/abs/2004.07728>`_
 ===========  ======  ==========
 
 No-Reference (NR)
 ^^^^^^^^^^^^^^^^^
 
 ===========  ======  ==========
 Acronym      Year    Metric
 ===========  ======  ==========
 TV           1937    `Total Variation <https://en.wikipedia.org/wiki/Total_variation>`_
 BRISQUE      2012    `Blind/Referenceless Image Spatial Quality Evaluator <https://ieeexplore.ieee.org/document/6272356>`_
+CLIP-IQA     2022    `CLIP-IQA <https://arxiv.org/pdf/2207.12396.pdf>`_
 ===========  ======  ==========
 
 Distribution-Based (DB)
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 ===========  ======  ==========
 Acronym      Year    Metric
@@ -215,32 +216,34 @@
 
 .. benchmark-section-start
 
 Benchmark
 ---------
 
 As part of our library we provide `code to benchmark <tests/results_benchmark.py>`_ all metrics on a set of common Mean Opinon Scores databases.
-Currently we support `TID2013`_,  `KADID10k`_ and `PIPAL`_.
+Currently we support several Full-Reference (`TID2013`_,  `KADID10k`_ and `PIPAL`_) and No-Reference (`KonIQ10k`_ and `LIVE-itW`_) datasets.
 You need to download them separately and provide path to images as an argument to the script.
 
 Here is an example how to evaluate SSIM and MS-SSIM metrics on TID2013 dataset:
 
 .. code-block:: bash
 
    python3 tests/results_benchmark.py --dataset tid2013 --metrics SSIM MS-SSIM --path ~/datasets/tid2013 --batch_size 16
 
-Below we provide a comparison between `Spearman's Rank Correlation cCoefficient <https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient>`_ (SRCC) values obtained with PIQ and reported in surveys.
+Below we provide a comparison between `Spearman's Rank Correlation Coefficient <https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient>`_ (SRCC) values obtained with PIQ and reported in surveys.
 Closer SRCC values indicate the higher degree of agreement between results of computations on given datasets.
 We do not report `Kendall rank correlation coefficient <https://en.wikipedia.org/wiki/Kendall_rank_correlation_coefficient>`_ (KRCC)
 as it is highly correlated with SRCC and provides limited additional information.
 We do not report `Pearson linear correlation coefficient <https://en.wikipedia.org/wiki/Pearson_correlation_coefficient>`_ (PLCC)
 as it's highly dependent on fitting method and is biased towards simple examples.
 
 For metrics that can take greyscale or colour images, ``c`` means chromatic version.
 
+Full-Reference (FR) Datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 ===========  ===========================  ===========================  ===========================
      \                  TID2013                    KADID10k                       PIPAL
 -----------  ---------------------------  ---------------------------  ---------------------------
   Source            PIQ / Reference            PIQ / Reference                PIQ / Reference
 ===========  ===========================  ===========================  ===========================
 PSNR         0.69 / 0.69 `TID2013`_       0.68 / -                     0.41 / 0.41 `PIPAL`_
 SSIM         0.72 / 0.64 `TID2013`_       0.72 / 0.72 `KADID10k`_      0.50 / 0.53 `PIPAL`_
@@ -260,30 +263,45 @@
 MDSI         0.89 / 0.89 `MDSI`_          0.89 / 0.89 `KADID10k`_      0.59 / -
 MS-GMSD      0.81 / 0.81 `MS-GMSD`_       0.85 / -                     0.59 / -
 MS-GMSDc     0.89 / 0.89 `MS-GMSD`_       0.87 / -                     0.59 / -
 LPIPS-VGG    0.67 / 0.67 `DISTS`_         0.72 / -                     0.57 / 0.58 `PIPAL`_
 PieAPP       0.84 / 0.88 `DISTS`_         0.87 / -                     0.70 / 0.71 `PIPAL`_
 DISTS        0.81 / 0.83 `DISTS`_         0.88 / -                     0.62 / 0.66 `PIPAL`_
 BRISQUE      0.37 / 0.84 `Eval2019`_      0.33 / 0.53 `KADID10k`_      0.21 / -
+CLIP-IQA     0.50 / -                     0.48 / -                     0.26 / -
 IS           0.26 / -                     0.25 / -                     0.09 / -
 FID          0.67 / -                     0.66 / -                     0.18 / -
 KID          0.42 / -                     0.66 / -                     0.12 / -
 MSID         0.21 / -                     0.32 / -                     0.01 / -
 GS           0.37 / -                     0.37 / -                     0.02 / -
 ===========  ===========================  ===========================  ===========================
 
+No-Reference (NR) Datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+===========  ===========================  ===========================
+     \                  KonIQ10k                    LIVE-itW
+-----------  ---------------------------  ---------------------------
+  Source            PIQ / Reference            PIQ / Reference
+===========  ===========================  ===========================
+BRISQUE      0.22 / -                     0.31 / -
+CLIP-IQA     0.68 / 0.68 `CLIP-IQA off`_  0.64 / 0.64 `CLIP-IQA off`_
+===========  ===========================  ===========================
+
 .. _TID2013: http://www.ponomarenko.info/tid2013.htm
 .. _KADID10k: http://database.mmsp-kn.de/kadid-10k-database.html
 .. _Eval2019: https://ieeexplore.ieee.org/abstract/document/8847307/
 .. _`MDSI`: https://arxiv.org/abs/1608.07433
 .. _MS-GMSD: https://ieeexplore.ieee.org/document/7952357
 .. _DISTS: https://arxiv.org/abs/2004.07728
 .. _HaarPSI: https://arxiv.org/abs/1607.06140
 .. _PIPAL: https://arxiv.org/pdf/2011.15002.pdf
 .. _IW-SSIM: https://ieeexplore.ieee.org/document/7442122
+.. _KonIQ10k: http://database.mmsp-kn.de/koniq-10k-database.html
+.. _LIVE-itW: https://live.ece.utexas.edu/research/ChallengeDB/index.html
+.. _CLIP-IQA off: https://github.com/IceClear/CLIP-IQA
 
 Unlike FR and NR IQMs, designed to compute an image-wise distance, the DB metrics compare distributions of *sets* of images.
 To address these problems, we adopt a different way of computing the DB IQMs proposed in `<https://arxiv.org/abs/2203.07809>`_.
 Instead of extracting features from the whole images, we crop them into overlapping tiles of size ``96 × 96`` with ``stride = 32``.
 This pre-processing allows us to treat each pair of images as a pair of distributions of tiles, enabling further comparison.
 The other stages of computing the DB IQMs are kept intact.
```

### Comparing `piq-0.7.1/piq/__init__.py` & `piq-0.8.0/piq/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.1"
+__version__ = "0.8.0"
 
 from .ssim import ssim, SSIMLoss
 from .ms_ssim import multi_scale_ssim, MultiScaleSSIMLoss
 from .msid import MSID
 from .fid import FID
 from .kid import KID
 from .pr import PR
@@ -18,7 +18,8 @@
 from .vsi import vsi, VSILoss
 from .mdsi import mdsi, MDSILoss
 from .haarpsi import haarpsi, HaarPSILoss
 from .srsim import srsim, SRSIMLoss
 from .pieapp import PieAPP
 from .dss import dss, DSSLoss
 from .iw_ssim import information_weighted_ssim, InformationWeightedSSIMLoss
+from .clip_iqa import CLIPIQA
```

### Comparing `piq-0.7.1/piq/base.py` & `piq-0.8.0/piq/base.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/brisque.py` & `piq-0.8.0/piq/brisque.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/dss.py` & `piq-0.8.0/piq/dss.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/feature_extractors/fid_inception.py` & `piq-0.8.0/piq/feature_extractors/fid_inception.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/fid.py` & `piq-0.8.0/piq/fid.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/fsim.py` & `piq-0.8.0/piq/fsim.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/functional/__init__.py` & `piq-0.8.0/piq/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/functional/base.py` & `piq-0.8.0/piq/functional/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 r"""General purpose functions"""
 from typing import Tuple, Union, Optional
 import torch
+from piq.utils import _parse_version
 
 
 def ifftshift(x: torch.Tensor) -> torch.Tensor:
     r""" Similar to np.fft.ifftshift but applies to PyTorch Tensors"""
     shift = [-(ax // 2) for ax in x.size()]
     return torch.roll(x, shift, tuple(range(len(shift))))
 
@@ -27,14 +28,19 @@
 
     if size[1] % 2:
         # Odd
         y = torch.arange(-(size[1] - 1) / 2, size[1] / 2, device=device, dtype=dtype) / (size[1] - 1)
     else:
         # Even
         y = torch.arange(- size[1] / 2, size[1] / 2, device=device, dtype=dtype) / size[1]
+    # Use indexing param depending on torch version
+    recommended_torch_version = _parse_version("1.10.0")
+    torch_version = _parse_version(torch.__version__)
+    if len(torch_version) > 0 and torch_version >= recommended_torch_version:
+        return torch.meshgrid(x, y, indexing='ij')
     return torch.meshgrid(x, y)
 
 
 def similarity_map(map_x: torch.Tensor, map_y: torch.Tensor, constant: float, alpha: float = 0.0) -> torch.Tensor:
     r""" Compute similarity_map between two tensors using Dice-like equation.
 
     Args:
```

### Comparing `piq-0.7.1/piq/functional/colour_conversion.py` & `piq-0.8.0/piq/functional/colour_conversion.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/functional/filters.py` & `piq-0.8.0/piq/functional/filters.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/functional/layers.py` & `piq-0.8.0/piq/functional/layers.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/functional/resize.py` & `piq-0.8.0/piq/functional/resize.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/gmsd.py` & `piq-0.8.0/piq/gmsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     y = y / float(data_range) * 255
 
     # Values from the paper
     if scale_weights is None:
         scale_weights = torch.tensor([0.096, 0.596, 0.289, 0.019], device=x.device, dtype=x.dtype)
     else:
         # Normalize scale weights
-        scale_weights = (scale_weights / scale_weights.sum())
+        scale_weights = scale_weights / scale_weights.sum()
 
     # Check that input is big enough
     num_scales = scale_weights.size(0)
     min_size = 2 ** num_scales + 1
 
     if x.size(-1) < min_size or x.size(-2) < min_size:
         raise ValueError(f'Invalid size of the input images, expected at least {min_size}x{min_size}.')
@@ -276,15 +276,19 @@
 
         # Generic loss parameters.
         self.reduction = reduction
 
         # Loss-specific parameters.
         self.data_range = data_range
 
-        self.scale_weights = scale_weights
+        if scale_weights is None:
+            self.register_buffer("scale_weights", torch.tensor([0.096, 0.596, 0.289, 0.019]))
+        else:
+            self.register_buffer("scale_weights", scale_weights)
+
         self.chromatic = chromatic
         self.alpha = alpha
         self.beta1 = beta1
         self.beta2 = beta2
         self.beta3 = beta3
         self.t = t
```

### Comparing `piq-0.7.1/piq/gs.py` & `piq-0.8.0/piq/gs.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/haarpsi.py` & `piq-0.8.0/piq/haarpsi.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/isc.py` & `piq-0.8.0/piq/isc.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/iw_ssim.py` & `piq-0.8.0/piq/iw_ssim.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/kid.py` & `piq-0.8.0/piq/kid.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/mdsi.py` & `piq-0.8.0/piq/mdsi.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/ms_ssim.py` & `piq-0.8.0/piq/ms_ssim.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     y = y / float(data_range)
 
     if scale_weights is None:
         # Values from MS-SSIM the paper
         scale_weights = torch.tensor([0.0448, 0.2856, 0.3001, 0.2363, 0.1333], dtype=x.dtype, device=x.device)
     else:
         # Normalize scale weights
-        scale_weights = (scale_weights / scale_weights.sum())
+        scale_weights = scale_weights / scale_weights.sum()
     if scale_weights.size(0) != scale_weights.numel():
         raise ValueError(f'Expected a vector of weights, got {scale_weights.dim()}D tensor')
 
     kernel = gaussian_filter(kernel_size, kernel_sigma, device=x.device, dtype=x.dtype).repeat(x.size(1), 1, 1, 1)
 
     _compute_msssim = _multi_scale_ssim_complex if x.dim() == 5 else _multi_scale_ssim
     msssim_val = _compute_msssim(
@@ -156,17 +156,17 @@
 
         # Generic loss parameters.
         self.reduction = reduction
 
         # Loss-specific parameters.
         if scale_weights is None:
             # Values from MS-SSIM paper
-            self.scale_weights = torch.tensor([0.0448, 0.2856, 0.3001, 0.2363, 0.1333])
+            self.register_buffer("scale_weights", torch.tensor([0.0448, 0.2856, 0.3001, 0.2363, 0.1333]))
         else:
-            self.scale_weights = scale_weights
+            self.register_buffer("scale_weights", scale_weights)
 
         self.kernel_size = kernel_size
         self.kernel_sigma = kernel_sigma
 
         # This check might look redundant because kernel size is checked within the ms-ssim function anyway.
         # However, this check allows to fail fast when the loss is being initialised and training has not been started.
         assert kernel_size % 2 == 1, f'Kernel size must be odd, got [{kernel_size}]'
```

### Comparing `piq-0.7.1/piq/msid.py` & `piq-0.8.0/piq/msid.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/perceptual.py` & `piq-0.8.0/piq/perceptual.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/pieapp.py` & `piq-0.8.0/piq/pieapp.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/pr.py` & `piq-0.8.0/piq/pr.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/psnr.py` & `piq-0.8.0/piq/psnr.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/srsim.py` & `piq-0.8.0/piq/srsim.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/ssim.py` & `piq-0.8.0/piq/ssim.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/tv.py` & `piq-0.8.0/piq/tv.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/utils/common.py` & `piq-0.8.0/piq/utils/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import torch
 import re
+import os
 import warnings
 
 from typing import Tuple, List, Optional, Union, Dict, Any
+from urllib.request import urlopen
 
 SEMVER_VERSION_PATTERN = re.compile(
     r"""
         ^
         (?P<major>0|[1-9]\d*)
         \.
         (?P<minor>0|[1-9]\d*)
@@ -58,16 +60,16 @@
 """
 
 
 def _validate_input(
         tensors: List[torch.Tensor],
         dim_range: Tuple[int, int] = (0, -1),
         data_range: Tuple[float, float] = (0., -1.),
-        # size_dim_range: Tuple[float, float] = (0., -1.),
         size_range: Optional[Tuple[int, int]] = None,
+        check_for_channels_first: bool = False
 ) -> None:
     r"""Check that input(-s)  satisfies the requirements
     Args:
         tensors: Tensors to check
         dim_range: Allowed number of dimensions. (min, max)
         data_range: Allowed range of values in tensors. (min, max)
         size_range: Dimensions to include in size comparison. (start_dim, end_dim + 1)
@@ -95,14 +97,19 @@
                 f'Expected number of dimensions to be between {dim_range[0]} and {dim_range[1]}, got {t.dim()}'
 
         if data_range[0] < data_range[1]:
             assert data_range[0] <= t.min(), \
                 f'Expected values to be greater or equal to {data_range[0]}, got {t.min()}'
             assert t.max() <= data_range[1], \
                 f'Expected values to be lower or equal to {data_range[1]}, got {t.max()}'
+            
+        if check_for_channels_first:
+            channels_last = t.shape[-1] in {1, 2, 3}
+            assert not channels_last, "Expected tensor to have channels first format, but got channels last. \
+                Please permute channels (e.g. t.permute(0, 3, 1, 2) for 4D tensors) and rerun."
 
 
 def _reduce(x: torch.Tensor, reduction: str = 'mean') -> torch.Tensor:
     r"""Reduce input in batch dimension if needed.
 
     Args:
         x: Tensor with shape (N, *).
@@ -152,7 +159,40 @@
 
     if match is None:
         warnings.warn(f"{version} is not a valid SemVer or PEP 440 string")
         return tuple()
 
     release = tuple(int(i) for i in match.group("release").split("."))
     return release
+
+
+def download_tensor(url: str, root: str, map_location: str = 'cpu') -> torch.Tensor:
+    r"""Downloads torch tensor and caches it. If already downloaded - loads from cache.
+
+    Args:
+        url: Web or file system path.
+        root: Absolute or relative path of the cache folder.
+
+    Returns:
+        Loaded torch tesnor.
+    """
+    os.makedirs(root, exist_ok=True)
+    filename = os.path.basename(url)
+    download_target = os.path.join(root, filename)
+    if os.path.isfile(download_target):
+        return torch.load(download_target, map_location=map_location)
+    
+    with urlopen(url) as source, open(download_target, "wb") as output:
+        while True:
+            buff = source.read(8192)
+            if not buff:
+                break
+
+            output.write(buff)
+
+    return torch.load(download_target, map_location=map_location)
+
+
+def is_sha256_hash(string: str) -> Optional[re.Match]:
+    """ Checks whether the provided sting is a valid SHA256 hash. """
+    pattern = re.compile("^[a-fA-F0-9]{64}$")
+    return pattern.match(string)
```

### Comparing `piq-0.7.1/piq/vif.py` & `piq-0.8.0/piq/vif.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq/vsi.py` & `piq-0.8.0/piq/vsi.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.1/piq.egg-info/PKG-INFO` & `piq-0.8.0/piq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piq
-Version: 0.7.1
+Version: 0.8.0
 Summary: Measures and metrics for image2image tasks. PyTorch.
 Home-page: https://github.com/photosynthesis-team/piq
 Author: Sergey Kastryulin
 Author-email: snk4tr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -184,34 +184,35 @@
 SSIM         2003    `Structural Similarity <https://en.wikipedia.org/wiki/Structural_similarity>`_
 MS-SSIM      2004    `Multi-Scale Structural Similarity <https://ieeexplore.ieee.org/abstract/document/1292216>`_
 IW-SSIM      2011    `Information Content Weighted Structural Similarity Index <https://ece.uwaterloo.ca/~z70wang/publications/IWSSIM.pdf>`_
 VIFp         2004    `Visual Information Fidelity <https://ieeexplore.ieee.org/document/1576816>`_
 FSIM         2011    `Feature Similarity Index Measure <https://ieeexplore.ieee.org/document/5705575>`_
 SR-SIM       2012    `Spectral Residual Based Similarity <https://sse.tongji.edu.cn/linzhang/ICIP12/ICIP-SR-SIM.pdf>`_
 GMSD         2013    `Gradient Magnitude Similarity Deviation <https://arxiv.org/abs/1308.3052>`_
+MS-GMSD      2017    `Multi-Scale Gradient Magnitude Similarity Deviation <https://ieeexplore.ieee.org/document/7952357>`_
 VSI          2014    `Visual Saliency-induced Index <https://ieeexplore.ieee.org/document/6873260>`_
 DSS          2015    `DCT Subband Similarity Index <https://ieeexplore.ieee.org/document/7351172>`_
 \-           2016    `Content Score <https://arxiv.org/abs/1508.06576>`_
 \-           2016    `Style Score <https://arxiv.org/abs/1508.06576>`_
 HaarPSI      2016    `Haar Perceptual Similarity Index <https://arxiv.org/abs/1607.06140>`_
 MDSI         2016    `Mean Deviation Similarity Index <https://arxiv.org/abs/1608.07433>`_
-MS-GMSD      2017    `Multi-Scale Gradient Magnitude Similarity Deviation <https://ieeexplore.ieee.org/document/7952357>`_
 LPIPS        2018    `Learned Perceptual Image Patch Similarity <https://arxiv.org/abs/1801.03924>`_
 PieAPP       2018    `Perceptual Image-Error Assessment through Pairwise Preference <https://arxiv.org/abs/1806.02067>`_
 DISTS        2020    `Deep Image Structure and Texture Similarity <https://arxiv.org/abs/2004.07728>`_
 ===========  ======  ==========
 
 No-Reference (NR)
 ^^^^^^^^^^^^^^^^^
 
 ===========  ======  ==========
 Acronym      Year    Metric
 ===========  ======  ==========
 TV           1937    `Total Variation <https://en.wikipedia.org/wiki/Total_variation>`_
 BRISQUE      2012    `Blind/Referenceless Image Spatial Quality Evaluator <https://ieeexplore.ieee.org/document/6272356>`_
+CLIP-IQA     2022    `CLIP-IQA <https://arxiv.org/pdf/2207.12396.pdf>`_
 ===========  ======  ==========
 
 Distribution-Based (DB)
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 ===========  ======  ==========
 Acronym      Year    Metric
@@ -228,32 +229,34 @@
 
 .. benchmark-section-start
 
 Benchmark
 ---------
 
 As part of our library we provide `code to benchmark <tests/results_benchmark.py>`_ all metrics on a set of common Mean Opinon Scores databases.
-Currently we support `TID2013`_,  `KADID10k`_ and `PIPAL`_.
+Currently we support several Full-Reference (`TID2013`_,  `KADID10k`_ and `PIPAL`_) and No-Reference (`KonIQ10k`_ and `LIVE-itW`_) datasets.
 You need to download them separately and provide path to images as an argument to the script.
 
 Here is an example how to evaluate SSIM and MS-SSIM metrics on TID2013 dataset:
 
 .. code-block:: bash
 
    python3 tests/results_benchmark.py --dataset tid2013 --metrics SSIM MS-SSIM --path ~/datasets/tid2013 --batch_size 16
 
-Below we provide a comparison between `Spearman's Rank Correlation cCoefficient <https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient>`_ (SRCC) values obtained with PIQ and reported in surveys.
+Below we provide a comparison between `Spearman's Rank Correlation Coefficient <https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient>`_ (SRCC) values obtained with PIQ and reported in surveys.
 Closer SRCC values indicate the higher degree of agreement between results of computations on given datasets.
 We do not report `Kendall rank correlation coefficient <https://en.wikipedia.org/wiki/Kendall_rank_correlation_coefficient>`_ (KRCC)
 as it is highly correlated with SRCC and provides limited additional information.
 We do not report `Pearson linear correlation coefficient <https://en.wikipedia.org/wiki/Pearson_correlation_coefficient>`_ (PLCC)
 as it's highly dependent on fitting method and is biased towards simple examples.
 
 For metrics that can take greyscale or colour images, ``c`` means chromatic version.
 
+Full-Reference (FR) Datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 ===========  ===========================  ===========================  ===========================
      \                  TID2013                    KADID10k                       PIPAL
 -----------  ---------------------------  ---------------------------  ---------------------------
   Source            PIQ / Reference            PIQ / Reference                PIQ / Reference
 ===========  ===========================  ===========================  ===========================
 PSNR         0.69 / 0.69 `TID2013`_       0.68 / -                     0.41 / 0.41 `PIPAL`_
 SSIM         0.72 / 0.64 `TID2013`_       0.72 / 0.72 `KADID10k`_      0.50 / 0.53 `PIPAL`_
@@ -273,30 +276,45 @@
 MDSI         0.89 / 0.89 `MDSI`_          0.89 / 0.89 `KADID10k`_      0.59 / -
 MS-GMSD      0.81 / 0.81 `MS-GMSD`_       0.85 / -                     0.59 / -
 MS-GMSDc     0.89 / 0.89 `MS-GMSD`_       0.87 / -                     0.59 / -
 LPIPS-VGG    0.67 / 0.67 `DISTS`_         0.72 / -                     0.57 / 0.58 `PIPAL`_
 PieAPP       0.84 / 0.88 `DISTS`_         0.87 / -                     0.70 / 0.71 `PIPAL`_
 DISTS        0.81 / 0.83 `DISTS`_         0.88 / -                     0.62 / 0.66 `PIPAL`_
 BRISQUE      0.37 / 0.84 `Eval2019`_      0.33 / 0.53 `KADID10k`_      0.21 / -
+CLIP-IQA     0.50 / -                     0.48 / -                     0.26 / -
 IS           0.26 / -                     0.25 / -                     0.09 / -
 FID          0.67 / -                     0.66 / -                     0.18 / -
 KID          0.42 / -                     0.66 / -                     0.12 / -
 MSID         0.21 / -                     0.32 / -                     0.01 / -
 GS           0.37 / -                     0.37 / -                     0.02 / -
 ===========  ===========================  ===========================  ===========================
 
+No-Reference (NR) Datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+===========  ===========================  ===========================
+     \                  KonIQ10k                    LIVE-itW
+-----------  ---------------------------  ---------------------------
+  Source            PIQ / Reference            PIQ / Reference
+===========  ===========================  ===========================
+BRISQUE      0.22 / -                     0.31 / -
+CLIP-IQA     0.68 / 0.68 `CLIP-IQA off`_  0.64 / 0.64 `CLIP-IQA off`_
+===========  ===========================  ===========================
+
 .. _TID2013: http://www.ponomarenko.info/tid2013.htm
 .. _KADID10k: http://database.mmsp-kn.de/kadid-10k-database.html
 .. _Eval2019: https://ieeexplore.ieee.org/abstract/document/8847307/
 .. _`MDSI`: https://arxiv.org/abs/1608.07433
 .. _MS-GMSD: https://ieeexplore.ieee.org/document/7952357
 .. _DISTS: https://arxiv.org/abs/2004.07728
 .. _HaarPSI: https://arxiv.org/abs/1607.06140
 .. _PIPAL: https://arxiv.org/pdf/2011.15002.pdf
 .. _IW-SSIM: https://ieeexplore.ieee.org/document/7442122
+.. _KonIQ10k: http://database.mmsp-kn.de/koniq-10k-database.html
+.. _LIVE-itW: https://live.ece.utexas.edu/research/ChallengeDB/index.html
+.. _CLIP-IQA off: https://github.com/IceClear/CLIP-IQA
 
 Unlike FR and NR IQMs, designed to compute an image-wise distance, the DB metrics compare distributions of *sets* of images.
 To address these problems, we adopt a different way of computing the DB IQMs proposed in `<https://arxiv.org/abs/2203.07809>`_.
 Instead of extracting features from the whole images, we crop them into overlapping tiles of size ``96 × 96`` with ``stride = 32``.
 This pre-processing allows us to treat each pair of images as a pair of distributions of tiles, enabling further comparison.
 The other stages of computing the DB IQMs are kept intact.
```

### Comparing `piq-0.7.1/piq.egg-info/SOURCES.txt` & `piq-0.8.0/piq.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.rst
 setup.py
 piq/__init__.py
 piq/base.py
 piq/brisque.py
+piq/clip_iqa.py
 piq/dss.py
 piq/fid.py
 piq/fsim.py
 piq/gmsd.py
 piq/gs.py
 piq/haarpsi.py
 piq/isc.py
@@ -27,14 +28,15 @@
 piq/vsi.py
 piq.egg-info/PKG-INFO
 piq.egg-info/SOURCES.txt
 piq.egg-info/dependency_links.txt
 piq.egg-info/requires.txt
 piq.egg-info/top_level.txt
 piq/feature_extractors/__init__.py
+piq/feature_extractors/clip.py
 piq/feature_extractors/fid_inception.py
 piq/functional/__init__.py
 piq/functional/base.py
 piq/functional/colour_conversion.py
 piq/functional/filters.py
 piq/functional/layers.py
 piq/functional/resize.py
```

### Comparing `piq-0.7.1/setup.py` & `piq-0.8.0/setup.py`

 * *Files identical despite different names*

