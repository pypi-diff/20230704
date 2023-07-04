# Comparing `tmp/download_stats-1.2.1.tar.gz` & `tmp/download_stats-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download_stats-1.2.1.tar", last modified: Tue Jul  4 06:44:27 2023, max compression
+gzip compressed data, was "download_stats-1.3.0.tar", last modified: Tue Jul  4 07:21:17 2023, max compression
```

## Comparing `download_stats-1.2.1.tar` & `download_stats-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.139559 download_stats-1.2.1/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    11357 2023-07-04 06:21:07.000000 download_stats-1.2.1/LICENSE
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      150 2023-07-04 06:21:07.000000 download_stats-1.2.1/MANIFEST.in
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3162 2023-07-04 06:44:27.139559 download_stats-1.2.1/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2340 2023-07-04 06:21:07.000000 download_stats-1.2.1/README.md
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.135558 download_stats-1.2.1/assets/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    15299 2023-07-04 06:21:07.000000 download_stats-1.2.1/assets/compare.png
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    68629 2023-07-04 06:21:07.000000 download_stats-1.2.1/assets/download_stats.png
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.135558 download_stats-1.2.1/reqs/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       73 2023-07-04 06:39:03.000000 download_stats-1.2.1/reqs/app.in
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1331 2023-07-04 06:39:12.000000 download_stats-1.2.1/reqs/app.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       22 2023-07-04 06:21:07.000000 download_stats-1.2.1/reqs/dev.in
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1840 2023-07-04 06:21:07.000000 download_stats-1.2.1/reqs/dev.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      217 2023-07-04 06:44:27.143559 download_stats-1.2.1/setup.cfg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3578 2023-07-04 06:44:23.000000 download_stats-1.2.1/setup.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.135558 download_stats-1.2.1/src/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.139559 download_stats-1.2.1/src/download_stats/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      170 2023-07-04 06:21:07.000000 download_stats-1.2.1/src/download_stats/__init__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.139559 download_stats-1.2.1/src/download_stats/__pycache__/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      397 2023-07-04 06:27:00.000000 download_stats-1.2.1/src/download_stats/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     5795 2023-07-04 06:27:00.000000 download_stats-1.2.1/src/download_stats/__pycache__/main.cpython-311.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4373 2023-07-04 06:34:45.000000 download_stats-1.2.1/src/download_stats/__pycache__/pepy.cpython-311.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2931 2023-07-04 06:27:00.000000 download_stats-1.2.1/src/download_stats/__pycache__/pypistats.cpython-311.pyc
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2812 2023-07-04 06:21:07.000000 download_stats-1.2.1/src/download_stats/main.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2352 2023-07-04 06:35:34.000000 download_stats-1.2.1/src/download_stats/pepy.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1790 2023-07-04 06:21:07.000000 download_stats-1.2.1/src/download_stats/pypistats.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 06:44:27.139559 download_stats-1.2.1/src/download_stats.egg-info/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3162 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      731 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       61 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/entry_points.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      444 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/requires.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       15 2023-07-04 06:44:27.000000 download_stats-1.2.1/src/download_stats.egg-info/top_level.txt
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.772064 download_stats-1.3.0/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    11357 2023-07-04 06:21:07.000000 download_stats-1.3.0/LICENSE
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      150 2023-07-04 06:21:07.000000 download_stats-1.3.0/MANIFEST.in
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3290 2023-07-04 07:21:17.772064 download_stats-1.3.0/PKG-INFO
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2468 2023-07-04 07:20:05.000000 download_stats-1.3.0/README.md
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.760062 download_stats-1.3.0/assets/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    15299 2023-07-04 06:21:07.000000 download_stats-1.3.0/assets/compare.png
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    68629 2023-07-04 06:21:07.000000 download_stats-1.3.0/assets/download_stats.png
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.764063 download_stats-1.3.0/reqs/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       73 2023-07-04 06:39:03.000000 download_stats-1.3.0/reqs/app.in
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1331 2023-07-04 06:39:12.000000 download_stats-1.3.0/reqs/app.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       22 2023-07-04 06:21:07.000000 download_stats-1.3.0/reqs/dev.in
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1840 2023-07-04 06:21:07.000000 download_stats-1.3.0/reqs/dev.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      217 2023-07-04 07:21:17.772064 download_stats-1.3.0/setup.cfg
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3578 2023-07-04 07:20:54.000000 download_stats-1.3.0/setup.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.756062 download_stats-1.3.0/src/
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.768063 download_stats-1.3.0/src/download_stats/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      170 2023-07-04 06:21:07.000000 download_stats-1.3.0/src/download_stats/__init__.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.772064 download_stats-1.3.0/src/download_stats/__pycache__/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      397 2023-07-04 06:27:00.000000 download_stats-1.3.0/src/download_stats/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     6794 2023-07-04 07:18:03.000000 download_stats-1.3.0/src/download_stats/__pycache__/main.cpython-311.pyc
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     4428 2023-07-04 07:17:24.000000 download_stats-1.3.0/src/download_stats/__pycache__/pepy.cpython-311.pyc
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2931 2023-07-04 06:27:00.000000 download_stats-1.3.0/src/download_stats/__pycache__/pypistats.cpython-311.pyc
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3210 2023-07-04 07:18:00.000000 download_stats-1.3.0/src/download_stats/main.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2487 2023-07-04 07:16:57.000000 download_stats-1.3.0/src/download_stats/pepy.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1790 2023-07-04 06:21:07.000000 download_stats-1.3.0/src/download_stats/pypistats.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-04 07:21:17.768063 download_stats-1.3.0/src/download_stats.egg-info/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3290 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      731 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       61 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      444 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/requires.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       15 2023-07-04 07:21:17.000000 download_stats-1.3.0/src/download_stats.egg-info/top_level.txt
```

### Comparing `download_stats-1.2.1/LICENSE` & `download_stats-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.1/PKG-INFO` & `download_stats-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download_stats
-Version: 1.2.1
+Version: 1.3.0
 Summary: Download stats for Python packages
 Home-page: UNKNOWN
 Author-email: arj.python@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/Abdur-RahmaanJ/download-stats/issues
 Project-URL: Source, https://github.com/Abdur-RahmaanJ/download-stats/
 Platform: UNKNOWN
@@ -40,14 +40,20 @@
 ![](https://github.com/Abdur-RahmaanJ/download-stats/raw/stable/assets/compare.png)
 
 
 ```
 $ download-stats --self # same as `download-stats download-stats`
 ```
 
+Total downloads
+
+```
+$ download-stats --total hooman shopyo download-stats meteomoris newsmoris shopcube honeybot jamstack
+```
+
 ## general
 
 ```python
 >>> from download_stats import stats 
 >>> stats('shopyo')
 {
     "total": "41327",
```

### Comparing `download_stats-1.2.1/README.md` & `download_stats-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 ![](https://github.com/Abdur-RahmaanJ/download-stats/raw/stable/assets/compare.png)
 
 
 ```
 $ download-stats --self # same as `download-stats download-stats`
 ```
 
+Total downloads
+
+```
+$ download-stats --total hooman shopyo download-stats meteomoris newsmoris shopcube honeybot jamstack
+```
+
 ## general
 
 ```python
 >>> from download_stats import stats 
 >>> stats('shopyo')
 {
     "total": "41327",
```

### Comparing `download_stats-1.2.1/assets/compare.png` & `download_stats-1.3.0/assets/compare.png`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.1/assets/download_stats.png` & `download_stats-1.3.0/assets/download_stats.png`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.1/reqs/app.txt` & `download_stats-1.3.0/reqs/app.txt`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.1/reqs/dev.txt` & `download_stats-1.3.0/reqs/dev.txt`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.1/setup.py` & `download_stats-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name="download_stats",  # Required
-    version="1.2.1",  # Required
+    version="1.3.0",  # Required
     description="Download stats for Python packages",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     # url="https://github.com/Abdur-RahmaanJ/greenBerry",  # Optional
     # author="Abdur-Rahmaan Janhangeer & contributors",  # Optional
     author_email="arj.python@gmail.com",  # Optional
     # Classifiers help users find your project by categorizing it.
```

### Comparing `download_stats-1.2.1/src/download_stats/__pycache__/main.cpython-311.pyc` & `download_stats-1.3.0/src/download_stats/__pycache__/main.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,22 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0x53baa364 (Tue Jul  4 06:21:07 2023 UTC)
-files sz: 2812
+moddate:  0xa8c7a364 (Tue Jul  4 07:18:00 2023 UTC)
+files sz: 3210
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c026d045a040100640064046c026d055a050100640064056c066d075a
       070100640064066c086d095a090100640064076c0a6d0b5a0b0100640064
       086c0c5a0c6409650d640a64086604640b84045a0e640c650f640a640866
       04640d84045a10640e650f6409650d640a64086606640f84045a11641084
-      005a1264085300
+      005a12641184005a1364085300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('stats',))
                  6 IMPORT_NAME              0 (download_stats.pepy)
                  8 IMPORT_FROM              1 (stats)
                 10 STORE_NAME               1 (stats)
