# Comparing `tmp/bondzai.bootstrap-framework-0.0.5.tar.gz` & `tmp/bondzai.bootstrap-framework-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.bootstrap-framework-0.0.5.tar", last modified: Thu Jun 22 17:12:20 2023, max compression
+gzip compressed data, was "bondzai.bootstrap-framework-0.0.6.tar", last modified: Tue Jul  4 09:33:48 2023, max compression
```

## Comparing `bondzai.bootstrap-framework-0.0.5.tar` & `bondzai.bootstrap-framework-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 17:12:20.332677 bondzai.bootstrap-framework-0.0.5/
--rwxrwxrwx   0 root         (0) root         (0)      547 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/NOTICE
--rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-22 17:12:20.333677 bondzai.bootstrap-framework-0.0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      141 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 17:12:19.815136 bondzai.bootstrap-framework-0.0.5/bondzai/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 17:12:20.122915 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/
--rwxrwxrwx   0 root         (0) root         (0)      212 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2696 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/bootstrap.py
--rwxrwxrwx   0 root         (0) root         (0)     9165 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_agent.py
--rwxrwxrwx   0 root         (0) root         (0)    14052 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_com.py
--rwxrwxrwx   0 root         (0) root         (0)     6101 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_config.py
--rwxrwxrwx   0 root         (0) root         (0)     2917 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/file_handler.py
--rwxrwxrwx   0 root         (0) root         (0)      333 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/logger.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 17:12:20.306936 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      700 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-22 17:12:19.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-22 17:12:18.000000 bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-06-22 17:11:07.000000 bondzai.bootstrap-framework-0.0.5/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      755 2023-06-22 17:12:20.337189 bondzai.bootstrap-framework-0.0.5/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:48.433927 bondzai.bootstrap-framework-0.0.6/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-04 09:33:48.434084 bondzai.bootstrap-framework-0.0.6/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      141 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:48.428964 bondzai.bootstrap-framework-0.0.6/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:48.431818 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/
+-rw-r--r--   0 theo       (501) staff       (20)      212 2023-07-04 09:33:39.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     2696 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/bootstrap.py
+-rw-r--r--   0 theo       (501) staff       (20)    10143 2023-07-04 09:33:39.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_agent.py
+-rw-r--r--   0 theo       (501) staff       (20)    14052 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_com.py
+-rw-r--r--   0 theo       (501) staff       (20)     7333 2023-07-04 09:33:39.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_config.py
+-rw-r--r--   0 theo       (501) staff       (20)     2917 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/file_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/logger.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:48.433613 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       52 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:33:48.000000 bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-04 09:32:32.000000 bondzai.bootstrap-framework-0.0.6/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      755 2023-07-04 09:33:48.434684 bondzai.bootstrap-framework-0.0.6/setup.cfg
```

### Comparing `bondzai.bootstrap-framework-0.0.5/NOTICE` & `bondzai.bootstrap-framework-0.0.6/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.5/PKG-INFO` & `bondzai.bootstrap-framework-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.5
+Version: 0.0.6
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/bootstrap.py` & `bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_agent.py` & `bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,66 +131,76 @@
     def load_initial_data(self):
         """
         Load all data from a given dataset
         Args:
         """
         dataset_definition = None
 
-        my_tar = self.config.preload_targz()
-        if my_tar.tar:
-            dataset_definition = self.config.load_initial_dataset_definition_targz(my_tar)
-
         ack = 0
