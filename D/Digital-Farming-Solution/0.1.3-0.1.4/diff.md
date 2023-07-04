# Comparing `tmp/Digital_Farming_Solution-0.1.3.tar.gz` & `tmp/Digital_Farming_Solution-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digital_Farming_Solution-0.1.3.tar", last modified: Fri Jun 30 09:08:47 2023, max compression
+gzip compressed data, was "Digital_Farming_Solution-0.1.4.tar", last modified: Tue Jul  4 10:25:45 2023, max compression
```

## Comparing `Digital_Farming_Solution-0.1.3.tar` & `Digital_Farming_Solution-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 09:08:47.393730 Digital_Farming_Solution-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-06-30 09:08:47.207816 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution/
--rw-rw-rw-   0        0        0     7800 2023-06-30 09:08:01.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution/Select_options.py
--rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:08:47.383755 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/
--rw-rw-rw-   0        0        0      609 2023-06-30 09:08:45.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-30 09:08:46.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 09:08:45.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-30 09:08:45.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      609 2023-06-30 09:08:47.391739 Digital_Farming_Solution-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-30 09:08:47.394727 Digital_Farming_Solution-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      771 2023-06-27 12:08:01.000000 Digital_Farming_Solution-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:25:45.246243 Digital_Farming_Solution-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-07-04 10:25:45.163462 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution/
+-rw-rw-rw-   0        0        0     8968 2023-07-04 10:19:08.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution/Select_options.py
+-rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:25:45.234274 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/
+-rw-rw-rw-   0        0        0      609 2023-07-04 10:25:44.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-04 10:25:44.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 10:25:44.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-04 10:25:44.000000 Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      609 2023-07-04 10:25:45.244247 Digital_Farming_Solution-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-04 10:25:45.247238 Digital_Farming_Solution-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-07-04 10:18:05.000000 Digital_Farming_Solution-0.1.4/setup.py
```

### Comparing `Digital_Farming_Solution-0.1.3/Digital_Farming_Solution/Select_options.py` & `Digital_Farming_Solution-0.1.4/Digital_Farming_Solution/Select_options.py`

 * *Files 23% similar despite different names*

```diff
@@ -96,14 +96,43 @@
     df_final = df_new.groupby(['% of Yield Range','Yeild Category']).agg(min=(Yield_column_name, 'min'),max=(Yield_column_name, 'max'), mean=(Yield_column_name, 'mean'),
                                                                          median=(Yield_column_name, 'median')).sort_values('mean')
     
     return df_final
 
 #############################################################################################################################################################################
 
+# Creating the function for Weather changes between the low and high yield
+
+def Weather_Change_With_Low_Vs_High_Yield(data,Yield_column,Weather_params):
+    
+    data = data[(data[Yield_column] > 0)]
+    
+    Weather_params.insert(0,Yield_column)
+    
+    # This is  for Low Category
+    df_low = data[data['Category'] == 'Low'].reset_index(drop=True)
+    df_low = df_low[Weather_params]
+    
+    df_low_final = df_low.describe().T
+    df_low_final = df_low_final[['min','max','mean']]
+
+    ## This is  for High category
+    df_high = data[data['Category'] == 'High'].reset_index(drop=True)
+    df_high = df_high[Weather_params]
+
+    df_high_final = df_high.describe().T
+    df_high_final = df_high_final[['min','max','mean']]
+    
+    # Concating the low and High  dataframe
+    df_high_wet = pd.concat([df_low_final,df_high_final],axis=1,keys=['Weather Range with Low Yield','Weather Range with High Yield'],names= ['Weather Parameter'])
+    
+    return df_high_wet
+
+####################################################################################################################################################################
+
 # Getting the delta change for palnting and Harvest dates
 def Delta_Change(data, Yield_cloumn, by, return_dataframe = True):
 
     # Storing the column Name
     column_name = by
     # Converting the string data type  into datetime format
 
@@ -159,15 +188,15 @@
         # Calculating the best planting dates
         data = data.groupby([column_name,'season']).agg(Avg_yield=(Yield_cloumn, 'mean')).reset_index()
         
         # strftime --> b for month (jan,feb) and d for day of the date
         data['Month_Date'] = data[column_name].apply(lambda x: x.strftime('%b-%d'))
 
         # Convert the 'dates' column to datetime format with a fake year
-        data['Month_Date'] = pd.to_datetime('2022-' + data['Month_Date'], format='%Y-%b-%d')
+        data['Month_Date'] = pd.to_datetime('2020-' + data['Month_Date'], format='%Y-%b-%d')
 
         # Sort the DataFrame by the 'dates' column
         data = data.sort_values(by='Month_Date').reset_index(drop=True)
 
         # Remove the fake year from the 'dates' column
         data['Month_Date'] = data['Month_Date'].dt.strftime('%b-%d')
 
@@ -188,15 +217,15 @@
         # Calculating the best planting dates
         data = data.groupby([column_name]).agg(Avg_yield=(Yield_cloumn, 'mean')).reset_index()
         
         # strftime --> b for month (jan,feb) and d for day of the date
         data['Month_Date'] = data[column_name].apply(lambda x: x.strftime('%b-%d'))
 
         # Convert the 'dates' column to datetime format with a fake year
-        data['Month_Date'] = pd.to_datetime('2022-' + data['Month_Date'], format='%Y-%b-%d')
+        data['Month_Date'] = pd.to_datetime('2020-' + data['Month_Date'], format='%Y-%b-%d')
 
         # Sort the DataFrame by the 'dates' column
         data = data.sort_values(by='Month_Date').reset_index(drop=True)
 
         # Remove the fake year from the 'dates' column
         data['Month_Date'] = data['Month_Date'].dt.strftime('%b-%d')
 
@@ -211,7 +240,9 @@
             fig = px.bar(data, x= 'Month_Date', y='Avg_yield')
             fig.update_layout(title = 'Best ' + column_name +' in the Season', yaxis_title = 'Average Yield') 
             fig.show()
         
 
 ################################################################################################################
 
+
+
```

### Comparing `Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/PKG-INFO` & `Digital_Farming_Solution-0.1.4/Digital_Farming_Solution.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital-Farming-Solution
-Version: 0.1.3
+Version: 0.1.4
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.3/PKG-INFO` & `Digital_Farming_Solution-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital_Farming_Solution
-Version: 0.1.3
+Version: 0.1.4
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.3/setup.py` & `Digital_Farming_Solution-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Digital_Farming_Solution",
-    version="0.1.3",
+    version="0.1.4",
     author="Bharatesha N S",
     author_email="bharatesha.ns.ext@bayer.com",
     description=" The packages are helps to the DFS Teams to perform some of the task easily.",
     long_description= 'By importing this packages we can work on easily and  get some meaningfull information.It is more siutable for the dataframe works and it will returnns the Dataframe.',
     long_description_content_type="text/markdown",
     packages=["Digital_Farming_Solution"],
     classifiers=[
```