@@ -94,19 +94,23 @@
                134 LOAD_CONST              10 ('return')
                136 LOAD_CONST               8 (None)
                138 BUILD_TUPLE              6
                140 LOAD_CONST              15 (<code object versions_table, file "/home/appinv/code/download-stats/src/download_stats/main.py", line 55>)
                142 MAKE_FUNCTION            4 (annotations)
                144 STORE_NAME              17 (versions_table)
    
-    74         146 LOAD_CONST              16 (<code object main, file "/home/appinv/code/download-stats/src/download_stats/main.py", line 74>)
+    74         146 LOAD_CONST              16 (<code object combined_downloads, file "/home/appinv/code/download-stats/src/download_stats/main.py", line 74>)
                148 MAKE_FUNCTION            0
-               150 STORE_NAME              18 (main)
-               152 LOAD_CONST               8 (None)
-               154 RETURN_VALUE
+               150 STORE_NAME              18 (combined_downloads)
+   
+    84         152 LOAD_CONST              17 (<code object main, file "/home/appinv/code/download-stats/src/download_stats/main.py", line 84>)
+               154 MAKE_FUNCTION            0
+               156 STORE_NAME              19 (main)
+               158 LOAD_CONST               8 (None)
+               160 RETURN_VALUE
    consts
       0
       ('stats',)
       ('recent',)
       ('system',)
       ('version',)
       ('Union',)
@@ -712,14 +716,109 @@
          filename   '/home/appinv/code/download-stats/src/download_stats/main.py'
          name       'versions_table'
          firstlineno 55
          lnotab
             0x02012001100128013e0156015201520152015401540234010c017e021c
             01
       code
+         argcount  : 1
+         nlocals   : 4
+         stacksize : 7
+         flags     : 3
+         code
+            0x970064017d017c0044005d277d027c0174010000000000000000000074
+            03000000000000000000007c02a6010000ab010000000000000000640219
+            000000000000000000a6010000ab0100000000000000007a0d00007d018c
+            28740500000000000000000000a6000000ab0000000000000000007d037c
+            03a00300000000000000000000000000000000000000006403a6010000ab
+            01000000000000000001007c03a003000000000000000000000000000000
+            00000000006404a00400000000000000000000000000000000000000007c
+            00a6010000ab010000000000000000a6010000ab01000000000000000001
+            007c03a00300000000000000000000000000000000000000006405740b00
+            0000000000000000007c01a6010000ab0100000000000000007a00000064
+            067a000000a6010000ab010000000000000000010064005300
+          74           0 RESUME                   0
+         
+          75           2 LOAD_CONST               1 (0)
+                       4 STORE_FAST               1 (total)
+         
+          76           6 LOAD_FAST                0 (projects)
+                       8 GET_ITER
+                 >>   10 FOR_ITER                39 (to 90)
+                      12 STORE_FAST               2 (p)
+         
+          77          14 LOAD_FAST                1 (total)
+                      16 LOAD_GLOBAL              1 (NULL + int)
+                      28 LOAD_GLOBAL              3 (NULL + stats)
+                      40 LOAD_FAST                2 (p)
+                      42 PRECALL                  1
+                      46 CALL                     1
+                      56 LOAD_CONST               2 ('total')
+                      58 BINARY_SUBSCR
+                      68 PRECALL                  1
+                      72 CALL                     1
+                      82 BINARY_OP               13 (+=)
+                      86 STORE_FAST               1 (total)
+                      88 JUMP_BACKWARD           40 (to 10)
+         
+          79     >>   90 LOAD_GLOBAL              5 (NULL + Console)
+                     102 PRECALL                  0
+                     106 CALL                     0
+                     116 STORE_FAST               3 (console)
+         
+          80         118 LOAD_FAST                3 (console)
+                     120 LOAD_METHOD              3 (print)
+                     142 LOAD_CONST               3 ('Total downloads for projects:')
+                     144 PRECALL                  1
+                     148 CALL                     1
+                     158 POP_TOP
+         
+          81         160 LOAD_FAST                3 (console)
+                     162 LOAD_METHOD              3 (print)
+                     184 LOAD_CONST               4 (', ')
+                     186 LOAD_METHOD              4 (join)
+                     208 LOAD_FAST                0 (projects)
+                     210 PRECALL                  1
+                     214 CALL                     1
+                     224 PRECALL                  1
+                     228 CALL                     1
+                     238 POP_TOP
+         
+          82         240 LOAD_FAST                3 (console)
+                     242 LOAD_METHOD              3 (print)
+                     264 LOAD_CONST               5 ('[green]')
+                     266 LOAD_GLOBAL             11 (NULL + str)
+                     278 LOAD_FAST                1 (total)
+                     280 PRECALL                  1
+                     284 CALL                     1
+                     294 BINARY_OP                0 (+)
+                     298 LOAD_CONST               6 ('[/green]')
+                     300 BINARY_OP                0 (+)
+                     304 PRECALL                  1
+                     308 CALL                     1
+                     318 POP_TOP
+                     320 LOAD_CONST               0 (None)
+                     322 RETURN_VALUE
+         consts
+            None
+            0
+            'total'
+            'Total downloads for projects:'
+            ', '
+            '[green]'
+            '[/green]'
+         names      ('int', 'stats', 'Console', 'print', 'join', 'str')
+         varnames   ('projects', 'total', 'p', 'console')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/appinv/code/download-stats/src/download_stats/main.py'
+         name       'combined_downloads'
+         firstlineno 74
+         lnotab 0x0201040108014c021c012a015001
+      code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000006a0200
             00000000000000a6010000ab01000000000000000064016b020000000072
@@ -734,124 +833,163 @@
             0000000000000064046b0200000000723e74010000000000000000000074
             02000000000000000000006a020000000000000000a6010000ab01000000
             000000000064056b05000000007221740f00000000000000000000740200
             0000000000000000006a0200000000000000006406640085021900000000
             0000000000a6010000ab0100000000000000000100740200000000000000
             0000006a020000000000000000640119000000000000000000a006000000
             0000000000000000000000000000000000a6000000ab0000000000000000
-            0064076b02000000007211740b000000000000000000006408a6010000ab
-            01000000000000000001006400530064005300
-          74           0 RESUME                   0
+            0064076b0200000000723e74010000000000000000000074020000000000
+            00000000006a020000000000000000a6010000ab01000000000000000064
+            056b05000000007221741100000000000000000000740200000000000000
+            0000006a02000000000000000064066400850219000000000000000000a6
+            010000ab01000000000000000001007402000000000000000000006a0200
+            00000000000000640119000000000000000000a006000000000000000000
+            0000000000000000000000a6000000ab00000000000000000064086b0200
+            0000007211740b000000000000000000006409a6010000ab010000000000
+            00000001006400530064005300
+          84           0 RESUME                   0
          
-          75           2 LOAD_GLOBAL              1 (NULL + len)
+          85           2 LOAD_GLOBAL              1 (NULL + len)
                       14 LOAD_GLOBAL              2 (sys)
                       26 LOAD_ATTR                2 (argv)
                       36 PRECALL                  1
                       40 CALL                     1
                       50 LOAD_CONST               1 (1)
                       52 COMPARE_OP               2 (==)
                       58 POP_JUMP_FORWARD_IF_FALSE    20 (to 100)
          
-          76          60 LOAD_GLOBAL              3 (NULL + sys)
+          86          60 LOAD_GLOBAL              3 (NULL + sys)
                       72 LOAD_ATTR                3 (exit)
                       82 LOAD_CONST               2 ('Package args needed!')
                       84 PRECALL                  1
                       88 CALL                     1
                       98 POP_TOP
          
