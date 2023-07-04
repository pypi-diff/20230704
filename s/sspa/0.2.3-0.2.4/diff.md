# Comparing `tmp/sspa-0.2.3.tar.gz` & `tmp/sspa-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspa-0.2.3.tar", last modified: Fri Jun 23 21:25:54 2023, max compression
+gzip compressed data, was "sspa-0.2.4.tar", last modified: Tue Jul  4 17:41:56 2023, max compression
```

## Comparing `sspa-0.2.3.tar` & `sspa-0.2.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.610908 sspa-0.2.3/
--rw-r--r--   0 cw2019     (501) staff       (20)    35149 2021-12-28 11:48:17.000000 sspa-0.2.3/LICENSE
--rw-r--r--   0 cw2019     (501) staff       (20)     6479 2023-06-23 21:25:54.610496 sspa-0.2.3/PKG-INFO
--rw-r--r--   0 cw2019     (501) staff       (20)     6051 2023-06-23 21:24:36.000000 sspa-0.2.3/README.md
--rw-r--r--   0 cw2019     (501) staff       (20)       38 2023-06-23 21:25:54.611046 sspa-0.2.3/setup.cfg
--rw-r--r--   0 cw2019     (501) staff       (20)      986 2023-06-23 21:10:23.000000 sspa-0.2.3/setup.py
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.255398 sspa-0.2.3/src/
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.274906 sspa-0.2.3/src/sspa/
--rw-r--r--   0 cw2019     (501) staff       (20)      608 2023-01-06 11:27:15.000000 sspa-0.2.3/src/sspa/__init__.py
--rw-r--r--   0 cw2019     (501) staff       (20)     7133 2023-06-21 17:20:00.000000 sspa-0.2.3/src/sspa/download_pathways.py
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.334696 sspa-0.2.3/src/sspa/example_data/
--rw-r--r--   0 cw2019     (501) staff       (20)  3458958 2022-02-15 11:17:29.000000 sspa-0.2.3/src/sspa/example_data/BXD_mouse_metabolomics.csv
--rw-r--r--   0 cw2019     (501) staff       (20)  3269754 2022-02-15 12:04:44.000000 sspa-0.2.3/src/sspa/example_data/BXD_mouse_metabolomics_raw_data.csv
--rw-r--r--   0 cw2019     (501) staff       (20)  1742398 2021-12-28 17:58:04.000000 sspa-0.2.3/src/sspa/example_data/Su_covid_metabolomics_processed.csv
--rw-r--r--   0 cw2019     (501) staff       (20)  2768383 2022-02-18 15:51:44.000000 sspa-0.2.3/src/sspa/example_data/Su_metab_data_raw.csv
--rw-r--r--   0 cw2019     (501) staff       (20)     2201 2022-10-11 12:11:57.000000 sspa-0.2.3/src/sspa/identifier_conversion.py
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.603366 sspa-0.2.3/src/sspa/pathway_databases/
--rw-r--r--   0 cw2019     (501) staff       (20) 30485396 2021-12-28 17:59:39.000000 sspa-0.2.3/src/sspa/pathway_databases/ChEBI2Reactome_All_Levels_R78.txt
--rw-r--r--   0 cw2019     (501) staff       (20)   172723 2021-06-07 08:24:37.000000 sspa-0.2.3/src/sspa/pathway_databases/KEGG_human_pathways_compounds_R98.csv
--rw-r--r--   0 cw2019     (501) staff       (20)   259274 2022-07-07 13:45:17.000000 sspa-0.2.3/src/sspa/pathway_databases/wikipathways-20220610-gmt-Homo_sapiens.gmt
--rw-r--r--   0 cw2019     (501) staff       (20)     4243 2022-09-16 11:23:22.000000 sspa-0.2.3/src/sspa/process_pathways.py
--rw-r--r--   0 cw2019     (501) staff       (20)     2897 2022-02-14 15:21:22.000000 sspa-0.2.3/src/sspa/process_pathways_dictionary.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1699 2022-09-16 19:04:09.000000 sspa-0.2.3/src/sspa/sspa_cluster.py
--rw-r--r--   0 cw2019     (501) staff       (20)     2621 2023-01-06 14:47:35.000000 sspa-0.2.3/src/sspa/sspa_fgsea.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1971 2023-01-05 16:12:18.000000 sspa-0.2.3/src/sspa/sspa_gsea.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1878 2023-01-06 14:47:35.000000 sspa-0.2.3/src/sspa/sspa_gsva.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1508 2022-09-16 19:01:36.000000 sspa-0.2.3/src/sspa/sspa_kpca.py
--rw-r--r--   0 cw2019     (501) staff       (20)     5359 2022-10-25 10:55:24.000000 sspa-0.2.3/src/sspa/sspa_ora.py
--rw-r--r--   0 cw2019     (501) staff       (20)     2476 2023-01-05 16:12:18.000000 sspa-0.2.3/src/sspa/sspa_ssGSEA.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1576 2022-09-16 19:02:23.000000 sspa-0.2.3/src/sspa/sspa_svd.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1613 2022-09-16 19:02:38.000000 sspa-0.2.3/src/sspa/sspa_zscore.py
--rw-r--r--   0 cw2019     (501) staff       (20)     3890 2023-02-21 10:51:51.000000 sspa-0.2.3/src/sspa/utils.py
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.277949 sspa-0.2.3/src/sspa.egg-info/
--rw-r--r--   0 cw2019     (501) staff       (20)     6479 2023-06-23 21:25:54.000000 sspa-0.2.3/src/sspa.egg-info/PKG-INFO
--rw-r--r--   0 cw2019     (501) staff       (20)     1018 2023-06-23 21:25:54.000000 sspa-0.2.3/src/sspa.egg-info/SOURCES.txt
--rw-r--r--   0 cw2019     (501) staff       (20)        1 2023-06-23 21:25:54.000000 sspa-0.2.3/src/sspa.egg-info/dependency_links.txt
--rw-r--r--   0 cw2019     (501) staff       (20)       76 2023-06-23 21:25:54.000000 sspa-0.2.3/src/sspa.egg-info/requires.txt
--rw-r--r--   0 cw2019     (501) staff       (20)        5 2023-06-23 21:25:54.000000 sspa-0.2.3/src/sspa.egg-info/top_level.txt
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.609507 sspa-0.2.3/tests/
--rw-r--r--   0 cw2019     (501) staff       (20)      586 2022-10-30 19:06:06.000000 sspa-0.2.3/tests/test_download_pathways.py
--rw-r--r--   0 cw2019     (501) staff       (20)     2782 2023-01-08 14:18:53.000000 sspa-0.2.3/tests/test_utils.py
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-07-04 17:41:56.041212 sspa-0.2.4/
+-rw-r--r--   0 cw2019     (501) staff       (20)    35149 2021-12-28 11:48:17.000000 sspa-0.2.4/LICENSE
+-rw-r--r--   0 cw2019     (501) staff       (20)     6479 2023-07-04 17:41:56.040620 sspa-0.2.4/PKG-INFO
+-rw-r--r--   0 cw2019     (501) staff       (20)     6051 2023-06-23 21:24:36.000000 sspa-0.2.4/README.md
+-rw-r--r--   0 cw2019     (501) staff       (20)       38 2023-07-04 17:41:56.041393 sspa-0.2.4/setup.cfg
+-rw-r--r--   0 cw2019     (501) staff       (20)      986 2023-07-04 17:39:59.000000 sspa-0.2.4/setup.py
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-07-04 17:41:55.594645 sspa-0.2.4/src/
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-07-04 17:41:55.608220 sspa-0.2.4/src/sspa/
+-rw-r--r--   0 cw2019     (501) staff       (20)      608 2023-01-06 11:27:15.000000 sspa-0.2.4/src/sspa/__init__.py
+-rw-r--r--   0 cw2019     (501) staff       (20)    10499 2023-07-04 17:38:33.000000 sspa-0.2.4/src/sspa/download_pathways.py
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-07-04 17:41:55.681585 sspa-0.2.4/src/sspa/example_data/
+-rw-r--r--   0 cw2019     (501) staff       (20)  3458958 2022-02-15 11:17:29.000000 sspa-0.2.4/src/sspa/example_data/BXD_mouse_metabolomics.csv
+-rw-r--r--   0 cw2019     (501) staff       (20)  3269754 2022-02-15 12:04:44.000000 sspa-0.2.4/src/sspa/example_data/BXD_mouse_metabolomics_raw_data.csv
+-rw-r--r--   0 cw2019     (501) staff       (20)  1742398 2021-12-28 17:58:04.000000 sspa-0.2.4/src/sspa/example_data/Su_covid_metabolomics_processed.csv
+-rw-r--r--   0 cw2019     (501) staff       (20)  2768383 2022-02-18 15:51:44.000000 sspa-0.2.4/src/sspa/example_data/Su_metab_data_raw.csv
+-rw-r--r--   0 cw2019     (501) staff       (20)     2201 2022-10-11 12:11:57.000000 sspa-0.2.4/src/sspa/identifier_conversion.py
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-07-04 17:41:56.034599 sspa-0.2.4/src/sspa/pathway_databases/
+-rw-r--r--   0 cw2019     (501) staff       (20) 30485396 2021-12-28 17:59:39.000000 sspa-0.2.4/src/sspa/pathway_databases/ChEBI2Reactome_All_Levels_R78.txt
+-rw-r--r--   0 cw2019     (501) staff       (20)   172723 2021-06-07 08:24:37.000000 sspa-0.2.4/src/sspa/pathway_databases/KEGG_human_pathways_compounds_R98.csv
+-rw-r--r--   0 cw2019     (501) staff       (20)   259274 2022-07-07 13:45:17.000000 sspa-0.2.4/src/sspa/pathway_databases/wikipathways-20220610-gmt-Homo_sapiens.gmt
+-rw-r--r--   0 cw2019     (501) staff       (20)     4586 2023-07-04 17:38:33.000000 sspa-0.2.4/src/sspa/process_pathways.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     2897 2022-02-14 15:21:22.000000 sspa-0.2.4/src/sspa/process_pathways_dictionary.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1699 2022-09-16 19:04:09.000000 sspa-0.2.4/src/sspa/sspa_cluster.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     2621 2023-01-06 14:47:35.000000 sspa-0.2.4/src/sspa/sspa_fgsea.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1971 2023-01-05 16:12:18.000000 sspa-0.2.4/src/sspa/sspa_gsea.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1878 2023-01-06 14:47:35.000000 sspa-0.2.4/src/sspa/sspa_gsva.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1508 2022-09-16 19:01:36.000000 sspa-0.2.4/src/sspa/sspa_kpca.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     5359 2022-10-25 10:55:24.000000 sspa-0.2.4/src/sspa/sspa_ora.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     2476 2023-01-05 16:12:18.000000 sspa-0.2.4/src/sspa/sspa_ssGSEA.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1576 2022-09-16 19:02:23.000000 sspa-0.2.4/src/sspa/sspa_svd.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1613 2022-09-16 19:02:38.000000 sspa-0.2.4/src/sspa/sspa_zscore.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     3680 2023-07-04 17:38:33.000000 sspa-0.2.4/src/sspa/utils.py
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-07-04 17:41:55.612095 sspa-0.2.4/src/sspa.egg-info/
+-rw-r--r--   0 cw2019     (501) staff       (20)     6479 2023-07-04 17:41:55.000000 sspa-0.2.4/src/sspa.egg-info/PKG-INFO
+-rw-r--r--   0 cw2019     (501) staff       (20)     1018 2023-07-04 17:41:55.000000 sspa-0.2.4/src/sspa.egg-info/SOURCES.txt
+-rw-r--r--   0 cw2019     (501) staff       (20)        1 2023-07-04 17:41:55.000000 sspa-0.2.4/src/sspa.egg-info/dependency_links.txt
+-rw-r--r--   0 cw2019     (501) staff       (20)       76 2023-07-04 17:41:55.000000 sspa-0.2.4/src/sspa.egg-info/requires.txt
+-rw-r--r--   0 cw2019     (501) staff       (20)        5 2023-07-04 17:41:55.000000 sspa-0.2.4/src/sspa.egg-info/top_level.txt
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-07-04 17:41:56.039705 sspa-0.2.4/tests/
+-rw-r--r--   0 cw2019     (501) staff       (20)      586 2022-10-30 19:06:06.000000 sspa-0.2.4/tests/test_download_pathways.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     2782 2023-01-08 14:18:53.000000 sspa-0.2.4/tests/test_utils.py
```

### Comparing `sspa-0.2.3/LICENSE` & `sspa-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/PKG-INFO` & `sspa-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspa
-Version: 0.2.3
+Version: 0.2.4
 Summary: Single sample pathway analysis tools for omics data
 Home-page: https://github.com/cwieder/sspa
 Author: Cecilia Wieder
 Author-email: cw2019@ic.ac.uk
 License: GNU 3.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sspa-0.2.3/README.md` & `sspa-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/setup.py` & `sspa-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='sspa',
