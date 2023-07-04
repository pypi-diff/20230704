# Comparing `tmp/JBioSeqTools-1.1.3.tar.gz` & `tmp/JBioSeqTools-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBioSeqTools-1.1.3.tar", last modified: Thu Dec 15 18:47:07 2022, max compression
+gzip compressed data, was "JBioSeqTools-1.1.4.tar", last modified: Tue Jul  4 09:43:22 2023, max compression
```

## Comparing `JBioSeqTools-1.1.3.tar` & `JBioSeqTools-1.1.4.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-12-15 18:47:07.779660 JBioSeqTools-1.1.3/
-drwxrwxrwx   0        0        0        0 2022-12-15 18:47:07.754782 JBioSeqTools-1.1.3/JBioSeqTools/
--rw-rw-rw-   0        0        0      344 2022-12-15 18:39:54.000000 JBioSeqTools-1.1.3/JBioSeqTools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-15 18:47:07.766044 JBioSeqTools-1.1.3/JBioSeqTools/api_elements/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.3/JBioSeqTools/api_elements/__init__.py
--rw-rw-rw-   0        0        0     6152 2022-12-15 18:39:44.000000 JBioSeqTools-1.1.3/JBioSeqTools/api_elements/api.py
-drwxrwxrwx   0        0        0        0 2022-12-15 18:47:07.770043 JBioSeqTools-1.1.3/JBioSeqTools/seq_tools/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.3/JBioSeqTools/seq_tools/__init__.py
--rw-rw-rw-   0        0        0    18688 2022-12-15 18:39:22.000000 JBioSeqTools-1.1.3/JBioSeqTools/seq_tools/seq_tools.py
-drwxrwxrwx   0        0        0        0 2022-12-15 18:47:07.773216 JBioSeqTools-1.1.3/JBioSeqTools/vector_build/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.3/JBioSeqTools/vector_build/__init__.py
--rw-rw-rw-   0        0        0    47505 2022-12-15 18:39:18.000000 JBioSeqTools-1.1.3/JBioSeqTools/vector_build/vector_build.py
-drwxrwxrwx   0        0        0        0 2022-12-15 18:47:07.777137 JBioSeqTools-1.1.3/JBioSeqTools/vector_graph/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.3/JBioSeqTools/vector_graph/__init__.py
--rw-rw-rw-   0        0        0     1965 2022-12-15 18:39:26.000000 JBioSeqTools-1.1.3/JBioSeqTools/vector_graph/graph_plot.py
-drwxrwxrwx   0        0        0        0 2022-12-15 18:47:07.763327 JBioSeqTools-1.1.3/JBioSeqTools.egg-info/
--rw-rw-rw-   0        0        0     1001 2022-12-15 18:47:06.000000 JBioSeqTools-1.1.3/JBioSeqTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2022-12-15 18:47:07.000000 JBioSeqTools-1.1.3/JBioSeqTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-15 18:47:06.000000 JBioSeqTools-1.1.3/JBioSeqTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2022-12-15 18:47:06.000000 JBioSeqTools-1.1.3/JBioSeqTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-12-15 18:47:07.000000 JBioSeqTools-1.1.3/JBioSeqTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     1001 2022-12-15 18:47:07.779660 JBioSeqTools-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2022-12-15 18:47:07.780923 JBioSeqTools-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1422 2022-12-15 18:39:58.000000 JBioSeqTools-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.999003 JBioSeqTools-1.1.4/
+drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.971984 JBioSeqTools-1.1.4/JBioSeqTools/
+-rw-rw-rw-   0        0        0      344 2022-12-15 18:39:54.000000 JBioSeqTools-1.1.4/JBioSeqTools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.985047 JBioSeqTools-1.1.4/JBioSeqTools/api_elements/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.4/JBioSeqTools/api_elements/__init__.py
+-rw-rw-rw-   0        0        0     6152 2022-12-15 18:39:44.000000 JBioSeqTools-1.1.4/JBioSeqTools/api_elements/api.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.985047 JBioSeqTools-1.1.4/JBioSeqTools/seq_tools/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.4/JBioSeqTools/seq_tools/__init__.py
+-rw-rw-rw-   0        0        0    18682 2023-07-04 08:31:50.000000 JBioSeqTools-1.1.4/JBioSeqTools/seq_tools/seq_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.985047 JBioSeqTools-1.1.4/JBioSeqTools/vector_build/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.4/JBioSeqTools/vector_build/__init__.py
+-rw-rw-rw-   0        0        0    47172 2023-07-04 08:30:28.000000 JBioSeqTools-1.1.4/JBioSeqTools/vector_build/vector_build.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.985047 JBioSeqTools-1.1.4/JBioSeqTools/vector_graph/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.4/JBioSeqTools/vector_graph/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-07-04 08:33:55.000000 JBioSeqTools-1.1.4/JBioSeqTools/vector_graph/graph_plot.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.971984 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/
+-rw-rw-rw-   0        0        0     1000 2023-07-04 09:43:22.000000 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2023-07-04 09:43:22.000000 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 09:43:22.000000 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-04 09:43:22.000000 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-04 09:43:22.000000 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1000 2023-07-04 09:43:22.999003 JBioSeqTools-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.999003 JBioSeqTools-1.1.4/data/
+-rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.1.4/data/backbone.xlsx
+-rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.1.4/data/codons.xlsx
+-rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.1.4/data/fluorescent_tag.xlsx
+-rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.1.4/data/linkers.xlsx
+-rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.1.4/data/promoters.xlsx
+-rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.1.4/data/regulators.xlsx
+-rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.1.4/data/restriction_enzymes.xlsx
+-rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.1.4/data/vectors.xlsx
+-rw-rw-rw-   0        0        0       42 2023-07-04 09:43:22.999003 JBioSeqTools-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1421 2023-07-04 08:37:40.000000 JBioSeqTools-1.1.4/setup.py
```

### Comparing `JBioSeqTools-1.1.3/JBioSeqTools/api_elements/api.py` & `JBioSeqTools-1.1.4/JBioSeqTools/api_elements/api.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.3/JBioSeqTools/seq_tools/seq_tools.py` & `JBioSeqTools-1.1.4/JBioSeqTools/seq_tools/seq_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 pd.options.mode.chained_assignment = None
 import numpy as np
 from tqdm import tqdm
 
 
 
