# Comparing `tmp/tllab_common-2023.6.1.tar.gz` & `tmp/tllab_common-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2023.6.1.tar", max compression
+gzip compressed data, was "tllab_common-2023.7.0.tar", max compression
```

## Comparing `tllab_common-2023.6.1.tar` & `tllab_common-2023.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.6.1/LICENSE
--rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.6.1/README.md
--rw-r--r--   0        0        0      890 2023-06-01 13:22:00.111940 tllab_common-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.6.1/tllab_common/__init__.py
--rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.6.1/tllab_common/findcells.py
--rw-r--r--   0        0        0     6333 2023-06-01 13:22:00.139940 tllab_common-2023.6.1/tllab_common/fit.py
--rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.6.1/tllab_common/misc.py
--rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.6.1/tllab_common/transform.txt
--rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.6.1/tllab_common/transforms.py
--rwxr-xr-x   0        0        0    69943 2023-05-16 13:02:07.073494 tllab_common-2023.6.1/tllab_common/wimread.py
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.7.0/LICENSE
+-rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.7.0/README.md
+-rw-r--r--   0        0        0      890 2023-07-04 13:05:29.543945 tllab_common-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.7.0/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.7.0/tllab_common/findcells.py
+-rw-r--r--   0        0        0     6333 2023-06-01 13:22:00.139940 tllab_common-2023.7.0/tllab_common/fit.py
+-rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.7.0/tllab_common/misc.py
+-rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.7.0/tllab_common/transform.txt
+-rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.7.0/tllab_common/transforms.py
+-rwxr-xr-x   0        0        0    70080 2023-07-04 13:03:46.359987 tllab_common-2023.7.0/tllab_common/wimread.py
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.7.0/PKG-INFO
```

### Comparing `tllab_common-2023.6.1/LICENSE` & `tllab_common-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.1/README.md` & `tllab_common-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.1/pyproject.toml` & `tllab_common-2023.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2023.6.1"
+version = "2023.7.0"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
```

### Comparing `tllab_common-2023.6.1/tllab_common/findcells.py` & `tllab_common-2023.7.0/tllab_common/findcells.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.1/tllab_common/fit.py` & `tllab_common-2023.7.0/tllab_common/fit.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.1/tllab_common/misc.py` & `tllab_common-2023.7.0/tllab_common/misc.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.1/tllab_common/transforms.py` & `tllab_common-2023.7.0/tllab_common/transforms.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.6.1/tllab_common/wimread.py` & `tllab_common-2023.7.0/tllab_common/wimread.py`

 * *Files 0% similar despite different names*

```diff
@@ -1094,15 +1094,15 @@
                 image = xmldata(image[0])
             return sorted(np.unique(image.search_all('DeltaT').values()))[:self.shape[4]]
         else:
             return (np.arange(self.shape[4]) * self.settimeinterval).tolist()
 
     @cached_property
     def timeinterval(self):
-        return float(np.diff(self.timeval).mean()) if len(self.timeval) > 1 else 1
+        return float(np.diff(self.timeval).mean()) if len(self.timeval) > 1 else self.settimeinterval
 
     @cached_property
     def piezoval(self):
         """ gives the height of the piezo and focus motor, only available when CylLensGUI was used
         """
         def upack(idx):
             time = list()
@@ -1490,23 +1490,25 @@
         if 'Hamamatsu' in self.metadata.search('Core-Camera', '')[0]:
             self.pxsizecam = 6.5
         self.title = self.metadata.search('Prefix')[0]
         self.acquisitiondate = self.metadata.search('Time')[0]
         self.exposuretime = [i / 1000 for i in self.metadata.search('Exposure-ms')]
         self.objective = self.metadata.search('ZeissObjectiveTurret-Label')[0]
         self.optovar = []
+        self.binning = int(self.metadata.search('Hamamatsu_sCMOS-Binning')[0][0])
         for o in self.metadata.search('ZeissOptovar-Label'):
             a = re.search(r'\d?\d*[,.]?\d+(?=x$)', o)
             if hasattr(a, 'group'):
                 self.optovar.append(float(a.group(0).replace(',', '.')))
         if self.pxsize == 0:
             self.magnification = int(re.findall(r'(\d+)x', self.objective, re.IGNORECASE)[0]) * self.optovar[0]
             self.pxsize = self.pxsizecam / self.magnification
         else:
             self.magnification = self.pxsizecam / self.pxsize
+        self.pxsize *= self.binning
         self.pcf = self.shape[2] * self.metadata.re_search(r'(?i)conversion\sfactor\scoeff', 1)
         self.filter = self.metadata.search('ZeissReflectorTurret-Label', self.filter)[0]
         self.track = [0] * self.shape[2]
         self.detector = list(range(self.shape[2]))
 
     def __frame__(self, c=0, z=0, t=0):
         return tifffile.imread(self.path / f"Pos{self.series}" / self.filedict[(c, z, t)])
```

### Comparing `tllab_common-2023.6.1/PKG-INFO` & `tllab_common-2023.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab-common
-Version: 2023.6.1
+Version: 2023.7.0
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.8,<4.0
```

