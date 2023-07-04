# Comparing `tmp/similarity_check-0.2.0.tar.gz` & `tmp/similarity_check-0.2.1.tar.gz`

## Comparing `similarity_check-0.2.0.tar` & `similarity_check-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 similarity_check-0.2.0/setup.cfg
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 similarity_check-0.2.0/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.2.0/src/similarity_check/__init__.py
--rw-r--r--   0        0        0    23682 2020-02-02 00:00:00.000000 similarity_check-0.2.0/src/similarity_check/checkers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.2.0/LICENSE
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 similarity_check-0.2.0/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 similarity_check-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 similarity_check-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 similarity_check-0.2.1/setup.cfg
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 similarity_check-0.2.1/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.2.1/src/similarity_check/__init__.py
+-rw-r--r--   0        0        0    23694 2020-02-02 00:00:00.000000 similarity_check-0.2.1/src/similarity_check/checkers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 similarity_check-0.2.1/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 similarity_check-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 similarity_check-0.2.1/PKG-INFO
```

### Comparing `similarity_check-0.2.0/setup.cfg` & `similarity_check-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 696d 696c 6172 6974 795f 6368   = similarity_ch
 00000020: 6563 6b0d 0a64 6573 6372 6970 7469 6f6e  eck..description
 00000030: 203d 2070 6163 6b61 6765 2066 6f72 206d   = package for m
 00000040: 6561 7375 7269 6e67 2074 6865 2073 696d  easuring the sim
 00000050: 696c 6172 6974 7920 6f66 2074 776f 2074  ilarity of two t
 00000060: 6578 7473 0d0a 7665 7273 696f 6e20 3d20  exts..version = 
-00000070: 302e 322e 300d 0a6c 6f6e 675f 6465 7363  0.2.0..long_desc
+00000070: 302e 322e 310d 0a6c 6f6e 675f 6465 7363  0.2.1..long_desc
 00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 000000a0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 000000b0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
 000000c0: 6d61 726b 646f 776e 0d0a 6175 7468 6f72  markdown..author
 000000d0: 203d 206d 6573 6861 7269 0d0a 6175 7468   = meshari..auth
 000000e0: 6f72 5f65 6d61 696c 203d 206d 6573 6861  or_email = mesha
```

### Comparing `similarity_check-0.2.0/src/similarity_check/checkers.py` & `similarity_check-0.2.1/src/similarity_check/checkers.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
 
             overall_weight = 0.0
             for _, source_col, weight in source_mapping:
                 if source_col not in source.columns:
                     msg = f'the following source_col ({source_col}) not found in source DataFrame cloumns'
                     raise KeyError(msg)
                 else:
-                    source.loc[:, source_col] = source.fillna('')
+                    source.loc[:, source_col] = source[source_col].fillna('')
                 overall_weight += weight
                 
             if overall_weight != 1.0:
                 msg = f'the sum of the provided weights must equal 1.0, the provided weights sum is: {overall_weight}'
                 raise ValueError(msg)
             
             self.source_df = source.reset_index(drop=True)
```

### Comparing `similarity_check-0.2.0/README.md` & `similarity_check-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `similarity_check-0.2.0/pyproject.toml` & `similarity_check-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "similarity_check"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="meshari", email="meshari34343@gmail.com" },
 ]
 description = "package for measuring the similarity of two texts"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `similarity_check-0.2.0/PKG-INFO` & `similarity_check-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity_check
-Version: 0.2.0
+Version: 0.2.1
 Summary: package for measuring the similarity of two texts
 Author-email: meshari <meshari34343@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

