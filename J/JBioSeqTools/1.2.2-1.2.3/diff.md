# Comparing `tmp/JBioSeqTools-1.2.2.tar.gz` & `tmp/JBioSeqTools-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBioSeqTools-1.2.2.tar", last modified: Tue Jul  4 13:35:53 2023, max compression
+gzip compressed data, was "JBioSeqTools-1.2.3.tar", last modified: Tue Jul  4 13:51:09 2023, max compression
```

## Comparing `JBioSeqTools-1.2.2.tar` & `JBioSeqTools-1.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 13:35:53.305820 JBioSeqTools-1.2.2/
-drwxrwxrwx   0        0        0        0 2023-07-04 13:35:53.274428 JBioSeqTools-1.2.2/JBioSeqTools/
--rw-rw-rw-   0        0        0      343 2023-07-04 13:35:17.000000 JBioSeqTools-1.2.2/JBioSeqTools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:35:53.274428 JBioSeqTools-1.2.2/JBioSeqTools/api_elements/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.2/JBioSeqTools/api_elements/__init__.py
--rw-rw-rw-   0        0        0     6152 2022-12-15 18:39:44.000000 JBioSeqTools-1.2.2/JBioSeqTools/api_elements/api.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:35:53.287458 JBioSeqTools-1.2.2/JBioSeqTools/seq_tools/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.2/JBioSeqTools/seq_tools/__init__.py
--rw-rw-rw-   0        0        0    18814 2023-07-04 13:19:52.000000 JBioSeqTools-1.2.2/JBioSeqTools/seq_tools/seq_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:35:53.287972 JBioSeqTools-1.2.2/JBioSeqTools/vector_build/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.2/JBioSeqTools/vector_build/__init__.py
--rw-rw-rw-   0        0        0    47582 2023-07-04 13:19:34.000000 JBioSeqTools-1.2.2/JBioSeqTools/vector_build/vector_build.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:35:53.287972 JBioSeqTools-1.2.2/JBioSeqTools/vector_graph/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.2/JBioSeqTools/vector_graph/__init__.py
--rw-rw-rw-   0        0        0     1966 2023-07-04 08:33:55.000000 JBioSeqTools-1.2.2/JBioSeqTools/vector_graph/graph_plot.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:35:53.274428 JBioSeqTools-1.2.2/JBioSeqTools.egg-info/
--rw-rw-rw-   0        0        0     1000 2023-07-04 13:35:52.000000 JBioSeqTools-1.2.2/JBioSeqTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      711 2023-07-04 13:35:53.000000 JBioSeqTools-1.2.2/JBioSeqTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 13:35:52.000000 JBioSeqTools-1.2.2/JBioSeqTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-04 13:35:52.000000 JBioSeqTools-1.2.2/JBioSeqTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-04 13:35:52.000000 JBioSeqTools-1.2.2/JBioSeqTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.2.2/LICENSE
--rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1000 2023-07-04 13:35:53.303501 JBioSeqTools-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 13:35:53.303501 JBioSeqTools-1.2.2/data/
--rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.2.2/data/backbone.xlsx
--rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.2.2/data/codons.xlsx
--rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.2.2/data/fluorescent_tag.xlsx
--rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.2.2/data/linkers.xlsx
--rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.2.2/data/promoters.xlsx
--rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.2.2/data/regulators.xlsx
--rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.2.2/data/restriction_enzymes.xlsx
--rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.2.2/data/vectors.xlsx
--rw-rw-rw-   0        0        0       42 2023-07-04 13:35:53.305820 JBioSeqTools-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1469 2023-07-04 13:35:20.000000 JBioSeqTools-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:51:09.427658 JBioSeqTools-1.2.3/
+drwxrwxrwx   0        0        0        0 2023-07-04 13:51:09.412035 JBioSeqTools-1.2.3/JBioSeqTools/
+-rw-rw-rw-   0        0        0      343 2023-07-04 13:50:22.000000 JBioSeqTools-1.2.3/JBioSeqTools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:51:09.412035 JBioSeqTools-1.2.3/JBioSeqTools/api_elements/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.3/JBioSeqTools/api_elements/__init__.py
+-rw-rw-rw-   0        0        0     6152 2023-07-04 13:48:18.000000 JBioSeqTools-1.2.3/JBioSeqTools/api_elements/api.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:51:09.412035 JBioSeqTools-1.2.3/JBioSeqTools/seq_tools/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.3/JBioSeqTools/seq_tools/__init__.py
+-rw-rw-rw-   0        0        0    18818 2023-07-04 13:48:33.000000 JBioSeqTools-1.2.3/JBioSeqTools/seq_tools/seq_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:51:09.412035 JBioSeqTools-1.2.3/JBioSeqTools/vector_build/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.3/JBioSeqTools/vector_build/__init__.py
+-rw-rw-rw-   0        0        0    47586 2023-07-04 13:49:53.000000 JBioSeqTools-1.2.3/JBioSeqTools/vector_build/vector_build.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:51:09.412035 JBioSeqTools-1.2.3/JBioSeqTools/vector_graph/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.3/JBioSeqTools/vector_graph/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-07-04 08:33:55.000000 JBioSeqTools-1.2.3/JBioSeqTools/vector_graph/graph_plot.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:51:09.412035 JBioSeqTools-1.2.3/JBioSeqTools.egg-info/
+-rw-rw-rw-   0        0        0     1000 2023-07-04 13:51:08.000000 JBioSeqTools-1.2.3/JBioSeqTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2023-07-04 13:51:09.000000 JBioSeqTools-1.2.3/JBioSeqTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 13:51:08.000000 JBioSeqTools-1.2.3/JBioSeqTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-04 13:51:09.000000 JBioSeqTools-1.2.3/JBioSeqTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-04 13:51:09.000000 JBioSeqTools-1.2.3/JBioSeqTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1000 2023-07-04 13:51:09.427658 JBioSeqTools-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 13:51:09.427658 JBioSeqTools-1.2.3/data/
+-rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.2.3/data/backbone.xlsx
+-rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.2.3/data/codons.xlsx
+-rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.2.3/data/fluorescent_tag.xlsx
+-rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.2.3/data/linkers.xlsx
+-rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.2.3/data/promoters.xlsx
+-rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.2.3/data/regulators.xlsx
+-rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.2.3/data/restriction_enzymes.xlsx
+-rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.2.3/data/vectors.xlsx
+-rw-rw-rw-   0        0        0       42 2023-07-04 13:51:09.427658 JBioSeqTools-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1469 2023-07-04 13:50:19.000000 JBioSeqTools-1.2.3/setup.py
```

### Comparing `JBioSeqTools-1.2.2/JBioSeqTools/api_elements/api.py` & `JBioSeqTools-1.2.3/JBioSeqTools/api_elements/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,27 +87,27 @@
                 
         genes_results['entrenz'][g] = tmp_dic
     
     return genes_results
 
 
 def create_cds_input_to_project(project, n, gene_info):