-          77     >>  100 LOAD_GLOBAL              2 (sys)
+          87     >>  100 LOAD_GLOBAL              2 (sys)
                      112 LOAD_ATTR                2 (argv)
                      122 LOAD_CONST               1 (1)
                      124 BINARY_SUBSCR
                      134 LOAD_METHOD              4 (startswith)
                      156 LOAD_CONST               3 ('--')
                      158 PRECALL                  1
                      162 CALL                     1
                      172 POP_JUMP_FORWARD_IF_TRUE    31 (to 236)
          
-          78         174 LOAD_GLOBAL             11 (NULL + summary_table)
+          88         174 LOAD_GLOBAL             11 (NULL + summary_table)
                      186 LOAD_GLOBAL              2 (sys)
                      198 LOAD_ATTR                2 (argv)
                      208 LOAD_CONST               1 (1)
                      210 BINARY_SUBSCR
                      220 PRECALL                  1
                      224 CALL                     1
                      234 POP_TOP
          
-          79     >>  236 LOAD_GLOBAL              2 (sys)
+          89     >>  236 LOAD_GLOBAL              2 (sys)
                      248 LOAD_ATTR                2 (argv)
                      258 LOAD_CONST               1 (1)
                      260 BINARY_SUBSCR
                      270 LOAD_METHOD              6 (casefold)
                      292 PRECALL                  0
                      296 CALL                     0
                      306 LOAD_CONST               4 ('--compare')
                      308 COMPARE_OP               2 (==)
                      314 POP_JUMP_FORWARD_IF_FALSE    62 (to 440)
          
-          80         316 LOAD_GLOBAL              1 (NULL + len)
+          90         316 LOAD_GLOBAL              1 (NULL + len)
                      328 LOAD_GLOBAL              2 (sys)
                      340 LOAD_ATTR                2 (argv)
                      350 PRECALL                  1
                      354 CALL                     1
                      364 LOAD_CONST               5 (3)
                      366 COMPARE_OP               5 (>=)
                      372 POP_JUMP_FORWARD_IF_FALSE    33 (to 440)
          
-          81         374 LOAD_GLOBAL             15 (NULL + compare_table)
+          91         374 LOAD_GLOBAL             15 (NULL + compare_table)
                      386 LOAD_GLOBAL              2 (sys)
                      398 LOAD_ATTR                2 (argv)
                      408 LOAD_CONST               6 (2)
                      410 LOAD_CONST               0 (None)
                      412 BUILD_SLICE              2
                      414 BINARY_SUBSCR
                      424 PRECALL                  1
                      428 CALL                     1
                      438 POP_TOP
          
-          82     >>  440 LOAD_GLOBAL              2 (sys)
+          92     >>  440 LOAD_GLOBAL              2 (sys)
                      452 LOAD_ATTR                2 (argv)
                      462 LOAD_CONST               1 (1)
                      464 BINARY_SUBSCR
                      474 LOAD_METHOD              6 (casefold)
                      496 PRECALL                  0
                      500 CALL                     0
-                     510 LOAD_CONST               7 ('--self')
+                     510 LOAD_CONST               7 ('--total')
                      512 COMPARE_OP               2 (==)
-                     518 POP_JUMP_FORWARD_IF_FALSE    17 (to 554)
+                     518 POP_JUMP_FORWARD_IF_FALSE    62 (to 644)
          
-          83         520 LOAD_GLOBAL             11 (NULL + summary_table)
-                     532 LOAD_CONST               8 ('download-stats')
-                     534 PRECALL                  1
-                     538 CALL                     1
-                     548 POP_TOP
-                     550 LOAD_CONST               0 (None)
-                     552 RETURN_VALUE
+          93         520 LOAD_GLOBAL              1 (NULL + len)
+                     532 LOAD_GLOBAL              2 (sys)
+                     544 LOAD_ATTR                2 (argv)
+                     554 PRECALL                  1
+                     558 CALL                     1
+                     568 LOAD_CONST               5 (3)
+                     570 COMPARE_OP               5 (>=)
+                     576 POP_JUMP_FORWARD_IF_FALSE    33 (to 644)
+         
+          94         578 LOAD_GLOBAL             17 (NULL + combined_downloads)
+                     590 LOAD_GLOBAL              2 (sys)
+                     602 LOAD_ATTR                2 (argv)
+                     612 LOAD_CONST               6 (2)
+                     614 LOAD_CONST               0 (None)
+                     616 BUILD_SLICE              2
+                     618 BINARY_SUBSCR
+                     628 PRECALL                  1
+                     632 CALL                     1
+                     642 POP_TOP
+         
+          95     >>  644 LOAD_GLOBAL              2 (sys)
+                     656 LOAD_ATTR                2 (argv)
+                     666 LOAD_CONST               1 (1)
+                     668 BINARY_SUBSCR
+                     678 LOAD_METHOD              6 (casefold)
+                     700 PRECALL                  0
+                     704 CALL                     0
+                     714 LOAD_CONST               8 ('--self')
+                     716 COMPARE_OP               2 (==)
+                     722 POP_JUMP_FORWARD_IF_FALSE    17 (to 758)
+         
+          96         724 LOAD_GLOBAL             11 (NULL + summary_table)
+                     736 LOAD_CONST               9 ('download-stats')
+                     738 PRECALL                  1
+                     742 CALL                     1
+                     752 POP_TOP
+                     754 LOAD_CONST               0 (None)
+                     756 RETURN_VALUE
          
-          82     >>  554 LOAD_CONST               0 (None)
-                     556 RETURN_VALUE
+          95     >>  758 LOAD_CONST               0 (None)
+                     760 RETURN_VALUE
          consts
             None
             1
             'Package args needed!'
             '--'
             '--compare'
             3
             2
+            '--total'
             '--self'
             'download-stats'
-         names      ('len', 'sys', 'argv', 'exit', 'startswith', 'summary_table', 'casefold', 'compare_table')
+         names      ('len', 'sys', 'argv', 'exit', 'startswith', 'summary_table', 'casefold', 'compare_table', 'combined_downloads')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/appinv/code/download-stats/src/download_stats/main.py'
          name       'main'
-         firstlineno 74
-         lnotab 0x02013a0128014a013e0150013a014201500122ff
-   names      ('download_stats.pepy', 'stats', 'download_stats.pypistats', 'recent', 'system', 'version', 'typing', 'Union', 'rich.console', 'Console', 'rich.table', 'Table', 'sys', 'str', 'summary_table', 'list', 'compare_table', 'versions_table', 'main')
+         firstlineno 84
+         lnotab 0x02013a0128014a013e0150013a01420150013a014201500122ff
+   names      ('download_stats.pepy', 'stats', 'download_stats.pypistats', 'recent', 'system', 'version', 'typing', 'Union', 'rich.console', 'Console', 'rich.table', 'Table', 'sys', 'str', 'summary_table', 'list', 'compare_table', 'versions_table', 'combined_downloads', 'main')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/appinv/code/download-stats/src/download_stats/main.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c010c010c010c020c010c0208021011101a1413
+   lnotab 0x00ff02010c010c010c010c010c020c010c0208021011101a1413060a
```

### Comparing `download_stats-1.2.1/src/download_stats/__pycache__/pepy.cpython-311.pyc` & `download_stats-1.3.0/src/download_stats/__pycache__/pepy.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0x82bda364 (Tue Jul  4 06:34:42 2023 UTC)
-files sz: 2373
+moddate:  0x69c7a364 (Tue Jul  4 07:16:57 2023 UTC)
+files sz: 2487
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 4
+   stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a050100640064046c066d075a070100640064056c086d095a
       090100640064066c0a6d0b5a0b0100640064076c0c6d0d5a0d0100640064
       086c0e5a0e640064086c0f5a0f0200650da6000000ab0000000000000000
-      005a1064096511640a65126604640b84045a1364085300
+      005a10640d640a6511640b65126604640c84055a1364085300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Service',))
                  6 IMPORT_NAME              0 (selenium.webdriver.chrome.service)
                  8 IMPORT_FROM              1 (Service)
                 10 STORE_NAME               1 (Service)
@@ -45,426 +45,441 @@
      5          50 LOAD_CONST               0 (0)
                 52 LOAD_CONST               5 (('webdriver',))
                 54 IMPORT_NAME              8 (selenium)
                 56 IMPORT_FROM              9 (webdriver)
                 58 STORE_NAME               9 (webdriver)
                 60 POP_TOP
    
