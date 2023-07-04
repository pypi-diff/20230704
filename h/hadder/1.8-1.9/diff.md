# Comparing `tmp/hadder-1.8.tar.gz` & `tmp/hadder-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hadder-1.8.tar", last modified: Wed Jun 28 07:08:28 2023, max compression
+gzip compressed data, was "hadder-1.9.tar", last modified: Tue Jul  4 01:45:18 2023, max compression
```

## Comparing `hadder-1.8.tar` & `hadder-1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-28 07:08:28.886664 hadder-1.8/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)    11357 2023-06-27 09:36:35.000000 hadder-1.8/LICENSE
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     3199 2023-06-28 07:08:28.886664 hadder-1.8/PKG-INFO
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     2901 2023-06-27 09:36:35.000000 hadder-1.8/README.md
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-28 07:08:28.886664 hadder-1.8/hadder/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     8549 2023-06-27 09:36:35.000000 hadder-1.8/hadder/__init__.py
--rw-rw-r--   0 dechin    (1001) dechin    (1001)      893 2023-06-27 09:36:35.000000 hadder-1.8/hadder/__main__.py
--rw-rw-r--   0 dechin    (1001) dechin    (1001)    40338 2023-06-27 09:36:35.000000 hadder-1.8/hadder/constants.py
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     6476 2023-06-28 07:07:08.000000 hadder-1.8/hadder/parsers.py
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-28 07:08:28.886664 hadder-1.8/hadder.egg-info/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     3199 2023-06-28 07:08:28.000000 hadder-1.8/hadder.egg-info/PKG-INFO
--rw-rw-r--   0 dechin    (1001) dechin    (1001)      251 2023-06-28 07:08:28.000000 hadder-1.8/hadder.egg-info/SOURCES.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        1 2023-06-28 07:08:28.000000 hadder-1.8/hadder.egg-info/dependency_links.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)       20 2023-06-28 07:08:28.000000 hadder-1.8/hadder.egg-info/requires.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        7 2023-06-28 07:08:28.000000 hadder-1.8/hadder.egg-info/top_level.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)       38 2023-06-28 07:08:28.890664 hadder-1.8/setup.cfg
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     1488 2023-06-28 07:07:50.000000 hadder-1.8/setup.py
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-07-04 01:45:18.299478 hadder-1.9/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)    11357 2023-06-27 09:36:35.000000 hadder-1.9/LICENSE
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     3199 2023-07-04 01:45:18.299478 hadder-1.9/PKG-INFO
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     2901 2023-06-27 09:36:35.000000 hadder-1.9/README.md
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-07-04 01:45:18.295478 hadder-1.9/hadder/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     8549 2023-06-27 09:36:35.000000 hadder-1.9/hadder/__init__.py
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)      893 2023-06-27 09:36:35.000000 hadder-1.9/hadder/__main__.py
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)    40338 2023-06-27 09:36:35.000000 hadder-1.9/hadder/constants.py
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     6059 2023-07-04 01:44:26.000000 hadder-1.9/hadder/parsers.py
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-07-04 01:45:18.299478 hadder-1.9/hadder.egg-info/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     3199 2023-07-04 01:45:18.000000 hadder-1.9/hadder.egg-info/PKG-INFO
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)      251 2023-07-04 01:45:18.000000 hadder-1.9/hadder.egg-info/SOURCES.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)        1 2023-07-04 01:45:18.000000 hadder-1.9/hadder.egg-info/dependency_links.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)       20 2023-07-04 01:45:18.000000 hadder-1.9/hadder.egg-info/requires.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)        7 2023-07-04 01:45:18.000000 hadder-1.9/hadder.egg-info/top_level.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)       38 2023-07-04 01:45:18.299478 hadder-1.9/setup.cfg
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     1488 2023-07-04 01:44:41.000000 hadder-1.9/setup.py
```

### Comparing `hadder-1.8/LICENSE` & `hadder-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hadder-1.8/PKG-INFO` & `hadder-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hadder
-Version: 1.8
+Version: 1.9
 Summary: Hydrogen adder for pdb protein files
 Home-page: https://gitee.com/dechin/hadder
 Author: Dechin CHEN
 Author-email: dechin.phy@gmail.com
 License: Apache 2.0 Licence
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `hadder-1.8/README.md` & `hadder-1.9/README.md`

 * *Files identical despite different names*