-    version='0.2.3',
+    version='0.2.4',
     packages=['sspa'],
     package_dir={'':'src'},
     url='https://github.com/cwieder/sspa',
     license='GNU 3.0',
     author='Cecilia Wieder',
     author_email='cw2019@ic.ac.uk',
     description='Single sample pathway analysis tools for omics data',
```

### Comparing `sspa-0.2.3/src/sspa/__init__.py` & `sspa-0.2.4/src/sspa/__init__.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/download_pathways.py` & `sspa-0.2.4/src/sspa/download_pathways.py`

 * *Files 22% similar despite different names*

```diff
@@ -70,54 +70,113 @@
         fpath = filepath + "/KEGG_" + organism + "_pathways_compounds_R" + str(version_no) + ".gmt"
         df.to_csv(fpath, sep="\t", header=False)
         print("KEGG DB file saved to " + fpath)
     print("Complete!")
 
     return df
 
-def download_reactome(organism, filepath=None):
+def download_reactome(organism, filepath=None, omics_type='metabolomics'):
     '''
     Function for Reactome pathway download
     Args:
         organism (str): Reactome organism name
         filepath (str): filepath (str): filepath to save pathway file to, default is None - save to variable
+        omics_type(str): type of omics pathways to download. Options are 'metabolomics', 'proteomics', or 'multiomics'
     Returns: 
         GMT-like pd.DataFrame containing Reactome pathways
     '''
     print("Beginning Reactome download...")
 