-     6          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               6 (('UserAgent',))
-                66 IMPORT_NAME             10 (fake_useragent)
-                68 IMPORT_FROM             11 (UserAgent)
-                70 STORE_NAME              11 (UserAgent)
+     7          62 LOAD_CONST               0 (0)
+                64 LOAD_CONST               6 (('get_random_user_agent',))
+                66 IMPORT_NAME             10 (latest_user_agents)
+                68 IMPORT_FROM             11 (get_random_user_agent)
+                70 STORE_NAME              11 (get_random_user_agent)
                 72 POP_TOP
    
-     7          74 LOAD_CONST               0 (0)
+     8          74 LOAD_CONST               0 (0)
                 76 LOAD_CONST               7 (('Console',))
                 78 IMPORT_NAME             12 (rich.console)
                 80 IMPORT_FROM             13 (Console)
                 82 STORE_NAME              13 (Console)
                 84 POP_TOP
    
-     8          86 LOAD_CONST               0 (0)
+     9          86 LOAD_CONST               0 (0)
                 88 LOAD_CONST               8 (None)
                 90 IMPORT_NAME             14 (time)
                 92 STORE_NAME              14 (time)
    
-     9          94 LOAD_CONST               0 (0)
+    10          94 LOAD_CONST               0 (0)
                 96 LOAD_CONST               8 (None)
                 98 IMPORT_NAME             15 (sys)
                100 STORE_NAME              15 (sys)
    
-    11         102 PUSH_NULL
+    12         102 PUSH_NULL
                104 LOAD_NAME               13 (Console)
                106 PRECALL                  0
                110 CALL                     0
                120 STORE_NAME              16 (console)
    
-    14         122 LOAD_CONST               9 ('project')
-               124 LOAD_NAME               17 (str)
-               126 LOAD_CONST              10 ('return')
-               128 LOAD_NAME               18 (dict)
-               130 BUILD_TUPLE              4
-               132 LOAD_CONST              11 (<code object stats, file "/home/appinv/code/download-stats/src/download_stats/pepy.py", line 14>)
-               134 MAKE_FUNCTION            4 (annotations)
-               136 STORE_NAME              19 (stats)
-               138 LOAD_CONST               8 (None)
-               140 RETURN_VALUE
+    15         122 LOAD_CONST              13 ((False,))
+               124 LOAD_CONST              10 ('project')
+               126 LOAD_NAME               17 (str)
+               128 LOAD_CONST              11 ('return')
+               130 LOAD_NAME               18 (dict)
+               132 BUILD_TUPLE              4
+               134 LOAD_CONST              12 (<code object stats, file "/home/appinv/code/download-stats/src/download_stats/pepy.py", line 15>)
+               136 MAKE_FUNCTION            5 (defaults, annotations)
+               138 STORE_NAME              19 (stats)
+               140 LOAD_CONST               8 (None)
+               142 RETURN_VALUE
    consts
       0
       ('Service',)
       ('ChromeDriverManager',)
       ('WebDriverWait',)
       ('Options',)
       ('webdriver',)
-      ('UserAgent',)
+      ('get_random_user_agent',)
       ('Console',)
       None
+      False
       'project'
       'return'
       code
-         argcount  : 1
-         nlocals   : 13
+         argcount  : 2
+         nlocals   : 12
          stacksize : 6
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
-            017c01a00100000000000000000000000000000000000000006401a60100
-            00ab01000000000000000001007c01a00100000000000000000000000000
-            000000000000006402a6010000ab01000000000000000001007c01a00100
+            027c02a00100000000000000000000000000000000000000006401a60100
+            00ab01000000000000000001007c02a00100000000000000000000000000
+            000000000000006402a6010000ab01000000000000000001007c02a00100
             000000000000000000000000000000000000006403a6010000ab01000000
-            000000000001007c01a00100000000000000000000000000000000000000
-            006404a6010000ab01000000000000000001007c01a00100000000000000
+            000000000001007c02a00100000000000000000000000000000000000000
+            006404a6010000ab01000000000000000001007c02a00100000000000000
             000000000000000000000000006405a6010000ab01000000000000000001
-            007c01a00100000000000000000000000000000000000000006406a60100
-            00ab01000000000000000001007c01a00100000000000000000000000000
-            000000000000006407a6010000ab01000000000000000001007c01a00200
+            007c02a00100000000000000000000000000000000000000006406a60100
+            00ab01000000000000000001007c02a00100000000000000000000000000
+            000000000000006407a6010000ab01000000000000000001007c02a00200
             00000000000000000000000000000000000000640864096701a6020000ab
-            02000000000000000001007c01a002000000000000000000000000000000
-            0000000000640a640ba6020000ab02000000000000000001007c01a00100
+            02000000000000000001007c02a002000000000000000000000000000000
+            0000000000640a640ba6020000ab02000000000000000001007c02a00100
             00000000000000000000000000000000000000640ca6010000ab01000000
             000000000001007407000000000000000000006a04000000000000000074
             0b00000000000000000000740d00000000000000000000a6000000ab0000
             00000000000000a0070000000000000000000000000000000000000000a6
-            000000ab000000000000000000a6010000ab0100000000000000007c01ac
-            0da6020000ab0200000000000000007d02640e640f6c086d097d036d0a7d
-            04010002007c04a6000000ab0000000000000000007d057c02a00b000000
-            00000000000000000000000000000000006410a6010000ab010000000000
-            00000001007c02a00c000000000000000000000000000000000000000064
-            1164127c056901a6020000ab0200000000000000000100741a0000000000
-            0000000000a00e00000000000000000000000000000000000000006413a6
-            010000ab01000000000000000035007d067c02a00f000000000000000000
-            000000000000000000000064147c009b009d02a6010000ab010000000000
-            00000001007421000000000000000000006a1100000000000000006415a6
-            010000ab0100000000000000000100640064006400a6020000ab02000000
-            000000000001006e0b230031007304770278035900770101005900010001
-            0009007c02a0120000000000000000000000000000000000000000641664
-            17a6020000ab0200000000000000007d07641884007c0764191900000000
-            00000000006a130000000000000000a01400000000000000000000000000
-            00000000000000641aa6010000ab0100000000000000004400a6000000ab
-            0000000000000000007d0867007d09640b7d0a742b000000000000000000
-            007c08a6010000ab01000000000000000044005d405c0200007d0b7d0c64
-            1b7c087c0b1900000000000000000076007202641c7d0a7c0a722d7c09a0
-            1600000000000000000000000000000000000000007c087c0b1900000000
-            0000000000a0140000000000000000000000000000000000000000a60000
-            00ab000000000000000000a6010000ab01000000000000000001008c416e
-            242300742e00000000000000000000240072170100743100000000000000
-            0000006a190000000000000000641da6010000ab01000000000000000001
-            0059006e0477007803590077017c076415190000000000000000006a1300
-            00000000000000a01a000000000000000000000000000000000000000064
-            1e641fa6020000ab0200000000000000007c076420190000000000000000
-            006a130000000000000000a01a0000000000000000000000000000000000
-            000000641e641fa6020000ab0200000000000000007c0764211900000000
-            00000000006a130000000000000000a01a00000000000000000000000000
-            00000000000000641e641fa6020000ab0200000000000000007c0964229c
-            045300
-          14           0 RESUME                   0
+            000000ab000000000000000000a6010000ab0100000000000000007c02ac
+            0da6020000ab0200000000000000007d03741100000000000000000000a6
+            000000ab0000000000000000007d047c03a0090000000000000000000000
+            000000000000000000640ea6010000ab01000000000000000001007c03a0
+            0a0000000000000000000000000000000000000000640f64107c046901a6
+            020000ab02000000000000000001007c01722d7c03a00b00000000000000
+            0000000000000000000000000064117c009b009d02a6010000ab01000000
+            000000000001007419000000000000000000006a0d000000000000000064
+            12a6010000ab01000000000000000001006e5e741c000000000000000000
+            00a00f00000000000000000000000000000000000000006413a6010000ab
+            01000000000000000035007d057c03a00b00000000000000000000000000
+            0000000000000064117c009b009d02a6010000ab01000000000000000001
+            007419000000000000000000006a0d00000000000000006412a6010000ab
+            0100000000000000000100640064006400a6020000ab0200000000000000
+            0001006e0b2300310073047702780359007701010059000100010009007c
+            03a010000000000000000000000000000000000000000064146415a60200
+            00ab0200000000000000007d06641684007c066417190000000000000000
+            006a110000000000000000a0120000000000000000000000000000000000
+            0000006418a6010000ab0100000000000000004400a6000000ab00000000
+            00000000007d0767007d08640b7d097427000000000000000000007c07a6
+            010000ab01000000000000000044005d405c0200007d0a7d0b64197c077c
+            0a1900000000000000000076007202641a7d097c09722d7c08a014000000
+            00000000000000000000000000000000007c077c0a190000000000000000
+            00a0120000000000000000000000000000000000000000a6000000ab0000
+            00000000000000a6010000ab01000000000000000001008c416e24230074
+            2a00000000000000000000240072170100742d000000000000000000006a
+            170000000000000000641ba6010000ab010000000000000000010059006e
+            0477007803590077017c066412190000000000000000006a110000000000
+            000000a0180000000000000000000000000000000000000000641c641da6
+            020000ab0200000000000000007c06641e190000000000000000006a1100
+            00000000000000a018000000000000000000000000000000000000000064
+            1c641da6020000ab0200000000000000007c06641f190000000000000000
+            006a110000000000000000a0180000000000000000000000000000000000
+            000000641c641da6020000ab0200000000000000007c0864209c045300
+          15           0 RESUME                   0
          