-    transcripts = {'name': [], 'ORF': [], 'sequence': []}
+    transcripts = {'name': [], 'SEQ': [], 'sequence': []}
     for gen in gene_info.index:
         transcripts['name'].append(gene_info['common_symbol'][gen])
-        transcripts['ORF'].append(str('ORF' + str(int(gen)+1)))
+        transcripts['SEQ'].append(str('SEQ' + str(int(gen)+1)))
         transcripts['sequence'].append(gene_info['choosen_transcript'][gen])
         
         
     project['transcripts']['sequences'] = pd.DataFrame(transcripts)
     project['transcripts']['sequences'] = pd.DataFrame(transcripts)
     
     transcript_list = []
     for i in range(1,n+1):
-        transcript_list.append(str('ORF'+str(i)))
+        transcript_list.append(str('SEQ'+str(i)))
         transcript_list.append(str('linker'+str(i)))
     
     transcript_list = transcript_list[0:len(transcript_list) - 1]
     project['elements']['transcripts'] = transcript_list
     
     return project
```

### Comparing `JBioSeqTools-1.2.2/JBioSeqTools/seq_tools/seq_tools.py` & `JBioSeqTools-1.2.3/JBioSeqTools/seq_tools/seq_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     return metadata
 
 
 
 
 
-def load_sequence(coding = True, upac_code:list() = ['A','C','T','G','N','M','R','W','S','Y','K','V','H','D','B'], **args):
+def load_sequence(coding = True, upac_code:list() = ['A','C','T','G','N','M','R','W','S','Y','K','V','H','D','B','U'], **args):
     check = True
     while (check == True):
         sequence = input('\n Enter sequence: ').replace('\\n', '\n')
         sequence = ''.join(c.upper() for c in sequence if c.isalpha())
     
     
         test = sequence