-     # get all pathways
-    url = 'https://reactome.org/download/current/ChEBI2Reactome_All_Levels.txt'
-    f = pd.read_csv(url, sep="\t", header=None)
-    
-    f.columns = ['CHEBI', 'pathway_ID', 'link', 'pathway_name', 'evidence_code', 'species']
-    f_filt = f[f.species == organism]
-    name_dict = dict(zip(f_filt['pathway_ID'], f_filt['pathway_name']))
-
-    groups = f_filt.groupby(['pathway_ID'])['CHEBI'].apply(list).to_dict()
-    groups = {k: list(set(v)) for k, v in groups.items()}
-
-    df = pd.DataFrame.from_dict(groups, orient='index', dtype="object")
-    pathways_df = df.dropna(axis=0, how='all', subset=df.columns.tolist()[1:])
-    pathways_df = df.dropna(axis=1, how='all')
-
-    pathways_df["Pathway_name"] = pathways_df.index.map(name_dict)
-    pathways_df.insert(0, 'Pathway_name', pathways_df.pop('Pathway_name'))
-
     # get release details
     release_data = requests.get('https://reactome.org/download/current/reactome_stable_ids.txt')
     version_no = release_data.text.split()[6]
 
-    if filepath:
-        fpath = filepath + "/Reactome_" + "_".join(organism.split())+ "_pathways_compounds_R" + str(version_no) + ".gmt"
-        pathways_df.to_csv(fpath, sep="\t", header=False)
-        print("Reactome DB file saved to " + fpath)
-    print("Complete!")
+    # get all pathways
+    if omics_type == 'metabolomics':
+        url = 'https://reactome.org/download/current/ChEBI2Reactome_All_Levels.txt'
+        f = pd.read_csv(url, sep="\t", header=None)
+        
+        f.columns = ['CHEBI', 'pathway_ID', 'link', 'pathway_name', 'evidence_code', 'species']
+        f_filt = f[f.species == organism]
+        name_dict = dict(zip(f_filt['pathway_ID'], f_filt['pathway_name']))
+        groups = f_filt.groupby(['pathway_ID'])['CHEBI'].apply(list).to_dict()
+        groups = {k: list(set(v)) for k, v in groups.items()}
+        df = pd.DataFrame.from_dict(groups, orient='index', dtype="object")
+        pathways_df = df.dropna(axis=0, how='all', subset=df.columns.tolist()[1:])
+        pathways_df = df.dropna(axis=1, how='all')
+        pathways_df["Pathway_name"] = pathways_df.index.map(name_dict)
+        pathways_df.insert(0, 'Pathway_name', pathways_df.pop('Pathway_name'))
+
+        if filepath:
+            fpath = filepath + "/Reactome_" + "_".join(organism.split())+ "_pathways_ChEBI_R" + str(version_no) + ".gmt"
+            pathways_df.to_csv(fpath, sep="\t", header=False)
+            print("Reactome DB file saved to " + fpath)
+        
+        print("Complete!")
+        return pathways_df
+
+    if omics_type == 'proteomics':
+        url = 'https://reactome.org/download/current/UniProt2Reactome_All_Levels.txt'
+        f = pd.read_csv(url, sep="\t", header=None)
+        
+        f.columns = ['UniProt', 'pathway_ID', 'link', 'pathway_name', 'evidence_code', 'species']
+        f_filt = f[f.species == organism]
+        name_dict = dict(zip(f_filt['pathway_ID'], f_filt['pathway_name']))
+        groups = f_filt.groupby(['pathway_ID'])['UniProt'].apply(list).to_dict()
+        groups = {k: list(set(v)) for k, v in groups.items()}
+        df = pd.DataFrame.from_dict(groups, orient='index', dtype="object")
+        pathways_df = df.dropna(axis=0, how='all', subset=df.columns.tolist()[1:])
+        pathways_df = df.dropna(axis=1, how='all')
+        pathways_df["Pathway_name"] = pathways_df.index.map(name_dict)
+        pathways_df.insert(0, 'Pathway_name', pathways_df.pop('Pathway_name'))
+
+        if filepath:
+            fpath = filepath + "/Reactome_" + "_".join(organism.split())+ "_pathways_UniProt_R" + str(version_no) + ".gmt"
+            pathways_df.to_csv(fpath, sep="\t", header=False)
+            print("Reactome DB file saved to " + fpath)
+        
+        print("Complete!")
+        return pathways_df
+
+    if omics_type == 'multiomics':
+        url_prot = 'https://reactome.org/download/current/UniProt2Reactome_All_Levels.txt'
+        url_metab = 'https://reactome.org/download/current/ChEBI2Reactome_All_Levels.txt'
+        
+        pathway_dfs = []
+        for url in [url_prot, url_metab]:
+            f = pd.read_csv(url, sep="\t", header=None)
+            
+            f.columns = ['molecule_ID', 'pathway_ID', 'link', 'pathway_name', 'evidence_code', 'species']
+            f_filt = f[f.species == organism]
+            name_dict = dict(zip(f_filt['pathway_ID'], f_filt['pathway_name']))
+            groups = f_filt.groupby(['pathway_ID'])['molecule_ID'].apply(list).to_dict()
+            groups = {k: list(set(v)) for k, v in groups.items()}
+            df = pd.DataFrame.from_dict(groups, orient='index', dtype="object")
+            pathways_df = df.dropna(axis=0, how='all', subset=df.columns.tolist()[1:])
+            pathways_df = df.dropna(axis=1, how='all')
+            pathways_df["Pathway_name"] = pathways_df.index.map(name_dict)
+            pathways_df.insert(0, 'Pathway_name', pathways_df.pop('Pathway_name'))
+            pathways_df.set_index([pathways_df.index, pathways_df['Pathway_name']], inplace=True)
+            pathways_df.drop(['Pathway_name'], axis=1, inplace=True)
+            pathway_dfs.append(pathways_df)
+        
+        # merge pathways on index
+        reactome_mo = pathway_dfs[0].merge(pathway_dfs[1], how='outer', left_index=True, right_index=True)    
+        reactome_mo = reactome_mo.reset_index(level=[1])
+
+        if filepath:
+            fpath = filepath + "/Reactome_" + "_".join(organism.split())+ "_pathways_multiomics_R" + str(version_no) + ".gmt"
+            reactome_mo.to_csv(fpath, sep="\t", header=False)
+            print("Reactome DB file saved to " + fpath)
+
+        print("Complete!")
+        return reactome_mo
+    
+
 