-          15           2 LOAD_GLOBAL              1 (NULL + Options)
+          16           2 LOAD_GLOBAL              1 (NULL + Options)
                       14 PRECALL                  0
                       18 CALL                     0
-                      28 STORE_FAST               1 (options)
+                      28 STORE_FAST               2 (options)
          
-          16          30 LOAD_FAST                1 (options)
+          17          30 LOAD_FAST                2 (options)
                       32 LOAD_METHOD              1 (add_argument)
                       54 LOAD_CONST               1 ('--headless')
                       56 PRECALL                  1
                       60 CALL                     1
                       70 POP_TOP
          
-          17          72 LOAD_FAST                1 (options)
+          18          72 LOAD_FAST                2 (options)
                       74 LOAD_METHOD              1 (add_argument)
                       96 LOAD_CONST               2 ('--incognito')
                       98 PRECALL                  1
                      102 CALL                     1
                      112 POP_TOP
          
-          18         114 LOAD_FAST                1 (options)
+          19         114 LOAD_FAST                2 (options)
                      116 LOAD_METHOD              1 (add_argument)
                      138 LOAD_CONST               3 ('--nogpu')
                      140 PRECALL                  1
                      144 CALL                     1
                      154 POP_TOP
          
-          19         156 LOAD_FAST                1 (options)
+          20         156 LOAD_FAST                2 (options)
                      158 LOAD_METHOD              1 (add_argument)
                      180 LOAD_CONST               4 ('--disable-gpu')
                      182 PRECALL                  1
                      186 CALL                     1
                      196 POP_TOP
          
-          20         198 LOAD_FAST                1 (options)
+          21         198 LOAD_FAST                2 (options)
                      200 LOAD_METHOD              1 (add_argument)
                      222 LOAD_CONST               5 ('--window-size=1280,1280')
                      224 PRECALL                  1
                      228 CALL                     1
                      238 POP_TOP
          
-          21         240 LOAD_FAST                1 (options)
+          22         240 LOAD_FAST                2 (options)
                      242 LOAD_METHOD              1 (add_argument)
                      264 LOAD_CONST               6 ('--no-sandbox')
                      266 PRECALL                  1
                      270 CALL                     1
                      280 POP_TOP
          
-          22         282 LOAD_FAST                1 (options)
+          23         282 LOAD_FAST                2 (options)
                      284 LOAD_METHOD              1 (add_argument)
                      306 LOAD_CONST               7 ('--enable-javascript')
                      308 PRECALL                  1
                      312 CALL                     1
                      322 POP_TOP
          
-          23         324 LOAD_FAST                1 (options)
+          24         324 LOAD_FAST                2 (options)
                      326 LOAD_METHOD              2 (add_experimental_option)
                      348 LOAD_CONST               8 ('excludeSwitches')
                      350 LOAD_CONST               9 ('enable-automation')
                      352 BUILD_LIST               1
                      354 PRECALL                  2
                      358 CALL                     2
                      368 POP_TOP
          
-          24         370 LOAD_FAST                1 (options)
+          25         370 LOAD_FAST                2 (options)
                      372 LOAD_METHOD              2 (add_experimental_option)
                      394 LOAD_CONST              10 ('useAutomationExtension')
                      396 LOAD_CONST              11 (False)
                      398 PRECALL                  2
                      402 CALL                     2
                      412 POP_TOP
          
-          25         414 LOAD_FAST                1 (options)
+          26         414 LOAD_FAST                2 (options)
                      416 LOAD_METHOD              1 (add_argument)
                      438 LOAD_CONST              12 ('--disable-blink-features=AutomationControlled')
                      440 PRECALL                  1
                      444 CALL                     1
                      454 POP_TOP
          
-          26         456 LOAD_GLOBAL              7 (NULL + webdriver)
+          27         456 LOAD_GLOBAL              7 (NULL + webdriver)
                      468 LOAD_ATTR                4 (Chrome)
                      478 LOAD_GLOBAL             11 (NULL + Service)
                      490 LOAD_GLOBAL             13 (NULL + ChromeDriverManager)
                      502 PRECALL                  0
                      506 CALL                     0
                      516 LOAD_METHOD              7 (install)
                      538 PRECALL                  0
                      542 CALL                     0
                      552 PRECALL                  1
                      556 CALL                     1
-                     566 LOAD_FAST                1 (options)
+                     566 LOAD_FAST                2 (options)
                      568 KW_NAMES                13
                      570 PRECALL                  2
                      574 CALL                     2
-                     584 STORE_FAST               2 (driver)
+                     584 STORE_FAST               3 (driver)
          