-def load_metadata(codons:str() = 'https://github.com/jkubis96/JBioSeqTools/blob/main/data/codons.xlsx?raw=true', restriction:str() = 'https://github.com/jkubis96/JBioSeqTools/blob/main/data/restriction_enzymes.xlsx?raw=true'):
+def load_metadata(codons:str() = '../data/codons.xlsx', restriction:str() = '../data/restriction_enzymes.xlsx'):
     codons = pd.read_excel(codons)
     restriction = pd.read_excel(restriction)
     
     metadata = {'codons':codons,'restriction':restriction}
 
     return metadata
 
@@ -54,15 +54,15 @@
                 
 
 
 
 
 def codon_otymization(sequence:str(), codons:pd.DataFrame, species:str()):
     codons = codons[codons['Species'] == species]
-    seq_codon = [sequence[y:y+3] for y in range(0, len(sequence), 3)]
+    seq_codon = [sequence[y:y+3].upper() for y in range(0, len(sequence), 3)]
     seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq][codons['Fraction'][codons['Triplet'] == seq].index[0]] for seq in seq_codon]
     seq_codon_fr = round(sum(seq_codon_fr) / len(seq_codon_fr),2)
     
     seq_codon_mean = ''.join(seq_codon).count('C')
     seq_codon_GC = (''.join(seq_codon).count('C') + ''.join(seq_codon).count('G')) / len(''.join(seq_codon)) * 100
     seq_aa = []
     for element in seq_codon:
@@ -175,17 +175,17 @@
 
 def check_restriction(sequence:str(), restriction:pd.DataFrame()):
 
     enzyme_restriction = {'name':[], 'restriction_place':[], 'restriction_sequence':[], 'start':[], 'stop':[]}
     
     for r in tqdm(restriction.index):
         check = True
-        if restriction['sequence'][r] in sequence:
+        if restriction['sequence'][r] in sequence.upper():
             while(check == True):
-                bmp = list(sequence)
+                bmp = list(sequence.upper())
                 for n in range(0,len(restriction['sequence'][r])):
                     for j in range(n,len(bmp)-len(restriction['sequence'][r])):
                        lower = j
                        upper = j + len(restriction['sequence'][r])
                        if upper < len(bmp) and ''.join(bmp[lower:upper]) == restriction['sequence'][r]:
                             enzyme_restriction['name'].append(restriction['name'][r])
                             enzyme_restriction['restriction_sequence'].append(restriction['sequence'][r])
@@ -195,23 +195,24 @@
                             check = False
 
                                
     enzyme_restriction = pd.DataFrame.from_dict(enzyme_restriction)
     enzyme_restriction = enzyme_restriction.drop_duplicates()
     enzyme_restriction = enzyme_restriction.reset_index(drop=True)
     
-    if len(enzyme_restriction) > 0:
+    if len(enzyme_restriction['name']) > 0:
         restriction_df = enzyme_restriction.copy()
         restriction_df['index'] = restriction_df.index
         restriction_df = restriction_df[['name', 'index']]
         restriction_df['index'] = [[x] for x in restriction_df['index']]
         restriction_df = restriction_df.groupby('name').agg({'index': 'sum'})
         restriction_df = restriction_df.reset_index()
     
-    if len(enzyme_restriction) == 0:
+    else:
+        restriction_df = enzyme_restriction
         print('\n Any restriction places were not found')
     
     return enzyme_restriction, restriction_df
 
 
 
 
@@ -248,15 +249,15 @@
 
 
 
 def repair_sequence(sequence:str(), codons:pd.DataFrame, restriction_df:pd.DataFrame(), restriction:pd.DataFrame(), enzyme_list:list(), species:str()):
     if len(restriction_df) != 0:
         not_repaired = []
         codons = codons[codons['Species'] == species]
-        seq_codon = [sequence[y:y+3] for y in range(0, len(sequence), 3)]
+        seq_codon = [sequence[y:y+3].upper() for y in range(0, len(sequence), 3)]
         seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq][codons['Fraction'][codons['Triplet'] == seq].index[0]] for seq in seq_codon]
         seq_codon_fr = round(sum(seq_codon_fr) / len(seq_codon_fr),2)
         seq_codon_GC = (''.join(seq_codon).count('C') + ''.join(seq_codon).count('G')) / len(''.join(seq_codon)) * 100
         
         seq_aa = []
         for element in seq_codon:
             tmp = codons['Amino acid'][codons['Triplet'] == element]
@@ -359,24 +360,26 @@
                                 check = False
     
                                    
         enzyme_restriction = pd.DataFrame.from_dict(enzyme_restriction)
         enzyme_restriction = enzyme_restriction.drop_duplicates()
         enzyme_restriction = enzyme_restriction.reset_index(drop=True)
         enzyme_restriction = enzyme_restriction[~enzyme_restriction['name'].isin(restriction_df['name'])]
-        restriction_df = enzyme_restriction
-        if len(enzyme_restriction) > 0:
+        
+        if len(enzyme_restriction['name']) > 0:
             restriction_df = enzyme_restriction.copy()
             restriction_df['index'] = restriction_df.index
             restriction_df = restriction_df[['name', 'index']]
             restriction_df['index'] = [[x] for x in restriction_df['index']]
             restriction_df = restriction_df.groupby('name').agg({'index': 'sum'})
             restriction_df = restriction_df.reset_index()
     