-        if dataset_definition:
-            outputs_definition = dataset_definition["outputs"]
-            dataset = dataset_definition["dataset"]
-
-            for my_data in dataset:
-                filename = my_data["data"]
-                output = my_data["output"]
-
-                is_classification = True
-                if "source_id" in my_data:
-                    sourceid = my_data["source_id"]
-                else: 
-                    # sourceid = 1
-                    raise Exception(f"issue during loading file {filename}, no source")
-
-                groundthruth_for_davinsy = []
-                for labeltype in output:
-                    label_type_id = outputs_definition[labeltype]["id"]
-                    label_value = output[labeltype]
-
-                    # manage regression here
-                    if "labels" in outputs_definition[labeltype]:
-                        label_value_id = outputs_definition[labeltype]["labels"][label_value]
+        dataset_list = self.config.get_targz_file_list()
+        for dataset_tar_path in dataset_list:
+            my_tar = self.config.preload_targz(dataset_tar_path)
+            if my_tar.tar:
+                dataset_definition = self.config.load_initial_dataset_definition_targz(my_tar)
+
+                if dataset_definition:
+                    outputs_definition = dataset_definition["outputs"]
+                    dataset = dataset_definition["dataset"]
+
+                    for my_data in dataset:
+                        filename = my_data["data"]
+                        output = my_data["output"]
+
+                        is_classification = True
+                        if "source_id" in my_data:
+                            sourceid = self.config.get_item_id("sources", my_data["source_id"])
+                            if not sourceid:
+                                sourceid = my_data["source_id"]
+                        else: 
+                            # sourceid = 1
+                            raise Exception(f"issue during loading file {filename}, no source")
+
+                        groundthruth_for_davinsy = []
+                        for labeltype in output:
+                            label_type_id = self.config.get_item_id("labels", labeltype)
+                            if not label_type_id:
+                                label_type_id = outputs_definition[labeltype].get("id", None)
+                            label_value = output[labeltype]
+
+                            # manage regression here
+                            if "labels" in outputs_definition[labeltype]:
+                                label_value_id = outputs_definition[labeltype]["labels"].get(label_value, None)
+
+                                if label_value_id is None:
+                                    raise Exception(f"Unable to find label value id for {label_value}")
+                                
+                                groundthruth_for_davinsy.append(label_type_id)
+                                groundthruth_for_davinsy.append(label_value_id)
+                            else:
+                                # only one vector supported for regression
+                                groundthruth_for_davinsy = label_value
+                                is_classification = False
                         