-          27         586 LOAD_CONST              14 (0)
-                     588 LOAD_CONST              15 (('get_latest_user_agents', 'get_random_user_agent'))
-                     590 IMPORT_NAME              8 (latest_user_agents)
-                     592 IMPORT_FROM              9 (get_latest_user_agents)
-                     594 STORE_FAST               3 (get_latest_user_agents)
-                     596 IMPORT_FROM             10 (get_random_user_agent)
-                     598 STORE_FAST               4 (get_random_user_agent)
-                     600 POP_TOP
-         
-          31         602 PUSH_NULL
-                     604 LOAD_FAST                4 (get_random_user_agent)
-                     606 PRECALL                  0
-                     610 CALL                     0
-                     620 STORE_FAST               5 (userAgent)
-         
-          32         622 LOAD_FAST                2 (driver)
-                     624 LOAD_METHOD             11 (execute_script)
-                     646 LOAD_CONST              16 ("Object.defineProperty(navigator, 'webdriver', {get: () => undefined})")
-                     648 PRECALL                  1
-                     652 CALL                     1
-                     662 POP_TOP
-         
-          33         664 LOAD_FAST                2 (driver)
-                     666 LOAD_METHOD             12 (execute_cdp_cmd)
-                     688 LOAD_CONST              17 ('Network.setUserAgentOverride')
-                     690 LOAD_CONST              18 ('userAgent')
-                     692 LOAD_FAST                5 (userAgent)
-                     694 BUILD_MAP                1
-                     696 PRECALL                  2
-                     700 CALL                     2
-                     710 POP_TOP
-         
-          34         712 LOAD_GLOBAL             26 (console)
-                     724 LOAD_METHOD             14 (status)
-                     746 LOAD_CONST              19 ('[bold green]Getting content...')
-                     748 PRECALL                  1
-                     752 CALL                     1
-                     762 BEFORE_WITH
-                     764 STORE_FAST               6 (status)
-         
-          35         766 LOAD_FAST                2 (driver)
-                     768 LOAD_METHOD             15 (get)
-                     790 LOAD_CONST              20 ('https://pepy.tech/project/')
-                     792 LOAD_FAST                0 (project)
-                     794 FORMAT_VALUE             0
-                     796 BUILD_STRING             2
-                     798 PRECALL                  1
-                     802 CALL                     1
-                     812 POP_TOP
-         
-          36         814 LOAD_GLOBAL             33 (NULL + time)
-                     826 LOAD_ATTR               17 (sleep)
-                     836 LOAD_CONST              21 (5)
-                     838 PRECALL                  1
-                     842 CALL                     1
-                     852 POP_TOP
-         
-          34         854 LOAD_CONST               0 (None)
-                     856 LOAD_CONST               0 (None)
-                     858 LOAD_CONST               0 (None)
-                     860 PRECALL                  2
-                     864 CALL                     2
-                     874 POP_TOP
-                     876 JUMP_FORWARD            11 (to 900)
-                 >>  878 PUSH_EXC_INFO
-                     880 WITH_EXCEPT_START
-                     882 POP_JUMP_FORWARD_IF_TRUE     4 (to 892)
-                     884 RERAISE                  2
-                 >>  886 COPY                     3
-                     888 POP_EXCEPT
-                     890 RERAISE                  1
-                 >>  892 POP_TOP
-                     894 POP_EXCEPT
-                     896 POP_TOP
+          32         586 LOAD_GLOBAL             17 (NULL + get_random_user_agent)
+                     598 PRECALL                  0
+                     602 CALL                     0
+                     612 STORE_FAST               4 (userAgent)
+         
+          33         614 LOAD_FAST                3 (driver)
+                     616 LOAD_METHOD              9 (execute_script)
+                     638 LOAD_CONST              14 ("Object.defineProperty(navigator, 'webdriver', {get: () => undefined})")
+                     640 PRECALL                  1
+                     644 CALL                     1
+                     654 POP_TOP
+         
+          34         656 LOAD_FAST                3 (driver)
+                     658 LOAD_METHOD             10 (execute_cdp_cmd)
+                     680 LOAD_CONST              15 ('Network.setUserAgentOverride')
+                     682 LOAD_CONST              16 ('userAgent')
+                     684 LOAD_FAST                4 (userAgent)
+                     686 BUILD_MAP                1
+                     688 PRECALL                  2
+                     692 CALL                     2
+                     702 POP_TOP
+         
+          36         704 LOAD_FAST                1 (no_rich)
+                     706 POP_JUMP_FORWARD_IF_FALSE    45 (to 798)
+         
+          37         708 LOAD_FAST                3 (driver)
+                     710 LOAD_METHOD             11 (get)
+                     732 LOAD_CONST              17 ('https://pepy.tech/project/')
+                     734 LOAD_FAST                0 (project)
+                     736 FORMAT_VALUE             0
+                     738 BUILD_STRING             2
+                     740 PRECALL                  1
+                     744 CALL                     1
+                     754 POP_TOP
+         
+          38         756 LOAD_GLOBAL             25 (NULL + time)
+                     768 LOAD_ATTR               13 (sleep)
+                     778 LOAD_CONST              18 (5)
+                     780 PRECALL                  1
+                     784 CALL                     1
+                     794 POP_TOP
+                     796 JUMP_FORWARD            94 (to 986)
+         
+          40     >>  798 LOAD_GLOBAL             28 (console)
+                     810 LOAD_METHOD             15 (status)
+                     832 LOAD_CONST              19 ('[bold green]Getting content...')
+                     834 PRECALL                  1
+                     838 CALL                     1
+                     848 BEFORE_WITH
+                     850 STORE_FAST               5 (status)
+         
+          41         852 LOAD_FAST                3 (driver)
+                     854 LOAD_METHOD             11 (get)
+                     876 LOAD_CONST              17 ('https://pepy.tech/project/')
+                     878 LOAD_FAST                0 (project)
+                     880 FORMAT_VALUE             0
+                     882 BUILD_STRING             2
+                     884 PRECALL                  1
+                     888 CALL                     1
                      898 POP_TOP
          