-    return pathways_df
 
 class MetExplorePaths:
     '''
     Class for downloading metexplore metabolic models in the form of pathways with mapped identifiers
 
     Attributes:
         model (str): identifier of genome scale metabolic model available on MetExplore
```

### Comparing `sspa-0.2.3/src/sspa/example_data/BXD_mouse_metabolomics.csv` & `sspa-0.2.4/src/sspa/example_data/BXD_mouse_metabolomics.csv`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/example_data/BXD_mouse_metabolomics_raw_data.csv` & `sspa-0.2.4/src/sspa/example_data/BXD_mouse_metabolomics_raw_data.csv`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/example_data/Su_covid_metabolomics_processed.csv` & `sspa-0.2.4/src/sspa/example_data/Su_covid_metabolomics_processed.csv`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/example_data/Su_metab_data_raw.csv` & `sspa-0.2.4/src/sspa/example_data/Su_metab_data_raw.csv`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/identifier_conversion.py` & `sspa-0.2.4/src/sspa/identifier_conversion.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/pathway_databases/ChEBI2Reactome_All_Levels_R78.txt` & `sspa-0.2.4/src/sspa/pathway_databases/ChEBI2Reactome_All_Levels_R78.txt`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/pathway_databases/KEGG_human_pathways_compounds_R98.csv` & `sspa-0.2.4/src/sspa/pathway_databases/KEGG_human_pathways_compounds_R98.csv`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/pathway_databases/wikipathways-20220610-gmt-Homo_sapiens.gmt` & `sspa-0.2.4/src/sspa/pathway_databases/wikipathways-20220610-gmt-Homo_sapiens.gmt`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/process_pathways.py` & `sspa-0.2.4/src/sspa/process_pathways.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import pandas as pd
 import pkg_resources
 import sspa.download_pathways 
 
-def process_reactome(organism, infile=None, download_latest=False, filepath=None):
+def process_reactome(organism, infile=None, download_latest=False, filepath=None, omics_type='metabolomics'):
     '''
     Function to load Reactome pathways 
     Args:
         organism (str): Reactome organism name
         infile (str): default None, provide a Reactome pathway file to process into the GMT-style dataframe 
         download_latest (Bool): Downloads the latest version of Reactome metabolic pathways
         filepath (str): filepath to save pathway file to, default is None - save to variable