-        if len(enzyme_restriction) == 0:
+        elif len(enzyme_restriction['name']) == 0:
+            restriction_df = enzyme_restriction
+
             print('\n Any new restriction places were created')
         else:
             print('\n New restriction places were created:')
             for name in enzyme_restriction['name']:
                 print(name)
     
     else:
@@ -384,19 +387,19 @@
         enzyme_restriction = pd.DataFrame.from_dict(enzyme_restriction)
         not_repaired = []
         final_sequence = sequence
         
     seq_tmp_GC = (sequence.count('C') + sequence.count('G')) / len(sequence) * 100
     seq_tmp_GC_2 = (final_sequence.count('C') + final_sequence.count('G')) / len(final_sequence) * 100
 
-    seq1 = [sequence[y:y+3] for y in range(0, len(sequence), 3)]
+    seq1 = [sequence[y:y+3].upper() for y in range(0, len(sequence), 3)]
     seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq][codons['Fraction'][codons['Triplet'] == seq].index[0]] for seq in seq1]
     seq_codon_fr = round(sum(seq_codon_fr) / len(seq_codon_fr),2)
     
-    seq2 = [final_sequence[y:y+3] for y in range(0, len(final_sequence), 3)]
+    seq2 = [final_sequence[y:y+3].upper() for y in range(0, len(final_sequence), 3)]
     seq_codon_fr2 = [codons['Fraction'][codons['Triplet'] == seq][codons['Fraction'][codons['Triplet'] == seq].index[0]] for seq in seq2]
     seq_codon_fr2 = round(sum(seq_codon_fr2) / len(seq_codon_fr2),2)
     
     df_final = {'status':[], 'sequence_na':[], 'frequence':[], 'GC%': []}
     df_final['status'].append('before_restriction_optimization')
     df_final['status'].append('after_restriction_optimization')
     df_final['sequence_na'].append(sequence)
```

### Comparing `JBioSeqTools-1.1.3/JBioSeqTools/vector_build/vector_build.py` & `JBioSeqTools-1.1.4/JBioSeqTools/vector_build/vector_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import pandas as pd
 pd.options.mode.chained_assignment = None
 import numpy as np
 from tqdm import tqdm
+import numpy as np
+import matplotlib.pyplot as plt
+import pandas as pd
 
 
 
-def load_metadata(codons:str() = 'https://github.com/jkubis96/JBioSeqTools/blob/main/data/codons.xlsx?raw=true', vectors:str() = 'https://github.com/jkubis96/JBioSeqTools/blob/main/data/vectors.xlsx?raw=true', linkers:str() = 'https://github.com/jkubis96/JBioSeqTools/blob/main/data/linkers.xlsx?raw=true', regulators:str() = 'https://github.com/jkubis96/JBioSeqTools/blob/main/data/regulators.xlsx?raw=true', fluorescent_tag:str() = 'https://github.com/jkubis96/JBioSeqTools/blob/main/data/fluorescent_tag.xlsx?raw=true', backbone:str() = 'https://github.com/jkubis96/JBioSeqTools/blob/main/data/backbone.xlsx?raw=true', promoters:str() = 'https://github.com/jkubis96/JBioSeqTools/blob/main/data/promoters.xlsx?raw=true', restriction:str() = 'https://github.com/jkubis96/JBioSeqTools/blob/main/data/restriction_enzymes.xlsx?raw=true'):
+def load_metadata(codons:str() = '../data/codons.xlsx', vectors:str() = '../data/vectors.xlsx', linkers:str() = '../data/linkers.xlsx', regulators:str() = '../data/regulators.xlsx', fluorescent_tag:str() = '../data/fluorescent_tag.xlsx', backbone:str() = '../data/backbone.xlsx', promoters:str() = '../data/promoters.xlsx', restriction:str() = '../data/restriction_enzymes.xlsx'):
     codons = pd.read_excel(codons)
     vectors = pd.read_excel(vectors)
     linkers = pd.read_excel(linkers)
     regulators = pd.read_excel(regulators)
     fluorescent_tag = pd.read_excel(fluorescent_tag)
     backbone = pd.read_excel(backbone)
     promoters = pd.read_excel(promoters)
     restriction = pd.read_excel(restriction)
     
     metadata = {'codons':codons, 'vectors':vectors, 'linkers':linkers, 'regulators':regulators, 'fluorescent_tag':fluorescent_tag, 'backbone':backbone, 'promoters':promoters, 'restriction':restriction}
 
     print('\n Metadata has loaded successfully')
     return metadata
 
