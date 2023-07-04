# Comparing `tmp/Signature_pywrapper-0.0.2.tar.gz` & `tmp/Signature_pywrapper-0.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signature_pywrapper-0.0.2.tar", last modified: Thu Jun 15 07:52:45 2023, max compression
+gzip compressed data, was "Signature_pywrapper-0.0.2.post1.tar", last modified: Tue Jul  4 17:37:57 2023, max compression
```

## Comparing `Signature_pywrapper-0.0.2.tar` & `Signature_pywrapper-0.0.2.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 07:52:45.493056 Signature_pywrapper-0.0.2/
--rw-rw-rw-   0        0        0     1100 2023-02-07 12:55:09.000000 Signature_pywrapper-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3398 2023-06-15 07:52:45.493056 Signature_pywrapper-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2461 2023-06-15 07:36:07.000000 Signature_pywrapper-0.0.2/README.md
--rw-rw-rw-   0        0        0     1344 2023-06-15 07:52:45.506122 Signature_pywrapper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-02-07 12:55:09.000000 Signature_pywrapper-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:52:45.412849 Signature_pywrapper-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 07:52:45.452895 Signature_pywrapper-0.0.2/src/Signature_pywrapper/
--rw-rw-rw-   0        0        0      143 2023-06-15 07:51:06.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/__init__.py
--rw-rw-rw-   0        0        0    58284 2020-01-22 14:10:16.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/commons-cli-1.5.0.jar
--rw-rw-rw-   0        0        0     2317 2023-06-02 12:59:46.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/eSignature.jar
--rw-rw-rw-   0        0        0     9449 2023-06-15 07:50:28.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/signature_wrapper.py
--rw-rw-rw-   0        0        0    97214 2023-06-02 08:29:00.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/signatures-1.2-SNAPSHOT.jar
--rw-rw-rw-   0        0        0     3448 2023-06-02 13:16:29.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:52:45.491056 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     3398 2023-06-15 07:52:45.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2023-06-15 07:52:45.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 07:52:45.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-06-15 07:52:45.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-15 07:52:45.000000 Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 17:37:57.876614 Signature_pywrapper-0.0.2.post1/
+-rw-rw-rw-   0        0        0     1100 2023-02-07 12:55:09.000000 Signature_pywrapper-0.0.2.post1/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-07-04 17:37:57.876614 Signature_pywrapper-0.0.2.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     2461 2023-06-15 07:36:07.000000 Signature_pywrapper-0.0.2.post1/README.md
+-rw-rw-rw-   0        0        0     1344 2023-07-04 17:37:57.876614 Signature_pywrapper-0.0.2.post1/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-02-07 12:55:09.000000 Signature_pywrapper-0.0.2.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:37:57.813687 Signature_pywrapper-0.0.2.post1/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 17:37:57.860981 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/
+-rw-rw-rw-   0        0        0      149 2023-07-04 17:37:23.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0    58284 2020-01-22 14:10:16.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/commons-cli-1.5.0.jar
+-rw-rw-rw-   0        0        0     2317 2023-06-02 12:59:46.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/eSignature.jar
+-rw-rw-rw-   0        0        0     9456 2023-07-02 16:01:52.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/signature_wrapper.py
+-rw-rw-rw-   0        0        0    97214 2023-06-02 08:29:00.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/signatures-1.2-SNAPSHOT.jar
+-rw-rw-rw-   0        0        0     3653 2023-07-04 17:33:26.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:37:57.876614 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-07-04 17:37:57.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-07-04 17:37:57.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 17:37:57.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-07-04 17:37:57.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-04 17:37:57.000000 Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper.egg-info/top_level.txt
```

### Comparing `Signature_pywrapper-0.0.2/LICENSE` & `Signature_pywrapper-0.0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.2/PKG-INFO` & `Signature_pywrapper-0.0.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signature_pywrapper
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: Python wrapper for signature molecular descriptors
 Home-page: https://github.com/OlivierBeq/Signature_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: signature molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

### Comparing `Signature_pywrapper-0.0.2/README.md` & `Signature_pywrapper-0.0.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.2/setup.cfg` & `Signature_pywrapper-0.0.2.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.2/src/Signature_pywrapper/commons-cli-1.5.0.jar` & `Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/commons-cli-1.5.0.jar`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.2/src/Signature_pywrapper/eSignature.jar` & `Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/eSignature.jar`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.2/src/Signature_pywrapper/signature_wrapper.py` & `Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/signature_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 DOI: 10.1021/ci0341823
 
 ###################################
 
 """)
 
     def _prepare_command(self, mols: List[Chem.Mol], depth: int) -> str:
-        """Create the ePaDEL command to be run to obtain molecular descriptors.
+        """Create the Signature command to be run to obtain molecular descriptors.
 
         :param mols: molecules to obtained molecular descriptors of
         :param depth: the depth of signatures to be computed
         :return: The command to run.
         """
         # 1) Ensure JRE is accessible
         with self.lock:
@@ -168,15 +168,15 @@
         values = pd.DataFrame(out)
         values.index.name = 'index'
         return values
 
     def _calculate(self, mols: List[Chem.Mol]) -> pd.DataFrame:
         """Calculate PaDEL descriptors on one process.
 
-        :param mols: RDkit molecules for which PaDEL descriptors should be calculated.
+        :param mols: RDkit molecules for which Signature descriptors should be calculated.
         :param depth: depth of each vertex's signature
         :return: a pandas DataFrame containing signature descriptor values and the path to the temp dir to be removed
         """
         results = []
         # Run command for each depth
         for i, depth in enumerate(self.depths):
             if i == 0:  # Avoid overwriting SD file
```

### Comparing `Signature_pywrapper-0.0.2/src/Signature_pywrapper/signatures-1.2-SNAPSHOT.jar` & `Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/signatures-1.2-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `Signature_pywrapper-0.0.2/src/Signature_pywrapper/utils.py` & `Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 def parse_numeric_to_null(value: str) -> Union[int, float]:
     """Parse a string representation of a number and return NaN."""
     return np.nan
 
 
 def install_jre(version: int = 11):
     """Install a Java Runtime Environment."""
-    path = get_jre_in_dir(_JRE_DIR)
+    path = get_jre_in_dir(_JRE_DIR, version)
     if len(path) == 0:
         # Could not find JRE, install it
         _ = _jre_install(version, jre=True)
-        path = get_jre_in_dir(_JRE_DIR)
+        path = get_jre_in_dir(_JRE_DIR, version)
     return path
 
 
 def make_temp_jre() -> Tuple[str, str]:
     """Copy the installed JRE to a temporary file.
 
     Allows multiprocessing capacities.
@@ -52,38 +52,41 @@
     # Make copy into dir
     shutil.copytree(install_path, os.path.join(outdir, 'jre'))
     # Find JRE in temp dir
     path = get_jre_in_dir(outdir)
     return outdir, path
 
 
-def get_jre_in_dir(dir: str):
+def get_jre_in_dir(dir: str, version: int = 11):
     """Recursively search the directory to find a JRE."""
-    path = glob.glob(os.path.join(dir, '**', 'server',
+    paths = glob.glob(os.path.join(dir, '**', 'server',
                                   'jvm.dll' if sys.platform == "win32" else 'libjvm.so'
                                   ), recursive=True)
+    path = [path for path in paths if f'jre-{version}' in path]
     if len(path):
         return path[0]
     return None
 
 
 def install_java(version: int = 11):
     """Install a Java Runtime Environment."""
-    path = get_java_in_dir(_JRE_DIR)
+    path = get_java_in_dir(_JRE_DIR, version)
     if path is None:
         # Could not find JRE, install it
         _ = _jre_install(version, jre=True)
-        path = get_java_in_dir(_JRE_DIR)
+        path = get_java_in_dir(_JRE_DIR, version)
     return path
 
-def get_java_in_dir(dir: str):
+
+def get_java_in_dir(dir: str, version: int):
     """Recursively search the directory to find a JRE."""
-    path = glob.glob(os.path.join(dir, '**', 'bin',
+    paths = glob.glob(os.path.join(dir, '**', 'bin',
                                   'java.exe' if sys.platform == "win32" else 'java'
                                   ), recursive=True)
+    path = [path for path in paths if f'jdk-{version}' in path]
     if len(path):
         return os.path.abspath(path[0])
     return None
 
 
 def mktempdir(suffix: str = None) -> str:
     """Return the path to a writeable temporary directory."""
@@ -93,14 +96,15 @@
 
 def mktempfile(suffix: str = None) -> str:
     """Return the path to a writeable temporary file."""
     file = tempfile.mkstemp(suffix=suffix)
     os.close(file[0])
     return file[1]
 
+
 def needsHs(mol: Chem.Mol) -> bool:
     """Return if the molecule lacks hydrogen atoms or not.
 
     :param mol: RDKit Molecule
     :return: True if the molecule lacks hydrogens.
     """
     for atom in mol.GetAtoms():
```

### Comparing `Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/PKG-INFO` & `Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signature-pywrapper
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: Python wrapper for signature molecular descriptors
 Home-page: https://github.com/OlivierBeq/Signature_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: signature molecular descriptors,cheminformatics,toxicoinformatics,QSAR
```

### Comparing `Signature_pywrapper-0.0.2/src/Signature_pywrapper.egg-info/SOURCES.txt` & `Signature_pywrapper-0.0.2.post1/src/Signature_pywrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

