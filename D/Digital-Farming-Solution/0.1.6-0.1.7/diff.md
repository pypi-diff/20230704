# Comparing `tmp/Digital_Farming_Solution-0.1.6.tar.gz` & `tmp/Digital_Farming_Solution-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digital_Farming_Solution-0.1.6.tar", last modified: Tue Jul  4 17:56:18 2023, max compression
+gzip compressed data, was "Digital_Farming_Solution-0.1.7.tar", last modified: Tue Jul  4 18:13:29 2023, max compression
```

## Comparing `Digital_Farming_Solution-0.1.6.tar` & `Digital_Farming_Solution-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 17:56:18.484777 Digital_Farming_Solution-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-07-04 17:56:18.331066 Digital_Farming_Solution-0.1.6/Digital_Farming_Solution/
--rw-rw-rw-   0        0        0     9099 2023-07-04 17:55:59.000000 Digital_Farming_Solution-0.1.6/Digital_Farming_Solution/Select_options.py
--rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.6/Digital_Farming_Solution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 17:56:18.443064 Digital_Farming_Solution-0.1.6/Digital_Farming_Solution.egg-info/
--rw-rw-rw-   0        0        0      609 2023-07-04 17:56:16.000000 Digital_Farming_Solution-0.1.6/Digital_Farming_Solution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-04 17:56:17.000000 Digital_Farming_Solution-0.1.6/Digital_Farming_Solution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 17:56:16.000000 Digital_Farming_Solution-0.1.6/Digital_Farming_Solution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-04 17:56:16.000000 Digital_Farming_Solution-0.1.6/Digital_Farming_Solution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      609 2023-07-04 17:56:18.473658 Digital_Farming_Solution-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-04 17:56:18.484777 Digital_Farming_Solution-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      771 2023-07-04 17:56:08.000000 Digital_Farming_Solution-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:13:29.615197 Digital_Farming_Solution-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-07-04 18:13:29.553251 Digital_Farming_Solution-0.1.7/Digital_Farming_Solution/
+-rw-rw-rw-   0        0        0     9185 2023-07-04 18:13:18.000000 Digital_Farming_Solution-0.1.7/Digital_Farming_Solution/Select_options.py
+-rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.7/Digital_Farming_Solution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:13:29.603495 Digital_Farming_Solution-0.1.7/Digital_Farming_Solution.egg-info/
+-rw-rw-rw-   0        0        0      609 2023-07-04 18:13:28.000000 Digital_Farming_Solution-0.1.7/Digital_Farming_Solution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-04 18:13:29.000000 Digital_Farming_Solution-0.1.7/Digital_Farming_Solution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 18:13:28.000000 Digital_Farming_Solution-0.1.7/Digital_Farming_Solution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-04 18:13:28.000000 Digital_Farming_Solution-0.1.7/Digital_Farming_Solution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      609 2023-07-04 18:13:29.612191 Digital_Farming_Solution-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-04 18:13:29.616735 Digital_Farming_Solution-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-07-04 18:13:13.000000 Digital_Farming_Solution-0.1.7/setup.py
```

### Comparing `Digital_Farming_Solution-0.1.6/Digital_Farming_Solution/Select_options.py` & `Digital_Farming_Solution-0.1.7/Digital_Farming_Solution/Select_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
 #################################################################
 
 # Creating the function for Yield binning Ranges Values
 def Yield_Binning_Ranges_Values(data,Yield_column_name):
     
     df_new = data[[Yield_column_name]]
+
+    #Removing low level outliers
+    df_new = df_new[(df_new[Yield_column_name] > 0)]
     
     #Removing the null values
     df_new.dropna(inplace=True)
     
     #Calculating the IQR
     col_values = list(df_new [Yield_column_name])
     
@@ -125,15 +128,15 @@
     df_high_final = df_high_final[['min','max','mean']]
     
     # Concating the low and High  dataframe
     df_low_high = pd.concat([df_low_final,df_high_final],axis=1,keys=['Weather Range with Low Yield','Weather Range with High Yield'],names= ['Weather Parameter'])
     
     # Droping the duplicate
     df_low_high = df_low_high.drop_duplicates()
-    
+
     return df_low_high
 
 ####################################################################################################################################################################
 
 # Getting the delta change for palnting and Harvest dates
 def Delta_Change(data, Yield_cloumn, by, return_dataframe = True):
```

### Comparing `Digital_Farming_Solution-0.1.6/Digital_Farming_Solution.egg-info/PKG-INFO` & `Digital_Farming_Solution-0.1.7/Digital_Farming_Solution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital-Farming-Solution
-Version: 0.1.6
+Version: 0.1.7
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.6/PKG-INFO` & `Digital_Farming_Solution-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital_Farming_Solution
-Version: 0.1.6
+Version: 0.1.7
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.6/setup.py` & `Digital_Farming_Solution-0.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Digital_Farming_Solution",
-    version="0.1.6",
+    version="0.1.7",
     author="Bharatesha N S",
     author_email="bharatesha.ns.ext@bayer.com",
     description=" The packages are helps to the DFS Teams to perform some of the task easily.",
     long_description= 'By importing this packages we can work on easily and  get some meaningfull information.It is more siutable for the dataframe works and it will returnns the Dataframe.',
     long_description_content_type="text/markdown",
     packages=["Digital_Farming_Solution"],
     classifiers=[
```