+
 def create_project(project_name:str()):
     project = {'project':str(project_name),'transcripts':{}, 'elements':{'promoter':{}, 'fluorescence':{}, 'linkers':{}, 'regulators': {}}, 'vector':{'eval':{}, 'elements':{}, 'fasta':{}, 'graph':{}}}
     return project
     
 
 def load_sequences(n:int(), project:dict(), coding = True, upac_code:list() = ['A','C','T','G','N','M','R','W','S','Y','K','V','H','D','B'], **args):
     transcripts = {'name': [], 'ORF': [], 'sequence': []}
@@ -341,23 +345,23 @@
     return project
 
 
 
 
 def codon_otymization(sequence:str(), codons:pd.DataFrame, species:str()):
     codons = codons[codons['Species'] == species]
-    seq_codon = [sequence[y:y+3] for y in range(0, len(sequence), 3)]
-    seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq][codons['Fraction'][codons['Triplet'] == seq].index[0]] for seq in seq_codon]
+    seq_codon = [sequence[y:y+3].upper() for y in range(0, len(sequence), 3)]
+    seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq.upper()][codons['Fraction'][codons['Triplet'] == seq.upper()].index[0]] for seq in seq_codon]
     seq_codon_fr = round(sum(seq_codon_fr) / len(seq_codon_fr),2)
     
     seq_codon_mean = ''.join(seq_codon).count('C')
     seq_codon_GC = (''.join(seq_codon).count('C') + ''.join(seq_codon).count('G')) / len(''.join(seq_codon)) * 100
     seq_aa = []
     for element in seq_codon:
-        tmp = codons['Amino acid'][codons['Triplet'] == element]
+        tmp = codons['Amino acid'][codons['Triplet'] == element.upper()]
         tmp = tmp.reset_index()
         seq_aa.append(tmp['Amino acid'][0])
         
     mean_GC = (len(sequence)-1)*58/100/len(sequence)*3
     
     seq_tmp = []
     
@@ -455,21 +459,20 @@
     project['transcripts']['sequences']['optimized_vector_sequence_GC'] = np.nan  
     project['transcripts']['sequences']['optimized_vector_sequence_frequence'] = np.nan  
     project['transcripts']['sequences']['sequence_aa'] = np.nan 
     for tn in range(0,len(project['transcripts']['sequences']['sequence'])):
             tmp = codon_otymization(project['transcripts']['sequences']['vector_sequence'][tn], codons, species)
             project['transcripts']['sequences']['vector_sequence_GC'][tn] = tmp['GC%'][0] 
             project['transcripts']['sequences']['vector_sequence_frequence'][tn] = tmp['frequence'][0] 
-            project['transcripts']['sequences']['optimized_vector_sequence'] = tmp['sequence_na'][1] 
+            project['transcripts']['sequences']['optimized_vector_sequence'][tn] = tmp['sequence_na'][1] 
             project['transcripts']['sequences']['optimized_vector_sequence_GC'][tn] = tmp['GC%'][1] 
             project['transcripts']['sequences']['optimized_vector_sequence_frequence'][tn] = tmp['frequence'][1] 
