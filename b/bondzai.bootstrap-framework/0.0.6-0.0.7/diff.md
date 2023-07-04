# Comparing `tmp/bondzai.bootstrap-framework-0.0.6.tar.gz` & `tmp/bondzai.bootstrap-framework-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.bootstrap-framework-0.0.6.tar", last modified: Tue Jul  4 09:33:48 2023, max compression
+gzip compressed data, was "bondzai.bootstrap-framework-0.0.7.tar", last modified: Tue Jul  4 14:20:38 2023, max compression
```

## Comparing `bondzai.bootstrap-framework-0.0.6.tar` & `bondzai.bootstrap-framework-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:48.433927 bondzai.bootstrap-framework-0.0.6/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-04 09:33:48.434084 bondzai.bootstrap-framework-0.0.6/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      141 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:48.428964 bondzai.bootstrap-framework-0.0.6/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:48.431818 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/
--rw-r--r--   0 theo       (501) staff       (20)      212 2023-07-04 09:33:39.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     2696 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/bootstrap.py
--rw-r--r--   0 theo       (501) staff       (20)    10143 2023-07-04 09:33:39.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_agent.py
--rw-r--r--   0 theo       (501) staff       (20)    14052 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_com.py
--rw-r--r--   0 theo       (501) staff       (20)     7333 2023-07-04 09:33:39.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_config.py
--rw-r--r--   0 theo       (501) staff       (20)     2917 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/file_handler.py
--rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/logger.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:48.433613 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       52 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      755 2023-07-04 09:33:48.434684 bondzai.bootstrap-framework-0.0.6/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:20:38.286749 bondzai.bootstrap-framework-0.0.7/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-04 14:20:38.286858 bondzai.bootstrap-framework-0.0.7/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      141 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:20:38.281118 bondzai.bootstrap-framework-0.0.7/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:20:38.284081 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/
+-rw-r--r--   0 theo       (501) staff       (20)      212 2023-07-04 14:20:27.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     2696 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/bootstrap.py
+-rw-r--r--   0 theo       (501) staff       (20)    10143 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_agent.py
+-rw-r--r--   0 theo       (501) staff       (20)    14052 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_com.py
+-rw-r--r--   0 theo       (501) staff       (20)     7338 2023-07-04 14:20:27.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_config.py
+-rw-r--r--   0 theo       (501) staff       (20)     3008 2023-07-04 14:20:27.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/file_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/logger.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:20:38.286441 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       52 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 14:20:38.000000 bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-04 14:19:57.000000 bondzai.bootstrap-framework-0.0.7/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      755 2023-07-04 14:20:38.287533 bondzai.bootstrap-framework-0.0.7/setup.cfg
```

### Comparing `bondzai.bootstrap-framework-0.0.6/NOTICE` & `bondzai.bootstrap-framework-0.0.7/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.6/PKG-INFO` & `bondzai.bootstrap-framework-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.6
+Version: 0.0.7
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/bootstrap.py` & `bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_agent.py` & `bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_agent.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_com.py` & `bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_com.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_config.py` & `bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/dvs_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         return True
 
     def get_item_id(self, item_type: str, label_key: str):
         if not self.association_table:
             if not self.load_association_table():
                 return None
             
-        for (label_id, key) in self.association_table.get(item_type, {}):
+        for (label_id, key) in self.association_table.get(item_type, {}).items():
             if key == label_key:
                 return int(label_id)
         
         return None
     
     def get_targz_file_list(self, path: Path = None):
         if path is None:
@@ -181,18 +181,17 @@
         return my_tar
     
     def close_targz(self,my_tar):
         my_tar.__del__()
 
     def load_initial_dataset_definition_targz(self,my_tar,path : Path = None):
         # my_tar = Tar(path)
-        dataset = my_tar.read_yml("./dataset.yml")
+        dataset = my_tar.read_yml("dataset.yml")
         return dataset
 
-
     def load_data_from_dataset_targz(self,my_tar,path : Path = None):
         
         bindata = my_tar.read_binary(path)
 
         return bindata
 
     def set_max_nb_raw_data (self,max_nb_raw_data:int):
```

### Comparing `bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/file_handler.py` & `bondzai.bootstrap-framework-0.0.7/bondzai/bootstrap_framework/file_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,22 +76,23 @@
     def __del__(self):
         if self.tar:
             self.tar.close()
 
     def read_yml(self,filepath):
         if self.tar is None:
             raise Exception(f"impossible to read yml {filepath}, tar file not found")
- 
+
+        filepath = filepath.replace("./", "")
         f = self.get_file(filepath)
         data = yaml.safe_load(f)
 
         return data
     
     def read_binary(self,filepath): # "./output/id10883_train9.bin"
         if self.tar is None:
             raise Exception(f"impossible to read binary {filepath}, tar file not found")
-
+        filepath = filepath.replace("./", "")
         f = self.get_file(filepath)
         if f is None:
             raise Exception(f" file {filepath} not found")
         d = f.read()
         return handle_binary_file_data(d)
```

### Comparing `bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/PKG-INFO` & `bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.6
+Version: 0.0.7
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/SOURCES.txt` & `bondzai.bootstrap-framework-0.0.7/bondzai.bootstrap_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.6/setup.cfg` & `bondzai.bootstrap-framework-0.0.7/setup.cfg`

 * *Files identical despite different names*