### Comparing `hadder-1.8/hadder/__init__.py` & `hadder-1.9/hadder/__init__.py`

 * *Files identical despite different names*

### Comparing `hadder-1.8/hadder/__main__.py` & `hadder-1.9/hadder/__main__.py`

 * *Files identical despite different names*

### Comparing `hadder-1.8/hadder/constants.py` & `hadder-1.9/hadder/constants.py`

 * *Files identical despite different names*

### Comparing `hadder-1.8/hadder/parsers.py` & `hadder-1.9/hadder/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,22 +45,18 @@
     init_res_names = []
     init_res_ids = []
     crds = []
     crd_group = []
     res_pointer = []
     flatten_atoms = []
     flatten_crds = []
-    atom14_positions = []
-    atom14_atom_exists = []
-    residx_atom14_to_atom37 = []
     for index, line in enumerate(lines):
         if 'END' in line or 'TER' in line:
             atom_names.append(atom_group)
             crds.append(crd_group)
-            atom14_positions.append(atom_pos)
             break
         if not line.startswith('ATOM'):
             continue
         atom_name = line[12:16].strip()
         if ignoreh and atom_name.startswith('H'):
             continue
         res_name = line[17:20].strip()
@@ -77,15 +73,14 @@
             res_ids.append(res_id)
             res_names.append(res_name)
             atom_group.append(atom_name)
             crd_group.append(crd)
             res_pointer.append(0)
             atom_pos = np.zeros((14, 3))
         elif res_id != res_ids[-1]:
-            atom14_positions.append(atom_pos)
             atom_pos = np.zeros((14, 3))
             atom_names.append(atom_group)
             crds.append(crd_group)
             atom_group = []
             crd_group = []
             res_ids.append(res_id)
             res_names.append(res_name)
@@ -94,15 +89,14 @@
             res_pointer.append(pointer)
         else:
             atom_group.append(atom_name)
             crd_group.append(crd)
         if index == len(lines) - 1:
             atom_names.append(atom_group)
             crds.append(crd_group)
-            atom14_positions.append(atom_pos)
     atom_names = atom_names
     res_names = res_names
     res_ids = np.array(res_ids, np.int32)
     crds = crds
     flatten_atoms = np.array(flatten_atoms, np.str_)
     flatten_crds = np.array(flatten_crds, np.float32)
     init_res_names = np.array(init_res_names)
@@ -116,20 +110,17 @@
             aatype[i] = resdict['HIS']
         elif res_names[i] == 'GLH':
             aatype[i] = resdict['GLY']
         elif res_names[i] == 'ASH':
             aatype[i] = resdict['ASP']
         else:
             aatype[i] = resdict[res_names[i]]
-    atom14_atom_exists = np.array(atom14_atom_exists, np.float32)
-
-    atom14_positions = np.array(atom14_positions, np.float32)
 
     return atom_names, res_names, res_ids, crds, res_pointer, flatten_atoms, flatten_crds, init_res_names, init_res_ids,\
-        residue_index, aatype, atom14_positions, atom14_atom_exists, residx_atom14_to_atom37
+        residue_index, aatype
 
 
 def gen_pdb(crd, atom_names, res_names, res_ids, pdb_name='temp.pdb'):
     """Write protein crd information into pdb format files.
     Args:
         crd(numpy.float32): The coordinates of protein atoms.
         atom_names(numpy.str_): The atom names differ from aminos.
```

### Comparing `hadder-1.8/hadder.egg-info/PKG-INFO` & `hadder-1.9/hadder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hadder
-Version: 1.8
+Version: 1.9
 Summary: Hydrogen adder for pdb protein files
 Home-page: https://gitee.com/dechin/hadder
 Author: Dechin CHEN
 Author-email: dechin.phy@gmail.com
 License: Apache 2.0 Licence
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `hadder-1.8/setup.py` & `hadder-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="hadder",
-    version="1.8",
+    version="1.9",
     description="Hydrogen adder for pdb protein files",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="Apache 2.0 Licence",
 
     url="https://gitee.com/dechin/hadder",
     author="Dechin CHEN",
```