-                        groundthruth_for_davinsy.append(label_type_id)
-                        groundthruth_for_davinsy.append(label_value_id)
-                    else:
-                        # only one vector supported for regression
-                        groundthruth_for_davinsy = label_value
-                        is_classification = False
-                
-                # raw_input = self.config.load_data_from_dataset(filename)
-                raw_input = self.config.load_data_from_dataset_targz(my_tar,filename)
-
-
-                if raw_input is None:
-                    raise Exception(f"issue during loading file {filename}")
-
-                logger.debug(f"loading file {filename}, GT {groundthruth_for_davinsy}")
-                sigVect = self.compute_raw_data(sourceid,data=raw_input)
-                if len(sigVect) < 1:
-                    raise Exception(f"Unable to process data len  {str(len(raw_input))}")
-
-                isLoaded = self.load_one_raw_data(is_classification,inputVect=sigVect, expectedOutput=groundthruth_for_davinsy)
-                ack += int(isLoaded)                
-        else:
-            logger.debug(" NO INITIAL DATASET")
+                        # raw_input = self.config.load_data_from_dataset(filename)
+                        raw_input = self.config.load_data_from_dataset_targz(my_tar,filename)
+
+                        if raw_input is None:
+                            raise Exception(f"issue during loading file {filename}")
+
+                        logger.debug(f"loading file {filename}, GT {groundthruth_for_davinsy}")
+                        sigVect = self.compute_raw_data(sourceid,data=raw_input)
+                        if len(sigVect) < 1:
+                            raise Exception(f"Unable to process data len  {str(len(raw_input))}")
+
+                        isLoaded = self.load_one_raw_data(is_classification,inputVect=sigVect, expectedOutput=groundthruth_for_davinsy)
+                        ack += int(isLoaded)                
+                else:
+                    logger.debug("INITIAL DATASET HAVE NO DEFINITION")
+
+                self.config.close_targz(my_tar)
         return ack
     
 
     def compute_raw_data(self, sourceid,data: np.ndarray) -> list:
         """
         Compute signature for a given vector
         Args:
```

### Comparing `bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_com.py` & `bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_com.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/dvs_config.py` & `bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/dvs_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import yaml
+import json
 from pathlib import Path
 
 from bondzai.davinsy_py.model import VirtualModel
 from bondzai.davinsy_py.operations import OperationRegistry
 from bondzai.davinsy_py.model import PreprocPhase
 
 from .file_handler import Tar, handle_binary_file_data
@@ -30,14 +31,16 @@
         self.rootPath = path       
 
         self.registry = OperationRegistry()
 
         self.vm = []
         self.nb_vm = 0
 
+        self.association_table = None
+
         self.max_raw_data = 0
         self.max_input_data = 0
         self.bootstrap_info = {}
         self.max_models = 0
         self.max_labels = 0
         self.max_reg_len = 0
         self.max_nb_raw_data = 3000
@@ -130,28 +133,63 @@
         
         with open(path, "rb") as f:
             if f is None:
                 raise Exception(f" file {path} not found")
             data = f.read()
         
         return handle_binary_file_data(data)
+    
+    def load_association_table(self, path: Path = None):
+        if path is None:
+            path = self.rootPath.parent / "config" / "lookup_table.json"
 
+        if not path.exists():
+            return 
+
+        if self.association_table is None:
+            self.association_table = {}
+
+        try:
+            table = {}
+            with open(path, "r") as fp:
+                table = json.load(fp)
+            self.association_table.update(table)
+        except Exception as e:
+            raise Exception(f"Unable to load association table {path} : {str(e)}")
+        
+        return True
+
+    def get_item_id(self, item_type: str, label_key: str):
+        if not self.association_table:
+            if not self.load_association_table():
+                return None
+            
+        for (label_id, key) in self.association_table.get(item_type, {}):
+            if key == label_key:
+                return int(label_id)
+        
+        return None
+    
+    def get_targz_file_list(self, path: Path = None):
+        if path is None:
+            path = self.rootPath / "datasets"
+        return [item for item in path.rglob("*.tar.gz") if item.is_file()]
 
-    def preload_targz(self,path : Path = None):
+    def preload_targz(self, path : Path = None):
         if path is None:
-            path = self.rootPath / "dataset.tar.gz"
+            path = self.rootPath / "datasets" / "dataset.tar.gz"
         my_tar = Tar(path)
         return my_tar
     
     def close_targz(self,my_tar):
         my_tar.__del__()
 
     def load_initial_dataset_definition_targz(self,my_tar,path : Path = None):
         # my_tar = Tar(path)
-        dataset = my_tar.read_yml("./myDataset.yml")
+        dataset = my_tar.read_yml("./dataset.yml")
         return dataset
 
 
     def load_data_from_dataset_targz(self,my_tar,path : Path = None):
         
         bindata = my_tar.read_binary(path)
```

### Comparing `bondzai.bootstrap-framework-0.0.5/bondzai/bootstrap_framework/file_handler.py` & `bondzai.bootstrap-framework-0.0.6/bondzai/bootstrap_framework/file_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/PKG-INFO` & `bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.5
+Version: 0.0.6
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.5/bondzai.bootstrap_framework.egg-info/SOURCES.txt` & `bondzai.bootstrap-framework-0.0.6/bondzai.bootstrap_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.5/setup.cfg` & `bondzai.bootstrap-framework-0.0.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 package_dir = 
 	= .
 zip_safe = True
 include_package_data = True
 namespace_packages = 
 	bondzai
 install_requires = 
-	bondzai.davinsy-py==0.0.3
+	bondzai.davinsy-py==0.0.4
 	numpy==1.24.3
 	pyyaml==6.0
 
 [options.packages.find]
 where = .
 
 [egg_info]
```