-          38     >>  900 NOP
-         
-          39         902 LOAD_FAST                2 (driver)
-                     904 LOAD_METHOD             18 (find_elements)
-                     926 LOAD_CONST              22 ('xpath')
-                     928 LOAD_CONST              23 ("//*[contains(@class,'MuiGrid-item')]")
-                     930 PRECALL                  2
-                     934 CALL                     2
-                     944 STORE_FAST               7 (elems)
-         
-          42         946 LOAD_CONST              24 (<code object <listcomp>, file "/home/appinv/code/download-stats/src/download_stats/pepy.py", line 42>)
-                     948 MAKE_FUNCTION            0
-                     950 LOAD_FAST                7 (elems)
-                     952 LOAD_CONST              25 (19)
-                     954 BINARY_SUBSCR
-                     964 LOAD_ATTR               19 (text)
-                     974 LOAD_METHOD             20 (split)
-                     996 LOAD_CONST              26 ('\n')
-                     998 PRECALL                  1
-                    1002 CALL                     1
-                    1012 GET_ITER
-                    1014 PRECALL                  0
-                    1018 CALL                     0
-                    1028 STORE_FAST               8 (by_version)
-         
-          44        1030 BUILD_LIST               0
-                    1032 STORE_FAST               9 (table_data)
-         
-          45        1034 LOAD_CONST              11 (False)
-                    1036 STORE_FAST              10 (start_version_collecting)
-         
-          46        1038 LOAD_GLOBAL             43 (NULL + enumerate)
-                    1050 LOAD_FAST                8 (by_version)
-                    1052 PRECALL                  1
-                    1056 CALL                     1
-                    1066 GET_ITER
-                 >> 1068 FOR_ITER                64 (to 1198)
-                    1070 UNPACK_SEQUENCE          2
-                    1074 STORE_FAST              11 (i)
-                    1076 STORE_FAST              12 (x)
-         
-          47        1078 LOAD_CONST              27 ('Sum')
-                    1080 LOAD_FAST                8 (by_version)
-                    1082 LOAD_FAST               11 (i)
-                    1084 BINARY_SUBSCR
-                    1094 CONTAINS_OP              0
-                    1096 POP_JUMP_FORWARD_IF_FALSE     2 (to 1102)
-         
-          48        1098 LOAD_CONST              28 (True)
-                    1100 STORE_FAST              10 (start_version_collecting)
-         
-          49     >> 1102 LOAD_FAST               10 (start_version_collecting)
-                    1104 POP_JUMP_FORWARD_IF_FALSE    45 (to 1196)
-         
-          50        1106 LOAD_FAST                9 (table_data)
-                    1108 LOAD_METHOD             22 (append)
-                    1130 LOAD_FAST                8 (by_version)
-                    1132 LOAD_FAST               11 (i)
-                    1134 BINARY_SUBSCR
-                    1144 LOAD_METHOD             20 (split)
-                    1166 PRECALL                  0
-                    1170 CALL                     0
-                    1180 PRECALL                  1
-                    1184 CALL                     1
-                    1194 POP_TOP
-                 >> 1196 JUMP_BACKWARD           65 (to 1068)
-         
-          46     >> 1198 JUMP_FORWARD            36 (to 1272)
-                 >> 1200 PUSH_EXC_INFO
-         
-          52        1202 LOAD_GLOBAL             46 (IndexError)
-                    1214 CHECK_EXC_MATCH
-                    1216 POP_JUMP_FORWARD_IF_FALSE    23 (to 1264)
-                    1218 POP_TOP
-         
-          53        1220 LOAD_GLOBAL             49 (NULL + sys)
-                    1232 LOAD_ATTR               25 (exit)
-                    1242 LOAD_CONST              29 ('Package could not be loaded!')
-                    1244 PRECALL                  1
-                    1248 CALL                     1
-                    1258 POP_TOP
-                    1260 POP_EXCEPT
-                    1262 JUMP_FORWARD             4 (to 1272)
-         
-          52     >> 1264 RERAISE                  0
-                 >> 1266 COPY                     3
-                    1268 POP_EXCEPT
-                    1270 RERAISE                  1
-         
-          56     >> 1272 LOAD_FAST                7 (elems)
-                    1274 LOAD_CONST              21 (5)
-                    1276 BINARY_SUBSCR
-                    1286 LOAD_ATTR               19 (text)
-                    1296 LOAD_METHOD             26 (replace)
-                    1318 LOAD_CONST              30 (',')
-                    1320 LOAD_CONST              31 ('')
-                    1322 PRECALL                  2
-                    1326 CALL                     2
-         
-          57        1336 LOAD_FAST                7 (elems)
-                    1338 LOAD_CONST              32 (7)
-                    1340 BINARY_SUBSCR
-                    1350 LOAD_ATTR               19 (text)
-                    1360 LOAD_METHOD             26 (replace)
-                    1382 LOAD_CONST              30 (',')
-                    1384 LOAD_CONST              31 ('')
-                    1386 PRECALL                  2
-                    1390 CALL                     2
-         
-          58        1400 LOAD_FAST                7 (elems)
-                    1402 LOAD_CONST              33 (9)
-                    1404 BINARY_SUBSCR
-                    1414 LOAD_ATTR               19 (text)
-                    1424 LOAD_METHOD             26 (replace)
-                    1446 LOAD_CONST              30 (',')
-                    1448 LOAD_CONST              31 ('')
-                    1450 PRECALL                  2
-                    1454 CALL                     2
-         
-          59        1464 LOAD_FAST                9 (table_data)
-         
-          55        1466 LOAD_CONST              34 (('total', '30_days', '7_days', 'by_version'))
-                    1468 BUILD_CONST_KEY_MAP      4
-                    1470 RETURN_VALUE
+          42         900 LOAD_GLOBAL             25 (NULL + time)
+                     912 LOAD_ATTR               13 (sleep)
+                     922 LOAD_CONST              18 (5)
+                     924 PRECALL                  1
+                     928 CALL                     1
+                     938 POP_TOP
+         
+          40         940 LOAD_CONST               0 (None)
+                     942 LOAD_CONST               0 (None)
+                     944 LOAD_CONST               0 (None)
+                     946 PRECALL                  2
+                     950 CALL                     2
+                     960 POP_TOP
+                     962 JUMP_FORWARD            11 (to 986)
+                 >>  964 PUSH_EXC_INFO
+                     966 WITH_EXCEPT_START
+                     968 POP_JUMP_FORWARD_IF_TRUE     4 (to 978)
+                     970 RERAISE                  2
+                 >>  972 COPY                     3
+                     974 POP_EXCEPT
+                     976 RERAISE                  1
+                 >>  978 POP_TOP
+                     980 POP_EXCEPT
+                     982 POP_TOP
+                     984 POP_TOP
+         
+          44     >>  986 NOP
+         
+          45         988 LOAD_FAST                3 (driver)
+                     990 LOAD_METHOD             16 (find_elements)
+                    1012 LOAD_CONST              20 ('xpath')
+                    1014 LOAD_CONST              21 ("//*[contains(@class,'MuiGrid-item')]")
+                    1016 PRECALL                  2
+                    1020 CALL                     2
+                    1030 STORE_FAST               6 (elems)
+         
+          48        1032 LOAD_CONST              22 (<code object <listcomp>, file "/home/appinv/code/download-stats/src/download_stats/pepy.py", line 48>)
+                    1034 MAKE_FUNCTION            0
+                    1036 LOAD_FAST                6 (elems)
+                    1038 LOAD_CONST              23 (19)
+                    1040 BINARY_SUBSCR
+                    1050 LOAD_ATTR               17 (text)
+                    1060 LOAD_METHOD             18 (split)
+                    1082 LOAD_CONST              24 ('\n')
+                    1084 PRECALL                  1
+                    1088 CALL                     1
+                    1098 GET_ITER
+                    1100 PRECALL                  0
+                    1104 CALL                     0
+                    1114 STORE_FAST               7 (by_version)
+         
+          50        1116 BUILD_LIST               0
+                    1118 STORE_FAST               8 (table_data)
+         
+          51        1120 LOAD_CONST              11 (False)
+                    1122 STORE_FAST               9 (start_version_collecting)
+         
+          52        1124 LOAD_GLOBAL             39 (NULL + enumerate)
+                    1136 LOAD_FAST                7 (by_version)
+                    1138 PRECALL                  1
+                    1142 CALL                     1
+                    1152 GET_ITER
+                 >> 1154 FOR_ITER                64 (to 1284)
+                    1156 UNPACK_SEQUENCE          2
+                    1160 STORE_FAST              10 (i)
+                    1162 STORE_FAST              11 (x)
+         
+          53        1164 LOAD_CONST              25 ('Sum')
+                    1166 LOAD_FAST                7 (by_version)
+                    1168 LOAD_FAST               10 (i)
+                    1170 BINARY_SUBSCR
+                    1180 CONTAINS_OP              0
+                    1182 POP_JUMP_FORWARD_IF_FALSE     2 (to 1188)
+         
+          54        1184 LOAD_CONST              26 (True)
+                    1186 STORE_FAST               9 (start_version_collecting)
+         
+          55     >> 1188 LOAD_FAST                9 (start_version_collecting)
+                    1190 POP_JUMP_FORWARD_IF_FALSE    45 (to 1282)
+         
+          56        1192 LOAD_FAST                8 (table_data)
+                    1194 LOAD_METHOD             20 (append)
+                    1216 LOAD_FAST                7 (by_version)
+                    1218 LOAD_FAST               10 (i)
+                    1220 BINARY_SUBSCR
+                    1230 LOAD_METHOD             18 (split)
+                    1252 PRECALL                  0
+                    1256 CALL                     0
+                    1266 PRECALL                  1
+                    1270 CALL                     1
+                    1280 POP_TOP
+                 >> 1282 JUMP_BACKWARD           65 (to 1154)
+         
+          52     >> 1284 JUMP_FORWARD            36 (to 1358)
+                 >> 1286 PUSH_EXC_INFO
+         
+          58        1288 LOAD_GLOBAL             42 (IndexError)
+                    1300 CHECK_EXC_MATCH
+                    1302 POP_JUMP_FORWARD_IF_FALSE    23 (to 1350)
+                    1304 POP_TOP
+         
+          59        1306 LOAD_GLOBAL             45 (NULL + sys)
+                    1318 LOAD_ATTR               23 (exit)
+                    1328 LOAD_CONST              27 ('Package could not be loaded!')
+                    1330 PRECALL                  1
+                    1334 CALL                     1
+                    1344 POP_TOP
+                    1346 POP_EXCEPT
+                    1348 JUMP_FORWARD             4 (to 1358)
+         
+          58     >> 1350 RERAISE                  0
+                 >> 1352 COPY                     3
+                    1354 POP_EXCEPT
+                    1356 RERAISE                  1
+         
+          62     >> 1358 LOAD_FAST                6 (elems)
+                    1360 LOAD_CONST              18 (5)
+                    1362 BINARY_SUBSCR
+                    1372 LOAD_ATTR               17 (text)
+                    1382 LOAD_METHOD             24 (replace)
+                    1404 LOAD_CONST              28 (',')
+                    1406 LOAD_CONST              29 ('')
+                    1408 PRECALL                  2
+                    1412 CALL                     2
+         
+          63        1422 LOAD_FAST                6 (elems)
+                    1424 LOAD_CONST              30 (7)
+                    1426 BINARY_SUBSCR
+                    1436 LOAD_ATTR               17 (text)
+                    1446 LOAD_METHOD             24 (replace)
+                    1468 LOAD_CONST              28 (',')
+                    1470 LOAD_CONST              29 ('')
+                    1472 PRECALL                  2
+                    1476 CALL                     2
+         
+          64        1486 LOAD_FAST                6 (elems)
+                    1488 LOAD_CONST              31 (9)
+                    1490 BINARY_SUBSCR
+                    1500 LOAD_ATTR               17 (text)
+                    1510 LOAD_METHOD             24 (replace)
+                    1532 LOAD_CONST              28 (',')
+                    1534 LOAD_CONST              29 ('')
+                    1536 PRECALL                  2
+                    1540 CALL                     2
+         
+          65        1550 LOAD_FAST                8 (table_data)
+         
+          61        1552 LOAD_CONST              32 (('total', '30_days', '7_days', 'by_version'))
+                    1554 BUILD_CONST_KEY_MAP      4
+                    1556 RETURN_VALUE
          ExceptionTable:
-           764 to 852 -> 878 [1] lasti
-           878 to 884 -> 886 [3] lasti
-           892 to 892 -> 886 [3] lasti
-           902 to 1196 -> 1200 [0]
-           1200 to 1258 -> 1266 [1] lasti
-           1264 to 1264 -> 1266 [1] lasti
+           850 to 938 -> 964 [1] lasti
+           964 to 970 -> 972 [3] lasti
+           978 to 978 -> 972 [3] lasti
+           988 to 1282 -> 1286 [0]
+           1286 to 1344 -> 1352 [1] lasti
+           1350 to 1350 -> 1352 [1] lasti
          consts
             None
             '--headless'
             '--incognito'
             '--nogpu'
             '--disable-gpu'
             '--window-size=1280,1280'
@@ -472,31 +487,29 @@
             '--enable-javascript'
             'excludeSwitches'
             'enable-automation'
             'useAutomationExtension'
             False
             '--disable-blink-features=AutomationControlled'
             ('service', 'options')
