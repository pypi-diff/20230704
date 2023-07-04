# Comparing `tmp/nkululeko-0.50.1.tar.gz` & `tmp/nkululeko-0.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.50.1.tar", last modified: Mon Jul  3 11:44:40 2023, max compression
+gzip compressed data, was "nkululeko-0.51.0.tar", last modified: Tue Jul  4 14:11:31 2023, max compression
```

## Comparing `nkululeko-0.50.1.tar` & `nkululeko-0.51.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-03 11:44:40.815566 nkululeko-0.50.1/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6852 2023-07-03 11:14:52.000000 nkululeko-0.50.1/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.50.1/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18652 2023-07-03 11:44:40.815566 nkululeko-0.50.1/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11247 2023-07-03 09:15:37.000000 nkululeko-0.50.1/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-03 11:44:40.815566 nkululeko-0.50.1/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.50.1/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.50.1/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.50.1/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.50.1/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.50.1/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-03 11:13:30.000000 nkululeko-0.50.1/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21714 2023-07-03 11:06:03.000000 nkululeko-0.50.1/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.50.1/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.50.1/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.50.1/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.50.1/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21195 2023-07-03 11:05:03.000000 nkululeko-0.50.1/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.50.1/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.50.1/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.50.1/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.50.1/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.50.1/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.50.1/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.50.1/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.50.1/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.50.1/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.50.1/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.50.1/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.50.1/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-07-03 11:08:36.000000 nkululeko-0.50.1/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.50.1/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.50.1/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3643 2023-07-03 11:42:57.000000 nkululeko-0.50.1/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.50.1/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.50.1/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.50.1/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.50.1/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.50.1/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.50.1/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.50.1/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.50.1/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.50.1/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.50.1/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.50.1/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.50.1/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.50.1/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.50.1/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.50.1/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.50.1/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.50.1/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.50.1/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.50.1/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6561 2023-07-03 11:09:57.000000 nkululeko-0.50.1/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.50.1/nkululeko/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.50.1/nkululeko/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.50.1/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.50.1/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.50.1/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.50.1/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.50.1/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.50.1/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.50.1/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9800 2023-07-03 11:04:05.000000 nkululeko-0.50.1/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-03 11:44:40.815566 nkululeko-0.50.1/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18652 2023-07-03 11:44:40.000000 nkululeko-0.50.1/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1649 2023-07-03 11:44:40.000000 nkululeko-0.50.1/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-03 11:44:40.000000 nkululeko-0.50.1/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-03 11:44:40.000000 nkululeko-0.50.1/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-03 11:44:40.000000 nkululeko-0.50.1/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.50.1/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-07-03 11:44:40.815566 nkululeko-0.50.1/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.50.1/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-04 14:11:31.934921 nkululeko-0.51.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6902 2023-07-04 08:40:45.000000 nkululeko-0.51.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.51.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18701 2023-07-04 14:11:31.934921 nkululeko-0.51.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11247 2023-07-03 09:15:37.000000 nkululeko-0.51.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-04 14:11:31.934921 nkululeko-0.51.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.51.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.51.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.51.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.51.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.51.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-04 08:40:13.000000 nkululeko-0.51.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20511 2023-07-04 13:47:08.000000 nkululeko-0.51.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2108 2023-07-04 08:05:22.000000 nkululeko-0.51.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.51.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.51.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.51.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21526 2023-07-04 13:54:56.000000 nkululeko-0.51.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.51.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.51.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.51.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.51.0/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.51.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.51.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.51.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.51.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.51.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.51.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.51.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.51.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-07-03 11:08:36.000000 nkululeko-0.51.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.51.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.51.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6643 2023-07-04 14:03:29.000000 nkululeko-0.51.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.51.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.51.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.51.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.51.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.51.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.51.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.51.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.51.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.51.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.51.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.51.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.51.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.51.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.51.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.51.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.51.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.51.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.51.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.51.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6637 2023-07-04 08:56:58.000000 nkululeko-0.51.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.51.0/nkululeko/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.51.0/nkululeko/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.51.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.51.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.51.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.51.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.51.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.51.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.51.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10461 2023-07-04 09:21:04.000000 nkululeko-0.51.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-04 14:11:31.934921 nkululeko-0.51.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18701 2023-07-04 14:11:31.000000 nkululeko-0.51.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1649 2023-07-04 14:11:31.000000 nkululeko-0.51.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-04 14:11:31.000000 nkululeko-0.51.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-04 14:11:31.000000 nkululeko-0.51.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-04 14:11:31.000000 nkululeko-0.51.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.51.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      958 2023-07-04 14:11:31.934921 nkululeko-0.51.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.51.0/setup.py
```

### Comparing `nkululeko-0.50.1/CHANGELOG.md` & `nkululeko-0.51.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.51.0
+--------------
+* added datafilter
+
 Version 0.50.1
 --------------
 * added caller information for debug and error messages in Util
 
 Version 0.50.0
 --------------
 * removed loso and added pre-selected logo (leave-one-group-out), aka folds