```

### Comparing `JBioSeqTools-1.2.2/JBioSeqTools/vector_build/vector_build.py` & `JBioSeqTools-1.2.3/JBioSeqTools/vector_build/vector_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,31 +27,31 @@
 
 
 def create_project(project_name:str()):
     project = {'project':str(project_name),'transcripts':{}, 'elements':{'promoter':{}, 'fluorescence':{}, 'linkers':{}, 'regulators': {}}, 'vector':{'eval':{}, 'elements':{}, 'fasta':{}, 'graph':{}}}
     return project
     
 
-def load_sequences(n:int(), project:dict(), coding = True, upac_code:list() = ['A','C','T','G','N','M','R','W','S','Y','K','V','H','D','B'], **args):
-    transcripts = {'name': [], 'ORF': [], 'sequence': []}
+def load_sequences(n:int(), project:dict(), coding = True, upac_code:list() = ['A','C','T','G','N','M','R','W','S','Y','K','V','H','D','B','U'], **args):
+    transcripts = {'name': [], 'SEQ': [], 'sequence': []}
     for i in range(1,n+1):
         check = True
         check_name = True
         while (check == True or check_name == True):
-            if str('ORF' + str(i)) not in args and check == True:
-                globals()[str('ORF' + str(i))] = input('Enter sequence ' + str('ORF'+str(i)) + ': ').replace('\\n', '\n')
-                globals()[str('ORF' + str(i))] = ''.join(c.upper() for c in eval(str('ORF' + str(i))) if c.isalpha())
-            if str('ORF' + str(i) + '_name') not in args and check_name == True:
-                globals()[str('ORF' + str(i) + '_name')] = input('Enter sequence name ' + str('ORF'+str(i)) + ': ')
-                globals()[str('ORF' + str(i) + '_name')] = eval(str('ORF' + str(i) + '_name')).upper()
-                
-            if str('ORF'+str(i)) in args:
-                test = args[str('ORF'+str(i))]
-                test = [args[str('ORF'+str(i))][y:y+3] for y in range(0, len(args[str('ORF'+str(i))]), 3)]
-                test2 = args[str('ORF'+str(i))].upper()
+            if str('SEQ' + str(i)) not in args and check == True:
+                globals()[str('SEQ' + str(i))] = input('Enter sequence ' + str('SEQ'+str(i)) + ': ').replace('\\n', '\n')
+                globals()[str('SEQ' + str(i))] = ''.join(c.upper() for c in eval(str('SEQ' + str(i))) if c.isalpha())
+            if str('SEQ' + str(i) + '_name') not in args and check_name == True:
+                globals()[str('SEQ' + str(i) + '_name')] = input('Enter sequence name ' + str('SEQ'+str(i)) + ': ')
+                globals()[str('SEQ' + str(i) + '_name')] = eval(str('SEQ' + str(i) + '_name')).upper()
+                
+            if str('SEQ'+str(i)) in args:
+                test = args[str('SEQ'+str(i))]
+                test = [args[str('SEQ'+str(i))][y:y+3] for y in range(0, len(args[str('SEQ'+str(i))]), 3)]
+                test2 = args[str('SEQ'+str(i))].upper()
                 test2 = list(test2)
                 
                 t2 = True
                 for h in test2:
                     if h not in upac_code:
                         t2 = False
                         break
