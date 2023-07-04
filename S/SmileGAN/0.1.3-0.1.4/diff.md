# Comparing `tmp/SmileGAN-0.1.3.tar.gz` & `tmp/SmileGAN-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SmileGAN-0.1.3.tar", last modified: Tue Nov 15 01:36:23 2022, max compression
+gzip compressed data, was "SmileGAN-0.1.4.tar", last modified: Tue Jul  4 09:08:14 2023, max compression
```

## Comparing `SmileGAN-0.1.3.tar` & `SmileGAN-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 zyang      (501) staff       (20)        0 2022-11-15 01:36:23.815685 SmileGAN-0.1.3/
--rw-r--r--   0 zyang      (501) staff       (20)     1069 2022-07-08 18:42:46.000000 SmileGAN-0.1.3/LICENSE
--rw-r--r--   0 zyang      (501) staff       (20)     8334 2022-11-15 01:36:23.815429 SmileGAN-0.1.3/PKG-INFO
--rw-r--r--   0 zyang      (501) staff       (20)     7886 2022-07-25 20:09:34.000000 SmileGAN-0.1.3/README.md
-drwxr-xr-x   0 zyang      (501) staff       (20)        0 2022-11-15 01:36:23.813188 SmileGAN-0.1.3/SmileGAN/
--rw-r--r--   0 zyang      (501) staff       (20)    14319 2022-11-15 01:32:47.000000 SmileGAN-0.1.3/SmileGAN/Smile_GAN_clustering.py
--rwxr-xr-x   0 zyang      (501) staff       (20)        0 2021-11-24 20:34:06.000000 SmileGAN-0.1.3/SmileGAN/__init__.py
--rw-r--r--   0 zyang      (501) staff       (20)     7646 2022-11-15 01:08:34.000000 SmileGAN-0.1.3/SmileGAN/clustering.py
--rw-r--r--   0 zyang      (501) staff       (20)     3175 2021-11-24 20:34:06.000000 SmileGAN-0.1.3/SmileGAN/data_loading.py
--rw-r--r--   0 zyang      (501) staff       (20)     3368 2022-11-15 01:18:02.000000 SmileGAN-0.1.3/SmileGAN/evaluate.py
--rw-r--r--   0 zyang      (501) staff       (20)     7826 2021-11-24 20:34:06.000000 SmileGAN-0.1.3/SmileGAN/model.py
--rw-r--r--   0 zyang      (501) staff       (20)     1273 2021-11-24 20:34:06.000000 SmileGAN-0.1.3/SmileGAN/modules.py
--rw-r--r--   0 zyang      (501) staff       (20)     3266 2021-11-24 20:34:06.000000 SmileGAN-0.1.3/SmileGAN/networks.py
--rw-r--r--   0 zyang      (501) staff       (20)    10645 2022-03-26 20:06:27.000000 SmileGAN-0.1.3/SmileGAN/utils.py
-drwxr-xr-x   0 zyang      (501) staff       (20)        0 2022-11-15 01:36:23.815101 SmileGAN-0.1.3/SmileGAN.egg-info/
--rw-r--r--   0 zyang      (501) staff       (20)     8334 2022-11-15 01:36:23.000000 SmileGAN-0.1.3/SmileGAN.egg-info/PKG-INFO
--rw-r--r--   0 zyang      (501) staff       (20)      385 2022-11-15 01:36:23.000000 SmileGAN-0.1.3/SmileGAN.egg-info/SOURCES.txt
--rw-r--r--   0 zyang      (501) staff       (20)        1 2022-11-15 01:36:23.000000 SmileGAN-0.1.3/SmileGAN.egg-info/dependency_links.txt
--rw-r--r--   0 zyang      (501) staff       (20)       89 2022-11-15 01:36:23.000000 SmileGAN-0.1.3/SmileGAN.egg-info/requires.txt
--rw-r--r--   0 zyang      (501) staff       (20)        9 2022-11-15 01:36:23.000000 SmileGAN-0.1.3/SmileGAN.egg-info/top_level.txt
--rw-r--r--   0 zyang      (501) staff       (20)       38 2022-11-15 01:36:23.815765 SmileGAN-0.1.3/setup.cfg
--rw-r--r--   0 zyang      (501) staff       (20)      851 2022-11-15 01:35:05.000000 SmileGAN-0.1.3/setup.py
+drwxr-xr-x   0 nyuyzj     (501) staff       (20)        0 2023-07-04 09:08:14.032240 SmileGAN-0.1.4/
+-rw-r--r--   0 nyuyzj     (501) staff       (20)     1069 2023-07-02 10:14:54.000000 SmileGAN-0.1.4/LICENSE
+-rw-r--r--   0 nyuyzj     (501) staff       (20)     9502 2023-07-04 09:08:14.031760 SmileGAN-0.1.4/PKG-INFO
+-rw-r--r--   0 nyuyzj     (501) staff       (20)     7900 2023-07-02 10:14:54.000000 SmileGAN-0.1.4/README.md
+drwxr-xr-x   0 nyuyzj     (501) staff       (20)        0 2023-07-04 09:08:14.027803 SmileGAN-0.1.4/SmileGAN/
+-rw-r--r--   0 nyuyzj     (501) staff       (20)    14319 2023-07-02 10:14:54.000000 SmileGAN-0.1.4/SmileGAN/Smile_GAN_clustering.py
+-rwxr-xr-x   0 nyuyzj     (501) staff       (20)        0 2023-07-02 10:14:54.000000 SmileGAN-0.1.4/SmileGAN/__init__.py
+-rw-r--r--   0 nyuyzj     (501) staff       (20)     7646 2023-07-02 10:14:54.000000 SmileGAN-0.1.4/SmileGAN/clustering.py
+-rw-r--r--   0 nyuyzj     (501) staff       (20)     3175 2023-07-02 10:14:54.000000 SmileGAN-0.1.4/SmileGAN/data_loading.py
+-rw-r--r--   0 nyuyzj     (501) staff       (20)     3224 2023-07-04 08:54:14.000000 SmileGAN-0.1.4/SmileGAN/evaluate.py
+-rw-r--r--   0 nyuyzj     (501) staff       (20)     7826 2023-07-02 10:14:54.000000 SmileGAN-0.1.4/SmileGAN/model.py
+-rw-r--r--   0 nyuyzj     (501) staff       (20)     1273 2023-07-02 10:14:54.000000 SmileGAN-0.1.4/SmileGAN/modules.py
+-rw-r--r--   0 nyuyzj     (501) staff       (20)     3266 2023-07-02 10:14:54.000000 SmileGAN-0.1.4/SmileGAN/networks.py
+-rw-r--r--   0 nyuyzj     (501) staff       (20)    10645 2023-07-02 10:14:54.000000 SmileGAN-0.1.4/SmileGAN/utils.py
+drwxr-xr-x   0 nyuyzj     (501) staff       (20)        0 2023-07-04 09:08:14.030743 SmileGAN-0.1.4/SmileGAN.egg-info/
+-rw-r--r--   0 nyuyzj     (501) staff       (20)     9502 2023-07-04 09:08:13.000000 SmileGAN-0.1.4/SmileGAN.egg-info/PKG-INFO
+-rw-r--r--   0 nyuyzj     (501) staff       (20)      385 2023-07-04 09:08:14.000000 SmileGAN-0.1.4/SmileGAN.egg-info/SOURCES.txt
+-rw-r--r--   0 nyuyzj     (501) staff       (20)        1 2023-07-04 09:08:13.000000 SmileGAN-0.1.4/SmileGAN.egg-info/dependency_links.txt
+-rw-r--r--   0 nyuyzj     (501) staff       (20)       89 2023-07-04 09:08:13.000000 SmileGAN-0.1.4/SmileGAN.egg-info/requires.txt
+-rw-r--r--   0 nyuyzj     (501) staff       (20)        9 2023-07-04 09:08:13.000000 SmileGAN-0.1.4/SmileGAN.egg-info/top_level.txt
+-rw-r--r--   0 nyuyzj     (501) staff       (20)       38 2023-07-04 09:08:14.032417 SmileGAN-0.1.4/setup.cfg
+-rw-r--r--   0 nyuyzj     (501) staff       (20)      851 2023-07-04 09:00:46.000000 SmileGAN-0.1.4/setup.py
```

### Comparing `SmileGAN-0.1.3/LICENSE` & `SmileGAN-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SmileGAN-0.1.3/PKG-INFO` & `SmileGAN-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: SmileGAN
-Version: 0.1.3
-Summary: A python implementation of Smile-GAN for semisupervised clustering
-Home-page: https://github.com/zhijian-yang/SmileGAN
-Author: zhijian.yang
-Author-email: zhijianyang@outlook.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Smile-GAN
 Smile-GAN is a semi-supervised clustering method which is designed to identify disease-related heterogeneity among the patient group. The model effectively avoid variations among normal control (CN) group and cluster patient based on disease related variations only. Semi-supervised clustering of Smile-GAN is achieved through joint training of the mapping and clustering function, where the mapping function can map CN subjects along different mapping directions depending on disease-related variations.
 
 ![image info](./datasets/Smile-GAN.png)
 
 ## License
 Copyright (c) 2016 University of Pennsylvania. All rights reserved. See[ https://www.cbica.upenn.edu/sbia/software/license.html](https://www.cbica.upenn.edu/sbia/software/license.html)
@@ -80,15 +67,15 @@
 
 output_dir = "PATH_OUTPUT_DIR"
 ncluster = 3
 start_saving_epoch = 9000
 max_epoch = 14000
 
 ## three parameters for stopping threshold
-WD = 0.11
+WD = 0.10
 AQ = 20
 cluster_loss = 0.0015
 
 ## one parameter for consensus method
 consensus_type = "highest_matching_clustering"
 ```
 
@@ -102,19 +89,17 @@
 
 ***consensus\_type***: Consensus_type need to be chosen from **"consensus\_clustering"** and **"highest\_matching\_clustering"**. It determines how the final consensus result is derived from k clustering results obtained through the k-fold hold-out CV procedure. **"highest\_matching\_clustering"** is recommended if Adjusted Random Index among k clustering results is greater than 0.3. Otherwise, **"consensus\_clustering"** might give more reliable consensus results. User can always use function **clustering\_result**, trained models and a different consensus\_type to rederive results with different consensus\_type without retraining.
 
 Some other parameters, ***lam***, ***mu***, ***batch\_size***, have default values but need to be changed in some cases:
 
 ***batch\_size***: Size of the batch for each training epoch. (Default to be 25) It is **necessary** to be reset to 1/10 - 1/20 of the PT sample size.
 
-***lam***: coefficient controlling the relative importance of cluster\_loss in training objective function. (Default to be 9) 
-
-***mu***: coefficient controlling the relative importance of change\_loss in training objective function. (Default to be 5). Can be reset to 5.5 or 6 if PT and CN does not have great differences and cluster\_loss does not converge during training procedure. 
-
+***lam***: coefficient controlling the relative importance of cluster\_loss in the training objective function. (Default to be 9) 
 
+***mu***: coefficient controlling the relative importance of change\_loss in the training objective function. (Default to be 5). It is **necessary** to try different values of ***mu*** (***mu*** = 1-7), and chose the value leading to the highest **ARI** (Adjusted Random Index).
 
 ```bash
 single_model_clustering(train_data, ncluster, start_saving_epoch, max_epoch,\
 					    output_dir, WD, AQ, cluster_loss, covariate=covariate)
 ```
 **single\_model\_clustering** performs clustering without cross validation. Since only one model is trained with this function, the model may be not representative or reproducible. Therefore, this function is ***not recommended***. The function automatically saves an csv file with clustering results and returns the same dataframe.
 
@@ -123,15 +108,15 @@
 ```bash				    
 fold_number = 10  # number of folds the leave-out cv runs
 data_fraction = 0.8 # fraction of data used in each fold
 cross_validated_clustering(train_data, ncluster, fold_number, data_fraction, start_saving_epoch, max_epoch,\
 					    output_dir, WD, AQ, cluster_loss, consensus_tpype, covariate=covariate)
 ```
 
-**cross\_validated\_clustering** performs clustering with leave-out cross validation. It is the ***recommended*** function for clustering. Since the CV process may take long training time on a normal desktop computer, the function enables early stop and later resumption. Users can set ***stop\_fold*** to be early stopping point and ***start\_fold*** depending on previous stopping point. The function automatically saves an csv file with clustering results and returns the same dataframe.
+**cross\_validated\_clustering** performs clustering with leave-out cross validation. It is the ***recommended*** function for clustering. Since the CV process may take long training time on a normal desktop computer, the function enables early stop and later resumption. Users can set ***stop\_fold*** to be early stopping point and ***start\_fold*** depending on previous stopping point. The function automatically saves an csv file with clustering results and the mean ARI value.
 
 ```					    
 model_dirs = ['PATH_TO_CHECKPOINT1','PATH_TO_CHECKPOINT2',...] #list of paths to previously saved checkpoints (with name 'converged_model_foldk' after cv process)
 cluster_label, cluster_probabilities, _, _ = clustering_result(model_dirs, 'highest_matching_clustering', train_data, covariate)
 ```
 **clustering\_result** is a function used for clustering patient data using previously saved models. Input data and covariate (optional) should be panda dataframe with same format shown before. Only PT data (can be inside or outside of training set), for which the user want to derive cluster memberships, need to be provided with diagnoses set to be 1.  ***The function returns cluster labels of PT data following the order of PT in the provided dataframe.*** If ***consensus\_type*** is chosen to be ***'highest\_matching\_clustering***, probabilities of each cluster will also be returned.
```

### Comparing `SmileGAN-0.1.3/README.md` & `SmileGAN-0.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,143 +1,155 @@
-# Smile-GAN
-Smile-GAN is a semi-supervised clustering method which is designed to identify disease-related heterogeneity among the patient group. The model effectively avoid variations among normal control (CN) group and cluster patient based on disease related variations only. Semi-supervised clustering of Smile-GAN is achieved through joint training of the mapping and clustering function, where the mapping function can map CN subjects along different mapping directions depending on disease-related variations.
-
-![image info](./datasets/Smile-GAN.png)
-
-## License
-Copyright (c) 2016 University of Pennsylvania. All rights reserved. See[ https://www.cbica.upenn.edu/sbia/software/license.html](https://www.cbica.upenn.edu/sbia/software/license.html)
-
-## Installation
-We highly recommend the users to install **Anaconda3** on your machine. After installing Anaconda3, Smile-GAN can be used following this procedure:
-
-We recommend the users to use the Conda virtual environment:
-
-```bash
-$ conda create --name smilegan python=3.8
-```
-Activate the virtual environment
-
-```bash
-$ conda activate smilegan
-```
-Install SmileGAN from PyPi:
-
-```bash
-$ pip install SmileGAN
-```
-
-
-
-## Input structure
-Main functions of SmileGAN basically takes two panda dataframes as data inputs, **data** and **covariate** (optional). Columns with name *'participant_id'* and *diagnosis* must exist in both dataframes. Some conventions for the group label/diagnosis: -1 represents healthy control (CN) and 1 represents patient (PT); categorical variables, such as sex, should be encoded to numbers: Female for 0 and Male for 1, for example. 
-
-Example for **data**:
-
-```bash
-participant_id    diagnosis    ROI1    ROI2 ...
-subject-1	    -1         325.4   603.4
-subject-2            1         260.5   580.3
-subject-3           -1         326.5   623.4
-subject-4            1         301.7   590.5
-subject-5            1	       293.1   595.1
-subject-6            1         287.8   608.9
-```
-Example for **covariate**
-
-```bash
-participant_id    diagnosis    age    sex ...
-subject-1	    -1         57.3   0
-subject-2 	     1         43.5   1
-subject-3           -1         53.8   1
-subject-4            1         56.0   0
-subject-5            1	       60.0   1
-subject-6            1         62.5   0
-```
-
-## Example
-We offer a toy dataset in the folder of SmileGAN/dataset.
-
-**Runing SmileGAN for clustering CN vs Subtype1 vs Subtype2 vs ...**
-
-```bash
-import pandas as pd
-from SmileGAN.Smile_GAN_clustering import single_model_clustering, cross_validated_clustering, clustering_result
-
-train_data = pd.read_csv('train_roi.csv')
-covariate = pd.read_csv('train_cov.csv')
-
-output_dir = "PATH_OUTPUT_DIR"
-ncluster = 3
-start_saving_epoch = 9000
-max_epoch = 14000
-
-## three parameters for stopping threshold
-WD = 0.11
-AQ = 20
-cluster_loss = 0.0015
-
-## one parameter for consensus method
-consensus_type = "highest_matching_clustering"
-```
-
-When using the package, ***WD***, ***AQ***, ***cluster\_loss***, ***consensus\_type*** need to be chosen empirically:
-
-***WD***: Wasserstein Distance measures the distance between generated PT data along each direction and real PT data. (**Recommended value**: 0.11-0.14)
-
-***AQ***: Alteration Quantity measures the number of participants who change cluster labels during last three traninig epochs. Low AQ implies convergence of training. (**Recommended value**: 1/20 of PT sample size)
-
-***cluster\_loss***: Cluster loss measures how well clustering function reconstruct sampled Z variable. (**Recommended value**: 0.0015-0.002)
-
-***consensus\_type***: Consensus_type need to be chosen from **"consensus\_clustering"** and **"highest\_matching\_clustering"**. It determines how the final consensus result is derived from k clustering results obtained through the k-fold hold-out CV procedure. **"highest\_matching\_clustering"** is recommended if Adjusted Random Index among k clustering results is greater than 0.3. Otherwise, **"consensus\_clustering"** might give more reliable consensus results. User can always use function **clustering\_result**, trained models and a different consensus\_type to rederive results with different consensus\_type without retraining.
-
-Some other parameters, ***lam***, ***mu***, ***batch\_size***, have default values but need to be changed in some cases:
-
-***batch\_size***: Size of the batch for each training epoch. (Default to be 25) It is **necessary** to be reset to 1/10 - 1/20 of the PT sample size.
-
-***lam***: coefficient controlling the relative importance of cluster\_loss in training objective function. (Default to be 9) 
-
-***mu***: coefficient controlling the relative importance of change\_loss in training objective function. (Default to be 5). Can be reset to 5.5 or 6 if PT and CN does not have great differences and cluster\_loss does not converge during training procedure. 
-
-
-
-```bash
-single_model_clustering(train_data, ncluster, start_saving_epoch, max_epoch,\
-					    output_dir, WD, AQ, cluster_loss, covariate=covariate)
-```
-**single\_model\_clustering** performs clustering without cross validation. Since only one model is trained with this function, the model may be not representative or reproducible. Therefore, this function is ***not recommended***. The function automatically saves an csv file with clustering results and returns the same dataframe.
-
-
-
-```bash				    
-fold_number = 10  # number of folds the leave-out cv runs
-data_fraction = 0.8 # fraction of data used in each fold
-cross_validated_clustering(train_data, ncluster, fold_number, data_fraction, start_saving_epoch, max_epoch,\
-					    output_dir, WD, AQ, cluster_loss, consensus_tpype, covariate=covariate)
-```
-
-**cross\_validated\_clustering** performs clustering with leave-out cross validation. It is the ***recommended*** function for clustering. Since the CV process may take long training time on a normal desktop computer, the function enables early stop and later resumption. Users can set ***stop\_fold*** to be early stopping point and ***start\_fold*** depending on previous stopping point. The function automatically saves an csv file with clustering results and returns the same dataframe.
-
-```					    
-model_dirs = ['PATH_TO_CHECKPOINT1','PATH_TO_CHECKPOINT2',...] #list of paths to previously saved checkpoints (with name 'converged_model_foldk' after cv process)
-cluster_label, cluster_probabilities, _, _ = clustering_result(model_dirs, 'highest_matching_clustering', train_data, covariate)
-```
-**clustering\_result** is a function used for clustering patient data using previously saved models. Input data and covariate (optional) should be panda dataframe with same format shown before. Only PT data (can be inside or outside of training set), for which the user want to derive cluster memberships, need to be provided with diagnoses set to be 1.  ***The function returns cluster labels of PT data following the order of PT in the provided dataframe.*** If ***consensus\_type*** is chosen to be ***'highest\_matching\_clustering***, probabilities of each cluster will also be returned. 
-
-
-## Citation
-If you use this package for research, please cite the following paper:
-
-
-```bash
-@article{yang2021BrainHeterogeneity,
-author = {Yang, Zhijian and Nasrallah, Ilya M. and Shou, Haochang and Wen, Junhao and Doshi, Jimit and Habes, Mohamad and Erus, Guray and Abdulkadir, Ahmed and Resnick, Susan M. and Albert, Marilyn S. and Maruff, Paul and Fripp, Jurgen and Morris, John C. and Wolk, David A. and Davatzikos, Christos and {iSTAGING Consortium} and {Baltimore Longitudinal Study of Aging (BLSA)} and {Alzheimer’s Disease Neuroimaging Initiative (ADNI)}},
-year = {2021},
-month = {12},
-pages = {},
-title = {A deep learning framework identifies dimensional representations of Alzheimer’s Disease from brain structure},
-volume = {12},
-journal = {Nature Communications},
-doi = {10.1038/s41467-021-26703-z}
-}
-```
-
-
+Metadata-Version: 2.1
+Name: SmileGAN
+Version: 0.1.4
+Summary: A python implementation of Smile-GAN for semisupervised clustering
+Home-page: https://github.com/zhijian-yang/SmileGAN
+Author: zhijian.yang
+Author-email: zhijianyang@outlook.com
+License: UNKNOWN
+Description: # Smile-GAN
+        Smile-GAN is a semi-supervised clustering method which is designed to identify disease-related heterogeneity among the patient group. The model effectively avoid variations among normal control (CN) group and cluster patient based on disease related variations only. Semi-supervised clustering of Smile-GAN is achieved through joint training of the mapping and clustering function, where the mapping function can map CN subjects along different mapping directions depending on disease-related variations.
+        
+        ![image info](./datasets/Smile-GAN.png)
+        
+        ## License
+        Copyright (c) 2016 University of Pennsylvania. All rights reserved. See[ https://www.cbica.upenn.edu/sbia/software/license.html](https://www.cbica.upenn.edu/sbia/software/license.html)
+        
+        ## Installation
+        We highly recommend the users to install **Anaconda3** on your machine. After installing Anaconda3, Smile-GAN can be used following this procedure:
+        
+        We recommend the users to use the Conda virtual environment:
+        
+        ```bash
+        $ conda create --name smilegan python=3.8
+        ```
+        Activate the virtual environment
+        
+        ```bash
+        $ conda activate smilegan
+        ```
+        Install SmileGAN from PyPi:
+        
+        ```bash
+        $ pip install SmileGAN
+        ```
+        
+        
+        
+        ## Input structure
+        Main functions of SmileGAN basically takes two panda dataframes as data inputs, **data** and **covariate** (optional). Columns with name *'participant_id'* and *diagnosis* must exist in both dataframes. Some conventions for the group label/diagnosis: -1 represents healthy control (CN) and 1 represents patient (PT); categorical variables, such as sex, should be encoded to numbers: Female for 0 and Male for 1, for example. 
+        
+        Example for **data**:
+        
+        ```bash
+        participant_id    diagnosis    ROI1    ROI2 ...
+        subject-1	    -1         325.4   603.4
+        subject-2            1         260.5   580.3
+        subject-3           -1         326.5   623.4
+        subject-4            1         301.7   590.5
+        subject-5            1	       293.1   595.1
+        subject-6            1         287.8   608.9
+        ```
+        Example for **covariate**
+        
+        ```bash
+        participant_id    diagnosis    age    sex ...
+        subject-1	    -1         57.3   0
+        subject-2 	     1         43.5   1
+        subject-3           -1         53.8   1
+        subject-4            1         56.0   0
+        subject-5            1	       60.0   1
+        subject-6            1         62.5   0
+        ```
+        
+        ## Example
+        We offer a toy dataset in the folder of SmileGAN/dataset.
+        
+        **Runing SmileGAN for clustering CN vs Subtype1 vs Subtype2 vs ...**
+        
+        ```bash
+        import pandas as pd
+        from SmileGAN.Smile_GAN_clustering import single_model_clustering, cross_validated_clustering, clustering_result
+        
+        train_data = pd.read_csv('train_roi.csv')
+        covariate = pd.read_csv('train_cov.csv')
+        
+        output_dir = "PATH_OUTPUT_DIR"
+        ncluster = 3
+        start_saving_epoch = 9000
+        max_epoch = 14000
+        
+        ## three parameters for stopping threshold
+        WD = 0.10
+        AQ = 20
+        cluster_loss = 0.0015
+        
+        ## one parameter for consensus method
+        consensus_type = "highest_matching_clustering"
+        ```
+        
+        When using the package, ***WD***, ***AQ***, ***cluster\_loss***, ***consensus\_type*** need to be chosen empirically:
+        
+        ***WD***: Wasserstein Distance measures the distance between generated PT data along each direction and real PT data. (**Recommended value**: 0.11-0.14)
+        
+        ***AQ***: Alteration Quantity measures the number of participants who change cluster labels during last three traninig epochs. Low AQ implies convergence of training. (**Recommended value**: 1/20 of PT sample size)
+        
+        ***cluster\_loss***: Cluster loss measures how well clustering function reconstruct sampled Z variable. (**Recommended value**: 0.0015-0.002)
+        
+        ***consensus\_type***: Consensus_type need to be chosen from **"consensus\_clustering"** and **"highest\_matching\_clustering"**. It determines how the final consensus result is derived from k clustering results obtained through the k-fold hold-out CV procedure. **"highest\_matching\_clustering"** is recommended if Adjusted Random Index among k clustering results is greater than 0.3. Otherwise, **"consensus\_clustering"** might give more reliable consensus results. User can always use function **clustering\_result**, trained models and a different consensus\_type to rederive results with different consensus\_type without retraining.
+        
+        Some other parameters, ***lam***, ***mu***, ***batch\_size***, have default values but need to be changed in some cases:
+        
+        ***batch\_size***: Size of the batch for each training epoch. (Default to be 25) It is **necessary** to be reset to 1/10 - 1/20 of the PT sample size.
+        
+        ***lam***: coefficient controlling the relative importance of cluster\_loss in the training objective function. (Default to be 9) 
+        
+        ***mu***: coefficient controlling the relative importance of change\_loss in the training objective function. (Default to be 5). It is **necessary** to try different values of ***mu*** (***mu*** = 1-7), and chose the value leading to the highest **ARI** (Adjusted Random Index).
+        
+        ```bash
+        single_model_clustering(train_data, ncluster, start_saving_epoch, max_epoch,\
+        					    output_dir, WD, AQ, cluster_loss, covariate=covariate)
+        ```
+        **single\_model\_clustering** performs clustering without cross validation. Since only one model is trained with this function, the model may be not representative or reproducible. Therefore, this function is ***not recommended***. The function automatically saves an csv file with clustering results and returns the same dataframe.
+        
+        
+        
+        ```bash				    
+        fold_number = 10  # number of folds the leave-out cv runs
+        data_fraction = 0.8 # fraction of data used in each fold
+        cross_validated_clustering(train_data, ncluster, fold_number, data_fraction, start_saving_epoch, max_epoch,\
+        					    output_dir, WD, AQ, cluster_loss, consensus_tpype, covariate=covariate)
+        ```
+        
+        **cross\_validated\_clustering** performs clustering with leave-out cross validation. It is the ***recommended*** function for clustering. Since the CV process may take long training time on a normal desktop computer, the function enables early stop and later resumption. Users can set ***stop\_fold*** to be early stopping point and ***start\_fold*** depending on previous stopping point. The function automatically saves an csv file with clustering results and the mean ARI value.
+        
+        ```					    
+        model_dirs = ['PATH_TO_CHECKPOINT1','PATH_TO_CHECKPOINT2',...] #list of paths to previously saved checkpoints (with name 'converged_model_foldk' after cv process)
+        cluster_label, cluster_probabilities, _, _ = clustering_result(model_dirs, 'highest_matching_clustering', train_data, covariate)
+        ```
+        **clustering\_result** is a function used for clustering patient data using previously saved models. Input data and covariate (optional) should be panda dataframe with same format shown before. Only PT data (can be inside or outside of training set), for which the user want to derive cluster memberships, need to be provided with diagnoses set to be 1.  ***The function returns cluster labels of PT data following the order of PT in the provided dataframe.*** If ***consensus\_type*** is chosen to be ***'highest\_matching\_clustering***, probabilities of each cluster will also be returned. 
+        
+        
+        ## Citation
+        If you use this package for research, please cite the following paper:
+        
+        
+        ```bash
+        @article{yang2021BrainHeterogeneity,
+        author = {Yang, Zhijian and Nasrallah, Ilya M. and Shou, Haochang and Wen, Junhao and Doshi, Jimit and Habes, Mohamad and Erus, Guray and Abdulkadir, Ahmed and Resnick, Susan M. and Albert, Marilyn S. and Maruff, Paul and Fripp, Jurgen and Morris, John C. and Wolk, David A. and Davatzikos, Christos and {iSTAGING Consortium} and {Baltimore Longitudinal Study of Aging (BLSA)} and {Alzheimer’s Disease Neuroimaging Initiative (ADNI)}},
+        year = {2021},
+        month = {12},
+        pages = {},
+        title = {A deep learning framework identifies dimensional representations of Alzheimer’s Disease from brain structure},
+        volume = {12},
+        journal = {Nature Communications},
+        doi = {10.1038/s41467-021-26703-z}
+        }
+        ```
+        
+        
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
```

### Comparing `SmileGAN-0.1.3/SmileGAN/Smile_GAN_clustering.py` & `SmileGAN-0.1.4/SmileGAN/Smile_GAN_clustering.py`

 * *Files identical despite different names*

### Comparing `SmileGAN-0.1.3/SmileGAN/clustering.py` & `SmileGAN-0.1.4/SmileGAN/clustering.py`

 * *Files identical despite different names*

### Comparing `SmileGAN-0.1.3/SmileGAN/data_loading.py` & `SmileGAN-0.1.4/SmileGAN/data_loading.py`

 * *Files identical despite different names*

### Comparing `SmileGAN-0.1.3/SmileGAN/evaluate.py` & `SmileGAN-0.1.4/SmileGAN/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,33 +27,29 @@
     distance=np.sum(np.square(mean_1-mean_2))+np.trace(std_1+std_2-2*sqrtm(sqrtm(std_2).dot(std_1).dot(sqrtm(std_2))))
     return  distance.real
 
 ## return mean wasserstein distance and wasserstein distance of each mapping direction
 def cal_validate_distance(model,mean,std,eva_data,independent,include_std):
     predicted_z=model.predict_cluster(eva_data)
     cluster=[[]for k in range(model.opt.ncluster)]
-    distance=[1000 for m in range(model.opt.ncluster)]
+    distance=[float('inf') for m in range(model.opt.ncluster)]
     adjusted_eva_data=eva_data.detach().numpy()
     for i in range(predicted_z.shape[0]):
         a=predicted_z[i].tolist().index(max(predicted_z[i].tolist()))
         cluster[a].append(adjusted_eva_data[i])
     for j in range(model.opt.ncluster):
         if len(cluster[j])>1:
             cluster_mean=np.mean(np.array(cluster[j]), axis=0)
             if independent:
                 cluster_std=np.std(np.array(cluster[j]), axis=0)
                 distance[j]=cal_w_distance(mean[j],cluster_mean,std[j],cluster_std,include_std)
             else:
                 cluster_std=np.cov(np.transpose(np.array(cluster[j])))
                 distance[j]=cal_w_distance_with_cov(mean[j],cluster_mean,std[j],cluster_std)
-    output=[0 for _ in range(model.opt.ncluster)]
-    for k in range(model.opt.ncluster):
-        if distance[k]!=1000:
-            output[k] = distance[k]
-    return np.mean(output),output
+    return np.mean(distance),distance
       
 def eval_w_distances(real_X,real_Y,model,independent,include_std):
     predict_Y=[]
     mean=[]
     std=[]
     for i in range(model.opt.ncluster):
         z, z_index = sample_z(real_X, model.opt.ncluster, fix_class=i)
```

### Comparing `SmileGAN-0.1.3/SmileGAN/model.py` & `SmileGAN-0.1.4/SmileGAN/model.py`

 * *Files identical despite different names*

### Comparing `SmileGAN-0.1.3/SmileGAN/modules.py` & `SmileGAN-0.1.4/SmileGAN/modules.py`

 * *Files identical despite different names*

### Comparing `SmileGAN-0.1.3/SmileGAN/networks.py` & `SmileGAN-0.1.4/SmileGAN/networks.py`

 * *Files identical despite different names*

### Comparing `SmileGAN-0.1.3/SmileGAN/utils.py` & `SmileGAN-0.1.4/SmileGAN/utils.py`

 * *Files identical despite different names*

### Comparing `SmileGAN-0.1.3/SmileGAN.egg-info/PKG-INFO` & `SmileGAN-0.1.4/SmileGAN.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,156 +1,155 @@
 Metadata-Version: 2.1
 Name: SmileGAN
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python implementation of Smile-GAN for semisupervised clustering
 Home-page: https://github.com/zhijian-yang/SmileGAN
 Author: zhijian.yang
 Author-email: zhijianyang@outlook.com
+License: UNKNOWN
+Description: # Smile-GAN
+        Smile-GAN is a semi-supervised clustering method which is designed to identify disease-related heterogeneity among the patient group. The model effectively avoid variations among normal control (CN) group and cluster patient based on disease related variations only. Semi-supervised clustering of Smile-GAN is achieved through joint training of the mapping and clustering function, where the mapping function can map CN subjects along different mapping directions depending on disease-related variations.
+        
+        ![image info](./datasets/Smile-GAN.png)
+        
+        ## License
+        Copyright (c) 2016 University of Pennsylvania. All rights reserved. See[ https://www.cbica.upenn.edu/sbia/software/license.html](https://www.cbica.upenn.edu/sbia/software/license.html)
+        
+        ## Installation
+        We highly recommend the users to install **Anaconda3** on your machine. After installing Anaconda3, Smile-GAN can be used following this procedure:
+        
+        We recommend the users to use the Conda virtual environment:
+        
+        ```bash
+        $ conda create --name smilegan python=3.8
+        ```
+        Activate the virtual environment
+        
+        ```bash
+        $ conda activate smilegan
+        ```
+        Install SmileGAN from PyPi:
+        
+        ```bash
+        $ pip install SmileGAN
+        ```
+        
+        
+        
+        ## Input structure
+        Main functions of SmileGAN basically takes two panda dataframes as data inputs, **data** and **covariate** (optional). Columns with name *'participant_id'* and *diagnosis* must exist in both dataframes. Some conventions for the group label/diagnosis: -1 represents healthy control (CN) and 1 represents patient (PT); categorical variables, such as sex, should be encoded to numbers: Female for 0 and Male for 1, for example. 
+        
+        Example for **data**:
+        
+        ```bash
+        participant_id    diagnosis    ROI1    ROI2 ...
+        subject-1	    -1         325.4   603.4
+        subject-2            1         260.5   580.3
+        subject-3           -1         326.5   623.4
+        subject-4            1         301.7   590.5
+        subject-5            1	       293.1   595.1
+        subject-6            1         287.8   608.9
+        ```
+        Example for **covariate**
+        
+        ```bash
+        participant_id    diagnosis    age    sex ...
+        subject-1	    -1         57.3   0
+        subject-2 	     1         43.5   1
+        subject-3           -1         53.8   1
+        subject-4            1         56.0   0
+        subject-5            1	       60.0   1
+        subject-6            1         62.5   0
+        ```
+        
+        ## Example
+        We offer a toy dataset in the folder of SmileGAN/dataset.
+        
+        **Runing SmileGAN for clustering CN vs Subtype1 vs Subtype2 vs ...**
+        
+        ```bash
+        import pandas as pd
+        from SmileGAN.Smile_GAN_clustering import single_model_clustering, cross_validated_clustering, clustering_result
+        
+        train_data = pd.read_csv('train_roi.csv')
+        covariate = pd.read_csv('train_cov.csv')
+        
+        output_dir = "PATH_OUTPUT_DIR"
+        ncluster = 3
+        start_saving_epoch = 9000
+        max_epoch = 14000
+        
+        ## three parameters for stopping threshold
+        WD = 0.10
+        AQ = 20
+        cluster_loss = 0.0015
+        
+        ## one parameter for consensus method
+        consensus_type = "highest_matching_clustering"
+        ```
+        
+        When using the package, ***WD***, ***AQ***, ***cluster\_loss***, ***consensus\_type*** need to be chosen empirically:
+        
+        ***WD***: Wasserstein Distance measures the distance between generated PT data along each direction and real PT data. (**Recommended value**: 0.11-0.14)
+        
+        ***AQ***: Alteration Quantity measures the number of participants who change cluster labels during last three traninig epochs. Low AQ implies convergence of training. (**Recommended value**: 1/20 of PT sample size)
+        
+        ***cluster\_loss***: Cluster loss measures how well clustering function reconstruct sampled Z variable. (**Recommended value**: 0.0015-0.002)
+        
+        ***consensus\_type***: Consensus_type need to be chosen from **"consensus\_clustering"** and **"highest\_matching\_clustering"**. It determines how the final consensus result is derived from k clustering results obtained through the k-fold hold-out CV procedure. **"highest\_matching\_clustering"** is recommended if Adjusted Random Index among k clustering results is greater than 0.3. Otherwise, **"consensus\_clustering"** might give more reliable consensus results. User can always use function **clustering\_result**, trained models and a different consensus\_type to rederive results with different consensus\_type without retraining.
+        
+        Some other parameters, ***lam***, ***mu***, ***batch\_size***, have default values but need to be changed in some cases:
+        
+        ***batch\_size***: Size of the batch for each training epoch. (Default to be 25) It is **necessary** to be reset to 1/10 - 1/20 of the PT sample size.
+        
+        ***lam***: coefficient controlling the relative importance of cluster\_loss in the training objective function. (Default to be 9) 
+        
+        ***mu***: coefficient controlling the relative importance of change\_loss in the training objective function. (Default to be 5). It is **necessary** to try different values of ***mu*** (***mu*** = 1-7), and chose the value leading to the highest **ARI** (Adjusted Random Index).
+        
+        ```bash
+        single_model_clustering(train_data, ncluster, start_saving_epoch, max_epoch,\
+        					    output_dir, WD, AQ, cluster_loss, covariate=covariate)
+        ```
+        **single\_model\_clustering** performs clustering without cross validation. Since only one model is trained with this function, the model may be not representative or reproducible. Therefore, this function is ***not recommended***. The function automatically saves an csv file with clustering results and returns the same dataframe.
+        
+        
+        
+        ```bash				    
+        fold_number = 10  # number of folds the leave-out cv runs
+        data_fraction = 0.8 # fraction of data used in each fold
+        cross_validated_clustering(train_data, ncluster, fold_number, data_fraction, start_saving_epoch, max_epoch,\
+        					    output_dir, WD, AQ, cluster_loss, consensus_tpype, covariate=covariate)
+        ```
+        
+        **cross\_validated\_clustering** performs clustering with leave-out cross validation. It is the ***recommended*** function for clustering. Since the CV process may take long training time on a normal desktop computer, the function enables early stop and later resumption. Users can set ***stop\_fold*** to be early stopping point and ***start\_fold*** depending on previous stopping point. The function automatically saves an csv file with clustering results and the mean ARI value.
+        
+        ```					    
+        model_dirs = ['PATH_TO_CHECKPOINT1','PATH_TO_CHECKPOINT2',...] #list of paths to previously saved checkpoints (with name 'converged_model_foldk' after cv process)
+        cluster_label, cluster_probabilities, _, _ = clustering_result(model_dirs, 'highest_matching_clustering', train_data, covariate)
+        ```
+        **clustering\_result** is a function used for clustering patient data using previously saved models. Input data and covariate (optional) should be panda dataframe with same format shown before. Only PT data (can be inside or outside of training set), for which the user want to derive cluster memberships, need to be provided with diagnoses set to be 1.  ***The function returns cluster labels of PT data following the order of PT in the provided dataframe.*** If ***consensus\_type*** is chosen to be ***'highest\_matching\_clustering***, probabilities of each cluster will also be returned. 
+        
+        
+        ## Citation
+        If you use this package for research, please cite the following paper:
+        
+        
+        ```bash
+        @article{yang2021BrainHeterogeneity,
+        author = {Yang, Zhijian and Nasrallah, Ilya M. and Shou, Haochang and Wen, Junhao and Doshi, Jimit and Habes, Mohamad and Erus, Guray and Abdulkadir, Ahmed and Resnick, Susan M. and Albert, Marilyn S. and Maruff, Paul and Fripp, Jurgen and Morris, John C. and Wolk, David A. and Davatzikos, Christos and {iSTAGING Consortium} and {Baltimore Longitudinal Study of Aging (BLSA)} and {Alzheimer’s Disease Neuroimaging Initiative (ADNI)}},
+        year = {2021},
+        month = {12},
+        pages = {},
+        title = {A deep learning framework identifies dimensional representations of Alzheimer’s Disease from brain structure},
+        volume = {12},
+        journal = {Nature Communications},
+        doi = {10.1038/s41467-021-26703-z}
+        }
+        ```
+        
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Smile-GAN
-Smile-GAN is a semi-supervised clustering method which is designed to identify disease-related heterogeneity among the patient group. The model effectively avoid variations among normal control (CN) group and cluster patient based on disease related variations only. Semi-supervised clustering of Smile-GAN is achieved through joint training of the mapping and clustering function, where the mapping function can map CN subjects along different mapping directions depending on disease-related variations.
-
-![image info](./datasets/Smile-GAN.png)
-
-## License
-Copyright (c) 2016 University of Pennsylvania. All rights reserved. See[ https://www.cbica.upenn.edu/sbia/software/license.html](https://www.cbica.upenn.edu/sbia/software/license.html)
-
-## Installation
-We highly recommend the users to install **Anaconda3** on your machine. After installing Anaconda3, Smile-GAN can be used following this procedure:
-
-We recommend the users to use the Conda virtual environment:
-
-```bash
-$ conda create --name smilegan python=3.8
-```
-Activate the virtual environment
-
-```bash
-$ conda activate smilegan
-```
-Install SmileGAN from PyPi:
-
-```bash
-$ pip install SmileGAN
-```
-
-
-
-## Input structure
-Main functions of SmileGAN basically takes two panda dataframes as data inputs, **data** and **covariate** (optional). Columns with name *'participant_id'* and *diagnosis* must exist in both dataframes. Some conventions for the group label/diagnosis: -1 represents healthy control (CN) and 1 represents patient (PT); categorical variables, such as sex, should be encoded to numbers: Female for 0 and Male for 1, for example. 
-
-Example for **data**:
-
-```bash
-participant_id    diagnosis    ROI1    ROI2 ...
-subject-1	    -1         325.4   603.4
-subject-2            1         260.5   580.3
-subject-3           -1         326.5   623.4
-subject-4            1         301.7   590.5
-subject-5            1	       293.1   595.1
-subject-6            1         287.8   608.9
-```
-Example for **covariate**
-
-```bash
-participant_id    diagnosis    age    sex ...
-subject-1	    -1         57.3   0
-subject-2 	     1         43.5   1
-subject-3           -1         53.8   1
-subject-4            1         56.0   0
-subject-5            1	       60.0   1
-subject-6            1         62.5   0
-```
-
-## Example
-We offer a toy dataset in the folder of SmileGAN/dataset.
-
-**Runing SmileGAN for clustering CN vs Subtype1 vs Subtype2 vs ...**
-
-```bash
-import pandas as pd
-from SmileGAN.Smile_GAN_clustering import single_model_clustering, cross_validated_clustering, clustering_result
-
-train_data = pd.read_csv('train_roi.csv')
-covariate = pd.read_csv('train_cov.csv')
-
-output_dir = "PATH_OUTPUT_DIR"
-ncluster = 3
-start_saving_epoch = 9000
-max_epoch = 14000
-
-## three parameters for stopping threshold
-WD = 0.11
-AQ = 20
-cluster_loss = 0.0015
-
-## one parameter for consensus method
-consensus_type = "highest_matching_clustering"
-```
-
-When using the package, ***WD***, ***AQ***, ***cluster\_loss***, ***consensus\_type*** need to be chosen empirically:
-
-***WD***: Wasserstein Distance measures the distance between generated PT data along each direction and real PT data. (**Recommended value**: 0.11-0.14)
-
-***AQ***: Alteration Quantity measures the number of participants who change cluster labels during last three traninig epochs. Low AQ implies convergence of training. (**Recommended value**: 1/20 of PT sample size)
-
-***cluster\_loss***: Cluster loss measures how well clustering function reconstruct sampled Z variable. (**Recommended value**: 0.0015-0.002)
-
-***consensus\_type***: Consensus_type need to be chosen from **"consensus\_clustering"** and **"highest\_matching\_clustering"**. It determines how the final consensus result is derived from k clustering results obtained through the k-fold hold-out CV procedure. **"highest\_matching\_clustering"** is recommended if Adjusted Random Index among k clustering results is greater than 0.3. Otherwise, **"consensus\_clustering"** might give more reliable consensus results. User can always use function **clustering\_result**, trained models and a different consensus\_type to rederive results with different consensus\_type without retraining.
-
-Some other parameters, ***lam***, ***mu***, ***batch\_size***, have default values but need to be changed in some cases:
-
-***batch\_size***: Size of the batch for each training epoch. (Default to be 25) It is **necessary** to be reset to 1/10 - 1/20 of the PT sample size.
-
-***lam***: coefficient controlling the relative importance of cluster\_loss in training objective function. (Default to be 9) 
-
-***mu***: coefficient controlling the relative importance of change\_loss in training objective function. (Default to be 5). Can be reset to 5.5 or 6 if PT and CN does not have great differences and cluster\_loss does not converge during training procedure. 
-
-
-
-```bash
-single_model_clustering(train_data, ncluster, start_saving_epoch, max_epoch,\
-					    output_dir, WD, AQ, cluster_loss, covariate=covariate)
-```
-**single\_model\_clustering** performs clustering without cross validation. Since only one model is trained with this function, the model may be not representative or reproducible. Therefore, this function is ***not recommended***. The function automatically saves an csv file with clustering results and returns the same dataframe.
-
-
-
-```bash				    
-fold_number = 10  # number of folds the leave-out cv runs
-data_fraction = 0.8 # fraction of data used in each fold
-cross_validated_clustering(train_data, ncluster, fold_number, data_fraction, start_saving_epoch, max_epoch,\
-					    output_dir, WD, AQ, cluster_loss, consensus_tpype, covariate=covariate)
-```
-
-**cross\_validated\_clustering** performs clustering with leave-out cross validation. It is the ***recommended*** function for clustering. Since the CV process may take long training time on a normal desktop computer, the function enables early stop and later resumption. Users can set ***stop\_fold*** to be early stopping point and ***start\_fold*** depending on previous stopping point. The function automatically saves an csv file with clustering results and returns the same dataframe.
-
-```					    
-model_dirs = ['PATH_TO_CHECKPOINT1','PATH_TO_CHECKPOINT2',...] #list of paths to previously saved checkpoints (with name 'converged_model_foldk' after cv process)
-cluster_label, cluster_probabilities, _, _ = clustering_result(model_dirs, 'highest_matching_clustering', train_data, covariate)
-```
-**clustering\_result** is a function used for clustering patient data using previously saved models. Input data and covariate (optional) should be panda dataframe with same format shown before. Only PT data (can be inside or outside of training set), for which the user want to derive cluster memberships, need to be provided with diagnoses set to be 1.  ***The function returns cluster labels of PT data following the order of PT in the provided dataframe.*** If ***consensus\_type*** is chosen to be ***'highest\_matching\_clustering***, probabilities of each cluster will also be returned. 
-
-
-## Citation
-If you use this package for research, please cite the following paper:
-
-
-```bash
-@article{yang2021BrainHeterogeneity,
-author = {Yang, Zhijian and Nasrallah, Ilya M. and Shou, Haochang and Wen, Junhao and Doshi, Jimit and Habes, Mohamad and Erus, Guray and Abdulkadir, Ahmed and Resnick, Susan M. and Albert, Marilyn S. and Maruff, Paul and Fripp, Jurgen and Morris, John C. and Wolk, David A. and Davatzikos, Christos and {iSTAGING Consortium} and {Baltimore Longitudinal Study of Aging (BLSA)} and {Alzheimer’s Disease Neuroimaging Initiative (ADNI)}},
-year = {2021},
-month = {12},
-pages = {},
-title = {A deep learning framework identifies dimensional representations of Alzheimer’s Disease from brain structure},
-volume = {12},
-journal = {Nature Communications},
-doi = {10.1038/s41467-021-26703-z}
-}
-```
-
-
```

### Comparing `SmileGAN-0.1.3/setup.py` & `SmileGAN-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SmileGAN",
-    version="0.1.3",
+    version="0.1.4",
     author="zhijian.yang",
     author_email="zhijianyang@outlook.com",
     description="A python implementation of Smile-GAN for semisupervised clustering",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhijian-yang/SmileGAN",
     packages=setuptools.find_packages(),
```