-            project['transcripts']['sequences']['sequence_aa'] = tmp['sequence_aa'][1]
+            project['transcripts']['sequences']['sequence_aa'][tn] = tmp['sequence_aa'][1]
             
 
-
     return project
 
 
 
 def choose_sequence_variant(project:dict(), **args):
     for i in  project['transcripts']['sequences'].index:
         if str('ORF_sv' + str(i+1)) not in args:
@@ -508,17 +511,17 @@
 
 def check_restriction(sequence:str(), restriction:pd.DataFrame()):
 
     enzyme_restriction = {'name':[], 'restriction_place':[], 'restriction_sequence':[], 'start':[], 'stop':[]}
     
     for r in tqdm(restriction.index):
         check = True
-        if restriction['sequence'][r] in sequence:
+        if restriction['sequence'][r] in sequence.upper():
             while(check == True):
-                bmp = list(sequence)
+                bmp = list(sequence.upper())
                 for n in range(0,len(restriction['sequence'][r])):
                     for j in range(n,len(bmp)-len(restriction['sequence'][r])):
                        lower = j
                        upper = j + len(restriction['sequence'][r])
                        if upper < len(bmp) and ''.join(bmp[lower:upper]) == restriction['sequence'][r]:
                             enzyme_restriction['name'].append(restriction['name'][r])
                             enzyme_restriction['restriction_sequence'].append(restriction['sequence'][r])
@@ -528,23 +531,24 @@
                             check = False
 
                                
     enzyme_restriction = pd.DataFrame.from_dict(enzyme_restriction)
     enzyme_restriction = enzyme_restriction.drop_duplicates()
     enzyme_restriction = enzyme_restriction.reset_index(drop=True)
     
-    if len(enzyme_restriction) > 0:
+    if len(enzyme_restriction['name']) > 0:
         restriction_df = enzyme_restriction.copy()
         restriction_df['index'] = restriction_df.index
         restriction_df = restriction_df[['name', 'index']]
         restriction_df['index'] = [[x] for x in restriction_df['index']]
         restriction_df = restriction_df.groupby('name').agg({'index': 'sum'})
         restriction_df = restriction_df.reset_index()
     
-    if len(enzyme_restriction) == 0:
+    else:
+        restriction_df = enzyme_restriction
         print('\n Any restriction places were not found')
     
     return enzyme_restriction, restriction_df
 
 
 
 
@@ -579,16 +583,16 @@
 
 
 
 def repair_sequences(sequence:str(), codons:pd.DataFrame, restriction_df:pd.DataFrame(), restriction:pd.DataFrame(), enzyme_list:list(), species:str()):
     if len(restriction_df) != 0:
         not_repaired = []
         codons = codons[codons['Species'] == species]
-        seq_codon = [sequence[y:y+3] for y in range(0, len(sequence), 3)]
-        seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq][codons['Fraction'][codons['Triplet'] == seq].index[0]] for seq in seq_codon]
+        seq_codon = [sequence[y:y+3].upper() for y in range(0, len(sequence), 3)]
+        seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq.upper()][codons['Fraction'][codons['Triplet'] == seq.upper()].index[0]] for seq in seq_codon]
         seq_codon_fr = round(sum(seq_codon_fr) / len(seq_codon_fr),2)
         seq_codon_GC = (''.join(seq_codon).count('C') + ''.join(seq_codon).count('G')) / len(''.join(seq_codon)) * 100
         
         seq_aa = []
         for element in seq_codon:
             tmp = codons['Amino acid'][codons['Triplet'] == element]
             tmp = tmp.reset_index()
@@ -671,15 +675,15 @@
         enzyme_restriction = {'name':[], 'restriction_place':[], 'restriction_sequence':[], 'sequence':[], 'start':[], 'stop':[]}
         
         print('\n Checking new restriction...')
         for r in tqdm(restriction.index):
             check = True
             if restriction['sequence'][r] in final_sequence:
                 while(check == True):
