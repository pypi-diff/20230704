# Comparing `tmp/omicverse-1.4.6.tar.gz` & `tmp/omicverse-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omicverse-1.4.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "omicverse-1.4.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `omicverse-1.4.6.tar` & `omicverse-1.4.7.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0    35823 2022-09-03 17:16:03.066315 omicverse-1.4.6/LICENSE
--rw-r--r--   0        0        0     6588 2023-07-03 13:00:37.272915 omicverse-1.4.6/README.md
--rw-r--r--   0        0        0    14340 2023-05-30 08:19:15.462907 omicverse-1.4.6/omicverse/.DS_Store
--rw-r--r--   0        0        0      320 2022-09-07 04:15:30.431190 omicverse-1.4.6/omicverse/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0      347 2023-05-30 08:29:23.892622 omicverse-1.4.6/omicverse/__init__.py
--rw-r--r--   0        0        0     6148 2023-04-03 18:27:15.377061 omicverse-1.4.6/omicverse/bulk/.DS_Store
--rw-r--r--   0        0        0    22181 2023-05-17 18:38:47.881174 omicverse-1.4.6/omicverse/bulk/_Deseq2.py
--rw-r--r--   0        0        0    21069 2023-07-04 03:40:00.025229 omicverse-1.4.6/omicverse/bulk/_Enrichment.py
--rw-r--r--   0        0        0    28860 2023-05-17 07:33:38.724769 omicverse-1.4.6/omicverse/bulk/_Gene_module.py
--rw-r--r--   0        0        0      591 2023-05-17 18:34:20.109930 omicverse-1.4.6/omicverse/bulk/__init__.py
--rw-r--r--   0        0        0   633338 2023-04-03 07:50:58.899031 omicverse-1.4.6/omicverse/bulk/_chm13.py
--rw-r--r--   0        0        0     1633 2022-09-06 14:17:42.730883 omicverse-1.4.6/omicverse/bulk/_df_apply.py
--rw-r--r--   0        0        0    42804 2022-09-06 14:17:42.731609 omicverse-1.4.6/omicverse/bulk/_dynamicTree.py
--rw-r--r--   0        0        0     6672 2023-04-05 07:48:28.207285 omicverse-1.4.6/omicverse/bulk/_network.py
--rw-r--r--   0        0        0    12290 2023-04-05 17:42:26.435325 omicverse-1.4.6/omicverse/bulk/_tcga.py
--rw-r--r--   0        0        0      275 2023-05-27 07:42:00.305669 omicverse-1.4.6/omicverse/bulk2single/__init__.py
--rw-r--r--   0        0        0    11376 2023-04-06 06:59:09.524952 omicverse-1.4.6/omicverse/bulk2single/_bulk2single.py
--rw-r--r--   0        0        0    13828 2023-07-04 03:40:49.861005 omicverse-1.4.6/omicverse/bulk2single/_bulktrajblend.py
--rw-r--r--   0        0        0    29806 2023-05-06 16:11:04.140905 omicverse-1.4.6/omicverse/bulk2single/_map_utils.py
--rw-r--r--   0        0        0    24978 2023-05-17 10:51:23.881340 omicverse-1.4.6/omicverse/bulk2single/_map_utils1.py
--rw-r--r--   0        0        0    12746 2023-04-14 09:44:12.354770 omicverse-1.4.6/omicverse/bulk2single/_single2spatial.py
--rw-r--r--   0        0        0    10462 2023-05-14 07:19:07.135859 omicverse-1.4.6/omicverse/bulk2single/_utils.py
--rw-r--r--   0        0        0     8560 2023-04-06 07:00:58.204356 omicverse-1.4.6/omicverse/bulk2single/_vae.py
--rw-r--r--   0        0        0       48 2023-05-30 08:00:53.496990 omicverse-1.4.6/omicverse/cylib/README.rst
--rw-r--r--   0        0        0       25 2023-05-31 17:51:38.764877 omicverse-1.4.6/omicverse/cylib/__init__.py
--rw-r--r--   0        0        0     3338 2023-05-31 17:55:48.200546 omicverse-1.4.6/omicverse/cylib/fast_utils.py
--rw-r--r--   0        0        0     1313 2023-05-30 08:00:53.497082 omicverse-1.4.6/omicverse/data_files/README.md
--rw-r--r--   0        0        0      613 2023-05-30 08:00:53.497137 omicverse-1.4.6/omicverse/data_files/apoptosis_human.gmt
--rw-r--r--   0        0        0      598 2023-05-30 08:00:53.497199 omicverse-1.4.6/omicverse/data_files/apoptosis_mouse.gmt
--rw-r--r--   0        0        0  1277787 2023-05-30 08:00:53.501091 omicverse-1.4.6/omicverse/data_files/c2.cp.v7.5.1.symbols.gmt
--rw-r--r--   0        0        0      597 2023-05-30 08:00:53.501212 omicverse-1.4.6/omicverse/data_files/cell_cycle_human.gmt
--rw-r--r--   0        0        0      597 2023-05-30 08:00:53.501283 omicverse-1.4.6/omicverse/data_files/cell_cycle_mouse.gmt
--rw-r--r--   0        0        0      222 2023-05-30 08:00:53.501354 omicverse-1.4.6/omicverse/data_files/emt_human.gmt
--rw-r--r--   0        0        0      230 2023-05-30 08:00:53.501426 omicverse-1.4.6/omicverse/data_files/gender_human.gmt
--rw-r--r--   0        0        0      142 2023-05-30 08:00:53.501498 omicverse-1.4.6/omicverse/data_files/gender_mouse.gmt
--rw-r--r--   0        0        0    48244 2023-05-30 08:00:53.501752 omicverse-1.4.6/omicverse/data_files/h.all.v7.5.1.symbols.gmt
--rw-r--r--   0        0        0     2725 2023-05-30 08:00:53.501840 omicverse-1.4.6/omicverse/data_files/human_lung.gmt
--rw-r--r--   0        0        0      743 2023-05-30 08:00:53.501906 omicverse-1.4.6/omicverse/data_files/human_t_cell_markers.gmt
--rw-r--r--   0        0        0      929 2023-05-30 08:00:53.502035 omicverse-1.4.6/omicverse/data_files/mitochondrial_genes_human.gmt
--rw-r--r--   0        0        0      930 2023-05-30 08:00:53.502100 omicverse-1.4.6/omicverse/data_files/mitochondrial_genes_mouse.gmt
--rw-r--r--   0        0        0      706 2023-05-30 08:00:53.502165 omicverse-1.4.6/omicverse/data_files/mouse_brain.gmt
--rw-r--r--   0        0        0     1931 2023-05-30 08:00:53.502238 omicverse-1.4.6/omicverse/data_files/mouse_liver.gmt
--rw-r--r--   0        0        0     4068 2023-05-30 08:00:53.502316 omicverse-1.4.6/omicverse/data_files/mouse_lung.gmt
--rw-r--r--   0        0        0      787 2023-05-30 08:00:53.502394 omicverse-1.4.6/omicverse/data_files/ribosomal_genes_human.gmt
--rw-r--r--   0        0        0      801 2023-05-30 08:00:53.502468 omicverse-1.4.6/omicverse/data_files/ribosomal_genes_mouse.gmt
--rw-r--r--   0        0        0       55 2022-09-07 09:33:07.470218 omicverse-1.4.6/omicverse/mofapy2/__init__.py
--rw-r--r--   0        0        0        0 2022-09-07 09:33:07.470284 omicverse-1.4.6/omicverse/mofapy2/build_model/__init__.py
--rw-r--r--   0        0        0    13189 2022-09-07 10:12:11.559603 omicverse-1.4.6/omicverse/mofapy2/build_model/build_model.py
--rw-r--r--   0        0        0    28425 2022-09-07 10:12:16.240298 omicverse-1.4.6/omicverse/mofapy2/build_model/init_model.py
--rw-r--r--   0        0        0    25076 2022-09-07 10:12:21.681277 omicverse-1.4.6/omicverse/mofapy2/build_model/save_model.py
--rw-r--r--   0        0        0      637 2022-09-07 10:12:26.660116 omicverse-1.4.6/omicverse/mofapy2/build_model/train_model.py
--rw-r--r--   0        0        0     3366 2022-09-07 10:12:30.366961 omicverse-1.4.6/omicverse/mofapy2/build_model/utils.py
--rw-r--r--   0        0        0      405 2022-09-07 09:33:07.470940 omicverse-1.4.6/omicverse/mofapy2/config.py
--rw-r--r--   0        0        0    26036 2022-09-07 10:13:08.257046 omicverse-1.4.6/omicverse/mofapy2/core/BayesNet.py
--rw-r--r--   0        0        0       21 2022-09-07 09:33:07.471206 omicverse-1.4.6/omicverse/mofapy2/core/__init__.py
--rw-r--r--   0        0        0      448 2022-09-07 09:33:07.471309 omicverse-1.4.6/omicverse/mofapy2/core/distributions/__init__.py
--rw-r--r--   0        0        0     3923 2022-09-07 09:33:07.471393 omicverse-1.4.6/omicverse/mofapy2/core/distributions/basic_distributions.py
--rw-r--r--   0        0        0     1301 2022-09-07 10:20:27.422096 omicverse-1.4.6/omicverse/mofapy2/core/distributions/bernoulli.py
--rw-r--r--   0        0        0     4709 2022-09-07 10:20:18.413617 omicverse-1.4.6/omicverse/mofapy2/core/distributions/bernoulli_gaussian.py
--rw-r--r--   0        0        0     1859 2022-09-07 10:20:33.345355 omicverse-1.4.6/omicverse/mofapy2/core/distributions/beta.py
--rw-r--r--   0        0        0     1928 2022-09-07 10:20:37.394428 omicverse-1.4.6/omicverse/mofapy2/core/distributions/binomial.py
--rw-r--r--   0        0        0     2061 2022-09-07 10:20:40.951879 omicverse-1.4.6/omicverse/mofapy2/core/distributions/gamma.py
--rw-r--r--   0        0        0    38150 2022-09-07 09:33:07.471983 omicverse-1.4.6/omicverse/mofapy2/core/distributions/multi_task_GP.py
--rw-r--r--   0        0        0    16083 2022-09-07 10:20:53.092939 omicverse-1.4.6/omicverse/mofapy2/core/distributions/multivariate_gaussian.py
--rw-r--r--   0        0        0     1663 2022-09-07 10:20:57.661446 omicverse-1.4.6/omicverse/mofapy2/core/distributions/poisson.py
--rw-r--r--   0        0        0     2223 2022-09-07 10:21:03.520320 omicverse-1.4.6/omicverse/mofapy2/core/distributions/univariate_gaussian.py
--rw-r--r--   0        0        0     5591 2022-09-07 09:33:07.472344 omicverse-1.4.6/omicverse/mofapy2/core/gp_utils.py
--rw-r--r--   0        0        0     1765 2022-09-07 09:33:07.472409 omicverse-1.4.6/omicverse/mofapy2/core/gpu_utils.py
--rw-r--r--   0        0        0     6291 2022-09-07 09:33:07.472554 omicverse-1.4.6/omicverse/mofapy2/core/nodes/Alpha_nodes.py
--rw-r--r--   0        0        0     4646 2022-09-07 10:16:08.287697 omicverse-1.4.6/omicverse/mofapy2/core/nodes/Kc_node.py
--rw-r--r--   0        0        0     3581 2022-09-07 10:16:52.659105 omicverse-1.4.6/omicverse/mofapy2/core/nodes/Kg_node.py
--rw-r--r--   0        0        0    49309 2022-09-07 10:22:30.858460 omicverse-1.4.6/omicverse/mofapy2/core/nodes/Sigma_node.py
--rwxr-xr-x   0        0        0     5327 2022-09-07 10:18:15.524786 omicverse-1.4.6/omicverse/mofapy2/core/nodes/Tau_nodes.py
--rw-r--r--   0        0        0     6551 2022-09-07 09:33:07.473126 omicverse-1.4.6/omicverse/mofapy2/core/nodes/Theta_nodes.py
--rw-r--r--   0        0        0     7911 2022-09-07 10:18:33.209503 omicverse-1.4.6/omicverse/mofapy2/core/nodes/U_nodes.py
--rwxr-xr-x   0        0        0    10037 2022-09-07 10:18:50.380099 omicverse-1.4.6/omicverse/mofapy2/core/nodes/W_nodes.py
--rw-r--r--   0        0        0     3577 2022-09-07 10:18:59.577240 omicverse-1.4.6/omicverse/mofapy2/core/nodes/Y_nodes.py
--rwxr-xr-x   0        0        0    15625 2022-09-07 10:19:28.866210 omicverse-1.4.6/omicverse/mofapy2/core/nodes/Z_nodes.py
--rw-r--r--   0        0        0     9248 2022-09-07 10:19:17.982574 omicverse-1.4.6/omicverse/mofapy2/core/nodes/Z_nodes_GP.py
--rw-r--r--   0        0        0     8127 2022-09-07 10:19:10.770163 omicverse-1.4.6/omicverse/mofapy2/core/nodes/Z_nodes_GP_mv.py
--rw-r--r--   0        0        0     7505 2022-09-07 10:19:37.520420 omicverse-1.4.6/omicverse/mofapy2/core/nodes/ZgU_node.py
--rw-r--r--   0        0        0      581 2022-09-07 09:33:07.473827 omicverse-1.4.6/omicverse/mofapy2/core/nodes/__init__.py
--rw-r--r--   0        0        0     3812 2022-09-07 10:14:43.810952 omicverse-1.4.6/omicverse/mofapy2/core/nodes/basic_nodes.py
--rw-r--r--   0        0        0     6837 2022-09-07 09:33:07.473999 omicverse-1.4.6/omicverse/mofapy2/core/nodes/multiview_nodes.py
--rw-r--r--   0        0        0    21096 2022-09-07 10:17:25.117004 omicverse-1.4.6/omicverse/mofapy2/core/nodes/nongaussian_nodes.py
--rw-r--r--   0        0        0    11994 2022-09-07 10:18:40.408370 omicverse-1.4.6/omicverse/mofapy2/core/nodes/variational_nodes.py
--rw-r--r--   0        0        0     3764 2022-09-07 09:33:07.474508 omicverse-1.4.6/omicverse/mofapy2/core/utils.py
--rw-r--r--   0        0        0        0 2022-09-07 09:33:07.474782 omicverse-1.4.6/omicverse/mofapy2/run/__init__.py
--rw-r--r--   0        0        0    70968 2023-05-18 07:48:53.001053 omicverse-1.4.6/omicverse/mofapy2/run/entry_point.py
--rw-r--r--   0        0        0   324931 2022-09-07 09:33:07.476317 omicverse-1.4.6/omicverse/mofapy2/run/test_data/view_0.txt
--rw-r--r--   0        0        0   324642 2022-09-07 09:33:07.477843 omicverse-1.4.6/omicverse/mofapy2/run/test_data/view_1.txt
--rw-r--r--   0        0        0   324951 2022-09-07 09:33:07.478979 omicverse-1.4.6/omicverse/mofapy2/run/test_data/view_2.txt
--rw-r--r--   0        0        0   996145 2022-09-07 09:33:07.483410 omicverse-1.4.6/omicverse/mofapy2/run/test_data/with_nas/500_0.txt
--rw-r--r--   0        0        0   996423 2022-09-07 09:33:07.486212 omicverse-1.4.6/omicverse/mofapy2/run/test_data/with_nas/500_1.txt
--rw-r--r--   0        0        0   995502 2022-09-07 09:33:07.486904 omicverse-1.4.6/omicverse/mofapy2/run/test_data/with_nas/500_2.txt
--rw-r--r--   0        0        0        0 2022-09-07 09:33:07.486988 omicverse-1.4.6/omicverse/mofapy2/simulate/__init__.py
--rw-r--r--   0        0        0     6509 2022-09-07 10:10:46.603319 omicverse-1.4.6/omicverse/mofapy2/simulate/simulate_mofa.py
--rw-r--r--   0        0        0       22 2022-09-07 09:33:07.487160 omicverse-1.4.6/omicverse/mofapy2/version.py
--rw-r--r--   0        0        0     1301 2022-09-07 04:15:14.083982 omicverse-1.4.6/omicverse/nocd/.ipynb_checkpoints/generate-checkpoint.py
--rw-r--r--   0        0        0     1681 2022-09-07 04:15:14.092998 omicverse-1.4.6/omicverse/nocd/.ipynb_checkpoints/sampler-checkpoint.py
--rw-r--r--   0        0        0     4558 2022-09-07 04:15:14.093212 omicverse-1.4.6/omicverse/nocd/.ipynb_checkpoints/train-checkpoint.py
--rw-r--r--   0        0        0     5051 2022-09-07 04:15:14.078134 omicverse-1.4.6/omicverse/nocd/.ipynb_checkpoints/utils-checkpoint.py
--rw-r--r--   0        0        0      120 2022-09-07 04:15:14.079001 omicverse-1.4.6/omicverse/nocd/__init__.py
--rw-r--r--   0        0        0     2163 2022-09-07 04:15:14.083601 omicverse-1.4.6/omicverse/nocd/data.py
--rw-r--r--   0        0        0     1301 2022-09-07 04:15:14.083982 omicverse-1.4.6/omicverse/nocd/generate.py
--rw-r--r--   0        0        0     4068 2022-09-07 04:18:20.582316 omicverse-1.4.6/omicverse/nocd/metrics/.ipynb_checkpoints/supervised-checkpoint.py
--rw-r--r--   0        0        0     3214 2022-09-07 04:15:14.085633 omicverse-1.4.6/omicverse/nocd/metrics/.ipynb_checkpoints/unsupervised-checkpoint.py
--rw-r--r--   0        0        0       54 2022-09-07 04:15:14.086034 omicverse-1.4.6/omicverse/nocd/metrics/__init__.py
--rw-r--r--   0        0        0     4068 2022-09-07 04:18:20.582316 omicverse-1.4.6/omicverse/nocd/metrics/supervised.py
--rw-r--r--   0        0        0     3214 2022-09-07 04:15:14.089087 omicverse-1.4.6/omicverse/nocd/metrics/unsupervised.py
--rw-r--r--   0        0        0       70 2022-09-07 04:15:14.090185 omicverse-1.4.6/omicverse/nocd/nn/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     4453 2022-09-07 04:15:14.092088 omicverse-1.4.6/omicverse/nocd/nn/.ipynb_checkpoints/decoder-checkpoint.py
--rw-r--r--   0        0        0     3505 2022-09-07 04:17:34.429490 omicverse-1.4.6/omicverse/nocd/nn/.ipynb_checkpoints/gcn-checkpoint.py
--rw-r--r--   0        0        0     3610 2022-09-07 04:17:50.594410 omicverse-1.4.6/omicverse/nocd/nn/.ipynb_checkpoints/imrpoved_gcn-checkpoint.py
--rw-r--r--   0        0        0       70 2022-09-07 04:15:14.090185 omicverse-1.4.6/omicverse/nocd/nn/__init__.py
--rw-r--r--   0        0        0     4453 2022-09-07 04:15:14.092088 omicverse-1.4.6/omicverse/nocd/nn/decoder.py
--rw-r--r--   0        0        0     3505 2022-09-07 04:17:34.429490 omicverse-1.4.6/omicverse/nocd/nn/gcn.py
--rw-r--r--   0        0        0     3610 2022-09-07 04:17:50.594410 omicverse-1.4.6/omicverse/nocd/nn/imrpoved_gcn.py
--rw-r--r--   0        0        0     1681 2022-09-07 04:15:14.092998 omicverse-1.4.6/omicverse/nocd/sampler.py
--rw-r--r--   0        0        0     4558 2022-09-07 04:15:14.093212 omicverse-1.4.6/omicverse/nocd/train.py
--rw-r--r--   0        0        0     5051 2022-09-07 04:15:14.093413 omicverse-1.4.6/omicverse/nocd/utils.py
--rw-r--r--   0        0        0     4414 2023-05-30 09:52:24.238706 omicverse-1.4.6/omicverse/omicverse.egg-info/PKG-INFO
--rw-r--r--   0        0        0    13619 2023-05-30 09:52:25.204543 omicverse-1.4.6/omicverse/omicverse.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-05-30 09:52:24.238892 omicverse-1.4.6/omicverse/omicverse.egg-info/dependency_links.txt
--rw-r--r--   0        0        0      350 2023-05-30 09:52:24.239060 omicverse-1.4.6/omicverse/omicverse.egg-info/requires.txt
--rw-r--r--   0        0        0       60 2023-05-30 09:52:24.239163 omicverse-1.4.6/omicverse/omicverse.egg-info/top_level.txt
--rw-r--r--   0        0        0      540 2023-05-30 12:45:44.272518 omicverse-1.4.6/omicverse/pp/__init__.py
--rw-r--r--   0        0        0    20944 2023-06-30 17:56:24.759600 omicverse-1.4.6/omicverse/pp/_preprocess.py
--rw-r--r--   0        0        0    16277 2023-06-04 08:31:35.638891 omicverse-1.4.6/omicverse/pp/_qc.py
--rw-r--r--   0        0        0     6148 2023-04-19 16:48:36.030388 omicverse-1.4.6/omicverse/single/.DS_Store
--rw-r--r--   0        0        0     8790 2022-09-03 17:16:03.070397 omicverse-1.4.6/omicverse/single/README.md
--rw-r--r--   0        0        0    61426 2023-06-26 23:50:36.692480 omicverse-1.4.6/omicverse/single/_SCSA.py
--rw-r--r--   0        0        0      683 2023-07-03 11:55:25.153988 omicverse-1.4.6/omicverse/single/__init__.py
--rw-r--r--   0        0        0    27360 2023-07-04 04:44:48.562227 omicverse-1.4.6/omicverse/single/_anno.py
--rw-r--r--   0        0        0     9315 2023-07-04 04:53:14.069596 omicverse-1.4.6/omicverse/single/_aucell.py
--rwxr-xr-x   0        0        0    21100 2022-09-07 05:59:40.809184 omicverse-1.4.6/omicverse/single/_cosg.py
--rw-r--r--   0        0        0    12142 2023-07-04 04:23:59.889080 omicverse-1.4.6/omicverse/single/_cpdb.py
--rw-r--r--   0        0        0    37915 2023-07-04 04:36:23.334945 omicverse-1.4.6/omicverse/single/_mofa.py
--rw-r--r--   0        0        0    10053 2023-05-27 09:28:40.824071 omicverse-1.4.6/omicverse/single/_nocd.py
--rw-r--r--   0        0        0    18135 2023-04-03 15:03:48.751508 omicverse-1.4.6/omicverse/single/_scdrug.py
--rw-r--r--   0        0        0    12302 2023-05-15 08:29:21.026574 omicverse-1.4.6/omicverse/single/_scgsea.py
--rw-r--r--   0        0        0     6881 2023-06-30 17:30:53.043169 omicverse-1.4.6/omicverse/single/_simba.py
--rw-r--r--   0        0        0    76671 2023-06-01 04:07:49.828205 omicverse-1.4.6/omicverse/single/_via.py
--rw-r--r--   0        0        0      119 2023-05-27 07:38:46.307128 omicverse-1.4.6/omicverse/utils/__init__.py
--rw-r--r--   0        0        0    20648 2023-07-04 04:33:59.513362 omicverse-1.4.6/omicverse/utils/_data.py
--rw-r--r--   0        0        0     2343 2023-06-01 08:49:06.326555 omicverse-1.4.6/omicverse/utils/_enum.py
--rw-r--r--   0        0        0    20283 2023-05-17 14:52:53.358978 omicverse-1.4.6/omicverse/utils/_genomics.py
--rw-r--r--   0        0        0     2520 2023-05-27 07:38:06.457609 omicverse-1.4.6/omicverse/utils/_mde.py
--rw-r--r--   0        0        0    20976 2023-07-03 12:16:48.885839 omicverse-1.4.6/omicverse/utils/_plot.py
--rw-r--r--   0        0        0      441 2023-04-07 07:58:16.954693 omicverse-1.4.6/omicverse/via/.idea/VIA.iml
--rw-r--r--   0        0        0      143 2023-04-07 07:58:16.954828 omicverse-1.4.6/omicverse/via/__init__.py
--rw-r--r--   0        0        0   195125 2023-06-05 08:57:05.073678 omicverse-1.4.6/omicverse/via/core.py
--rw-r--r--   0        0        0     9600 2023-04-08 07:58:12.917564 omicverse-1.4.6/omicverse/via/datasets_via.py
--rw-r--r--   0        0        0   160685 2023-04-07 08:26:01.905887 omicverse-1.4.6/omicverse/via/examples.py
--rw-r--r--   0        0        0   145530 2023-04-07 16:00:02.788869 omicverse-1.4.6/omicverse/via/plotting_via.py
--rw-r--r--   0        0        0    74940 2023-07-04 04:15:25.007972 omicverse-1.4.6/omicverse/via/utils_via.py
--rw-r--r--   0        0        0     7987 2023-04-07 07:58:16.958047 omicverse-1.4.6/omicverse/via/windmap.py
--rw-r--r--   0        0        0     1872 2023-07-04 04:55:20.031792 omicverse-1.4.6/pyproject.toml
--rw-r--r--   0        0        0     8528 1970-01-01 00:00:00.000000 omicverse-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-09-03 17:16:03.066315 omicverse-1.4.7/LICENSE
+-rw-r--r--   0        0        0     6588 2023-07-03 13:00:37.272915 omicverse-1.4.7/README.md
+-rw-r--r--   0        0        0    14340 2023-05-30 08:19:15.462907 omicverse-1.4.7/omicverse/.DS_Store
+-rw-r--r--   0        0        0      320 2022-09-07 04:15:30.431190 omicverse-1.4.7/omicverse/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0      347 2023-05-30 08:29:23.892622 omicverse-1.4.7/omicverse/__init__.py
+-rw-r--r--   0        0        0     6148 2023-04-03 18:27:15.377061 omicverse-1.4.7/omicverse/bulk/.DS_Store
+-rw-r--r--   0        0        0    22181 2023-05-17 18:38:47.881174 omicverse-1.4.7/omicverse/bulk/_Deseq2.py
+-rw-r--r--   0        0        0    21069 2023-07-04 03:40:00.025229 omicverse-1.4.7/omicverse/bulk/_Enrichment.py
+-rw-r--r--   0        0        0    28860 2023-05-17 07:33:38.724769 omicverse-1.4.7/omicverse/bulk/_Gene_module.py
+-rw-r--r--   0        0        0      591 2023-05-17 18:34:20.109930 omicverse-1.4.7/omicverse/bulk/__init__.py
+-rw-r--r--   0        0        0   633338 2023-04-03 07:50:58.899031 omicverse-1.4.7/omicverse/bulk/_chm13.py
+-rw-r--r--   0        0        0     1633 2022-09-06 14:17:42.730883 omicverse-1.4.7/omicverse/bulk/_df_apply.py
+-rw-r--r--   0        0        0    42804 2022-09-06 14:17:42.731609 omicverse-1.4.7/omicverse/bulk/_dynamicTree.py
+-rw-r--r--   0        0        0     6672 2023-04-05 07:48:28.207285 omicverse-1.4.7/omicverse/bulk/_network.py
+-rw-r--r--   0        0        0    12290 2023-04-05 17:42:26.435325 omicverse-1.4.7/omicverse/bulk/_tcga.py
+-rw-r--r--   0        0        0      275 2023-05-27 07:42:00.305669 omicverse-1.4.7/omicverse/bulk2single/__init__.py
+-rw-r--r--   0        0        0    11376 2023-04-06 06:59:09.524952 omicverse-1.4.7/omicverse/bulk2single/_bulk2single.py
+-rw-r--r--   0        0        0    13828 2023-07-04 03:40:49.861005 omicverse-1.4.7/omicverse/bulk2single/_bulktrajblend.py
+-rw-r--r--   0        0        0    29806 2023-05-06 16:11:04.140905 omicverse-1.4.7/omicverse/bulk2single/_map_utils.py
+-rw-r--r--   0        0        0    24978 2023-05-17 10:51:23.881340 omicverse-1.4.7/omicverse/bulk2single/_map_utils1.py
+-rw-r--r--   0        0        0    12746 2023-04-14 09:44:12.354770 omicverse-1.4.7/omicverse/bulk2single/_single2spatial.py
+-rw-r--r--   0        0        0    10462 2023-05-14 07:19:07.135859 omicverse-1.4.7/omicverse/bulk2single/_utils.py
+-rw-r--r--   0        0        0     8560 2023-04-06 07:00:58.204356 omicverse-1.4.7/omicverse/bulk2single/_vae.py
+-rw-r--r--   0        0        0       48 2023-05-30 08:00:53.496990 omicverse-1.4.7/omicverse/cylib/README.rst
+-rw-r--r--   0        0        0       25 2023-05-31 17:51:38.764877 omicverse-1.4.7/omicverse/cylib/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-31 17:55:48.200546 omicverse-1.4.7/omicverse/cylib/fast_utils.py
+-rw-r--r--   0        0        0     1313 2023-05-30 08:00:53.497082 omicverse-1.4.7/omicverse/data_files/README.md
+-rw-r--r--   0        0        0      613 2023-05-30 08:00:53.497137 omicverse-1.4.7/omicverse/data_files/apoptosis_human.gmt
+-rw-r--r--   0        0        0      598 2023-05-30 08:00:53.497199 omicverse-1.4.7/omicverse/data_files/apoptosis_mouse.gmt
+-rw-r--r--   0        0        0  1277787 2023-05-30 08:00:53.501091 omicverse-1.4.7/omicverse/data_files/c2.cp.v7.5.1.symbols.gmt
+-rw-r--r--   0        0        0      597 2023-05-30 08:00:53.501212 omicverse-1.4.7/omicverse/data_files/cell_cycle_human.gmt
+-rw-r--r--   0        0        0      597 2023-05-30 08:00:53.501283 omicverse-1.4.7/omicverse/data_files/cell_cycle_mouse.gmt
+-rw-r--r--   0        0        0      222 2023-05-30 08:00:53.501354 omicverse-1.4.7/omicverse/data_files/emt_human.gmt
+-rw-r--r--   0        0        0      230 2023-05-30 08:00:53.501426 omicverse-1.4.7/omicverse/data_files/gender_human.gmt
+-rw-r--r--   0        0        0      142 2023-05-30 08:00:53.501498 omicverse-1.4.7/omicverse/data_files/gender_mouse.gmt
+-rw-r--r--   0        0        0    48244 2023-05-30 08:00:53.501752 omicverse-1.4.7/omicverse/data_files/h.all.v7.5.1.symbols.gmt
+-rw-r--r--   0        0        0     2725 2023-05-30 08:00:53.501840 omicverse-1.4.7/omicverse/data_files/human_lung.gmt
+-rw-r--r--   0        0        0      743 2023-05-30 08:00:53.501906 omicverse-1.4.7/omicverse/data_files/human_t_cell_markers.gmt
+-rw-r--r--   0        0        0      929 2023-05-30 08:00:53.502035 omicverse-1.4.7/omicverse/data_files/mitochondrial_genes_human.gmt
+-rw-r--r--   0        0        0      930 2023-05-30 08:00:53.502100 omicverse-1.4.7/omicverse/data_files/mitochondrial_genes_mouse.gmt
+-rw-r--r--   0        0        0      706 2023-05-30 08:00:53.502165 omicverse-1.4.7/omicverse/data_files/mouse_brain.gmt
+-rw-r--r--   0        0        0     1931 2023-05-30 08:00:53.502238 omicverse-1.4.7/omicverse/data_files/mouse_liver.gmt
+-rw-r--r--   0        0        0     4068 2023-05-30 08:00:53.502316 omicverse-1.4.7/omicverse/data_files/mouse_lung.gmt
+-rw-r--r--   0        0        0      787 2023-05-30 08:00:53.502394 omicverse-1.4.7/omicverse/data_files/ribosomal_genes_human.gmt
+-rw-r--r--   0        0        0      801 2023-05-30 08:00:53.502468 omicverse-1.4.7/omicverse/data_files/ribosomal_genes_mouse.gmt
+-rw-r--r--   0        0        0       55 2022-09-07 09:33:07.470218 omicverse-1.4.7/omicverse/mofapy2/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-07 09:33:07.470284 omicverse-1.4.7/omicverse/mofapy2/build_model/__init__.py
+-rw-r--r--   0        0        0    13189 2022-09-07 10:12:11.559603 omicverse-1.4.7/omicverse/mofapy2/build_model/build_model.py
+-rw-r--r--   0        0        0    28425 2022-09-07 10:12:16.240298 omicverse-1.4.7/omicverse/mofapy2/build_model/init_model.py
+-rw-r--r--   0        0        0    25076 2022-09-07 10:12:21.681277 omicverse-1.4.7/omicverse/mofapy2/build_model/save_model.py
+-rw-r--r--   0        0        0      637 2022-09-07 10:12:26.660116 omicverse-1.4.7/omicverse/mofapy2/build_model/train_model.py
+-rw-r--r--   0        0        0     3366 2022-09-07 10:12:30.366961 omicverse-1.4.7/omicverse/mofapy2/build_model/utils.py
+-rw-r--r--   0        0        0      405 2022-09-07 09:33:07.470940 omicverse-1.4.7/omicverse/mofapy2/config.py
+-rw-r--r--   0        0        0    26036 2022-09-07 10:13:08.257046 omicverse-1.4.7/omicverse/mofapy2/core/BayesNet.py
+-rw-r--r--   0        0        0       21 2022-09-07 09:33:07.471206 omicverse-1.4.7/omicverse/mofapy2/core/__init__.py
+-rw-r--r--   0        0        0      448 2022-09-07 09:33:07.471309 omicverse-1.4.7/omicverse/mofapy2/core/distributions/__init__.py
+-rw-r--r--   0        0        0     3923 2022-09-07 09:33:07.471393 omicverse-1.4.7/omicverse/mofapy2/core/distributions/basic_distributions.py
+-rw-r--r--   0        0        0     1301 2022-09-07 10:20:27.422096 omicverse-1.4.7/omicverse/mofapy2/core/distributions/bernoulli.py
+-rw-r--r--   0        0        0     4709 2022-09-07 10:20:18.413617 omicverse-1.4.7/omicverse/mofapy2/core/distributions/bernoulli_gaussian.py
+-rw-r--r--   0        0        0     1859 2022-09-07 10:20:33.345355 omicverse-1.4.7/omicverse/mofapy2/core/distributions/beta.py
+-rw-r--r--   0        0        0     1928 2022-09-07 10:20:37.394428 omicverse-1.4.7/omicverse/mofapy2/core/distributions/binomial.py
+-rw-r--r--   0        0        0     2061 2022-09-07 10:20:40.951879 omicverse-1.4.7/omicverse/mofapy2/core/distributions/gamma.py
+-rw-r--r--   0        0        0    38150 2022-09-07 09:33:07.471983 omicverse-1.4.7/omicverse/mofapy2/core/distributions/multi_task_GP.py
+-rw-r--r--   0        0        0    16083 2022-09-07 10:20:53.092939 omicverse-1.4.7/omicverse/mofapy2/core/distributions/multivariate_gaussian.py
+-rw-r--r--   0        0        0     1663 2022-09-07 10:20:57.661446 omicverse-1.4.7/omicverse/mofapy2/core/distributions/poisson.py
+-rw-r--r--   0        0        0     2223 2022-09-07 10:21:03.520320 omicverse-1.4.7/omicverse/mofapy2/core/distributions/univariate_gaussian.py
+-rw-r--r--   0        0        0     5591 2022-09-07 09:33:07.472344 omicverse-1.4.7/omicverse/mofapy2/core/gp_utils.py
+-rw-r--r--   0        0        0     1765 2022-09-07 09:33:07.472409 omicverse-1.4.7/omicverse/mofapy2/core/gpu_utils.py
+-rw-r--r--   0        0        0     6291 2022-09-07 09:33:07.472554 omicverse-1.4.7/omicverse/mofapy2/core/nodes/Alpha_nodes.py
+-rw-r--r--   0        0        0     4646 2022-09-07 10:16:08.287697 omicverse-1.4.7/omicverse/mofapy2/core/nodes/Kc_node.py
+-rw-r--r--   0        0        0     3581 2022-09-07 10:16:52.659105 omicverse-1.4.7/omicverse/mofapy2/core/nodes/Kg_node.py
+-rw-r--r--   0        0        0    49309 2022-09-07 10:22:30.858460 omicverse-1.4.7/omicverse/mofapy2/core/nodes/Sigma_node.py
+-rwxr-xr-x   0        0        0     5327 2022-09-07 10:18:15.524786 omicverse-1.4.7/omicverse/mofapy2/core/nodes/Tau_nodes.py
+-rw-r--r--   0        0        0     6551 2022-09-07 09:33:07.473126 omicverse-1.4.7/omicverse/mofapy2/core/nodes/Theta_nodes.py
+-rw-r--r--   0        0        0     7911 2022-09-07 10:18:33.209503 omicverse-1.4.7/omicverse/mofapy2/core/nodes/U_nodes.py
+-rwxr-xr-x   0        0        0    10037 2022-09-07 10:18:50.380099 omicverse-1.4.7/omicverse/mofapy2/core/nodes/W_nodes.py
+-rw-r--r--   0        0        0     3577 2022-09-07 10:18:59.577240 omicverse-1.4.7/omicverse/mofapy2/core/nodes/Y_nodes.py
+-rwxr-xr-x   0        0        0    15625 2022-09-07 10:19:28.866210 omicverse-1.4.7/omicverse/mofapy2/core/nodes/Z_nodes.py
+-rw-r--r--   0        0        0     9248 2022-09-07 10:19:17.982574 omicverse-1.4.7/omicverse/mofapy2/core/nodes/Z_nodes_GP.py
+-rw-r--r--   0        0        0     8127 2022-09-07 10:19:10.770163 omicverse-1.4.7/omicverse/mofapy2/core/nodes/Z_nodes_GP_mv.py
+-rw-r--r--   0        0        0     7505 2022-09-07 10:19:37.520420 omicverse-1.4.7/omicverse/mofapy2/core/nodes/ZgU_node.py
+-rw-r--r--   0        0        0      581 2022-09-07 09:33:07.473827 omicverse-1.4.7/omicverse/mofapy2/core/nodes/__init__.py
+-rw-r--r--   0        0        0     3812 2022-09-07 10:14:43.810952 omicverse-1.4.7/omicverse/mofapy2/core/nodes/basic_nodes.py
+-rw-r--r--   0        0        0     6837 2022-09-07 09:33:07.473999 omicverse-1.4.7/omicverse/mofapy2/core/nodes/multiview_nodes.py
+-rw-r--r--   0        0        0    21096 2022-09-07 10:17:25.117004 omicverse-1.4.7/omicverse/mofapy2/core/nodes/nongaussian_nodes.py
+-rw-r--r--   0        0        0    11994 2022-09-07 10:18:40.408370 omicverse-1.4.7/omicverse/mofapy2/core/nodes/variational_nodes.py
+-rw-r--r--   0        0        0     3764 2022-09-07 09:33:07.474508 omicverse-1.4.7/omicverse/mofapy2/core/utils.py
+-rw-r--r--   0        0        0        0 2022-09-07 09:33:07.474782 omicverse-1.4.7/omicverse/mofapy2/run/__init__.py
+-rw-r--r--   0        0        0    70968 2023-05-18 07:48:53.001053 omicverse-1.4.7/omicverse/mofapy2/run/entry_point.py
+-rw-r--r--   0        0        0   324931 2022-09-07 09:33:07.476317 omicverse-1.4.7/omicverse/mofapy2/run/test_data/view_0.txt
+-rw-r--r--   0        0        0   324642 2022-09-07 09:33:07.477843 omicverse-1.4.7/omicverse/mofapy2/run/test_data/view_1.txt
+-rw-r--r--   0        0        0   324951 2022-09-07 09:33:07.478979 omicverse-1.4.7/omicverse/mofapy2/run/test_data/view_2.txt
+-rw-r--r--   0        0        0   996145 2022-09-07 09:33:07.483410 omicverse-1.4.7/omicverse/mofapy2/run/test_data/with_nas/500_0.txt
+-rw-r--r--   0        0        0   996423 2022-09-07 09:33:07.486212 omicverse-1.4.7/omicverse/mofapy2/run/test_data/with_nas/500_1.txt
+-rw-r--r--   0        0        0   995502 2022-09-07 09:33:07.486904 omicverse-1.4.7/omicverse/mofapy2/run/test_data/with_nas/500_2.txt
+-rw-r--r--   0        0        0        0 2022-09-07 09:33:07.486988 omicverse-1.4.7/omicverse/mofapy2/simulate/__init__.py
+-rw-r--r--   0        0        0     6509 2022-09-07 10:10:46.603319 omicverse-1.4.7/omicverse/mofapy2/simulate/simulate_mofa.py
+-rw-r--r--   0        0        0       22 2022-09-07 09:33:07.487160 omicverse-1.4.7/omicverse/mofapy2/version.py
+-rw-r--r--   0        0        0     1301 2022-09-07 04:15:14.083982 omicverse-1.4.7/omicverse/nocd/.ipynb_checkpoints/generate-checkpoint.py
+-rw-r--r--   0        0        0     1681 2022-09-07 04:15:14.092998 omicverse-1.4.7/omicverse/nocd/.ipynb_checkpoints/sampler-checkpoint.py
+-rw-r--r--   0        0        0     4558 2022-09-07 04:15:14.093212 omicverse-1.4.7/omicverse/nocd/.ipynb_checkpoints/train-checkpoint.py
+-rw-r--r--   0        0        0     5051 2022-09-07 04:15:14.078134 omicverse-1.4.7/omicverse/nocd/.ipynb_checkpoints/utils-checkpoint.py
+-rw-r--r--   0        0        0      120 2022-09-07 04:15:14.079001 omicverse-1.4.7/omicverse/nocd/__init__.py
+-rw-r--r--   0        0        0     2163 2022-09-07 04:15:14.083601 omicverse-1.4.7/omicverse/nocd/data.py
+-rw-r--r--   0        0        0     1301 2022-09-07 04:15:14.083982 omicverse-1.4.7/omicverse/nocd/generate.py
+-rw-r--r--   0        0        0     4068 2022-09-07 04:18:20.582316 omicverse-1.4.7/omicverse/nocd/metrics/.ipynb_checkpoints/supervised-checkpoint.py
+-rw-r--r--   0        0        0     3214 2022-09-07 04:15:14.085633 omicverse-1.4.7/omicverse/nocd/metrics/.ipynb_checkpoints/unsupervised-checkpoint.py
+-rw-r--r--   0        0        0       54 2022-09-07 04:15:14.086034 omicverse-1.4.7/omicverse/nocd/metrics/__init__.py
+-rw-r--r--   0        0        0     4068 2022-09-07 04:18:20.582316 omicverse-1.4.7/omicverse/nocd/metrics/supervised.py
+-rw-r--r--   0        0        0     3214 2022-09-07 04:15:14.089087 omicverse-1.4.7/omicverse/nocd/metrics/unsupervised.py
+-rw-r--r--   0        0        0       70 2022-09-07 04:15:14.090185 omicverse-1.4.7/omicverse/nocd/nn/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     4453 2022-09-07 04:15:14.092088 omicverse-1.4.7/omicverse/nocd/nn/.ipynb_checkpoints/decoder-checkpoint.py
+-rw-r--r--   0        0        0     3505 2022-09-07 04:17:34.429490 omicverse-1.4.7/omicverse/nocd/nn/.ipynb_checkpoints/gcn-checkpoint.py
+-rw-r--r--   0        0        0     3610 2022-09-07 04:17:50.594410 omicverse-1.4.7/omicverse/nocd/nn/.ipynb_checkpoints/imrpoved_gcn-checkpoint.py
+-rw-r--r--   0        0        0       70 2022-09-07 04:15:14.090185 omicverse-1.4.7/omicverse/nocd/nn/__init__.py
+-rw-r--r--   0        0        0     4453 2022-09-07 04:15:14.092088 omicverse-1.4.7/omicverse/nocd/nn/decoder.py
+-rw-r--r--   0        0        0     3505 2022-09-07 04:17:34.429490 omicverse-1.4.7/omicverse/nocd/nn/gcn.py
+-rw-r--r--   0        0        0     3610 2022-09-07 04:17:50.594410 omicverse-1.4.7/omicverse/nocd/nn/imrpoved_gcn.py
+-rw-r--r--   0        0        0     1681 2022-09-07 04:15:14.092998 omicverse-1.4.7/omicverse/nocd/sampler.py
+-rw-r--r--   0        0        0     4558 2022-09-07 04:15:14.093212 omicverse-1.4.7/omicverse/nocd/train.py
+-rw-r--r--   0        0        0     5051 2022-09-07 04:15:14.093413 omicverse-1.4.7/omicverse/nocd/utils.py
+-rw-r--r--   0        0        0     4414 2023-05-30 09:52:24.238706 omicverse-1.4.7/omicverse/omicverse.egg-info/PKG-INFO
+-rw-r--r--   0        0        0    13619 2023-05-30 09:52:25.204543 omicverse-1.4.7/omicverse/omicverse.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-05-30 09:52:24.238892 omicverse-1.4.7/omicverse/omicverse.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0      350 2023-05-30 09:52:24.239060 omicverse-1.4.7/omicverse/omicverse.egg-info/requires.txt
+-rw-r--r--   0        0        0       60 2023-05-30 09:52:24.239163 omicverse-1.4.7/omicverse/omicverse.egg-info/top_level.txt
+-rw-r--r--   0        0        0      540 2023-05-30 12:45:44.272518 omicverse-1.4.7/omicverse/pp/__init__.py
+-rw-r--r--   0        0        0    20944 2023-06-30 17:56:24.759600 omicverse-1.4.7/omicverse/pp/_preprocess.py
+-rw-r--r--   0        0        0    16277 2023-06-04 08:31:35.638891 omicverse-1.4.7/omicverse/pp/_qc.py
+-rw-r--r--   0        0        0     6148 2023-04-19 16:48:36.030388 omicverse-1.4.7/omicverse/single/.DS_Store
+-rw-r--r--   0        0        0     8790 2022-09-03 17:16:03.070397 omicverse-1.4.7/omicverse/single/README.md
+-rw-r--r--   0        0        0    61426 2023-06-26 23:50:36.692480 omicverse-1.4.7/omicverse/single/_SCSA.py
+-rw-r--r--   0        0        0      683 2023-07-03 11:55:25.153988 omicverse-1.4.7/omicverse/single/__init__.py
+-rw-r--r--   0        0        0    27379 2023-07-04 05:23:56.110145 omicverse-1.4.7/omicverse/single/_anno.py
+-rw-r--r--   0        0        0     9315 2023-07-04 04:53:14.069596 omicverse-1.4.7/omicverse/single/_aucell.py
+-rwxr-xr-x   0        0        0    21100 2022-09-07 05:59:40.809184 omicverse-1.4.7/omicverse/single/_cosg.py
+-rw-r--r--   0        0        0    12142 2023-07-04 04:23:59.889080 omicverse-1.4.7/omicverse/single/_cpdb.py
+-rw-r--r--   0        0        0    37915 2023-07-04 04:36:23.334945 omicverse-1.4.7/omicverse/single/_mofa.py
+-rw-r--r--   0        0        0    10053 2023-05-27 09:28:40.824071 omicverse-1.4.7/omicverse/single/_nocd.py
+-rw-r--r--   0        0        0    18135 2023-04-03 15:03:48.751508 omicverse-1.4.7/omicverse/single/_scdrug.py
+-rw-r--r--   0        0        0    12302 2023-05-15 08:29:21.026574 omicverse-1.4.7/omicverse/single/_scgsea.py
+-rw-r--r--   0        0        0     6881 2023-06-30 17:30:53.043169 omicverse-1.4.7/omicverse/single/_simba.py
+-rw-r--r--   0        0        0    76671 2023-06-01 04:07:49.828205 omicverse-1.4.7/omicverse/single/_via.py
+-rw-r--r--   0        0        0      119 2023-05-27 07:38:46.307128 omicverse-1.4.7/omicverse/utils/__init__.py
+-rw-r--r--   0        0        0    20648 2023-07-04 04:33:59.513362 omicverse-1.4.7/omicverse/utils/_data.py
+-rw-r--r--   0        0        0     2343 2023-06-01 08:49:06.326555 omicverse-1.4.7/omicverse/utils/_enum.py
+-rw-r--r--   0        0        0    20283 2023-05-17 14:52:53.358978 omicverse-1.4.7/omicverse/utils/_genomics.py
+-rw-r--r--   0        0        0     2520 2023-05-27 07:38:06.457609 omicverse-1.4.7/omicverse/utils/_mde.py
+-rw-r--r--   0        0        0    20976 2023-07-03 12:16:48.885839 omicverse-1.4.7/omicverse/utils/_plot.py
+-rw-r--r--   0        0        0      441 2023-04-07 07:58:16.954693 omicverse-1.4.7/omicverse/via/.idea/VIA.iml
+-rw-r--r--   0        0        0      143 2023-04-07 07:58:16.954828 omicverse-1.4.7/omicverse/via/__init__.py
+-rw-r--r--   0        0        0   195125 2023-06-05 08:57:05.073678 omicverse-1.4.7/omicverse/via/core.py
+-rw-r--r--   0        0        0     9600 2023-04-08 07:58:12.917564 omicverse-1.4.7/omicverse/via/datasets_via.py
+-rw-r--r--   0        0        0   160685 2023-04-07 08:26:01.905887 omicverse-1.4.7/omicverse/via/examples.py
+-rw-r--r--   0        0        0   145530 2023-04-07 16:00:02.788869 omicverse-1.4.7/omicverse/via/plotting_via.py
+-rw-r--r--   0        0        0    74991 2023-07-04 06:04:06.418576 omicverse-1.4.7/omicverse/via/utils_via.py
+-rw-r--r--   0        0        0     7987 2023-04-07 07:58:16.958047 omicverse-1.4.7/omicverse/via/windmap.py
+-rw-r--r--   0        0        0     1872 2023-07-04 06:02:25.504971 omicverse-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0     8528 1970-01-01 00:00:00.000000 omicverse-1.4.7/PKG-INFO
```

### Comparing `omicverse-1.4.6/LICENSE` & `omicverse-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/README.md` & `omicverse-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/.DS_Store` & `omicverse-1.4.7/omicverse/.DS_Store`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk/.DS_Store` & `omicverse-1.4.7/omicverse/bulk/.DS_Store`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk/_Deseq2.py` & `omicverse-1.4.7/omicverse/bulk/_Deseq2.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk/_Enrichment.py` & `omicverse-1.4.7/omicverse/bulk/_Enrichment.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk/_Gene_module.py` & `omicverse-1.4.7/omicverse/bulk/_Gene_module.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk/__init__.py` & `omicverse-1.4.7/omicverse/bulk/__init__.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk/_chm13.py` & `omicverse-1.4.7/omicverse/bulk/_chm13.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk/_df_apply.py` & `omicverse-1.4.7/omicverse/bulk/_df_apply.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk/_dynamicTree.py` & `omicverse-1.4.7/omicverse/bulk/_dynamicTree.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk/_network.py` & `omicverse-1.4.7/omicverse/bulk/_network.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk/_tcga.py` & `omicverse-1.4.7/omicverse/bulk/_tcga.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk2single/_bulk2single.py` & `omicverse-1.4.7/omicverse/bulk2single/_bulk2single.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk2single/_bulktrajblend.py` & `omicverse-1.4.7/omicverse/bulk2single/_bulktrajblend.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk2single/_map_utils.py` & `omicverse-1.4.7/omicverse/bulk2single/_map_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk2single/_map_utils1.py` & `omicverse-1.4.7/omicverse/bulk2single/_map_utils1.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk2single/_single2spatial.py` & `omicverse-1.4.7/omicverse/bulk2single/_single2spatial.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk2single/_utils.py` & `omicverse-1.4.7/omicverse/bulk2single/_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/bulk2single/_vae.py` & `omicverse-1.4.7/omicverse/bulk2single/_vae.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/cylib/fast_utils.py` & `omicverse-1.4.7/omicverse/cylib/fast_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/README.md` & `omicverse-1.4.7/omicverse/data_files/README.md`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/apoptosis_human.gmt` & `omicverse-1.4.7/omicverse/data_files/apoptosis_human.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/apoptosis_mouse.gmt` & `omicverse-1.4.7/omicverse/data_files/apoptosis_mouse.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/c2.cp.v7.5.1.symbols.gmt` & `omicverse-1.4.7/omicverse/data_files/c2.cp.v7.5.1.symbols.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/cell_cycle_human.gmt` & `omicverse-1.4.7/omicverse/data_files/cell_cycle_human.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/cell_cycle_mouse.gmt` & `omicverse-1.4.7/omicverse/data_files/cell_cycle_mouse.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/h.all.v7.5.1.symbols.gmt` & `omicverse-1.4.7/omicverse/data_files/h.all.v7.5.1.symbols.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/human_lung.gmt` & `omicverse-1.4.7/omicverse/data_files/human_lung.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/human_t_cell_markers.gmt` & `omicverse-1.4.7/omicverse/data_files/human_t_cell_markers.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/mitochondrial_genes_human.gmt` & `omicverse-1.4.7/omicverse/data_files/mitochondrial_genes_human.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/mitochondrial_genes_mouse.gmt` & `omicverse-1.4.7/omicverse/data_files/mitochondrial_genes_mouse.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/mouse_brain.gmt` & `omicverse-1.4.7/omicverse/data_files/mouse_brain.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/mouse_liver.gmt` & `omicverse-1.4.7/omicverse/data_files/mouse_liver.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/mouse_lung.gmt` & `omicverse-1.4.7/omicverse/data_files/mouse_lung.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/ribosomal_genes_human.gmt` & `omicverse-1.4.7/omicverse/data_files/ribosomal_genes_human.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/data_files/ribosomal_genes_mouse.gmt` & `omicverse-1.4.7/omicverse/data_files/ribosomal_genes_mouse.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/build_model/build_model.py` & `omicverse-1.4.7/omicverse/mofapy2/build_model/build_model.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/build_model/init_model.py` & `omicverse-1.4.7/omicverse/mofapy2/build_model/init_model.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/build_model/save_model.py` & `omicverse-1.4.7/omicverse/mofapy2/build_model/save_model.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/build_model/train_model.py` & `omicverse-1.4.7/omicverse/mofapy2/build_model/train_model.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/build_model/utils.py` & `omicverse-1.4.7/omicverse/mofapy2/build_model/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/BayesNet.py` & `omicverse-1.4.7/omicverse/mofapy2/core/BayesNet.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/distributions/basic_distributions.py` & `omicverse-1.4.7/omicverse/mofapy2/core/distributions/basic_distributions.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/distributions/bernoulli.py` & `omicverse-1.4.7/omicverse/mofapy2/core/distributions/bernoulli.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/distributions/bernoulli_gaussian.py` & `omicverse-1.4.7/omicverse/mofapy2/core/distributions/bernoulli_gaussian.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/distributions/beta.py` & `omicverse-1.4.7/omicverse/mofapy2/core/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/distributions/binomial.py` & `omicverse-1.4.7/omicverse/mofapy2/core/distributions/binomial.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/distributions/gamma.py` & `omicverse-1.4.7/omicverse/mofapy2/core/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/distributions/multi_task_GP.py` & `omicverse-1.4.7/omicverse/mofapy2/core/distributions/multi_task_GP.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/distributions/multivariate_gaussian.py` & `omicverse-1.4.7/omicverse/mofapy2/core/distributions/multivariate_gaussian.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/distributions/poisson.py` & `omicverse-1.4.7/omicverse/mofapy2/core/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/distributions/univariate_gaussian.py` & `omicverse-1.4.7/omicverse/mofapy2/core/distributions/univariate_gaussian.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/gp_utils.py` & `omicverse-1.4.7/omicverse/mofapy2/core/gp_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/gpu_utils.py` & `omicverse-1.4.7/omicverse/mofapy2/core/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/Alpha_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/Alpha_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/Kc_node.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/Kc_node.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/Kg_node.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/Kg_node.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/Sigma_node.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/Sigma_node.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/Tau_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/Tau_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/Theta_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/Theta_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/U_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/U_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/W_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/W_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/Y_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/Y_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/Z_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/Z_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/Z_nodes_GP.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/Z_nodes_GP.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/Z_nodes_GP_mv.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/Z_nodes_GP_mv.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/ZgU_node.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/ZgU_node.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/__init__.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/basic_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/multiview_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/multiview_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/nongaussian_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/nongaussian_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/nodes/variational_nodes.py` & `omicverse-1.4.7/omicverse/mofapy2/core/nodes/variational_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/core/utils.py` & `omicverse-1.4.7/omicverse/mofapy2/core/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/run/entry_point.py` & `omicverse-1.4.7/omicverse/mofapy2/run/entry_point.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/run/test_data/view_0.txt` & `omicverse-1.4.7/omicverse/mofapy2/run/test_data/view_0.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/run/test_data/view_1.txt` & `omicverse-1.4.7/omicverse/mofapy2/run/test_data/view_1.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/run/test_data/view_2.txt` & `omicverse-1.4.7/omicverse/mofapy2/run/test_data/view_2.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/run/test_data/with_nas/500_0.txt` & `omicverse-1.4.7/omicverse/mofapy2/run/test_data/with_nas/500_0.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/run/test_data/with_nas/500_1.txt` & `omicverse-1.4.7/omicverse/mofapy2/run/test_data/with_nas/500_1.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/run/test_data/with_nas/500_2.txt` & `omicverse-1.4.7/omicverse/mofapy2/run/test_data/with_nas/500_2.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/mofapy2/simulate/simulate_mofa.py` & `omicverse-1.4.7/omicverse/mofapy2/simulate/simulate_mofa.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/.ipynb_checkpoints/generate-checkpoint.py` & `omicverse-1.4.7/omicverse/nocd/.ipynb_checkpoints/generate-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/.ipynb_checkpoints/sampler-checkpoint.py` & `omicverse-1.4.7/omicverse/nocd/.ipynb_checkpoints/sampler-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/.ipynb_checkpoints/train-checkpoint.py` & `omicverse-1.4.7/omicverse/nocd/.ipynb_checkpoints/train-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/.ipynb_checkpoints/utils-checkpoint.py` & `omicverse-1.4.7/omicverse/nocd/.ipynb_checkpoints/utils-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/data.py` & `omicverse-1.4.7/omicverse/nocd/data.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/generate.py` & `omicverse-1.4.7/omicverse/nocd/generate.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/metrics/.ipynb_checkpoints/supervised-checkpoint.py` & `omicverse-1.4.7/omicverse/nocd/metrics/.ipynb_checkpoints/supervised-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/metrics/.ipynb_checkpoints/unsupervised-checkpoint.py` & `omicverse-1.4.7/omicverse/nocd/metrics/.ipynb_checkpoints/unsupervised-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/metrics/supervised.py` & `omicverse-1.4.7/omicverse/nocd/metrics/supervised.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/metrics/unsupervised.py` & `omicverse-1.4.7/omicverse/nocd/metrics/unsupervised.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/nn/.ipynb_checkpoints/decoder-checkpoint.py` & `omicverse-1.4.7/omicverse/nocd/nn/.ipynb_checkpoints/decoder-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/nn/.ipynb_checkpoints/gcn-checkpoint.py` & `omicverse-1.4.7/omicverse/nocd/nn/.ipynb_checkpoints/gcn-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/nn/.ipynb_checkpoints/imrpoved_gcn-checkpoint.py` & `omicverse-1.4.7/omicverse/nocd/nn/.ipynb_checkpoints/imrpoved_gcn-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/nn/decoder.py` & `omicverse-1.4.7/omicverse/nocd/nn/decoder.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/nn/gcn.py` & `omicverse-1.4.7/omicverse/nocd/nn/gcn.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/nn/imrpoved_gcn.py` & `omicverse-1.4.7/omicverse/nocd/nn/imrpoved_gcn.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/sampler.py` & `omicverse-1.4.7/omicverse/nocd/sampler.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/train.py` & `omicverse-1.4.7/omicverse/nocd/train.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/nocd/utils.py` & `omicverse-1.4.7/omicverse/nocd/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/omicverse.egg-info/PKG-INFO` & `omicverse-1.4.7/omicverse/omicverse.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/omicverse.egg-info/SOURCES.txt` & `omicverse-1.4.7/omicverse/omicverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/pp/__init__.py` & `omicverse-1.4.7/omicverse/pp/__init__.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/pp/_preprocess.py` & `omicverse-1.4.7/omicverse/pp/_preprocess.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/pp/_qc.py` & `omicverse-1.4.7/omicverse/pp/_qc.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/.DS_Store` & `omicverse-1.4.7/omicverse/single/.DS_Store`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/README.md` & `omicverse-1.4.7/omicverse/single/README.md`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/_SCSA.py` & `omicverse-1.4.7/omicverse/single/_SCSA.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/__init__.py` & `omicverse-1.4.7/omicverse/single/__init__.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/_anno.py` & `omicverse-1.4.7/omicverse/single/_anno.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,16 +597,16 @@
         Arguments:
             save_obs_name: column name for cell type annotation in adata.obs
         
         """
         print('...projecting MeC scores')
         self.pdata=metatime.mecmapper.projectMecAnn(self.adata, self.mecmodel.mec_score)
         projmat, mecscores = metatime.annotator.pdataToTable(self.pdata, self.mectable, gcol = self.clustercol)
-        projmat, gpred, gpreddict = metatime.annotator(projmat,  self.mecnamedict, gcol = self.clustercol)
-        self.adata = metatime.saveToAdata( self.adata, projmat )
+        projmat, gpred, gpreddict = metatime.annotator.annotator(projmat,  self.mecnamedict, gcol = self.clustercol)
+        self.adata = metatime.annotator.saveToAdata( self.adata, projmat)
         #self.pdata = annotator.saveToPdata( self.pdata, self.adata, projmat )
         self.adata.obs[save_obs_name] = self.adata.obs['{}_{}'.format(save_obs_name,self.clustercol)].str.split(': ').str.get(1)
         #self.pdata.obs[save_obs_name] = self.pdata.obs['{}_{}'.format(save_obs_name,self.clustercol)].str.split(': ').str.get(1)
         self.adata.obs['Major_{}'.format(save_obs_name)]=[i.split('_')[0] for i in self.adata.obs[save_obs_name]]
         #self.pdata.obs['Major_{}'.format(save_obs_name)]=[i.split('_')[0] for i in self.pdata.obs[save_obs_name]]
         print('......The predicted celltype have been saved in obs.{}'.format(save_obs_name))
         print('......The predicted major celltype have been saved in obs.Major_{}'.format(save_obs_name))
```

