# Comparing `tmp/Digital_Farming_Solution-0.1.4.tar.gz` & `tmp/Digital_Farming_Solution-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digital_Farming_Solution-0.1.4.tar", last modified: Tue Jul  4 10:25:45 2023, max compression
+gzip compressed data, was "Digital_Farming_Solution-0.1.5.tar", last modified: Tue Jul  4 11:20:32 2023, max compression
```

## Comparing `Digital_Farming_Solution-0.1.4.tar` & `Digital_Farming_Solution-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 10:25:45.246243 Digital_Farming_Solution-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-07-04 10:25:45.163462 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution/
--rw-rw-rw-   0        0        0     8968 2023-07-04 10:19:08.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution/Select_options.py
--rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:25:45.234274 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/
--rw-rw-rw-   0        0        0      609 2023-07-04 10:25:44.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-04 10:25:44.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 10:25:44.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-04 10:25:44.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      609 2023-07-04 10:25:45.244247 Digital_Farming_Solution-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-04 10:25:45.247238 Digital_Farming_Solution-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      771 2023-07-04 10:18:05.000000 Digital_Farming_Solution-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:20:32.015136 Digital_Farming_Solution-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-07-04 11:20:31.752490 Digital_Farming_Solution-0.1.5/Digital_Farming_Solution/
+-rw-rw-rw-   0        0        0     9015 2023-07-04 11:20:16.000000 Digital_Farming_Solution-0.1.5/Digital_Farming_Solution/Select_options.py
+-rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.5/Digital_Farming_Solution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:20:31.897104 Digital_Farming_Solution-0.1.5/Digital_Farming_Solution.egg-info/
+-rw-rw-rw-   0        0        0      609 2023-07-04 11:20:30.000000 Digital_Farming_Solution-0.1.5/Digital_Farming_Solution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-04 11:20:31.000000 Digital_Farming_Solution-0.1.5/Digital_Farming_Solution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 11:20:30.000000 Digital_Farming_Solution-0.1.5/Digital_Farming_Solution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-04 11:20:30.000000 Digital_Farming_Solution-0.1.5/Digital_Farming_Solution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      609 2023-07-04 11:20:31.965268 Digital_Farming_Solution-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-04 11:20:32.017130 Digital_Farming_Solution-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-07-04 11:20:13.000000 Digital_Farming_Solution-0.1.5/setup.py
```

### Comparing `Digital_Farming_Solution-0.1.4/Digital_Farming_Solution/Select_options.py` & `Digital_Farming_Solution-0.1.5/Digital_Farming_Solution/Select_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,16 @@
     return df_final
 
 #############################################################################################################################################################################
 
 # Creating the function for Weather changes between the low and high yield
 
 def Weather_Change_With_Low_Vs_High_Yield(data,Yield_column,Weather_params):
+
+    data = Yield_Binning(data,Yield_column)
     
     data = data[(data[Yield_column] > 0)]
     
     Weather_params.insert(0,Yield_column)
     
     # This is  for Low Category
     df_low = data[data['Category'] == 'Low'].reset_index(drop=True)
@@ -119,17 +121,17 @@
     df_high = data[data['Category'] == 'High'].reset_index(drop=True)
     df_high = df_high[Weather_params]
 
     df_high_final = df_high.describe().T
     df_high_final = df_high_final[['min','max','mean']]
     
     # Concating the low and High  dataframe
-    df_high_wet = pd.concat([df_low_final,df_high_final],axis=1,keys=['Weather Range with Low Yield','Weather Range with High Yield'],names= ['Weather Parameter'])
+    df_low_high = pd.concat([df_low_final,df_high_final],axis=1,keys=['Weather Range with Low Yield','Weather Range with High Yield'],names= ['Weather Parameter'])
     
-    return df_high_wet
+    return df_low_high
 
 ####################################################################################################################################################################
 
 # Getting the delta change for palnting and Harvest dates
 def Delta_Change(data, Yield_cloumn, by, return_dataframe = True):
 
     # Storing the column Name
```

### Comparing `Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/PKG-INFO` & `Digital_Farming_Solution-0.1.5/Digital_Farming_Solution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital-Farming-Solution
-Version: 0.1.4
+Version: 0.1.5
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.4/PKG-INFO` & `Digital_Farming_Solution-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital_Farming_Solution
-Version: 0.1.4
+Version: 0.1.5
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.4/setup.py` & `Digital_Farming_Solution-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Digital_Farming_Solution",
-    version="0.1.4",
+    version="0.1.5",
     author="Bharatesha N S",
     author_email="bharatesha.ns.ext@bayer.com",
     description=" The packages are helps to the DFS Teams to perform some of the task easily.",
     long_description= 'By importing this packages we can work on easily and  get some meaningfull information.It is more siutable for the dataframe works and it will returnns the Dataframe.',
     long_description_content_type="text/markdown",
     packages=["Digital_Farming_Solution"],
     classifiers=[
```