@@ -66,31 +66,31 @@
                 elif (t2 == False):
                     print("\n Wrong sequence " + str(i) + ". The sequence contains letters not included in UPAC code. UPAC: ")
                     print(upac_code)
                     check = True
                     
                 else:
                     check = False
-                if (len(args[str('ORF' + str(i) + '_name')]) == 0):
+                if (len(args[str('SEQ' + str(i) + '_name')]) == 0):
                     print("\n Wrong name.  Enter sequence name")
                     check_name = True
                     
                 else:
                     check_name = False
                     
                 if check_name == False and check == False:
-                    transcripts['name'].append(globals()[str('ORF' + str(i) + '_name')].upper())
-                    transcripts['ORF'].append(str('ORF' + str(i)))
-                    transcripts['sequence'].append(''.join(c.upper() for c in globals()[str('ORF' + str(i))] if c.isalpha()))
+                    transcripts['name'].append(globals()[str('SEQ' + str(i) + '_name')].upper())
+                    transcripts['SEQ'].append(str('SEQ' + str(i)))
+                    transcripts['sequence'].append(''.join(c.upper() for c in globals()[str('SEQ' + str(i))] if c.isalpha()))
                 
                 
             else:
-                test = globals()[str('ORF'+str(i))]
-                test = [globals()[str('ORF'+str(i))][y:y+3] for y in range(0, len(globals()[str('ORF'+str(i))]), 3)]
-                test2 = globals()[str('ORF'+str(i))].upper()
+                test = globals()[str('SEQ'+str(i))]
+                test = [globals()[str('SEQ'+str(i))][y:y+3] for y in range(0, len(globals()[str('SEQ'+str(i))]), 3)]
+                test2 = globals()[str('SEQ'+str(i))].upper()
                 test2 = list(test2)
                 
                 t2 = True
                 for h in test2:
                     if h not in upac_code:
                         t2 = False
                         break
@@ -106,32 +106,32 @@
                     print("\n Wrong sequence " + str(i) + ". The sequence contains letters not included in UPAC code. UPAC: ")
                     print(upac_code)
                     check = True
                     
                     
                 else:
                     check = False
-                if (len(globals()[str('ORF' + str(i) + '_name')]) == 0):
+                if (len(globals()[str('SEQ' + str(i) + '_name')]) == 0):
                     print("\n Wrong name.  Enter sequence name")
                     check_name = True
                     
                 else:
                     check_name = False
                     
                 if check_name == False and check == False:
-                    transcripts['name'].append(globals()[str('ORF' + str(i) + '_name')].upper())
-                    transcripts['ORF'].append(str('ORF' + str(i)))
-                    transcripts['sequence'].append(''.join(c.upper() for c in globals()[str('ORF' + str(i))] if c.isalpha()))
-                    del globals()[str('ORF' + str(i) + '_name')], globals()[str('ORF' + str(i))]
+                    transcripts['name'].append(globals()[str('SEQ' + str(i) + '_name')].upper())
+                    transcripts['SEQ'].append(str('SEQ' + str(i)))
+                    transcripts['sequence'].append(''.join(c.upper() for c in globals()[str('SEQ' + str(i))] if c.isalpha()))
+                    del globals()[str('SEQ' + str(i) + '_name')], globals()[str('SEQ' + str(i))]
 
      
     transcripts = pd.DataFrame(transcripts)
     transcript_list = []
     for i in range(1,n+1):
-        transcript_list.append(str('ORF'+str(i)))
+        transcript_list.append(str('SEQ'+str(i)))
         transcript_list.append(str('linker'+str(i)))
     
     transcript_list = transcript_list[0:len(transcript_list) - 1]
     project['transcripts']['sequences'] = transcripts
     project['elements']['transcripts'] = transcript_list
     
     return project  
@@ -473,38 +473,38 @@
 
     return project
 
 
 
 def choose_sequence_variant(project:dict(), **args):
     for i in  project['transcripts']['sequences'].index:
-        if str('ORF_sv' + str(i+1)) not in args:
+        if str('SEQ_sv' + str(i+1)) not in args:
             print('-------------------------------------------------------------')
-            print('name : ' + str( project['transcripts']['sequences']['ORF'][i] + ' -> ' +  project['transcripts']['sequences']['name'][i]))
+            print('name : ' + str( project['transcripts']['sequences']['SEQ'][i] + ' -> ' +  project['transcripts']['sequences']['name'][i]))
             print('**************************************************************')
             print('Before optimization:')
             print('* GC % : ' + str( project['transcripts']['sequences']['vector_sequence_GC'][i]))
             print('* Mean codon frequence : ' + str( project['transcripts']['sequences']['vector_sequence_frequence'][i]))
             print('**************************************************************')
             print('After optimization:')
             print('* GC % : ' + str( project['transcripts']['sequences']['optimized_vector_sequence_GC'][i]))
             print('* Mean codon frequence : ' + str( project['transcripts']['sequences']['optimized_vector_sequence_frequence'][i]))
             print('Choose sequence: optimized [o] or not optimized [n]')
     
             
             check = True
             while (check == True):
-                locals()[str('ORF_sv' + str(i+1))] = input('\n Writte your choose [o/n]: ')
-                if str('ORF_sv' + str(i+1)) in locals() and locals()[str('ORF_sv' + str(i+1))] == 'o' or str('ORF_sv' + str(i+1)) in locals() and locals()[str('ORF_sv' + str(i+1))] == 'n':
+                locals()[str('SEQ_sv' + str(i+1))] = input('\n Writte your choose [o/n]: ')
+                if str('SEQ_sv' + str(i+1)) in locals() and locals()[str('SEQ_sv' + str(i+1))] == 'o' or str('SEQ_sv' + str(i+1)) in locals() and locals()[str('SEQ_sv' + str(i+1))] == 'n':
                     check = False
                     
                 
-        if str('ORF_sv' + str(i+1)) in locals() and locals()[str('ORF_sv' + str(i+1))] == 'o' :
+        if str('SEQ_sv' + str(i+1)) in locals() and locals()[str('SEQ_sv' + str(i+1))] == 'o' :
             project['transcripts']['sequences']['vector_sequence'][i] = project['transcripts']['sequences']['optimized_vector_sequence'][i]
-        if str('ORF_sv' + str(i+1)) in args and args[str('ORF_sv' + str(i+1))] == 'o' :
+        if str('SEQ_sv' + str(i+1)) in args and args[str('SEQ_sv' + str(i+1))] == 'o' :
             project['transcripts']['sequences']['vector_sequence'][i] = project['transcripts']['sequences']['optimized_vector_sequence'][i]
 
         
     
     return project       
                 
 
@@ -743,15 +743,15 @@
 
 def choose_restriction_vector(project:dict(), restriction:pd.DataFrame()):
     project['transcripts']['sequences']['enzymes'] = ''
     for trans in project['transcripts']['sequences'].index:
         index = pd.DataFrame(project['transcripts']['sequences']['enzymes_df'][trans])
         index.index = index[1]
         index.index = range(0, len(index[1]))
-        print("\n Choose enzymes for " + str(project['transcripts']['sequences']['ORF']))
+        print("\n Choose enzymes for " + str(project['transcripts']['sequences']['SEQ']))
         project['transcripts']['sequences']['enzymes'][trans] = choose_restriction_to_remove(index).tolist()
         
     return project
         
 
 
 
@@ -799,15 +799,15 @@
 def eval_vector(project:dict(), vectors:pd.DataFrame(), vector_type:str(), **args):
     
     vectors = vectors[vectors['vector_type'] == vector_type]
     for element, n in enumerate(vectors.index):
         locals()[str(vectors['component'][n])] = vectors['sequence'][n]
       
     for element, n in enumerate(project['transcripts']['sequences'].index):