-                    bmp = list(final_sequence)
+                    bmp = list(final_sequence.upper())
                     for n in range(0,len(restriction['sequence'][r])):
                         for j in range(n,len(bmp)-len(restriction['sequence'][r])):
                            lower = j
                            upper = j + len(restriction['sequence'][r])
                            if upper < len(bmp) and ''.join(bmp[lower:upper]) == restriction['sequence'][r]:
                                 enzyme_restriction['name'].append(restriction['name'][r])
                                 enzyme_restriction['restriction_sequence'].append(restriction['sequence'][r])
@@ -690,28 +694,29 @@
                                 check = False
     
                                    
         enzyme_restriction = pd.DataFrame.from_dict(enzyme_restriction)
         enzyme_restriction = enzyme_restriction.drop_duplicates()
         enzyme_restriction = enzyme_restriction.reset_index(drop=True)
         enzyme_restriction = enzyme_restriction[~enzyme_restriction['name'].isin(restriction_df['name'])]
-        restriction_df = enzyme_restriction
-        if len(enzyme_restriction) > 0:
+        
+        if len(enzyme_restriction['name']) > 0:
             restriction_df = enzyme_restriction.copy()
             restriction_df['index'] = restriction_df.index
             restriction_df = restriction_df[['name', 'index']]
             restriction_df['index'] = [[x] for x in restriction_df['index']]
             restriction_df = restriction_df.groupby('name').agg({'index': 'sum'})
             restriction_df = restriction_df.reset_index()
     
-        if len(enzyme_restriction) == 0:
-            print('\n Any new restriction places were not created')
+        elif len(enzyme_restriction['name']) == 0:
+            restriction_df = enzyme_restriction
+            print('\n Any new restriction places were created')
         else:
             print('\n New restriction places were created:')
-            for name in np.unique(enzyme_restriction['name']):
+            for name in enzyme_restriction['name']:
                 print(name)
     
     else:
         enzyme_restriction = {'name':[], 'restriction_place':[], 'restriction_sequence':[], 'start':[], 'stop':[]}
         enzyme_restriction = pd.DataFrame.from_dict(enzyme_restriction)
         not_repaired = []
         final_sequence = sequence
@@ -721,15 +726,15 @@
 
 
 
 def find_restriction_vector(project:dict(), restriction:pd.DataFrame()):
     project['transcripts']['sequences']['full_restriction'] = ''
     project['transcripts']['sequences']['enzymes_df'] = ''
     for trans in project['transcripts']['sequences'].index:
-        full, coordinates = check_restriction(str( project['transcripts']['sequences']['vector_sequence'][trans]), restriction)
+        full, coordinates = check_restriction(str(project['transcripts']['sequences']['vector_sequence'][trans]), restriction)
         project['transcripts']['sequences']['full_restriction'][trans] = full.to_records(index=True)
         project['transcripts']['sequences']['enzymes_df'][trans] =  np.array(coordinates)
         
     return project
         
 
 
@@ -867,41 +872,37 @@
     project['vector']['elements'] = data_frame
     project['vector']['fasta'] = fasta
      
     return project
 
 
 
-import numpy as np
-import matplotlib.pyplot as plt
-import pandas as pd
 
 def vector_plot_project(project, title:str()):
     
     vector_df = pd.DataFrame(project['vector']['elements'])
 
     vector_df = vector_df.sort_index(ascending=False)
     
     explode = []
     for i in vector_df['element']:
         if i in 'backbone_element':
-            explode.append(0)
+            explode.append(-0.2)
         else:
-            explode.append(0.1)
+            explode.append(0)
             
     
     labels = []
     for i in vector_df['element']:
         if i in 'backbone_element':
             labels.append('')
         else:
             labels.append(i)
     
-    
-    
+
     
     fig, ax = plt.subplots(figsize=(10, 10), subplot_kw=dict(aspect="equal"))
     
     
     wedges, texts = ax.pie(vector_df['length'],explode = explode, startangle=90)
     
     