+        omics_type(str): If using download_latest, specify type of omics pathways to download. Options are 'metabolomics', 'proteomics', or 'multiomics'
     Returns: 
         GMT-like pd.DataFrame containing Reactome pathways
     '''
 
     # Process CHEBI to reactome data
 
     if download_latest:
-        pathways_df = sspa.download_pathways.download_reactome(organism, filepath)
+        pathways_df = sspa.download_pathways.download_reactome(organism, filepath, omics_type)
         return pathways_df
-
+    
     else:
+        if omics_type != 'metabolomics':
+            raise ValueError('Proteomics/multi-omics pathways only accessible when download_latest=True')
         if infile == None or infile == "R78":
             stream = pkg_resources.resource_stream(__name__, 'pathway_databases/ChEBI2Reactome_All_Levels_R78.txt')
             f = pd.read_csv(stream, sep="\t", header=None, encoding='latin-1')
         else:
             f = pd.read_csv(infile, sep="\t", header=None)
         f.columns = ['CHEBI', 'pathway_ID', 'link', 'pathway_name', 'evidence_code', 'species']
         f_filt = f[f.species == organism]
```

### Comparing `sspa-0.2.3/src/sspa/process_pathways_dictionary.py` & `sspa-0.2.4/src/sspa/process_pathways_dictionary.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/sspa_cluster.py` & `sspa-0.2.4/src/sspa/sspa_cluster.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/sspa_fgsea.py` & `sspa-0.2.4/src/sspa/sspa_fgsea.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/sspa_gsea.py` & `sspa-0.2.4/src/sspa/sspa_gsea.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/sspa_gsva.py` & `sspa-0.2.4/src/sspa/sspa_gsva.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/sspa_kpca.py` & `sspa-0.2.4/src/sspa/sspa_kpca.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/sspa_ora.py` & `sspa-0.2.4/src/sspa/sspa_ora.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/sspa_ssGSEA.py` & `sspa-0.2.4/src/sspa/sspa_ssGSEA.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/sspa_svd.py` & `sspa-0.2.4/src/sspa/sspa_svd.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/sspa_zscore.py` & `sspa-0.2.4/src/sspa/sspa_zscore.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/src/sspa/utils.py` & `sspa-0.2.4/src/sspa/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,25 +53,19 @@
         raise ValueError('More than two metadata classes detected. Only two metadata classes are supported in ORA.')
 
     disease = matrix_copy[matrix_copy["Target"] == 0]
     disease = disease.drop(['Target'], axis=1)
     ctrl = matrix_copy[matrix_copy["Target"] != 0]
     ctrl = ctrl.drop(['Target'], axis=1)
     matrix_copy = matrix_copy.drop(['Target'], axis=1)
-
-    # disease = matrix.loc[matrix["Target"] == 0]
-    # disease.drop(['Target'], axis=1, inplace=True)
-    # ctrl = matrix.loc[matrix["Target"] != 0]
-    # ctrl.drop(['Target'], axis=1, inplace=True)
-    # matrix = matrix.drop(['Target'], axis=1)
     
     if testtype == "mwu":
-        pvalues = stats.mannwhitneyu(disease, ctrl, axis=0)[1]
+        pvalues = stats.mannwhitneyu(disease, ctrl, nan_policy='omit', axis=0)[1]
     else:
-        pvalues = stats.ttest_ind(disease, ctrl)[1]
+        pvalues = stats.ttest_ind(disease, ctrl, nan_policy='omit')[1]
 
     padj = sm.stats.multipletests(pvalues, 0.05, method=multiple_correction_method)
     results = pd.DataFrame(zip(metabolites, pvalues, padj[1]),
                            columns=["Entity", "P-value", "P-adjust"])
     return results
```

### Comparing `sspa-0.2.3/src/sspa.egg-info/PKG-INFO` & `sspa-0.2.4/src/sspa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspa
-Version: 0.2.3
+Version: 0.2.4
 Summary: Single sample pathway analysis tools for omics data
 Home-page: https://github.com/cwieder/sspa
 Author: Cecilia Wieder
 Author-email: cw2019@ic.ac.uk
 License: GNU 3.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sspa-0.2.3/src/sspa.egg-info/SOURCES.txt` & `sspa-0.2.4/src/sspa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/tests/test_download_pathways.py` & `sspa-0.2.4/tests/test_download_pathways.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.3/tests/test_utils.py` & `sspa-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

