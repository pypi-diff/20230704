# Comparing `tmp/mly-0.3.4.5.tar.gz` & `tmp/mly-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly-0.3.4.5.tar", last modified: Mon Jun 12 16:22:40 2023, max compression
+gzip compressed data, was "mly-0.5.2.tar", last modified: Tue Jul  4 14:04:58 2023, max compression
```

## Comparing `mly-0.3.4.5.tar` & `mly-0.5.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.146598 mly-0.3.4.5/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-0.3.4.5/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      499 2023-06-12 16:22:40.146598 mly-0.3.4.5/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.3.4.5/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.130598 mly-0.3.4.5/mly/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.3.4.5/mly/SRD.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.3.4.5/mly/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10219 2023-05-16 10:32:51.000000 mly-0.3.4.5/mly/createFileSystem.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.138598 mly-0.3.4.5/mly/datatools/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      155 2023-06-09 13:56:57.000000 mly-0.3.4.5/mly/datatools/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22280 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/datatools/core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28108 2023-06-09 10:58:15.000000 mly-0.3.4.5/mly/datatools/datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    91676 2023-06-09 11:06:25.000000 mly-0.3.4.5/mly/datatools/generator.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.142598 mly-0.3.4.5/mly/datatools/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/datatools/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/datatools/tests/test_core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/datatools/tests/test_datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4975 2023-06-09 11:10:13.000000 mly-0.3.4.5/mly/datatools/tests/test_generator.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18459 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/exceptions.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.3.4.5/mly/mlTools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.3.4.5/mly/models.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    12353 2023-05-04 12:56:19.000000 mly-0.3.4.5/mly/null_energy_map.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7316 2023-06-09 11:13:40.000000 mly-0.3.4.5/mly/offlinefar.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-05-04 12:56:19.000000 mly-0.3.4.5/mly/plugins.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10134 2023-05-04 12:56:19.000000 mly-0.3.4.5/mly/projectwave.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.3.4.5/mly/simulateddetectornoise.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.145598 mly-0.3.4.5/mly/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.3.4.5/mly/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.3.4.5/mly/tests/test_init.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.3.4.5/mly/tests/test_tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13014 2023-05-04 12:56:19.000000 mly-0.3.4.5/mly/tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126803 2023-06-09 13:52:48.000000 mly-0.3.4.5/mly/validators.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/waveforms.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.135598 mly-0.3.4.5/mly.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      499 2023-06-12 16:22:40.000000 mly-0.3.4.5/mly.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      733 2023-06-12 16:22:40.000000 mly-0.3.4.5/mly.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-06-12 16:22:40.000000 mly-0.3.4.5/mly.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       96 2023-06-12 16:22:40.000000 mly-0.3.4.5/mly.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-06-12 16:22:40.000000 mly-0.3.4.5/mly.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-06-12 16:22:40.147598 mly-0.3.4.5/setup.cfg
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      956 2023-06-12 16:21:50.000000 mly-0.3.4.5/setup.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.495301 mly-0.5.2/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-0.5.2/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      497 2023-07-04 14:04:58.496301 mly-0.5.2/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.5.2/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.406300 mly-0.5.2/mly/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.5.2/mly/SRD.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.5.2/mly/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10014 2023-06-15 11:06:15.000000 mly-0.5.2/mly/createFileSystem.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.415300 mly-0.5.2/mly/datatools/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      155 2023-06-09 13:56:57.000000 mly-0.5.2/mly/datatools/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22332 2023-06-20 13:25:10.000000 mly-0.5.2/mly/datatools/core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28108 2023-06-09 10:58:15.000000 mly-0.5.2/mly/datatools/datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    91856 2023-06-20 13:25:12.000000 mly-0.5.2/mly/datatools/generator.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.488300 mly-0.5.2/mly/datatools/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:56:02.000000 mly-0.5.2/mly/datatools/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-05-09 14:56:02.000000 mly-0.5.2/mly/datatools/tests/test_core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-05-09 14:56:02.000000 mly-0.5.2/mly/datatools/tests/test_datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4975 2023-06-09 11:10:13.000000 mly-0.5.2/mly/datatools/tests/test_generator.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18633 2023-06-15 10:28:37.000000 mly-0.5.2/mly/exceptions.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.5.2/mly/mlTools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.5.2/mly/models.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    12353 2023-05-04 12:56:19.000000 mly-0.5.2/mly/null_energy_map.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7316 2023-06-09 11:13:40.000000 mly-0.5.2/mly/offlinefar.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-05-04 12:56:19.000000 mly-0.5.2/mly/plugins.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10153 2023-06-23 11:18:28.000000 mly-0.5.2/mly/projectwave.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.5.2/mly/simulateddetectornoise.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.494301 mly-0.5.2/mly/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.5.2/mly/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.5.2/mly/tests/test_init.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.5.2/mly/tests/test_tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13037 2023-06-30 12:02:21.000000 mly-0.5.2/mly/tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126803 2023-06-09 13:52:48.000000 mly-0.5.2/mly/validators.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-05-09 14:56:02.000000 mly-0.5.2/mly/waveforms.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.410300 mly-0.5.2/mly.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      497 2023-07-04 14:04:58.000000 mly-0.5.2/mly.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      733 2023-07-04 14:04:58.000000 mly-0.5.2/mly.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-04 14:04:58.000000 mly-0.5.2/mly.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       96 2023-07-04 14:04:58.000000 mly-0.5.2/mly.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-04 14:04:58.000000 mly-0.5.2/mly.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-07-04 14:04:58.497301 mly-0.5.2/setup.cfg
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      954 2023-07-04 12:47:36.000000 mly-0.5.2/setup.py
```

### Comparing `mly-0.3.4.5/LICENSE` & `mly-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/SRD.py` & `mly-0.5.2/mly/SRD.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/createFileSystem.py` & `mly-0.5.2/mly/createFileSystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # import copy
 # from math import ceil
 from dqsegdb2.query import query_segments
 from gwpy.io.kerberos import kinit
 
 from .simulateddetectornoise import *
 from .tools import dirlist,  fromCategorical, correlate,internalLags,circularTimeSlides