@@ -918,16 +919,16 @@
         connectionstyle = "angle,angleA=0,angleB={}".format(ang)
         kw["arrowprops"].update({"connectionstyle": connectionstyle})
         if len(labels[i]) > 0:
             n += 0.25
             ax.annotate(labels[i], xy=(x, y), xytext=(1.4*x+(n*x/4), y*1.1+(n*y/4)),
                         horizontalalignment=horizontalalignment, fontsize=20, weight="bold", **kw)
     
-    circle1 = plt.Circle( (0,0), 1, color='black')
-    circle2 = plt.Circle( (0,0), 0.95, color='white')
+    circle1 = plt.Circle( (0,0), 0.85, color='black')
+    circle2 = plt.Circle( (0,0), 0.8, color='white')
     
     ax.text(0.5, 0.5, str(title + '\n length: ' + str(sum(vector_df['length'])) + 'nc'), transform = ax.transAxes, va = 'center', ha = 'center', backgroundcolor = 'white', weight="bold", fontsize = 25)
     
     p=plt.gcf()
     p.gca().add_artist(circle1)
     p.gca().add_artist(circle2)
```

### Comparing `JBioSeqTools-1.1.3/JBioSeqTools/vector_graph/graph_plot.py` & `JBioSeqTools-1.1.4/JBioSeqTools/vector_graph/graph_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 def vector_plot(vector_df:pd.DataFrame(), title:str()):
     vector_df = vector_df.sort_index(ascending=False)
     
     explode = []
     for i in vector_df['element']:
         if i in 'backbone_element':
-            explode.append(0)
+            explode.append(-0.2)
         else:
-            explode.append(0.1)
+            explode.append(0)
             
     
     labels = []
     for i in vector_df['element']:
         if i in 'backbone_element':
             labels.append('')
         else:
```

### Comparing `JBioSeqTools-1.1.3/JBioSeqTools.egg-info/PKG-INFO` & `JBioSeqTools-1.1.4/JBioSeqTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.1.3
+Version: 1.1.4
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
-Keywords: sequence,optimization,vectors,AAV,GC,restriction enzimes
+Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 License-File: LICENSE
```

### Comparing `JBioSeqTools-1.1.3/LICENSE` & `JBioSeqTools-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.3/PKG-INFO` & `JBioSeqTools-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.1.3
+Version: 1.1.4
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
-Keywords: sequence,optimization,vectors,AAV,GC,restriction enzimes
+Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 License-File: LICENSE
```

### Comparing `JBioSeqTools-1.1.3/README.md` & `JBioSeqTools-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.3/setup.py` & `JBioSeqTools-1.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.3' 
+VERSION = '1.1.4' 
 DESCRIPTION = 'JBioSeqTools'
 LONG_DESCRIPTION = 'JBioSeqTools is the python library for biological sequence optimization (GC % content & codon frequency) for better expression of different species cells in vivo. It also allows building AAV vectors with the possibility of choosing sequences between ITRs such as transcript, promoter, enhancer, and molecular fluorescent tag. Finally, the user obtains ready for order construct with a whole sequence and visualization. Package description  on https://github.com/jkubis96/JBioSeqTools'
 
 # Setting up
 setup(
         name="JBioSeqTools", 
         version=VERSION,
         author="Jakub Kubis",
         author_email="jbiosystem@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         install_requires=['pandas', 'tqdm', 'matplotlib', 'numpy', 'requests'],       
-        keywords=['sequence', 'optimization', 'vectors', 'AAV', 'GC', 'restriction enzimes'],
+        keywords=['sequence', 'optimization', 'vectors', 'AAV', 'GC', 'restriction enzyme'],
         license = 'MIT',
         classifiers = [
             "Development Status :: 3 - Alpha",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
             "Operating System :: POSIX :: Linux",
```