### Comparing `omicverse-1.4.6/omicverse/single/_aucell.py` & `omicverse-1.4.7/omicverse/single/_aucell.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/_cosg.py` & `omicverse-1.4.7/omicverse/single/_cosg.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/_cpdb.py` & `omicverse-1.4.7/omicverse/single/_cpdb.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/_mofa.py` & `omicverse-1.4.7/omicverse/single/_mofa.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/_nocd.py` & `omicverse-1.4.7/omicverse/single/_nocd.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/_scdrug.py` & `omicverse-1.4.7/omicverse/single/_scdrug.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/_scgsea.py` & `omicverse-1.4.7/omicverse/single/_scgsea.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/_simba.py` & `omicverse-1.4.7/omicverse/single/_simba.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/single/_via.py` & `omicverse-1.4.7/omicverse/single/_via.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/utils/_data.py` & `omicverse-1.4.7/omicverse/utils/_data.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/utils/_enum.py` & `omicverse-1.4.7/omicverse/utils/_enum.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/utils/_genomics.py` & `omicverse-1.4.7/omicverse/utils/_genomics.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/utils/_mde.py` & `omicverse-1.4.7/omicverse/utils/_mde.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/utils/_plot.py` & `omicverse-1.4.7/omicverse/utils/_plot.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/via/core.py` & `omicverse-1.4.7/omicverse/via/core.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/via/datasets_via.py` & `omicverse-1.4.7/omicverse/via/datasets_via.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/via/examples.py` & `omicverse-1.4.7/omicverse/via/examples.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/via/plotting_via.py` & `omicverse-1.4.7/omicverse/via/plotting_via.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/omicverse/via/utils_via.py` & `omicverse-1.4.7/omicverse/via/utils_via.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from scipy.sparse import issparse, spmatrix
 import hnswlib
 import time
 import matplotlib
 import igraph as ig
 import matplotlib.pyplot as plt
 from matplotlib.path import get_path_collection_extents