-from .datatools import DataPod, DataSet
+from .datatools import DataPod, DataSet, generator
 
 from .exceptions import *
 from gwpy.time import to_gps,from_gps
 from gwpy.segments import DataQualityFlag
 from gwpy.segments import Segment,SegmentList
 
 # from gwpy.io.kerberos import kinit
@@ -147,15 +147,16 @@
 
     dagman = Dagman(name='createFileSystemDagman',
             submit=submit)
     job_list=[]
 
     kwstr=""
     for k in kwargs:
-        kwstr+=(","+k+"="+str(kwargs[k]))       
+        if k not in ['accounting_group_user','accounting_group']:
+            kwstr+=(","+k+"="+str(kwargs[k]))       
         
     if backgroundType=='real':
         
         dates = check_dates(dates)
 
 
         segments = getSegments(duration = duration
@@ -184,33 +185,25 @@
             segmentFileName = str(int(segments[i][0]))+'-'+str(int(segments[i][1]))+'_'+str(size)
             
         elif backgroundType=='optimal':
             size = kwargs['maxSegmentSize']
             segmentFileName = 'optimalNoise-No'+str(i+1)+'_'+str(size)
             
         with open(masterDirectory+'script_'+segmentFileName+'.py','w') as f:
-            f.write('#! /usr/bin/env python3\n')
-            f.write('import sys \n')
+            f.write('#! /usr/bin/env python\n')
 
-            usr=os.getcwd().split('/')[2]
-            if os.path.exists('/home/'+usr+'/mly'):
-                f.write("sys.path.append('/home/"+usr+"/mly')\n")
-            else:
-                f.write("sys.path.append('/home/mly/mly/')\n")
-
-
-            f.write('from mly.datatools import DataPod, DataSet\n\n')
+            f.write('from mly.datatools import DataPod, DataSet, generator\n\n')
             
             f.write("import time\n\n")
             f.write("t0=time.time()\n")
             
 
             if backgroundType == 'optimal':
                 for det in detectors:
-                    comand=( "SET = DataSet.generator(\n"
+                    comand=( "SET = generator(\n"
                              +24*" "+"duration = "+str(duration)+"\n"
                              +24*" "+",fs = "+str(fs)+"\n"
                              +24*" "+",size = "+str(size)+"\n"
                              +24*" "+",detectors = '"+det+"'\n"
                              +24*" "+",labels = "+str(labels)+"\n"
                              +24*" "+",backgroundType = '"+str(backgroundType)+"'\n"
                              +24*" "+",windowSize ="+str(windowSize)+"\n"
@@ -219,15 +212,15 @@
             
                     f.write(comand+'\n\n')
                 f.write("print(time.time()-t0)\n")
 
             else:
                 #f.write("sys.path.append('"+date_list_path[:-1]+"')\n")
                 for det in detectors:
-                    comand=( "SET = DataSet.generator(\n"
+                    comand=( "SET = generator(\n"
                              +24*" "+"duration = "+str(duration)+"\n"
                              +24*" "+",fs = "+str(fs)+"\n"
                              +24*" "+",size = "+str(size)+"\n"
                              +24*" "+",detectors = '"+det+"'\n"
                              +24*" "+",labels = "+str(labels)+"\n"
                              +24*" "+",backgroundType = '"+str(backgroundType)+"'\n"
                              +24*" "+",noiseSourceFile = "+str([[segments[i][0],segments[i][1]]])+"\n"
```

### Comparing `mly-0.3.4.5/mly/datatools/core.py` & `mly-0.5.2/mly/datatools/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
                 newShape.insert(0,len(detectors))
                 ind = [list(self.strain.shape).index(i) for i in newShape]
                 self.strain = np.transpose(self.strain, ind)
                 print("Needed shape change of the strain occured")
                 self._detectors = detectors
             # ---> If not, an error occures.
             else:
-                raise IndexError("detectors must be as many as the strain")
+                raise IndexError(f"detectors ({len(detectors)}) must be as many as the strain inputs ({self.strain.shape[0]})")
 
     @property
     def gps(self):
         return self._gps  
     @gps.setter
     def gps(self,gps):
         # # GPS is optional or a list of positive numbers.
```

### Comparing `mly-0.3.4.5/mly/datatools/datatools.py` & `mly-0.5.2/mly/datatools/datatools.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/datatools/generator.py` & `mly-0.5.2/mly/datatools/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2088,18 +2088,26 @@
     if 'psd' in dataset[0].pluginDict and 'psd' not in kwargs['plugins']: kwargs['plugins'].append('psd')
     # if 'snr'+dataset[0].detectors[0] in dataset[0].pluginDict and 'snr' not in kwargs['plugins']: 
     #     kwargs['plugins'].append('snr')
     
 
     newSet=generator(**kwargs)
 
+
     for i in range(len(dataset)):
         dataset[i].strain=np.vstack((dataset[i].strain,newSet[i].strain))
-        dataset[i].detectors+=newSet[i].detectors
+
+        if isinstance(dataset[i].detectors,str):
+            dataset[i].detectors = list(dataset[i].detectors) + newSet[i].detectors
+        else:
+            dataset[i].detectors = dataset[i].detectors + newSet[i].detectors
+
+
         dataset[i].gps+=newSet[i].gps
+
         if 'psd' in kwargs['plugins']: dataset[i].psd+=newSet[i].psd
         # if 'snr' in kwargs['plugins']:
         #     for d in newSet[i].detectors:
         #         dataset[i].addPlugIn(newSet[i].pluginDict['snr'+d])        
         if 'correlation' in dataset[i].pluginDict:
             dataset[i].addPlugIn(dataset[i].pluginDict['correlation'])
```

### Comparing `mly-0.3.4.5/mly/datatools/tests/test_core.py` & `mly-0.5.2/mly/datatools/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/datatools/tests/test_generator.py` & `mly-0.5.2/mly/datatools/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/exceptions.py` & `mly-0.5.2/mly/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,19 @@
         raise ValueError('windowSize needs to be bigger than the duration')
     
     return windowSize
 
 def check_dates(dates):
     
     from gwpy.time import to_gps
-
-    gps_start = to_gps(dates[0])
-    gps_end = to_gps(dates[1])
+    # For the occation where a segment is passed
+    if len(dates)==1: dates=dates[0]
+    
+    gps_start = to_gps(dates[0]) if isinstance(dates[0],str) else dates[0]
+    gps_end = to_gps(dates[1]) if isinstance(dates[1],str) else dates[1]
     
     if gps_start > gps_end:
         raise ValueError("Not valid date.")
     else:
         return (gps_start, gps_end)
     
 def check_observingFlags(observingFlags=None, **kwargs):
```

### Comparing `mly-0.3.4.5/mly/mlTools.py` & `mly-0.5.2/mly/mlTools.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/models.py` & `mly-0.5.2/mly/models.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/null_energy_map.py` & `mly-0.5.2/mly/null_energy_map.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/offlinefar.py` & `mly-0.5.2/mly/offlinefar.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/plugins.py` & `mly-0.5.2/mly/plugins.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/projectwave.py` & `mly-0.5.2/mly/projectwave.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import random
 import numpy as np
 import matplotlib.pyplot as plt
 
 from pycbc.waveform import get_td_waveform
 from pycbc.waveform import get_fd_waveform
 from pycbc.detector import Detector
-from pycbc.types.timeseries import TimeSeries
+from pycbc.types.timeseries import TimeSeries as PTimeSeries
 
 
 def projectWave(sourceWaveform
                 ,detectors
                 ,fs
                 ,declination=None
                 ,rightAscension=None
@@ -47,17 +47,18 @@
             raise TypeError("File format is not supported")
             
     if outputFormat == None: 
         outputFormat='TXT'
     if isinstance(destinationFile,str) and destinationFile[-1]!="/":
         destinationFile=destinationFile+"/"
     
-    # Making the polarisation data into TimeSeries objects
-    hp=TimeSeries(h[0],delta_t=1./fs,epoch=time)         
-    hc=TimeSeries(h[1],delta_t=1./fs,epoch=time) 
+    # Making the polarisation data into PTimeSeries objects
+
+    hp=PTimeSeries(h[0],delta_t=1./fs,epoch=time)         
+    hc=PTimeSeries(h[1],delta_t=1./fs,epoch=time) 
     
     
     hrss=np.sqrt(np.sum(h[0]**2+h[1]**2)/fs)
     
     # Checking the detectors input
     if not all(d in ['H1','L1','V1'] for d in detectors):
         if all(d+'1' in ['H1','L1','V1'] for d in detectors):
```

### Comparing `mly-0.3.4.5/mly/simulateddetectornoise.py` & `mly-0.5.2/mly/simulateddetectornoise.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/tests/__init__.py` & `mly-0.5.2/mly/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/tests/test_init.py` & `mly-0.5.2/mly/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/tests/test_tools.py` & `mly-0.5.2/mly/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/tools.py` & `mly-0.5.2/mly/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import numpy as np
-import matplotlib.pyplot as plt
-from math import ceil 
-from gwpy.timeseries import TimeSeries
-from gwpy.io.kerberos import kinit
-from gwpy.segments import DataQualityFlag
-from gwpy.segments import Segment,SegmentList
-from gwpy.time import to_gps
-from gwpy.time import from_gps
-from dqsegdb2.query import query_segments
 import os
-import time
-import pandas as pd
+
+# import matplotlib.pyplot as plt
+# from math import ceil 
+# from gwpy.timeseries import TimeSeries
+# from gwpy.io.kerberos import kinit
+# from gwpy.segments import DataQualityFlag
+# from gwpy.segments import Segment,SegmentList
+# from gwpy.time import to_gps
+# from gwpy.time import from_gps
+# from dqsegdb2.query import query_segments
+# import time
+# import pandas as pd
 ################################################################################
 
 def dirlist(filename,exclude=None):   
     """
     Function that returns the a list of the files
     in a directory with options for exclutions.
```

### Comparing `mly-0.3.4.5/mly/validators.py` & `mly-0.5.2/mly/validators.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly/waveforms.py` & `mly-0.5.2/mly/waveforms.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/mly.egg-info/SOURCES.txt` & `mly-0.5.2/mly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.5/setup.py` & `mly-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mly",
-    version="0.3.4.5",
+    version="0.5.2",
     author="Vasileios Skliris",
     author_email='vas.skliris@gmail.com',
     description='This tool helps you create training and testing data for ML to use for gravitational wave detection.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://pypi.python.org/pypi/mly/',
     packages=setuptools.find_packages(),
```