```

### Comparing `nkululeko-0.50.1/LICENSE` & `nkululeko-0.51.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/PKG-INFO` & `nkululeko-0.51.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.50.1
+Version: 0.51.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nkululeko
 * [Overview](#overview)
@@ -211,14 +211,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.51.0
+--------------
+* added datafilter
+
 Version 0.50.1
 --------------
 * added caller information for debug and error messages in Util
 
 Version 0.50.0
 --------------
 * removed loso and added pre-selected logo (leave-one-group-out), aka folds
```

### Comparing `nkululeko-0.50.1/README.md` & `nkululeko-0.51.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/augment.py` & `nkululeko-0.51.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/augmenter.py` & `nkululeko-0.51.0/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/cacheddataset.py` & `nkululeko-0.51.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/dataset.py` & `nkululeko-0.51.0/nkululeko/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from random import sample
 from nkululeko.util import Util
 from nkululeko.plots import Plots
 import nkululeko.glob_conf as glob_conf
 import os.path
 from audformat.utils import duration
 import nkululeko.filter_data as filter
+from nkululeko.filter_data import DataFilter
 
 class Dataset:
     """ Class to represent datasets"""
     name = '' # An identifier for the dataset
     config = None # The configuration 
     db = None # The database object
     df = None # The whole dataframe
@@ -63,32 +64,33 @@
 
     def load(self):
         """Load the dataframe with files, speakers and task labels"""
         # store the dataframe
         store = self.util.get_path('store')
         store_file = f'{store}{self.name}.pkl'
         self.util.debug(f'{self.name}: loading ...')
-        root = self._load_db()
+        self.root = self._load_db()
 #        self.got_speaker, self.got_gender = False, False 
         if not self.start_fresh and os.path.isfile(store_file):
             self.util.debug(f'{self.name}: reusing previously stored file {store_file}')
             self.df = pd.read_pickle(store_file)
             self.is_labeled = self.target in self.df
             self.got_gender = 'gender' in self.df
             self.got_age = 'age' in self.df
             self.got_speaker = 'speaker' in self.df
+            self.util.copy_flags(self, self.df)
             self.util.debug(f'{self.name}: loaded with {self.df.shape[0]} '\
                 f'samples: got targets: {self.is_labeled}, got speakers: {self.got_speaker}, '\
                 f'got sexes: {self.got_gender}')        
             return
         tables = self._get_tables()
         self.util.debug(f'{self.name}: loading tables: {tables}')
         #db = audb.load(root, )
         # map the audio file paths 
-        self.db.map_files(lambda x: os.path.join(root, x))
+        self.db.map_files(lambda x: os.path.join(self.root, x))
         # the dataframes (potentially more than one) with at least the file names
         df_files = self.util.config_val_data(self.name, 'files_tables', '[\'files\']')
         df_files_tables =  ast.literal_eval(df_files)
         # The label for the target column 
         self.col_label = self.util.config_val_data(self.name, 'label', self.target)
         df, self.is_labeled, self.got_speaker, self.got_gender, self.got_age = self._get_df_for_lists(self.db, df_files_tables)
         if False in {self.is_labeled, self.got_speaker, self.got_gender, self.got_age}:
@@ -111,67 +113,41 @@
                     df['age'] = df_target['age']
             except audformat.core.errors.BadKeyError:
                 pass
 
         if self.is_labeled:
             # remember the target in case they get labelencoded later
             df['class_label'] = df[self.target]
-        df.is_labeled = self.is_labeled
-        df.got_gender = self.got_gender
-        df.got_age = self.got_age
-        df.got_speaker = self.got_speaker
+
         self.df = df
-        self.df.is_labeled = self.is_labeled
         self.util.debug(f'Loaded database {self.name} with {df.shape[0]} '\
             f'samples: got targets: {self.is_labeled}, got speakers: {self.got_speaker}, '\
             f'got sexes: {self.got_gender}, got age: {self.got_age}')
 
 
     def prepare(self):
+        # ensure segmented index
+        self.df = self.util.make_segmented_index(self.df)
+        self.util.copy_flags(self, self.df)
+        # add duration
+        if 'duration' not in self.df:
+            start = self.df.index.get_level_values(1)
+            end = self.df.index.get_level_values(2)
+            self.df['duration']=(end-start).total_seconds()
+
         # Perform some filtering if desired
         required = eval(self.util.config_val_data(self.name, 'required', 'False'))
         if required:
             pre = self.df.shape[0]
             self.df = self.df[self.df[required].notna()]
             post = self.df.shape[0]
             self.util.debug(f'{self.name}: kept {post} samples with {required} (from {pre}, filtered {pre-post})')
-        samples_per_speaker = self.util.config_val_data(self.name, 'max_samples_per_speaker', False)
-        if samples_per_speaker:
-            pre = self.df.shape[0]
-            self.df = filter.limit_speakers(self.df, int(samples_per_speaker))            
-            post = self.df.shape[0]
-            self.util.debug(f'{self.name}: kept {post} samples with {samples_per_speaker} per speaker (from {pre}, filtered {pre-post})')
-        if self.limit:
-            pre = self.df.shape[0]
-            self.df = self.df.sample(self.limit)
-            post = self.df.shape[0]
-            self.util.debug(f'{self.name}: limited to {post} samples (from {pre}, filtered {pre-post})')
-        sex = self.util.config_val('DATA', 'sex', False)
-        if sex:
-            # for experiments that do separate sex models
-            pre = self.df.shape[0]
-            self.df = self.df[self.df.gender==sex]
-            post = self.df.shape[0]
-            self.util.debug(f'{self.name}: limited to {post} samples with sex {sex} (from {pre}, filtered {pre-post})')
-            self.df.is_labeled = self.is_labeled
-            self.df.got_gender = self.got_gender
-            self.df.got_speaker = self.got_speaker
-        min_dur = self.util.config_val_data(self.name, 'min_duration_of_sample', False)
-        if min_dur:
-            pre = self.df.shape[0]
-            self.df = filter.filter_min_dur(self.df, min_dur)
-            post = self.df.shape[0]
-            self.util.debug(f'{self.name}: dropped {pre-post} shorter than {min_dur} seconds (from {pre} to {post} samples)')
 
-        max_dur = self.util.config_val_data(self.name, 'max_duration_of_sample', False)
-        if max_dur:
-            pre = self.df.shape[0]
-            self.df = filter.filter_max_dur(self.df, max_dur)
-            post = self.df.shape[0]
-            self.util.debug(f'{self.name}: dropped {pre-post} longer than {max_dur} seconds (from {pre} to {post} samples)')
+        datafilter = DataFilter(self.df)
+        self.df = datafilter.all_filters(data_name=self.name)
 
         self.util.debug(f'{self.name}: loaded data with {self.df.shape[0]} '\
             f'samples: got targets: {self.is_labeled}, got speakers: {self.got_speaker}, '\
             f'got sexes: {self.got_gender}')
 
         if self.got_speaker and self.util.config_val_data(self.name, 'rename_speakers', False):
             # we might need to append the database name to all speakers in case other datbaases have the same speaker names
@@ -249,14 +225,15 @@
             # check if the splits have been computed previously (not for speaker split)
             if os.path.isfile(storage_train) and os.path.isfile(storage_test):
                 # if self.util.config_val_data(self.name, 'test_tables', False):
                 self.util.debug(f'splits: reusing previously stored test file {storage_test}')
                 self.df_test = pd.read_pickle(storage_test)
                 self.util.debug(f'splits: reusing previously stored train file {storage_train}')
                 self.df_train = pd.read_pickle(storage_train)
+
                 return
             elif os.path.isfile(storage_train):
                 self.util.debug(f'splits: reusing previously stored train file {storage_train}')
                 self.df_train = pd.read_pickle(storage_train)
                 self.df_test = pd.DataFrame()
                 return
             elif os.path.isfile(storage_test):
@@ -287,14 +264,18 @@
                     testdf = pd.concat([testdf, self.db.tables[test_table].df]) 
             entry_train_tables = self.util.config_val_data(self.name, 'train_tables', False)
             if entry_train_tables: 
                 train_tables =  ast.literal_eval(entry_train_tables)
                 for train_table in train_tables:
                     traindf = pd.concat([traindf, self.db.tables[train_table].df])
             # use only the train and test samples that were not perhaps filtered out by an earlier processing step
+            #testdf.index.map(lambda x: os.path.join(self.root, x))
+#            testdf.index = testdf.index.to_series().apply(lambda x: self.root+x)
+            testdf = testdf.set_index(audformat.utils.to_segmented_index(testdf.index, allow_nat=False))
+            traindf = traindf.set_index(audformat.utils.to_segmented_index(traindf.index, allow_nat=False))
             self.df_test = self.df.loc[self.df.index.intersection(testdf.index)]
             self.df_train = self.df.loc[self.df.index.intersection(traindf.index)]
             # it might be necessary to copy the target values 
             try:
                 self.df_test[self.target] = testdf[self.target]
             except KeyError:
                 pass # if the dataframe is empty
```

### Comparing `nkululeko-0.50.1/nkululeko/dataset_csv.py` & `nkululeko-0.51.0/nkululeko/dataset_csv.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,17 +30,20 @@
         self.got_target = True
         self.is_labeled = self.got_target
         self.start_fresh = eval(self.util.config_val('DATA', 'no_reuse', 'False'))
         if self.is_labeled and not 'class_label' in self.df.columns:
             self.df['class_label'] = self.df[self.target]
         if 'gender' in df.columns:
             self.got_gender = True 
+        if 'age' in df.columns:
+            self.got_age = True 
         if 'speaker' in df.columns:
             self.got_speaker = True
             ns = df['speaker'].nunique()
             print(f'num of speakers: {ns}')
+
         self.util.debug(f'Loaded database {self.name} with {df.shape[0]} '\
             f'samples: got targets: {self.got_target}, got speakers: {self.got_speaker}, '\
             f'got sexes: {self.got_gender}')
 
     def prepare(self):
         super().prepare()
```

### Comparing `nkululeko-0.50.1/nkululeko/dataset_ravdess.py` & `nkululeko-0.51.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/demo.py` & `nkululeko-0.51.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/demo_predictor.py` & `nkululeko-0.51.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/experiment.py` & `nkululeko-0.51.0/nkululeko/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 from nkululeko.filter_data import filter_min_dur
 from nkululeko.runmanager import Runmanager
 from nkululeko.test_predictor import Test_predictor
 from nkululeko.feats_analyser import FeatureAnalyser
 from nkululeko.util import Util
 from nkululeko.feature_extractor import FeatureExtractor
 from nkululeko.plots import Plots
+from nkululeko.filter_data import DataFilter
 import nkululeko.glob_conf as glob_conf
 from nkululeko.demo_predictor import Demo_predictor
 import ast # To convert strings to objects
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder
 from nkululeko.scaler import Scaler
 import pickle
 import audformat
+import audeer 
 
 class Experiment:
     """Main class specifying an experiment
     
     """
     
 
@@ -32,14 +34,16 @@
         Parameters
         ----------
         config_obj : a config parser object that sets the experiment parameters and being set as a global object.
         """
 
         self.set_globals(config_obj)
         self.name = glob_conf.config['EXP']['name']
+        self.root = glob_conf.config['EXP']['root']
+        audeer.mkdir(self.root+self.name) # create the experiment directory
         self.util = Util('experiment')
         glob_conf.set_util(self.util)
         self.loso = self.util.config_val('MODEL', 'loso', False)
         self.logo = self.util.config_val('MODEL', 'logo', False)
         self.xfoldx = self.util.config_val('MODEL', 'k_fold_cross', False)
         self.start = time.process_time()
 
@@ -145,52 +149,55 @@
             if strategy == 'cross_data':
                 train_dbs = ast.literal_eval(glob_conf.config['DATA']['trains'])
                 test_dbs = ast.literal_eval(glob_conf.config['DATA']['tests'])
                 for dn in train_dbs:
                     d = self.datasets[dn]
                     d.prepare_labels()
                     self.df_train = self.df_train.append(self.util.make_segmented_index(d.df))
-                    self.df_train.is_labeled = d.is_labeled
+                    self.util.copy_flags(d, self.df_train)
                 for dn in test_dbs:
                     d = self.datasets[dn]
                     d.prepare_labels()
                     self.df_test = self.df_test.append(self.util.make_segmented_index(d.df))
-                    self.df_test.is_labeled = d.is_labeled
+                    self.util.copy_flags(d, self.df_test)
             elif strategy == 'traintest':
                 # default: train vs. test combined from all datasets
                 for d in self.datasets.values():
                     d.split()
                     d.prepare_labels()
-                    self.df_train = pd.concat([self.df_train, self.util.make_segmented_index(d.df_train)])
-                    self.df_train.is_labeled = d.is_labeled
-                    self.df_test = pd.concat([self.df_test, self.util.make_segmented_index(d.df_test)])
-                    self.df_test.is_labeled = d.is_labeled
+                    self.df_train = pd.concat([self.df_train, d.df_train])
+                    self.util.copy_flags(d, self.df_train)
+                    self.df_test = pd.concat([self.df_test, d.df_test])
+                    self.util.copy_flags(d, self.df_test)
             else:
                 self.util.error(f'unknown strategy: {strategy}')
             # save the file lists to disk for later reuse
             store = self.util.get_path('store')
             storage_test = f'{store}testdf.csv'
             storage_train = f'{store}traindf.csv'
             self.df_test.to_csv(storage_test)
             self.df_train.to_csv(storage_train)
 
-        self.df_train.got_gender = self.got_gender
-        self.df_train.got_age = self.got_age
-        self.df_train.got_speaker = self.got_speaker
-        self.df_test.got_gender = self.got_gender
-        self.df_test.got_speaker = self.got_speaker
-        self.df_test.got_age = self.got_age
-
+        self.util.copy_flags(self, self.df_test)
+        self.util.copy_flags(self, self.df_train)
         # Check for filters
-        min_dur_test = self.util.config_val('DATA', 'min_dur_test', False)
-        if min_dur_test:
-            pre = self.df_test.shape[0]
-            self.df_test = filter_min_dur(self.df_test, min_dur_test)
-            post = self.df_test.shape[0]
-            self.util.debug(f'Dropped {pre-post} test samples shorter than {min_dur_test} seconds (from {pre} to {post} samples)')
+        filter_sample_selection = self.util.config_val('DATA', 'filter.sample_selection', 'all')
+        if filter_sample_selection=='all':
+            datafilter = DataFilter(self.df_train)
+            self.df_train = datafilter.all_filters()
+            datafilter = DataFilter(self.df_test)
+            self.df_test = datafilter.all_filters()
+        elif filter_sample_selection=='train':
+            datafilter = DataFilter(self.df_train)
+            self.df_train = datafilter.all_filters()
+        elif filter_sample_selection=='test':
+            datafilter = DataFilter(self.df_test)
+            self.df_test = datafilter.all_filters()
+        else:
+            self.util.error(f'unkown filter sample selection specifier {filter_sample_selection}, should be [all | train | test]')
 
         # encode the labels
         if self.util.exp_is_classification():
             datatype = self.util.config_val('DATA', 'type', 'dummy')
             if datatype == 'continuous':
                 if self.df_test.is_labeled:
                     # remember the target in case they get labelencoded later
```

### Comparing `nkululeko-0.50.1/nkululeko/explore.py` & `nkululeko-0.51.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_analyser.py` & `nkululeko-0.51.0/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_audmodel.py` & `nkululeko-0.51.0/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.51.0/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_clap.py` & `nkululeko-0.51.0/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_import.py` & `nkululeko-0.51.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_mld.py` & `nkululeko-0.51.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_opensmile.py` & `nkululeko-0.51.0/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_oxbow.py` & `nkululeko-0.51.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_praat.py` & `nkululeko-0.51.0/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_trill.py` & `nkululeko-0.51.0/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feats_wav2vec2.py` & `nkululeko-0.51.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feature_extractor.py` & `nkululeko-0.51.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/featureset.py` & `nkululeko-0.51.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/feinberg_praat.py` & `nkululeko-0.51.0/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/loss_ccc.py` & `nkululeko-0.51.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/loss_softf1loss.py` & `nkululeko-0.51.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/model.py` & `nkululeko-0.51.0/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/model_cnn.py` & `nkululeko-0.51.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/model_gmm.py` & `nkululeko-0.51.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/model_knn.py` & `nkululeko-0.51.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/model_knn_reg.py` & `nkululeko-0.51.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/model_mlp.py` & `nkululeko-0.51.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/model_mlp_regression.py` & `nkululeko-0.51.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/model_svm.py` & `nkululeko-0.51.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/modelrunner.py` & `nkululeko-0.51.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/nkululeko.py` & `nkululeko-0.51.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/plots.py` & `nkululeko-0.51.0/nkululeko/plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 class Plots():
     
     def __init__(self):
         """Initializing the util system"""
         self.util = Util('plots')
         self.format = self.util.config_val('PLOT', 'format', 'png')
+        
+    def plot_distributions(self, df, name, filename):
+        pass
 
     def describe_df(self, name, df, target, filename):
         """Make a stacked barplot of samples and speakers per sex and target values. speaker, gender and target columns must be present"""
         fig_dir = self.util.get_path('fig_dir')+'../' # one up because of the runs 
         sampl_num = df.shape[0]
         sex_col = 'gender'
         if target == 'gender':
```

### Comparing `nkululeko-0.50.1/nkululeko/randomsplicer.py` & `nkululeko-0.51.0/nkululeko/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/randomsplicing.py` & `nkululeko-0.51.0/nkululeko/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/reporter.py` & `nkululeko-0.51.0/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/runmanager.py` & `nkululeko-0.51.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/scaler.py` & `nkululeko-0.51.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/syllable_nuclei.py` & `nkululeko-0.51.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/test.py` & `nkululeko-0.51.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/test_predictor.py` & `nkululeko-0.51.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/nkululeko/util.py` & `nkululeko-0.51.0/nkululeko/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -85,14 +85,18 @@
 
 
     def get_save_name(self):
         """Return a relative path to a name to save the experiment"""
         store = self.get_path('store')
         return f'{store}/{self.get_exp_name()}.pkl'
 
+    def is_categorical(array_like):
+        """Check if a dataframe column is categorical"""
+        return array_like.dtype.name == 'category'
+
 
     def get_res_dir(self):
         root = glob_conf.config['EXP']['root']
         name = glob_conf.config['EXP']['name']
         dir_name = f'{root}{name}/results/'
         audeer.mkdir(dir_name)
         return dir_name
@@ -253,10 +257,21 @@
             return pd.read_pickle(name)
         elif format == 'csv':
             return audformat.utils.read_csv(name)
         else:
             self.error(f'unkown store format: {format}')
 
     def copy_flags(self, df_source, df_target):
-        df_target.is_labeled = df_source.is_labeled
-        df_target.got_gender = df_source.got_gender
-        df_target.got_speaker = df_source.got_speaker
+        if hasattr(df_source, 'is_labeled'):
+            df_target.is_labeled = df_source.is_labeled
+        if hasattr(df_source, 'is_test'):
+            df_target.is_test = df_source.is_test
+        if hasattr(df_source, 'is_train'):
+            df_target.is_train = df_source.is_train
+        if hasattr(df_source, 'is_val'):
+            df_target.is_val = df_source.is_val
+        if hasattr(df_source, 'got_gender'):
+            df_target.got_gender = df_source.got_gender
+        if hasattr(df_source, 'got_age'):
+            df_target.got_age = df_source.got_age
+        if hasattr(df_source, 'got_speaker'):
+            df_target.got_speaker = df_source.got_speaker
```

### Comparing `nkululeko-0.50.1/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.51.0/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.50.1
+Version: 0.51.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nkululeko
 * [Overview](#overview)
@@ -211,14 +211,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.51.0
+--------------
+* added datafilter
+
 Version 0.50.1
 --------------
 * added caller information for debug and error messages in Util
 
 Version 0.50.0
 --------------
 * removed loso and added pre-selected logo (leave-one-group-out), aka folds
```

### Comparing `nkululeko-0.50.1/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.51.0/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.50.1/setup.cfg` & `nkululeko-0.51.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/felixbur/nkululeko
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find:
 install_requires = 
 	audeer
 	audformat
```