-import s_gd2
+from ..utils import global_imports
 from scipy.spatial.distance import pdist, squareform
 from sklearn.preprocessing import normalize
 import random
 from collections import Counter
 import scipy
 import pygam as pg
 from scipy.sparse.csgraph import minimum_spanning_tree, connected_components
@@ -443,16 +443,18 @@
     -------
     Y : array-like, embedded data [n_sample, ndim]
     """
 
     N = D.shape[0]
     D = squareform(D)
     # Metric MDS from s_gd2
+    global_imports("s_gd2")
     Y = s_gd2.mds_direct(N, D, init=init, random_seed=random_state)
     return Y
+
 def classic(D, n_components=2, random_state=None):
 
     """Fast CMDS using random SVD
     Parameters
     ----------
     D : array-like, shape=[n_samples, n_samples]
         pairwise distances
```

### Comparing `omicverse-1.4.6/omicverse/via/windmap.py` & `omicverse-1.4.7/omicverse/via/windmap.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.4.6/pyproject.toml` & `omicverse-1.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "wheel", "flit_core >=3.4,<4","Cython"]
 build-backend = "flit_core.buildapi"
 
 
 
 [project]
 name = "omicverse"
-version = "1.4.6"
+version = "1.4.7"
 description = "OmicVerse: A single pipeline for exploring the entire transcriptome universe"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "Zehua Zeng", email = "starlitnightly@163.com"},
 ]
```

### Comparing `omicverse-1.4.6/PKG-INFO` & `omicverse-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omicverse
-Version: 1.4.6
+Version: 1.4.7
 Summary: OmicVerse: A single pipeline for exploring the entire transcriptome universe
 Keywords: bioinformatics,deep-learning,single-cell,bulk RNA-seq
 Author-email: Zehua Zeng <starlitnightly@163.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