-        locals()[str(project['transcripts']['sequences']['ORF'][n])] = project['transcripts']['sequences']['vector_sequence'][n]
+        locals()[str(project['transcripts']['sequences']['SEQ'][n])] = project['transcripts']['sequences']['vector_sequence'][n]
     
     elements =  project['vector']['eval'].split()
     tf =  [x != '+' for x in elements]
     elemensts = [i for indx,i in enumerate(elements) if tf[indx] == True]
 
     
     for element, n in enumerate(project['elements']):
@@ -862,16 +862,16 @@
     data_frame['element'] = new_element
     data_frame = data_frame.reset_index(drop=True)
     
     
     for n in data_frame.index: 
        if str(data_frame['element'][n]) + '_name' in locals():
            data_frame['element'][n] = data_frame['element'][n] + ' : ' + eval(str(data_frame['element'][n]) + '_name')
-       elif str(data_frame['element'][n]) in list(project['transcripts']['sequences']['ORF']):
-            data_frame['element'][n] = data_frame['element'][n] + ' : ' + str(project['transcripts']['sequences']['name'][project['transcripts']['sequences']['ORF'] == str(data_frame['element'][n])][project['transcripts']['sequences']['name'][project['transcripts']['sequences']['ORF'] == str(data_frame['element'][n])].index[0]])
+       elif str(data_frame['element'][n]) in list(project['transcripts']['sequences']['SEQ']):
+            data_frame['element'][n] = data_frame['element'][n] + ' : ' + str(project['transcripts']['sequences']['name'][project['transcripts']['sequences']['SEQ'] == str(data_frame['element'][n])][project['transcripts']['sequences']['name'][project['transcripts']['sequences']['SEQ'] == str(data_frame['element'][n])].index[0]])
 
 
 
     project['vector']['elements'] = data_frame
     project['vector']['fasta'] = fasta
      
     return project
```

### Comparing `JBioSeqTools-1.2.2/JBioSeqTools/vector_graph/graph_plot.py` & `JBioSeqTools-1.2.3/JBioSeqTools/vector_graph/graph_plot.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/JBioSeqTools.egg-info/PKG-INFO` & `JBioSeqTools-1.2.3/JBioSeqTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.2.2
+Version: 1.2.3
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-1.2.2/JBioSeqTools.egg-info/SOURCES.txt` & `JBioSeqTools-1.2.3/JBioSeqTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/LICENSE` & `JBioSeqTools-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/PKG-INFO` & `JBioSeqTools-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.2.2
+Version: 1.2.3
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-1.2.2/README.md` & `JBioSeqTools-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/data/backbone.xlsx` & `JBioSeqTools-1.2.3/data/backbone.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/data/codons.xlsx` & `JBioSeqTools-1.2.3/data/codons.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/data/fluorescent_tag.xlsx` & `JBioSeqTools-1.2.3/data/fluorescent_tag.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/data/linkers.xlsx` & `JBioSeqTools-1.2.3/data/linkers.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/data/promoters.xlsx` & `JBioSeqTools-1.2.3/data/promoters.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/data/regulators.xlsx` & `JBioSeqTools-1.2.3/data/regulators.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/data/restriction_enzymes.xlsx` & `JBioSeqTools-1.2.3/data/restriction_enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/data/vectors.xlsx` & `JBioSeqTools-1.2.3/data/vectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.2.2/setup.py` & `JBioSeqTools-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.2' 
+VERSION = '1.2.3' 
 DESCRIPTION = 'JBioSeqTools'
 LONG_DESCRIPTION = 'JBioSeqTools is the python library for biological sequence optimization (GC % content & codon frequency) for better expression of different species cells in vivo. It also allows building AAV vectors with the possibility of choosing sequences between ITRs such as transcript, promoter, enhancer, and molecular fluorescent tag. Finally, the user obtains ready for order construct with a whole sequence and visualization. Package description  on https://github.com/jkubis96/JBioSeqTools'
 
 # Setting up
 setup(
         name="JBioSeqTools", 
         version=VERSION,
```