-            0
-            ('get_latest_user_agents', 'get_random_user_agent')
             "Object.defineProperty(navigator, 'webdriver', {get: () => undefined})"
             'Network.setUserAgentOverride'
             'userAgent'
-            '[bold green]Getting content...'
             'https://pepy.tech/project/'
             5
+            '[bold green]Getting content...'
             'xpath'
             "//*[contains(@class,'MuiGrid-item')]"
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code 0x970067007c005d047d017c0191028c055300
-                42           0 RESUME                   0
+                48           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                 4 (to 16)
                              8 STORE_FAST               1 (e)
                             10 LOAD_FAST                1 (e)
                             12 LIST_APPEND              2
                             14 JUMP_BACKWARD            5 (to 6)
@@ -504,38 +517,39 @@
                consts
                names      ()
                varnames   ('.0', 'e')
                freevars   ()
                cellvars   ()
                filename   '/home/appinv/code/download-stats/src/download_stats/pepy.py'
                name       '<listcomp>'
-               firstlineno 42
+               firstlineno 48
                lnotab 0x
             19
             '\n'
             'Sum'
             True
             'Package could not be loaded!'
             ','
             ''
             7
             9
             ('total', '30_days', '7_days', 'by_version')
-         names      ('Options', 'add_argument', 'add_experimental_option', 'webdriver', 'Chrome', 'Service', 'ChromeDriverManager', 'install', 'latest_user_agents', 'get_latest_user_agents', 'get_random_user_agent', 'execute_script', 'execute_cdp_cmd', 'console', 'status', 'get', 'time', 'sleep', 'find_elements', 'text', 'split', 'enumerate', 'append', 'IndexError', 'sys', 'exit', 'replace')
-         varnames   ('project', 'options', 'driver', 'get_latest_user_agents', 'get_random_user_agent', 'userAgent', 'status', 'elems', 'by_version', 'table_data', 'start_version_collecting', 'i', 'x')
+         names      ('Options', 'add_argument', 'add_experimental_option', 'webdriver', 'Chrome', 'Service', 'ChromeDriverManager', 'install', 'get_random_user_agent', 'execute_script', 'execute_cdp_cmd', 'get', 'time', 'sleep', 'console', 'status', 'find_elements', 'text', 'split', 'enumerate', 'append', 'IndexError', 'sys', 'exit', 'replace')
+         varnames   ('project', 'no_rich', 'options', 'driver', 'userAgent', 'status', 'elems', 'by_version', 'table_data', 'start_version_collecting', 'i', 'x')
          freevars   ()
          cellvars   ()
          filename   '/home/appinv/code/download-stats/src/download_stats/pepy.py'
          name       'stats'
-         firstlineno 14
+         firstlineno 15
          lnotab
-            0x02011c012a012a012a012a012a012a012a012e012c012a018201100414
-            012a0130013601300128fe2e0402012c0354020401040128011401040104
-            015cfc040612012cff080440014001400102fc
-   names      ('selenium.webdriver.chrome.service', 'Service', 'webdriver_manager.chrome', 'ChromeDriverManager', 'selenium.webdriver.support.ui', 'WebDriverWait', 'selenium.webdriver.chrome.options', 'Options', 'selenium', 'webdriver', 'fake_useragent', 'UserAgent', 'rich.console', 'Console', 'time', 'sys', 'console', 'str', 'dict', 'stats')
+            0x02011c012a012a012a012a012a012a012a012e012c012a0182051c012a
+            013002040130012a023601300128fe2e0402012c03540204010401280114
+            01040104015cfc040612012cff080440014001400102fc
+      (False,)
+   names      ('selenium.webdriver.chrome.service', 'Service', 'webdriver_manager.chrome', 'ChromeDriverManager', 'selenium.webdriver.support.ui', 'WebDriverWait', 'selenium.webdriver.chrome.options', 'Options', 'selenium', 'webdriver', 'latest_user_agents', 'get_random_user_agent', 'rich.console', 'Console', 'time', 'sys', 'console', 'str', 'dict', 'stats')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/appinv/code/download-stats/src/download_stats/pepy.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c010c010c010c010c010c01080108021403
+   lnotab 0x00ff02010c010c010c010c010c020c010c01080108021403
```

### Comparing `download_stats-1.2.1/src/download_stats/__pycache__/pypistats.cpython-311.pyc` & `download_stats-1.3.0/src/download_stats/__pycache__/pypistats.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.1/src/download_stats/main.py` & `download_stats-1.3.0/src/download_stats/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,20 +67,33 @@
     for i, r in enumerate(data['by_version']):
         if i > 0:
             table.add_row(r[0], r[1], r[2], r[3], r[4], r[5])
 
     console = Console()
     console.print(table)
 
+def combined_downloads(projects):
+    total = 0
+    for p in projects:
+        total += int(stats(p)['total'])
+
+    console = Console()
+    console.print('Total downloads for projects:')
+    console.print(', '.join(projects))
+    console.print('[green]'+str(total)+'[/green]')
+
 def main():
     if len(sys.argv) == 1:
         sys.exit('Package args needed!')
     if not sys.argv[1].startswith('--'):
         summary_table(sys.argv[1])
     if sys.argv[1].casefold() == '--compare':
         if len(sys.argv) >= 3:
             compare_table(sys.argv[2:])
+    if sys.argv[1].casefold() == '--total':
+        if len(sys.argv) >= 3:
+            combined_downloads(sys.argv[2:])
     if sys.argv[1].casefold() == '--self':
         summary_table('download-stats')
```

### Comparing `download_stats-1.2.1/src/download_stats/pepy.py` & `download_stats-1.3.0/src/download_stats/pepy.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from rich.console import Console
 import time
 import sys
 
 console = Console()
 
 
-def stats(project: str) -> dict:
+def stats(project: str, no_rich=False) -> dict:
     options = Options()
     options.add_argument('--headless')
     options.add_argument("--incognito")
     options.add_argument("--nogpu")
     options.add_argument("--disable-gpu")
     options.add_argument("--window-size=1280,1280")
     options.add_argument("--no-sandbox")
@@ -28,17 +28,22 @@
     
     #ua = UserAgent()
     #ua = get_random_user_agent()
     #userAgent = ua.random
     userAgent = get_random_user_agent()
     driver.execute_script("Object.defineProperty(navigator, 'webdriver', {get: () => undefined})")
     driver.execute_cdp_cmd('Network.setUserAgentOverride', {"userAgent": userAgent})
-    with console.status("[bold green]Getting content...") as status:
+
+    if no_rich:
         driver.get(f'https://pepy.tech/project/{project}')
         time.sleep(5)
+    else:
+        with console.status("[bold green]Getting content...") as status:
+            driver.get(f'https://pepy.tech/project/{project}')
+            time.sleep(5)
 
     try:
         elems = driver.find_elements('xpath', "//*[contains(@class,'MuiGrid-item')]")
         # for i, e in enumerate(elems):
         #     print(i, e.text)
         by_version = [e for e in elems[19].text.split('\n')]
```

### Comparing `download_stats-1.2.1/src/download_stats/pypistats.py` & `download_stats-1.3.0/src/download_stats/pypistats.py`

 * *Files identical despite different names*

### Comparing `download_stats-1.2.1/src/download_stats.egg-info/PKG-INFO` & `download_stats-1.3.0/src/download_stats.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download-stats
-Version: 1.2.1
+Version: 1.3.0
 Summary: Download stats for Python packages
 Home-page: UNKNOWN
 Author-email: arj.python@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/Abdur-RahmaanJ/download-stats/issues
 Project-URL: Source, https://github.com/Abdur-RahmaanJ/download-stats/
 Platform: UNKNOWN
@@ -40,14 +40,20 @@
 ![](https://github.com/Abdur-RahmaanJ/download-stats/raw/stable/assets/compare.png)
 
 
 ```
 $ download-stats --self # same as `download-stats download-stats`
 ```
 
+Total downloads
+
+```
+$ download-stats --total hooman shopyo download-stats meteomoris newsmoris shopcube honeybot jamstack
+```
+
 ## general
 
 ```python
 >>> from download_stats import stats 
 >>> stats('shopyo')
 {
     "total": "41327",
```

### Comparing `download_stats-1.2.1/src/download_stats.egg-info/SOURCES.txt` & `download_stats-1.3.0/src/download_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

