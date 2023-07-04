# Comparing `tmp/st_blogpost_component-0.0.4.tar.gz` & `tmp/st_blogpost_component-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_blogpost_component-0.0.4.tar", last modified: Tue Jul  4 17:08:58 2023, max compression
+gzip compressed data, was "st_blogpost_component-0.0.5.tar", last modified: Tue Jul  4 17:53:45 2023, max compression
```

## Comparing `st_blogpost_component-0.0.4.tar` & `st_blogpost_component-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:08:58.256250 st_blogpost_component-0.0.4/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1063 2023-07-04 03:12:34.000000 st_blogpost_component-0.0.4/LICENSE
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       57 2023-07-04 04:48:07.000000 st_blogpost_component-0.0.4/MANIFEST.in
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 17:08:58.256250 st_blogpost_component-0.0.4/PKG-INFO
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       38 2023-07-04 17:08:58.256250 st_blogpost_component-0.0.4/setup.cfg
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      628 2023-07-04 17:08:45.000000 st_blogpost_component-0.0.4/setup.py
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:08:58.248250 st_blogpost_component-0.0.4/st_blogpost_component/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     3749 2023-07-04 17:07:00.000000 st_blogpost_component-0.0.4/st_blogpost_component/__init__.py
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:08:58.248250 st_blogpost_component-0.0.4/st_blogpost_component/frontend/
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:08:58.252250 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      691 2023-07-04 17:06:53.000000 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/asset-manifest.json
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   197459 2023-07-04 17:06:35.000000 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/bootstrap.min.css
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2087 2023-07-04 17:06:53.000000 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/index.html
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:08:58.248250 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:08:58.256250 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   557241 2023-07-04 17:06:53.000000 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2243 2023-07-04 17:06:53.000000 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)  2141267 2023-07-04 17:06:53.000000 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1642 2023-07-04 17:06:53.000000 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/main.060e67f4.chunk.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     4665 2023-07-04 17:06:53.000000 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/main.060e67f4.chunk.js.map
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1584 2023-07-04 17:06:53.000000 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     8369 2023-07-04 17:06:53.000000 st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:08:58.252250 st_blogpost_component-0.0.4/st_blogpost_component.egg-info/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 17:08:58.000000 st_blogpost_component-0.0.4/st_blogpost_component.egg-info/PKG-INFO
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      955 2023-07-04 17:08:58.000000 st_blogpost_component-0.0.4/st_blogpost_component.egg-info/SOURCES.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)        1 2023-07-04 17:08:58.000000 st_blogpost_component-0.0.4/st_blogpost_component.egg-info/dependency_links.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       16 2023-07-04 17:08:58.000000 st_blogpost_component-0.0.4/st_blogpost_component.egg-info/requires.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       22 2023-07-04 17:08:58.000000 st_blogpost_component-0.0.4/st_blogpost_component.egg-info/top_level.txt
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:53:45.370092 st_blogpost_component-0.0.5/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1063 2023-07-04 03:12:34.000000 st_blogpost_component-0.0.5/LICENSE
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       57 2023-07-04 04:48:07.000000 st_blogpost_component-0.0.5/MANIFEST.in
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 17:53:45.370092 st_blogpost_component-0.0.5/PKG-INFO
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       38 2023-07-04 17:53:45.370092 st_blogpost_component-0.0.5/setup.cfg
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      628 2023-07-04 17:52:57.000000 st_blogpost_component-0.0.5/setup.py
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:53:45.362091 st_blogpost_component-0.0.5/st_blogpost_component/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     3532 2023-07-04 17:52:14.000000 st_blogpost_component-0.0.5/st_blogpost_component/__init__.py
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:53:45.362091 st_blogpost_component-0.0.5/st_blogpost_component/frontend/
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:53:45.366091 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      691 2023-07-04 17:53:08.000000 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/asset-manifest.json
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   197459 2023-07-04 17:52:50.000000 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/bootstrap.min.css
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2087 2023-07-04 17:53:08.000000 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/index.html
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:53:45.362091 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:53:45.370092 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   557241 2023-07-04 17:53:08.000000 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2243 2023-07-04 17:53:08.000000 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)  2141267 2023-07-04 17:53:08.000000 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1676 2023-07-04 17:53:08.000000 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/main.5833844e.chunk.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     4845 2023-07-04 17:53:08.000000 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/main.5833844e.chunk.js.map
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1584 2023-07-04 17:53:08.000000 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     8369 2023-07-04 17:53:08.000000 st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 17:53:45.362091 st_blogpost_component-0.0.5/st_blogpost_component.egg-info/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 17:53:45.000000 st_blogpost_component-0.0.5/st_blogpost_component.egg-info/PKG-INFO
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      955 2023-07-04 17:53:45.000000 st_blogpost_component-0.0.5/st_blogpost_component.egg-info/SOURCES.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)        1 2023-07-04 17:53:45.000000 st_blogpost_component-0.0.5/st_blogpost_component.egg-info/dependency_links.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       16 2023-07-04 17:53:45.000000 st_blogpost_component-0.0.5/st_blogpost_component.egg-info/requires.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       22 2023-07-04 17:53:45.000000 st_blogpost_component-0.0.5/st_blogpost_component.egg-info/top_level.txt
```

### Comparing `st_blogpost_component-0.0.4/LICENSE` & `st_blogpost_component-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.4/setup.py` & `st_blogpost_component-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_blogpost_component",
-    version="0.0.4",
+    version="0.0.5",
     author="YM",
     author_email="",
     description="",
     long_description="custom component to display blog post card for personal blog",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/__init__.py` & `st_blogpost_component-0.0.5/st_blogpost_component/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,235 +1,221 @@
 00000000: 696d 706f 7274 206f 730a 696d 706f 7274  import os.import
 00000010: 2073 7472 6561 6d6c 6974 2e63 6f6d 706f   streamlit.compo
 00000020: 6e65 6e74 732e 7631 2061 7320 636f 6d70  nents.v1 as comp
-00000030: 6f6e 656e 7473 0a0a 2320 4372 6561 7465  onents..# Create
-00000040: 2061 205f 5245 4c45 4153 4520 636f 6e73   a _RELEASE cons
-00000050: 7461 6e74 2e20 5765 276c 6c20 7365 7420  tant. We'll set 
-00000060: 7468 6973 2074 6f20 4661 6c73 6520 7768  this to False wh
-00000070: 696c 6520 7765 2772 6520 6465 7665 6c6f  ile we're develo
-00000080: 7069 6e67 0a23 2074 6865 2063 6f6d 706f  ping.# the compo
-00000090: 6e65 6e74 2c20 616e 6420 5472 7565 2077  nent, and True w
-000000a0: 6865 6e20 7765 2772 6520 7265 6164 7920  hen we're ready 
-000000b0: 746f 2070 6163 6b61 6765 2061 6e64 2064  to package and d
-000000c0: 6973 7472 6962 7574 6520 6974 2e0a 2320  istribute it..# 
-000000d0: 2854 6869 7320 6973 2c20 6f66 2063 6f75  (This is, of cou
-000000e0: 7273 652c 206f 7074 696f 6e61 6c20 2d20  rse, optional - 
-000000f0: 7468 6572 6520 6172 6520 696e 6e75 6d65  there are innume
-00000100: 7261 626c 6520 7761 7973 2074 6f20 6d61  rable ways to ma
-00000110: 6e61 6765 2079 6f75 720a 2320 7265 6c65  nage your.# rele
-00000120: 6173 6520 7072 6f63 6573 732e 290a 5f52  ase process.)._R
-00000130: 454c 4541 5345 203d 2054 7275 650a 0a23  ELEASE = True..#
-00000140: 2044 6563 6c61 7265 2061 2053 7472 6561   Declare a Strea
-00000150: 6d6c 6974 2063 6f6d 706f 6e65 6e74 2e20  mlit component. 
-00000160: 6064 6563 6c61 7265 5f63 6f6d 706f 6e65  `declare_compone
-00000170: 6e74 6020 7265 7475 726e 7320 6120 6675  nt` returns a fu
-00000180: 6e63 7469 6f6e 0a23 2074 6861 7420 6973  nction.# that is
-00000190: 2075 7365 6420 746f 2063 7265 6174 6520   used to create 
-000001a0: 696e 7374 616e 6365 7320 6f66 2074 6865  instances of the
-000001b0: 2063 6f6d 706f 6e65 6e74 2e20 5765 2772   component. We'r
-000001c0: 6520 6e61 6d69 6e67 2074 6869 730a 2320  e naming this.# 
-000001d0: 6675 6e63 7469 6f6e 2022 5f63 6f6d 706f  function "_compo
-000001e0: 6e65 6e74 5f66 756e 6322 2c20 7769 7468  nent_func", with
-000001f0: 2061 6e20 756e 6465 7273 636f 7265 2070   an underscore p
-00000200: 7265 6669 782c 2062 6563 6175 7365 2077  refix, because w
-00000210: 6520 646f 6e27 7420 7761 6e74 0a23 2074  e don't want.# t
-00000220: 6f20 6578 706f 7365 2069 7420 6469 7265  o expose it dire
-00000230: 6374 6c79 2074 6f20 7573 6572 732e 2049  ctly to users. I
-00000240: 6e73 7465 6164 2c20 7765 2077 696c 6c20  nstead, we will 
-00000250: 6372 6561 7465 2061 2063 7573 746f 6d20  create a custom 
-00000260: 7772 6170 7065 720a 2320 6675 6e63 7469  wrapper.# functi
-00000270: 6f6e 2c20 6265 6c6f 772c 2074 6861 7420  on, below, that 
-00000280: 7769 6c6c 2073 6572 7665 2061 7320 6f75  will serve as ou
-00000290: 7220 636f 6d70 6f6e 656e 7427 7320 7075  r component's pu
-000002a0: 626c 6963 2041 5049 2e0a 0a23 2049 7427  blic API...# It'
-000002b0: 7320 776f 7274 6820 6e6f 7469 6e67 2074  s worth noting t
-000002c0: 6861 7420 7468 6973 2063 616c 6c20 746f  hat this call to
-000002d0: 2060 6465 636c 6172 655f 636f 6d70 6f6e   `declare_compon
-000002e0: 656e 7460 2069 7320 7468 650a 2320 2a6f  ent` is the.# *o
-000002f0: 6e6c 7920 7468 696e 672a 2079 6f75 206e  nly thing* you n
-00000300: 6565 6420 746f 2064 6f20 746f 2063 7265  eed to do to cre
-00000310: 6174 6520 7468 6520 6269 6e64 696e 6720  ate the binding 
-00000320: 6265 7477 6565 6e20 5374 7265 616d 6c69  between Streamli
-00000330: 7420 616e 640a 2320 796f 7572 2063 6f6d  t and.# your com
-00000340: 706f 6e65 6e74 2066 726f 6e74 656e 642e  ponent frontend.
-00000350: 2045 7665 7279 7468 696e 6720 656c 7365   Everything else
-00000360: 2077 6520 646f 2069 6e20 7468 6973 2066   we do in this f
-00000370: 696c 6520 6973 2073 696d 706c 7920 610a  ile is simply a.
-00000380: 2320 6265 7374 2070 7261 6374 6963 652e  # best practice.
-00000390: 0a0a 6966 206e 6f74 205f 5245 4c45 4153  ..if not _RELEAS
-000003a0: 453a 0a20 2020 205f 636f 6d70 6f6e 656e  E:.    _componen
-000003b0: 745f 6675 6e63 203d 2063 6f6d 706f 6e65  t_func = compone
-000003c0: 6e74 732e 6465 636c 6172 655f 636f 6d70  nts.declare_comp
-000003d0: 6f6e 656e 7428 0a20 2020 2020 2020 2023  onent(.        #
-000003e0: 2057 6520 6769 7665 2074 6865 2063 6f6d   We give the com
-000003f0: 706f 6e65 6e74 2061 2073 696d 706c 652c  ponent a simple,
-00000400: 2064 6573 6372 6970 7469 7665 206e 616d   descriptive nam
-00000410: 6520 2822 6d79 5f63 6f6d 706f 6e65 6e74  e ("my_component
-00000420: 220a 2020 2020 2020 2020 2320 646f 6573  ".        # does
-00000430: 206e 6f74 2066 6974 2074 6869 7320 6269   not fit this bi
-00000440: 6c6c 2c20 736f 2070 6c65 6173 6520 6368  ll, so please ch
-00000450: 6f6f 7365 2073 6f6d 6574 6869 6e67 2062  oose something b
-00000460: 6574 7465 7220 666f 7220 796f 7572 0a20  etter for your. 
-00000470: 2020 2020 2020 2023 206f 776e 2063 6f6d         # own com
-00000480: 706f 6e65 6e74 203a 290a 2020 2020 2020  ponent :).      
-00000490: 2020 226d 795f 636f 6d70 6f6e 656e 7422    "my_component"
-000004a0: 2c0a 2020 2020 2020 2020 2320 5061 7373  ,.        # Pass
-000004b0: 2060 7572 6c60 2068 6572 6520 746f 2074   `url` here to t
-000004c0: 656c 6c20 5374 7265 616d 6c69 7420 7468  ell Streamlit th
-000004d0: 6174 2074 6865 2063 6f6d 706f 6e65 6e74  at the component
-000004e0: 2077 696c 6c20 6265 2073 6572 7665 640a   will be served.
-000004f0: 2020 2020 2020 2020 2320 6279 2074 6865          # by the
-00000500: 206c 6f63 616c 2064 6576 2073 6572 7665   local dev serve
-00000510: 7220 7468 6174 2079 6f75 2072 756e 2076  r that you run v
-00000520: 6961 2060 6e70 6d20 7275 6e20 7374 6172  ia `npm run star
-00000530: 7460 2e0a 2020 2020 2020 2020 2320 2854  t`..        # (T
-00000540: 6869 7320 6973 2075 7365 6675 6c20 7768  his is useful wh
-00000550: 696c 6520 796f 7572 2063 6f6d 706f 6e65  ile your compone
-00000560: 6e74 2069 7320 696e 2064 6576 656c 6f70  nt is in develop
-00000570: 6d65 6e74 2e29 0a20 2020 2020 2020 2075  ment.).        u
-00000580: 726c 3d22 6874 7470 3a2f 2f31 3932 2e31  rl="http://192.1
-00000590: 3638 2e32 2e34 363a 3330 3031 2f22 2c0a  68.2.46:3001/",.
-000005a0: 2020 2020 290a 656c 7365 3a0a 2020 2020      ).else:.    
-000005b0: 2320 5768 656e 2077 6527 7265 2064 6973  # When we're dis
-000005c0: 7472 6962 7574 696e 6720 6120 7072 6f64  tributing a prod
-000005d0: 7563 7469 6f6e 2076 6572 7369 6f6e 206f  uction version o
-000005e0: 6620 7468 6520 636f 6d70 6f6e 656e 742c  f the component,
-000005f0: 2077 6527 6c6c 0a20 2020 2023 2072 6570   we'll.    # rep
-00000600: 6c61 6365 2074 6865 2060 7572 6c60 2070  lace the `url` p
-00000610: 6172 616d 2077 6974 6820 6070 6174 6860  aram with `path`
-00000620: 2c20 616e 6420 706f 696e 7420 6974 2074  , and point it t
-00000630: 6f20 746f 2074 6865 2063 6f6d 706f 6e65  o to the compone
-00000640: 6e74 2773 0a20 2020 2023 2062 7569 6c64  nt's.    # build
-00000650: 2064 6972 6563 746f 7279 3a0a 2020 2020   directory:.    
-00000660: 7061 7265 6e74 5f64 6972 203d 206f 732e  parent_dir = os.
-00000670: 7061 7468 2e64 6972 6e61 6d65 286f 732e  path.dirname(os.
-00000680: 7061 7468 2e61 6273 7061 7468 285f 5f66  path.abspath(__f
-00000690: 696c 655f 5f29 290a 2020 2020 6275 696c  ile__)).    buil
-000006a0: 645f 6469 7220 3d20 6f73 2e70 6174 682e  d_dir = os.path.
-000006b0: 6a6f 696e 2870 6172 656e 745f 6469 722c  join(parent_dir,
-000006c0: 2022 6672 6f6e 7465 6e64 2f62 7569 6c64   "frontend/build
-000006d0: 2229 0a20 2020 205f 636f 6d70 6f6e 656e  ").    _componen
-000006e0: 745f 6675 6e63 203d 2063 6f6d 706f 6e65  t_func = compone
-000006f0: 6e74 732e 6465 636c 6172 655f 636f 6d70  nts.declare_comp
-00000700: 6f6e 656e 7428 226d 795f 636f 6d70 6f6e  onent("my_compon
-00000710: 656e 7422 2c20 7061 7468 3d62 7569 6c64  ent", path=build
-00000720: 5f64 6972 290a 0a0a 2320 4372 6561 7465  _dir)...# Create
-00000730: 2061 2077 7261 7070 6572 2066 756e 6374   a wrapper funct
-00000740: 696f 6e20 666f 7220 7468 6520 636f 6d70  ion for the comp
-00000750: 6f6e 656e 742e 2054 6869 7320 6973 2061  onent. This is a
-00000760: 6e20 6f70 7469 6f6e 616c 0a23 2062 6573  n optional.# bes
-00000770: 7420 7072 6163 7469 6365 202d 2077 6520  t practice - we 
-00000780: 636f 756c 6420 7369 6d70 6c79 2065 7870  could simply exp
-00000790: 6f73 6520 7468 6520 636f 6d70 6f6e 656e  ose the componen
-000007a0: 7420 6675 6e63 7469 6f6e 2072 6574 7572  t function retur
-000007b0: 6e65 6420 6279 0a23 2060 6465 636c 6172  ned by.# `declar
-000007c0: 655f 636f 6d70 6f6e 656e 7460 2061 6e64  e_component` and
-000007d0: 2063 616c 6c20 6974 2064 6f6e 652e 2054   call it done. T
-000007e0: 6865 2077 7261 7070 6572 2061 6c6c 6f77  he wrapper allow
-000007f0: 7320 7573 2074 6f20 6375 7374 6f6d 697a  s us to customiz
-00000800: 650a 2320 6f75 7220 636f 6d70 6f6e 656e  e.# our componen
-00000810: 7427 7320 4150 493a 2077 6520 6361 6e20  t's API: we can 
-00000820: 7072 652d 7072 6f63 6573 7320 6974 7320  pre-process its 
-00000830: 696e 7075 7420 6172 6773 2c20 706f 7374  input args, post
-00000840: 2d70 726f 6365 7373 2069 7473 0a23 206f  -process its.# o
-00000850: 7574 7075 7420 7661 6c75 652c 2061 6e64  utput value, and
-00000860: 2061 6464 2061 2064 6f63 7374 7269 6e67   add a docstring
-00000870: 2066 6f72 2075 7365 7273 2e0a 6465 6620   for users..def 
-00000880: 626c 6f67 5f63 6172 645f 636f 6d70 6f6e  blog_card_compon
-00000890: 656e 7428 7469 746c 652c 2073 7562 7469  ent(title, subti
-000008a0: 746c 652c 206c 696e 6b2c 2067 6974 6875  tle, link, githu
-000008b0: 622c 2069 6d67 5f70 6174 682c 2064 6573  b, img_path, des
-000008c0: 6372 6970 7469 6f6e 2c20 706f 7374 293a  cription, post):
-000008d0: 0a20 2020 2022 2222 4372 6561 7465 2061  .    """Create a
-000008e0: 206e 6577 2069 6e73 7461 6e63 6520 6f66   new instance of
-000008f0: 2022 6361 7264 5f63 6f6d 706f 6e65 6e74   "card_component
-00000900: 222e 0a20 2020 2022 2222 0a20 2020 2023  "..    """.    #
-00000910: 2074 6865 2062 656c 6f77 2069 6e69 7469   the below initi
-00000920: 616c 697a 6573 2074 6865 2072 6561 6374  alizes the react
-00000930: 2063 6f6d 706f 6e65 6e74 2028 696e 2043   component (in C
-00000940: 6172 6443 6f6d 706f 6e65 6e74 2e74 7378  ardComponent.tsx
-00000950: 290a 2020 2020 636f 6d70 6f6e 656e 745f  ).    component_
-00000960: 7661 6c75 6520 3d20 5f63 6f6d 706f 6e65  value = _compone
-00000970: 6e74 5f66 756e 6328 0a20 2020 2020 2020  nt_func(.       
-00000980: 2074 6974 6c65 3d74 6974 6c65 2c0a 2020   title=title,.  
-00000990: 2020 2020 2020 7375 6274 6974 6c65 3d73        subtitle=s
-000009a0: 7562 7469 746c 652c 0a20 2020 2020 2020  ubtitle,.       
-000009b0: 2064 6573 6372 6970 7469 6f6e 3d64 6573   description=des
-000009c0: 6372 6970 7469 6f6e 2c0a 2020 2020 2020  cription,.      
-000009d0: 2020 6c69 6e6b 3d6c 696e 6b2c 0a20 2020    link=link,.   
-000009e0: 2020 2020 2067 6974 6875 623d 6769 7468       github=gith
-000009f0: 7562 2c0a 2020 2020 2020 2020 706f 7374  ub,.        post
-00000a00: 3d70 6f73 742c 0a20 2020 2020 2020 2069  =post,.        i
-00000a10: 6d67 5f70 6174 683d 696d 675f 7061 7468  mg_path=img_path
-00000a20: 0a20 2020 2029 0a0a 2020 2020 2320 5765  .    )..    # We
-00000a30: 2063 6f75 6c64 206d 6f64 6966 7920 7468   could modify th
-00000a40: 6520 7661 6c75 6520 7265 7475 726e 6564  e value returned
-00000a50: 2066 726f 6d20 7468 6520 636f 6d70 6f6e   from the compon
-00000a60: 656e 7420 6966 2077 6520 7761 6e74 6564  ent if we wanted
-00000a70: 2e0a 2020 2020 2320 5468 6572 6527 7320  ..    # There's 
-00000a80: 6e6f 206e 6565 6420 746f 2064 6f20 7468  no need to do th
-00000a90: 6973 2069 6e20 6f75 7220 7369 6d70 6c65  is in our simple
-00000aa0: 2065 7861 6d70 6c65 202d 2062 7574 2069   example - but i
-00000ab0: 7427 7320 616e 206f 7074 696f 6e2e 0a20  t's an option.. 
-00000ac0: 2020 2072 6574 7572 6e20 636f 6d70 6f6e     return compon
-00000ad0: 656e 745f 7661 6c75 650a 0a0a 2320 4164  ent_value...# Ad
-00000ae0: 6420 736f 6d65 2074 6573 7420 636f 6465  d some test code
-00000af0: 2074 6f20 706c 6179 2077 6974 6820 7468   to play with th
-00000b00: 6520 636f 6d70 6f6e 656e 7420 7768 696c  e component whil
-00000b10: 6520 6974 2773 2069 6e20 6465 7665 6c6f  e it's in develo
-00000b20: 706d 656e 742e 0a23 2044 7572 696e 6720  pment..# During 
-00000b30: 6465 7665 6c6f 706d 656e 742c 2077 6520  development, we 
-00000b40: 6361 6e20 7275 6e20 7468 6973 206a 7573  can run this jus
-00000b50: 7420 6173 2077 6520 776f 756c 6420 616e  t as we would an
-00000b60: 7920 6f74 6865 7220 5374 7265 616d 6c69  y other Streamli
-00000b70: 740a 2320 6170 703a 2060 2420 7374 7265  t.# app: `$ stre
-00000b80: 616d 6c69 7420 7275 6e20 6d79 5f63 6f6d  amlit run my_com
-00000b90: 706f 6e65 6e74 2f5f 5f69 6e69 745f 5f2e  ponent/__init__.
-00000ba0: 7079 600a 6966 206e 6f74 205f 5245 4c45  py`.if not _RELE
-00000bb0: 4153 453a 0a20 2020 2069 6d70 6f72 7420  ASE:.    import 
-00000bc0: 7374 7265 616d 6c69 7420 6173 2073 740a  streamlit as st.
-00000bd0: 0a20 2020 2073 742e 7375 6268 6561 6465  .    st.subheade
-00000be0: 7228 2243 6f6d 706f 6e65 6e74 2077 6974  r("Component wit
-00000bf0: 6820 636f 6e73 7461 6e74 2061 7267 7322  h constant args"
-00000c00: 290a 0a20 2020 2023 2043 7265 6174 6520  )..    # Create 
-00000c10: 616e 2069 6e73 7461 6e63 6520 6f66 206f  an instance of o
-00000c20: 7572 2063 6f6d 706f 6e65 6e74 2077 6974  ur component wit
-00000c30: 6820 6120 636f 6e73 7461 6e74 2060 6e61  h a constant `na
-00000c40: 6d65 6020 6172 672c 2061 6e64 0a20 2020  me` arg, and.   
-00000c50: 2023 2070 7269 6e74 2069 7473 206f 7574   # print its out
-00000c60: 7075 7420 7661 6c75 652e 0a20 2020 2075  put value..    u
-00000c70: 726c 203d 2062 6c6f 675f 6361 7264 5f63  rl = blog_card_c
-00000c80: 6f6d 706f 6e65 6e74 2822 5065 7273 6f6e  omponent("Person
-00000c90: 616c 2062 6163 6b65 6e64 222c 2022 5079  al backend", "Py
-00000ca0: 7468 6f6e 3a20 4661 7374 4170 692c 2053  thon: FastApi, S
-00000cb0: 514c 4d6f 6465 6c2c 2052 6561 6374 3a72  QLModel, React:r
-00000cc0: 6561 6374 2d61 646d 696e 222c 2022 6874  eact-admin", "ht
-00000cd0: 7470 733a 2f2f 7065 7273 6f6e 616c 2d73  tps://personal-s
-00000ce0: 6974 652d 6261 636b 656e 642d 7072 6f64  ite-backend-prod
-00000cf0: 7563 7469 6f6e 2e75 702e 7261 696c 7761  uction.up.railwa
-00000d00: 792e 6170 702f 646f 6373 222c 2022 6874  y.app/docs", "ht
-00000d10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000d20: 2f79 6173 7369 6e65 2d6d 6865 6468 6269  /yassine-mhedhbi
-00000d30: 2f70 6572 736f 6e61 6c2d 7369 7465 2d62  /personal-site-b
-00000d40: 6163 6b65 6e64 222c 2022 6874 7470 3a2f  ackend", "http:/
-00000d50: 2f64 7269 7665 2e67 6f6f 676c 652e 636f  /drive.google.co
-00000d60: 6d2f 7563 3f65 7870 6f72 743d 7669 6577  m/uc?export=view
-00000d70: 2669 643d 3149 437a 3552 3266 6d67 6d31  &id=1ICz5R2fmgm1
-00000d80: 476e 5257 5871 3064 3430 4750 6375 4937  GnRWXq0d40GPcuI7
-00000d90: 5174 5670 7722 2c20 2264 6573 6331 222c  QtVpw", "desc1",
-00000da0: 2022 706f 7374 3122 290a 2020 2020 7072   "post1").    pr
-00000db0: 696e 7428 7572 6c29 0a20 2020 2068 6964  int(url).    hid
-00000dc0: 655f 7374 7265 616d 6c69 745f 7374 796c  e_streamlit_styl
-00000dd0: 6520 3d20 2222 220a 2020 2020 2020 2020  e = """.        
-00000de0: 2020 2020 3c73 7479 6c65 3e0a 2020 2020      <style>.    
-00000df0: 2020 2020 2020 2020 234d 6169 6e4d 656e          #MainMen
-00000e00: 7520 7b76 6973 6962 696c 6974 793a 2068  u {visibility: h
-00000e10: 6964 6465 6e3b 7d0a 2020 2020 2020 2020  idden;}.        
-00000e20: 2020 2020 666f 6f74 6572 207b 7669 7369      footer {visi
-00000e30: 6269 6c69 7479 3a20 6869 6464 656e 3b7d  bility: hidden;}
-00000e40: 0a20 2020 2020 2020 2020 2020 203c 2f73  .            </s
-00000e50: 7479 6c65 3e0a 2020 2020 2020 2020 2020  tyle>.          
-00000e60: 2020 2222 220a 2020 2020 7374 2e6d 6172    """.    st.mar
-00000e70: 6b64 6f77 6e28 6869 6465 5f73 7472 6561  kdown(hide_strea
-00000e80: 6d6c 6974 5f73 7479 6c65 2c20 756e 7361  mlit_style, unsa
-00000e90: 6665 5f61 6c6c 6f77 5f68 746d 6c3d 5472  fe_allow_html=Tr
-00000ea0: 7565 2920 0a                             ue) .
+00000030: 6f6e 656e 7473 0a69 6d70 6f72 7420 7265  onents.import re
+00000040: 7175 6573 7473 0a23 2043 7265 6174 6520  quests.# Create 
+00000050: 6120 5f52 454c 4541 5345 2063 6f6e 7374  a _RELEASE const
+00000060: 616e 742e 2057 6527 6c6c 2073 6574 2074  ant. We'll set t
+00000070: 6869 7320 746f 2046 616c 7365 2077 6869  his to False whi
+00000080: 6c65 2077 6527 7265 2064 6576 656c 6f70  le we're develop
+00000090: 696e 670a 2320 7468 6520 636f 6d70 6f6e  ing.# the compon
+000000a0: 656e 742c 2061 6e64 2054 7275 6520 7768  ent, and True wh
+000000b0: 656e 2077 6527 7265 2072 6561 6479 2074  en we're ready t
+000000c0: 6f20 7061 636b 6167 6520 616e 6420 6469  o package and di
+000000d0: 7374 7269 6275 7465 2069 742e 0a23 2028  stribute it..# (
+000000e0: 5468 6973 2069 732c 206f 6620 636f 7572  This is, of cour
+000000f0: 7365 2c20 6f70 7469 6f6e 616c 202d 2074  se, optional - t
+00000100: 6865 7265 2061 7265 2069 6e6e 756d 6572  here are innumer
+00000110: 6162 6c65 2077 6179 7320 746f 206d 616e  able ways to man
+00000120: 6167 6520 796f 7572 0a23 2072 656c 6561  age your.# relea
+00000130: 7365 2070 726f 6365 7373 2e29 0a5f 5245  se process.)._RE
+00000140: 4c45 4153 4520 3d20 5472 7565 0a0a 2320  LEASE = True..# 
+00000150: 4465 636c 6172 6520 6120 5374 7265 616d  Declare a Stream
+00000160: 6c69 7420 636f 6d70 6f6e 656e 742e 2060  lit component. `
+00000170: 6465 636c 6172 655f 636f 6d70 6f6e 656e  declare_componen
+00000180: 7460 2072 6574 7572 6e73 2061 2066 756e  t` returns a fun
+00000190: 6374 696f 6e0a 2320 7468 6174 2069 7320  ction.# that is 
+000001a0: 7573 6564 2074 6f20 6372 6561 7465 2069  used to create i
+000001b0: 6e73 7461 6e63 6573 206f 6620 7468 6520  nstances of the 
+000001c0: 636f 6d70 6f6e 656e 742e 2057 6527 7265  component. We're
+000001d0: 206e 616d 696e 6720 7468 6973 0a23 2066   naming this.# f
+000001e0: 756e 6374 696f 6e20 225f 636f 6d70 6f6e  unction "_compon
+000001f0: 656e 745f 6675 6e63 222c 2077 6974 6820  ent_func", with 
+00000200: 616e 2075 6e64 6572 7363 6f72 6520 7072  an underscore pr
+00000210: 6566 6978 2c20 6265 6361 7573 6520 7765  efix, because we
+00000220: 2064 6f6e 2774 2077 616e 740a 2320 746f   don't want.# to
+00000230: 2065 7870 6f73 6520 6974 2064 6972 6563   expose it direc
+00000240: 746c 7920 746f 2075 7365 7273 2e20 496e  tly to users. In
+00000250: 7374 6561 642c 2077 6520 7769 6c6c 2063  stead, we will c
+00000260: 7265 6174 6520 6120 6375 7374 6f6d 2077  reate a custom w
+00000270: 7261 7070 6572 0a23 2066 756e 6374 696f  rapper.# functio
+00000280: 6e2c 2062 656c 6f77 2c20 7468 6174 2077  n, below, that w
+00000290: 696c 6c20 7365 7276 6520 6173 206f 7572  ill serve as our
+000002a0: 2063 6f6d 706f 6e65 6e74 2773 2070 7562   component's pub
+000002b0: 6c69 6320 4150 492e 0a0a 2320 4974 2773  lic API...# It's
+000002c0: 2077 6f72 7468 206e 6f74 696e 6720 7468   worth noting th
+000002d0: 6174 2074 6869 7320 6361 6c6c 2074 6f20  at this call to 
+000002e0: 6064 6563 6c61 7265 5f63 6f6d 706f 6e65  `declare_compone
+000002f0: 6e74 6020 6973 2074 6865 0a23 202a 6f6e  nt` is the.# *on
+00000300: 6c79 2074 6869 6e67 2a20 796f 7520 6e65  ly thing* you ne
+00000310: 6564 2074 6f20 646f 2074 6f20 6372 6561  ed to do to crea
+00000320: 7465 2074 6865 2062 696e 6469 6e67 2062  te the binding b
+00000330: 6574 7765 656e 2053 7472 6561 6d6c 6974  etween Streamlit
+00000340: 2061 6e64 0a23 2079 6f75 7220 636f 6d70   and.# your comp
+00000350: 6f6e 656e 7420 6672 6f6e 7465 6e64 2e20  onent frontend. 
+00000360: 4576 6572 7974 6869 6e67 2065 6c73 6520  Everything else 
+00000370: 7765 2064 6f20 696e 2074 6869 7320 6669  we do in this fi
+00000380: 6c65 2069 7320 7369 6d70 6c79 2061 0a23  le is simply a.#
+00000390: 2062 6573 7420 7072 6163 7469 6365 2e0a   best practice..
+000003a0: 0a69 6620 6e6f 7420 5f52 454c 4541 5345  .if not _RELEASE
+000003b0: 3a0a 2020 2020 5f63 6f6d 706f 6e65 6e74  :.    _component
+000003c0: 5f66 756e 6320 3d20 636f 6d70 6f6e 656e  _func = componen
+000003d0: 7473 2e64 6563 6c61 7265 5f63 6f6d 706f  ts.declare_compo
+000003e0: 6e65 6e74 280a 2020 2020 2020 2020 2320  nent(.        # 
+000003f0: 5765 2067 6976 6520 7468 6520 636f 6d70  We give the comp
+00000400: 6f6e 656e 7420 6120 7369 6d70 6c65 2c20  onent a simple, 
+00000410: 6465 7363 7269 7074 6976 6520 6e61 6d65  descriptive name
+00000420: 2028 226d 795f 636f 6d70 6f6e 656e 7422   ("my_component"
+00000430: 0a20 2020 2020 2020 2023 2064 6f65 7320  .        # does 
+00000440: 6e6f 7420 6669 7420 7468 6973 2062 696c  not fit this bil
+00000450: 6c2c 2073 6f20 706c 6561 7365 2063 686f  l, so please cho
+00000460: 6f73 6520 736f 6d65 7468 696e 6720 6265  ose something be
+00000470: 7474 6572 2066 6f72 2079 6f75 720a 2020  tter for your.  
+00000480: 2020 2020 2020 2320 6f77 6e20 636f 6d70        # own comp
+00000490: 6f6e 656e 7420 3a29 0a20 2020 2020 2020  onent :).       
+000004a0: 2022 6d79 5f63 6f6d 706f 6e65 6e74 222c   "my_component",
+000004b0: 0a20 2020 2020 2020 2023 2050 6173 7320  .        # Pass 
+000004c0: 6075 726c 6020 6865 7265 2074 6f20 7465  `url` here to te
+000004d0: 6c6c 2053 7472 6561 6d6c 6974 2074 6861  ll Streamlit tha
+000004e0: 7420 7468 6520 636f 6d70 6f6e 656e 7420  t the component 
+000004f0: 7769 6c6c 2062 6520 7365 7276 6564 0a20  will be served. 
+00000500: 2020 2020 2020 2023 2062 7920 7468 6520         # by the 
+00000510: 6c6f 6361 6c20 6465 7620 7365 7276 6572  local dev server
+00000520: 2074 6861 7420 796f 7520 7275 6e20 7669   that you run vi
+00000530: 6120 606e 706d 2072 756e 2073 7461 7274  a `npm run start
+00000540: 602e 0a20 2020 2020 2020 2023 2028 5468  `..        # (Th
+00000550: 6973 2069 7320 7573 6566 756c 2077 6869  is is useful whi
+00000560: 6c65 2079 6f75 7220 636f 6d70 6f6e 656e  le your componen
+00000570: 7420 6973 2069 6e20 6465 7665 6c6f 706d  t is in developm
+00000580: 656e 742e 290a 2020 2020 2020 2020 7572  ent.).        ur
+00000590: 6c3d 2268 7474 703a 2f2f 3139 322e 3136  l="http://192.16
+000005a0: 382e 322e 3436 3a33 3030 312f 222c 0a20  8.2.46:3001/",. 
+000005b0: 2020 2029 0a65 6c73 653a 0a20 2020 2023     ).else:.    #
+000005c0: 2057 6865 6e20 7765 2772 6520 6469 7374   When we're dist
+000005d0: 7269 6275 7469 6e67 2061 2070 726f 6475  ributing a produ
+000005e0: 6374 696f 6e20 7665 7273 696f 6e20 6f66  ction version of
+000005f0: 2074 6865 2063 6f6d 706f 6e65 6e74 2c20   the component, 
+00000600: 7765 276c 6c0a 2020 2020 2320 7265 706c  we'll.    # repl
+00000610: 6163 6520 7468 6520 6075 726c 6020 7061  ace the `url` pa
+00000620: 7261 6d20 7769 7468 2060 7061 7468 602c  ram with `path`,
+00000630: 2061 6e64 2070 6f69 6e74 2069 7420 746f   and point it to
+00000640: 2074 6f20 7468 6520 636f 6d70 6f6e 656e   to the componen
+00000650: 7427 730a 2020 2020 2320 6275 696c 6420  t's.    # build 
+00000660: 6469 7265 6374 6f72 793a 0a20 2020 2070  directory:.    p
+00000670: 6172 656e 745f 6469 7220 3d20 6f73 2e70  arent_dir = os.p
+00000680: 6174 682e 6469 726e 616d 6528 6f73 2e70  ath.dirname(os.p
+00000690: 6174 682e 6162 7370 6174 6828 5f5f 6669  ath.abspath(__fi
+000006a0: 6c65 5f5f 2929 0a20 2020 2062 7569 6c64  le__)).    build
+000006b0: 5f64 6972 203d 206f 732e 7061 7468 2e6a  _dir = os.path.j
+000006c0: 6f69 6e28 7061 7265 6e74 5f64 6972 2c20  oin(parent_dir, 
+000006d0: 2266 726f 6e74 656e 642f 6275 696c 6422  "frontend/build"
+000006e0: 290a 2020 2020 5f63 6f6d 706f 6e65 6e74  ).    _component
+000006f0: 5f66 756e 6320 3d20 636f 6d70 6f6e 656e  _func = componen
+00000700: 7473 2e64 6563 6c61 7265 5f63 6f6d 706f  ts.declare_compo
+00000710: 6e65 6e74 2822 6d79 5f63 6f6d 706f 6e65  nent("my_compone
+00000720: 6e74 222c 2070 6174 683d 6275 696c 645f  nt", path=build_
+00000730: 6469 7229 0a0a 0a23 2043 7265 6174 6520  dir)...# Create 
+00000740: 6120 7772 6170 7065 7220 6675 6e63 7469  a wrapper functi
+00000750: 6f6e 2066 6f72 2074 6865 2063 6f6d 706f  on for the compo
+00000760: 6e65 6e74 2e20 5468 6973 2069 7320 616e  nent. This is an
+00000770: 206f 7074 696f 6e61 6c0a 2320 6265 7374   optional.# best
+00000780: 2070 7261 6374 6963 6520 2d20 7765 2063   practice - we c
+00000790: 6f75 6c64 2073 696d 706c 7920 6578 706f  ould simply expo
+000007a0: 7365 2074 6865 2063 6f6d 706f 6e65 6e74  se the component
+000007b0: 2066 756e 6374 696f 6e20 7265 7475 726e   function return
+000007c0: 6564 2062 790a 2320 6064 6563 6c61 7265  ed by.# `declare
+000007d0: 5f63 6f6d 706f 6e65 6e74 6020 616e 6420  _component` and 
+000007e0: 6361 6c6c 2069 7420 646f 6e65 2e20 5468  call it done. Th
+000007f0: 6520 7772 6170 7065 7220 616c 6c6f 7773  e wrapper allows
+00000800: 2075 7320 746f 2063 7573 746f 6d69 7a65   us to customize
+00000810: 0a23 206f 7572 2063 6f6d 706f 6e65 6e74  .# our component
+00000820: 2773 2041 5049 3a20 7765 2063 616e 2070  's API: we can p
+00000830: 7265 2d70 726f 6365 7373 2069 7473 2069  re-process its i
+00000840: 6e70 7574 2061 7267 732c 2070 6f73 742d  nput args, post-
+00000850: 7072 6f63 6573 7320 6974 730a 2320 6f75  process its.# ou
+00000860: 7470 7574 2076 616c 7565 2c20 616e 6420  tput value, and 
+00000870: 6164 6420 6120 646f 6373 7472 696e 6720  add a docstring 
+00000880: 666f 7220 7573 6572 732e 0a64 6566 2062  for users..def b
+00000890: 6c6f 675f 6361 7264 5f63 6f6d 706f 6e65  log_card_compone
+000008a0: 6e74 2869 643d 4e6f 6e65 2c20 7469 746c  nt(id=None, titl
+000008b0: 653d 4e6f 6e65 2c20 7375 6274 6974 6c65  e=None, subtitle
+000008c0: 3d4e 6f6e 652c 2064 6573 6372 6970 7469  =None, descripti
+000008d0: 6f6e 3d4e 6f6e 652c 2064 6174 653d 4e6f  on=None, date=No
+000008e0: 6e65 2c20 6769 7468 7562 3d4e 6f6e 652c  ne, github=None,
+000008f0: 2075 726c 3d4e 6f6e 652c 2070 6f73 743d   url=None, post=
+00000900: 4e6f 6e65 2c20 696d 675f 7061 7468 3d4e  None, img_path=N
+00000910: 6f6e 6529 3a0a 2020 2020 2222 2243 7265  one):.    """Cre
+00000920: 6174 6520 6120 6e65 7720 696e 7374 616e  ate a new instan
+00000930: 6365 206f 6620 2263 6172 645f 636f 6d70  ce of "card_comp
+00000940: 6f6e 656e 7422 2e0a 2020 2020 2222 220a  onent"..    """.
+00000950: 2020 2020 2320 7468 6520 6265 6c6f 7720      # the below 
+00000960: 696e 6974 6961 6c69 7a65 7320 7468 6520  initializes the 
+00000970: 7265 6163 7420 636f 6d70 6f6e 656e 7420  react component 
+00000980: 2869 6e20 4361 7264 436f 6d70 6f6e 656e  (in CardComponen
+00000990: 742e 7473 7829 0a20 2020 2063 6f6d 706f  t.tsx).    compo
+000009a0: 6e65 6e74 5f76 616c 7565 203d 205f 636f  nent_value = _co
+000009b0: 6d70 6f6e 656e 745f 6675 6e63 280a 2020  mponent_func(.  
+000009c0: 2020 2020 2020 6964 203d 6964 2c0a 2020        id =id,.  
+000009d0: 2020 2020 2020 7469 746c 653d 7469 746c        title=titl
+000009e0: 652c 0a20 2020 2020 2020 2073 7562 7469  e,.        subti
+000009f0: 746c 653d 7375 6274 6974 6c65 2c0a 2020  tle=subtitle,.  
+00000a00: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00000a10: 6e3d 6465 7363 7269 7074 696f 6e2c 0a20  n=description,. 
+00000a20: 2020 2020 2020 2075 726c 3d75 726c 2c0a         url=url,.
+00000a30: 2020 2020 2020 2020 6769 7468 7562 3d67          github=g
+00000a40: 6974 6875 622c 0a20 2020 2020 2020 2070  ithub,.        p
+00000a50: 6f73 743d 706f 7374 2c0a 2020 2020 2020  ost=post,.      
+00000a60: 2020 696d 675f 7061 7468 3d69 6d67 5f70    img_path=img_p
+00000a70: 6174 682c 0a20 2020 2020 2020 2064 6174  ath,.        dat
+00000a80: 653d 6461 7465 0a20 2020 2029 0a0a 2020  e=date.    )..  
+00000a90: 2020 2320 5765 2063 6f75 6c64 206d 6f64    # We could mod
+00000aa0: 6966 7920 7468 6520 7661 6c75 6520 7265  ify the value re
+00000ab0: 7475 726e 6564 2066 726f 6d20 7468 6520  turned from the 
+00000ac0: 636f 6d70 6f6e 656e 7420 6966 2077 6520  component if we 
+00000ad0: 7761 6e74 6564 2e0a 2020 2020 2320 5468  wanted..    # Th
+00000ae0: 6572 6527 7320 6e6f 206e 6565 6420 746f  ere's no need to
+00000af0: 2064 6f20 7468 6973 2069 6e20 6f75 7220   do this in our 
+00000b00: 7369 6d70 6c65 2065 7861 6d70 6c65 202d  simple example -
+00000b10: 2062 7574 2069 7427 7320 616e 206f 7074   but it's an opt
+00000b20: 696f 6e2e 0a20 2020 2072 6574 7572 6e20  ion..    return 
+00000b30: 636f 6d70 6f6e 656e 745f 7661 6c75 650a  component_value.
+00000b40: 0a0a 2320 4164 6420 736f 6d65 2074 6573  ..# Add some tes
+00000b50: 7420 636f 6465 2074 6f20 706c 6179 2077  t code to play w
+00000b60: 6974 6820 7468 6520 636f 6d70 6f6e 656e  ith the componen
+00000b70: 7420 7768 696c 6520 6974 2773 2069 6e20  t while it's in 
+00000b80: 6465 7665 6c6f 706d 656e 742e 0a23 2044  development..# D
+00000b90: 7572 696e 6720 6465 7665 6c6f 706d 656e  uring developmen
+00000ba0: 742c 2077 6520 6361 6e20 7275 6e20 7468  t, we can run th
+00000bb0: 6973 206a 7573 7420 6173 2077 6520 776f  is just as we wo
+00000bc0: 756c 6420 616e 7920 6f74 6865 7220 5374  uld any other St
+00000bd0: 7265 616d 6c69 740a 2320 6170 703a 2060  reamlit.# app: `
+00000be0: 2420 7374 7265 616d 6c69 7420 7275 6e20  $ streamlit run 
+00000bf0: 6d79 5f63 6f6d 706f 6e65 6e74 2f5f 5f69  my_component/__i
+00000c00: 6e69 745f 5f2e 7079 600a 6966 206e 6f74  nit__.py`.if not
+00000c10: 205f 5245 4c45 4153 453a 0a20 2020 2069   _RELEASE:.    i
+00000c20: 6d70 6f72 7420 7374 7265 616d 6c69 7420  mport streamlit 
+00000c30: 6173 2073 740a 0a20 2020 2073 742e 7375  as st..    st.su
+00000c40: 6268 6561 6465 7228 2243 6f6d 706f 6e65  bheader("Compone
+00000c50: 6e74 2077 6974 6820 636f 6e73 7461 6e74  nt with constant
+00000c60: 2061 7267 7322 290a 0a20 2020 2023 2043   args")..    # C
+00000c70: 7265 6174 6520 616e 2069 6e73 7461 6e63  reate an instanc
+00000c80: 6520 6f66 206f 7572 2063 6f6d 706f 6e65  e of our compone
+00000c90: 6e74 2077 6974 6820 6120 636f 6e73 7461  nt with a consta
+00000ca0: 6e74 2060 6e61 6d65 6020 6172 672c 2061  nt `name` arg, a
+00000cb0: 6e64 0a20 2020 2023 2070 7269 6e74 2069  nd.    # print i
+00000cc0: 7473 206f 7574 7075 7420 7661 6c75 650a  ts output value.
+00000cd0: 2020 2020 2370 7269 6e74 2875 726c 290a      #print(url).
+00000ce0: 2020 2020 6869 6465 5f73 7472 6561 6d6c      hide_streaml
+00000cf0: 6974 5f73 7479 6c65 203d 2022 2222 0a20  it_style = """. 
+00000d00: 2020 2020 2020 2020 2020 203c 7374 796c             <styl
+00000d10: 653e 0a20 2020 2020 2020 2020 2020 2023  e>.            #
+00000d20: 4d61 696e 4d65 6e75 207b 7669 7369 6269  MainMenu {visibi
+00000d30: 6c69 7479 3a20 6869 6464 656e 3b7d 0a20  lity: hidden;}. 
+00000d40: 2020 2020 2020 2020 2020 2066 6f6f 7465             foote
+00000d50: 7220 7b76 6973 6962 696c 6974 793a 2068  r {visibility: h
+00000d60: 6964 6465 6e3b 7d0a 2020 2020 2020 2020  idden;}.        
+00000d70: 2020 2020 3c2f 7374 796c 653e 0a20 2020      </style>.   
+00000d80: 2020 2020 2020 2020 2022 2222 0a20 2020           """.   
+00000d90: 2073 742e 6d61 726b 646f 776e 2868 6964   st.markdown(hid
+00000da0: 655f 7374 7265 616d 6c69 745f 7374 796c  e_streamlit_styl
+00000db0: 652c 2075 6e73 6166 655f 616c 6c6f 775f  e, unsafe_allow_
+00000dc0: 6874 6d6c 3d54 7275 6529 200a            html=True) .
```

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/asset-manifest.json` & `st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/asset-manifest.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.84375%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.5833844e.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.5833844e.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.5833844e.chunk.js.map'}"}*

```diff
@@ -1,17 +1,17 @@
 {
     "entrypoints": [
         "static/js/runtime-main.0f051bbb.js",
         "static/js/2.cc3b77fa.chunk.js",
-        "static/js/main.060e67f4.chunk.js"
+        "static/js/main.5833844e.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.060e67f4.chunk.js",
-        "main.js.map": "./static/js/main.060e67f4.chunk.js.map",
+        "main.js": "./static/js/main.5833844e.chunk.js",
+        "main.js.map": "./static/js/main.5833844e.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.0f051bbb.js",
         "runtime-main.js.map": "./static/js/runtime-main.0f051bbb.js.map",
         "static/js/2.cc3b77fa.chunk.js": "./static/js/2.cc3b77fa.chunk.js",
         "static/js/2.cc3b77fa.chunk.js.LICENSE.txt": "./static/js/2.cc3b77fa.chunk.js.LICENSE.txt",
         "static/js/2.cc3b77fa.chunk.js.map": "./static/js/2.cc3b77fa.chunk.js.map"
     }
 }
```

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/bootstrap.min.css` & `st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/index.html` & `st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,p=t[0],f=t[1],i=t[2],c=0,s=[];c<p.length;c++)l=p[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in f)Object.prototype.hasOwnProperty.call(f,n)&&(e[n]=f[n]);for(a&&a(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,p=1;p<r.length;p++){var f=r[p];0!==o[f]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var p=this.webpackJsonpst_blogpost_component=this.webpackJsonpst_blogpost_component||[],f=p.push.bind(p);p.push=t,p=p.slice();for(var i=0;i<p.length;i++)t(p[i]);var a=f;r()}([])</script><script src="./static/js/2.cc3b77fa.chunk.js"></script><script src="./static/js/main.060e67f4.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,p=t[0],f=t[1],i=t[2],c=0,s=[];c<p.length;c++)l=p[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in f)Object.prototype.hasOwnProperty.call(f,n)&&(e[n]=f[n]);for(a&&a(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,p=1;p<r.length;p++){var f=r[p];0!==o[f]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var p=this.webpackJsonpst_blogpost_component=this.webpackJsonpst_blogpost_component||[],f=p.push.bind(p);p.push=t,p=p.slice();for(var i=0;i<p.length;i++)t(p[i]);var a=f;r()}([])</script><script src="./static/js/2.cc3b77fa.chunk.js"></script><script src="./static/js/main.5833844e.chunk.js"></script></body></html>
```

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js` & `st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt` & `st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map` & `st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/main.060e67f4.chunk.js` & `st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/main.5833844e.chunk.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,81 +1,83 @@
 (this.webpackJsonpst_blogpost_component = this.webpackJsonpst_blogpost_component || []).push([
     [0], {
         67: function(t, e, n) {
             "use strict";
             n.r(e);
             var r = n(4),
                 s = n.n(r),
-                c = n(53),
-                a = n.n(c),
+                a = n(53),
+                c = n.n(a),
                 i = n(0),
                 o = n(1),
                 l = n(2),
                 p = n(3),
                 b = n(47),
-                j = n(92),
-                u = n(95),
+                u = n(92),
+                j = n(95),
                 d = n(96),
                 h = n(97),
-                O = n(94),
-                g = n(98),
+                g = n(94),
+                O = n(98),
                 x = n(91),
                 m = n(9),
                 f = function(t) {
                     Object(l.a)(n, t);
                     var e = Object(p.a)(n);
 
                     function n() {
                         var t;
                         Object(o.a)(this, n);
-                        for (var r = arguments.length, s = new Array(r), c = 0; c < r; c++) s[c] = arguments[c];
+                        for (var r = arguments.length, s = new Array(r), a = 0; a < r; a++) s[a] = arguments[a];
                         return (t = e.call.apply(e, [this].concat(s))).state = {
                             url: null
                         }, t.render = function() {
                             var e = t.props.args.title,
                                 n = t.props.args.subtitle,
                                 r = t.props.args.description,
-                                s = t.props.args.link,
-                                c = t.props.args.github,
-                                a = t.props.args.img_path,
-                                i = t.props.args.post;
+                                s = t.props.args.url,
+                                a = t.props.args.github,
+                                c = t.props.args.img_path,
+                                i = t.props.args.post,
+                                o = t.props.args.date;
                             return Object(m.jsx)("div", {
                                 style: {
                                     padding: "0.5rem"
                                 },
-                                children: Object(m.jsxs)(j.a, {
+                                children: Object(m.jsxs)(u.a, {
                                     variant: "outlined",
-                                    children: [Object(m.jsx)(u.a, {
-                                        title: e
+                                    children: [Object(m.jsx)(j.a, {
+                                        title: e,
+                                        subheader: o
                                     }), Object(m.jsx)(d.a, {
                                         component: "img",
                                         height: "200",
-                                        src: a
-                                    }), Object(m.jsx)(u.a, {
+                                        src: c
+                                    }), Object(m.jsx)(j.a, {
                                         subheader: n
                                     }), Object(m.jsx)(h.a, {
-                                        children: Object(m.jsx)(O.a, {
+                                        children: Object(m.jsx)(g.a, {
                                             variant: "body2",
                                             children: r
                                         })
-                                    }), Object(m.jsxs)(g.a, {
+                                    }), Object(m.jsxs)(O.a, {
                                         disableSpacing: !0,
                                         children: [Object(m.jsx)(x.a, {
                                             size: "small",
                                             onClick: function() {
-                                                return window.open(c, "_blank")
+                                                return window.open(a, "_blank")
                                             },
                                             children: "github"
                                         }), s && Object(m.jsx)(x.a, {
                                             size: "small",
                                             onClick: function() {
                                                 return window.open(s, "_blank")
                                             },
                                             children: "link"
-                                        }), Object(m.jsx)(x.a, {
+                                        }), i && Object(m.jsx)(x.a, {
                                             size: "small",
                                             onClick: function() {
                                                 return t.setState((function() {
                                                     return {
                                                         url: i
                                                     }
                                                 }), (function() {
@@ -88,17 +90,17 @@
                                 })
                             })
                         }, t
                     }
                     return Object(i.a)(n)
                 }(b.b),
                 k = Object(b.c)(f);
-            a.a.render(Object(m.jsx)(s.a.StrictMode, {
+            c.a.render(Object(m.jsx)(s.a.StrictMode, {
                 children: Object(m.jsx)(k, {})
             }), document.getElementById("root"))
         }
     },
     [
         [67, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.060e67f4.chunk.js.map
+//# sourceMappingURL=main.5833844e.chunk.js.map
```

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/main.060e67f4.chunk.js.map` & `st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/main.5833844e.chunk.js.map`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8061224489795918%*

 * *Differences: {"'file'": "'static/js/main.5833844e.chunk.js'",*

 * * "'mappings'": "'8QAcMA,EAAa,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GAmDhB,OAnDgBP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KACVM,MAAQ,CAAEC,IAAK,MAAMZ,EAErBa,OAAS,WAGd,IAAMC,EAAQd,EAAKe,MAAMV,KAAY,MAC/BW,EAAWhB,EAAKe,MAAMV,KAAe,SACrCY,EAAOjB,EAAKe,MAAMV,KAAkB,YACpCa,EAAOlB,EAAKe,MAAMV,KAAU,IAC5Bc,EAASnB,EAAKe,MAAMV […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.060e67f4.chunk.js",
-    "mappings": "8QAcMA,EAAa,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GAgDhB,OAhDgBP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KACVM,MAAQ,CAAEC,IAAK,MAAMZ,EAErBa,OAAS,WAGd,IAAMC,EAAQd,EAAKe,MAAMV,KAAY,MAC/BW,EAAWhB,EAAKe,MAAMV,KAAe,SACrCY,EAAOjB,EAAKe,MAAMV,KAAkB,YACpCa,EAAOlB,EAAKe,MAAMV,KAAW,KAC7Bc,EAASnB,EAAKe,MAAMV,KAAa,OACjCe,EAAWpB,EAAKe,MAAMV,KAAe,SACrCgB,EAAOrB,EAAKe,MAAMV,KAAW,KAEnC,OACEiB,cAAA,OAAKC,MAAO,CAAEC,QAAS,UAAWC,SAChCC,eAACC,IAAI,CAACC,QAAQ,WAAUH,SAAA,CACtBH,cAACO,IAAU,CAACf,MAAOA,IACnBQ,cAACQ,IAAS,CAACC,UAAU,MAAMC,OAAO,MAAMC,IAAKb,IAC7CE,cAACO,IAAU,CAACK,UAAWlB,IACvBM,cAACa,IAAW,CAAAV,SACVH,cAACc,IAAU,CAACR,QAAQ,QAAOH,SAAER,MAE/BS,eAACW,IAAW,CAACC,gBAAc,EAAAb,SAAA,CACzBH,cAACiB,IAAM,CAACC,KAAK,QAAQC,QAAS,kBAAMC,OAAOC,KAAKxB,EAAQ,SAAS,EAACM,SAAC,WAGlEP,GACCI,cAACiB,IAAM,CAACC,KAAK,QAAQC,QAAS,kBAAMC,OAAOC,KAAKzB,EAAM,SAAS,EAACO,SAAC,SAKnEH,cAACiB,IAAM,CACLC,KAAK,QACLC,QAAS,kBACPzC,EAAK4C,UACH,iBAAO,CAAEhC,IAAKS,EAAM,IACpB,kBAAMwB,IAAUC,kBAAkB9C,EAAKW,MAAMC,IAAI,GAClD,EACFa,SACF,wBAOX,EAACzB,CAAA,QAAA+C,YAAApD,EAAA,CAhDgB,CAASqD,KAoDbC,cAAwBtD,GC9DvCuD,IAASrC,OACPS,cAAC6B,IAAMC,WAAU,CAAA3B,SACfH,cAAC+B,EAAQ,MAEXC,SAASC,eAAe,Q",
+    "file": "static/js/main.5833844e.chunk.js",
+    "mappings": "8QAcMA,EAAa,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GAmDhB,OAnDgBP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KACVM,MAAQ,CAAEC,IAAK,MAAMZ,EAErBa,OAAS,WAGd,IAAMC,EAAQd,EAAKe,MAAMV,KAAY,MAC/BW,EAAWhB,EAAKe,MAAMV,KAAe,SACrCY,EAAOjB,EAAKe,MAAMV,KAAkB,YACpCa,EAAOlB,EAAKe,MAAMV,KAAU,IAC5Bc,EAASnB,EAAKe,MAAMV,KAAa,OACjCe,EAAWpB,EAAKe,MAAMV,KAAe,SACrCgB,EAAOrB,EAAKe,MAAMV,KAAW,KAC7BiB,EAAOtB,EAAKe,MAAMV,KAAW,KAEnC,OACEkB,cAAA,OAAKC,MAAO,CAAEC,QAAS,UAAWC,SAChCC,eAACC,IAAI,CAACC,QAAQ,WAAUH,SAAA,CACtBH,cAACO,IAAU,CAAChB,MAAOA,EAAOiB,UAAWT,IACrCC,cAACS,IAAS,CAACC,UAAU,MAAMC,OAAO,MAAMC,IAAKf,IAC7CG,cAACO,IAAU,CAACC,UAAWf,IACvBO,cAACa,IAAW,CAAAV,SACVH,cAACc,IAAU,CAACR,QAAQ,QAAOH,SAAET,MAE/BU,eAACW,IAAW,CAACC,gBAAc,EAAAb,SAAA,CACzBH,cAACiB,IAAM,CAACC,KAAK,QAAQC,QAAS,kBAAMC,OAAOC,KAAKzB,EAAQ,SAAS,EAACO,SAAC,WAGlER,GACCK,cAACiB,IAAM,CAACC,KAAK,QAAQC,QAAS,kBAAMC,OAAOC,KAAK1B,EAAM,SAAS,EAACQ,SAAC,SAKlEL,GACCE,cAACiB,IAAM,CACLC,KAAK,QACLC,QAAS,kBACP1C,EAAK6C,UACH,iBAAO,CAAEjC,IAAKS,EAAM,IACpB,kBAAMyB,IAAUC,kBAAkB/C,EAAKW,MAAMC,IAAI,GAClD,EACFc,SACF,wBAQb,EAAC1B,CAAA,QAAAgD,YAAArD,EAAA,CAnDgB,CAASsD,KAuDbC,cAAwBvD,GCjEvCwD,IAAStC,OACPU,cAAC6B,IAAMC,WAAU,CAAA3B,SACfH,cAAC+B,EAAQ,MAEXC,SAASC,eAAe,Q",
     "names": [
         "CardComponent",
         "_StreamlitComponentBa",
         "_inherits",
         "_super",
         "_createSuper",
         "_this",
@@ -25,27 +25,28 @@
         "props",
         "subtitle",
         "body",
         "link",
         "github",
         "img_link",
         "post",
+        "date",
         "_jsx",
         "style",
         "padding",
         "children",
         "_jsxs",
         "Card",
         "variant",
         "CardHeader",
+        "subheader",
         "CardMedia",
         "component",
         "height",
         "src",
-        "subheader",
         "CardContent",
         "Typography",
         "CardActions",
         "disableSpacing",
         "Button",
         "size",
         "onClick",
@@ -66,12 +67,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "PostCard.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport Card from \"@mui/material/Card\"\nimport CardHeader from \"@mui/material/CardHeader\"\nimport CardMedia from \"@mui/material/CardMedia\"\nimport CardContent from \"@mui/material/CardContent\"\nimport { Typography, CardActions } from \"@mui/material\"\nimport Button from \"@mui/material/Button\"\n\n// the `render()` function is called when component is re-rendered\nclass CardComponent extends StreamlitComponentBase<any> {\n  public state = { url: null }\n\n  public render = (): ReactNode => {\n    // Arguments that are passed to the plugin in Python are accessible\n    // via `this.props.args`\n    const title = this.props.args[\"title\"]\n    const subtitle = this.props.args[\"subtitle\"]\n    const body = this.props.args[\"description\"]\n    const link = this.props.args[\"link\"]\n    const github = this.props.args[\"github\"]\n    const img_link = this.props.args[\"img_path\"]\n    const post = this.props.args[\"post\"]\n\n    return (\n      <div style={{ padding: \"0.5rem\" }}>\n        <Card variant=\"outlined\">\n          <CardHeader title={title} />\n          <CardMedia component=\"img\" height=\"200\" src={img_link} />\n          <CardHeader subheader={subtitle} />\n          <CardContent>\n            <Typography variant=\"body2\">{body}</Typography>\n          </CardContent>\n          <CardActions disableSpacing>\n            <Button size=\"small\" onClick={() => window.open(github, \"_blank\")}>\n              github\n            </Button>\n            {link && (\n              <Button size=\"small\" onClick={() => window.open(link, \"_blank\")}>\n                link\n              </Button>\n            )}\n\n            <Button\n              size=\"small\"\n              onClick={() =>\n                this.setState(\n                  () => ({ url: post }),\n                  () => Streamlit.setComponentValue(this.state.url)\n                )\n              }\n            >\n              Open Article\n            </Button>\n          </CardActions>\n        </Card>\n      </div>\n    )\n  }\n}\n\n// connection between component and Streamlit\nexport default withStreamlitConnection(CardComponent)\n",
+        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport Card from \"@mui/material/Card\"\nimport CardHeader from \"@mui/material/CardHeader\"\nimport CardMedia from \"@mui/material/CardMedia\"\nimport CardContent from \"@mui/material/CardContent\"\nimport { Typography, CardActions } from \"@mui/material\"\nimport Button from \"@mui/material/Button\"\n\n// the `render()` function is called when component is re-rendered\nclass CardComponent extends StreamlitComponentBase<any> {\n  public state = { url: null }\n\n  public render = (): ReactNode => {\n    // Arguments that are passed to the plugin in Python are accessible\n    // via `this.props.args`\n    const title = this.props.args[\"title\"]\n    const subtitle = this.props.args[\"subtitle\"]\n    const body = this.props.args[\"description\"]\n    const link = this.props.args[\"url\"]\n    const github = this.props.args[\"github\"]\n    const img_link = this.props.args[\"img_path\"]\n    const post = this.props.args[\"post\"]\n    const date = this.props.args[\"date\"]\n\n    return (\n      <div style={{ padding: \"0.5rem\" }}>\n        <Card variant=\"outlined\">\n          <CardHeader title={title} subheader={date} />\n          <CardMedia component=\"img\" height=\"200\" src={img_link} />\n          <CardHeader subheader={subtitle} />\n          <CardContent>\n            <Typography variant=\"body2\">{body}</Typography>\n          </CardContent>\n          <CardActions disableSpacing>\n            <Button size=\"small\" onClick={() => window.open(github, \"_blank\")}>\n              github\n            </Button>\n            {link && (\n              <Button size=\"small\" onClick={() => window.open(link, \"_blank\")}>\n                link\n              </Button>\n            )}\n\n            {post && (\n              <Button\n                size=\"small\"\n                onClick={() =>\n                  this.setState(\n                    () => ({ url: post }),\n                    () => Streamlit.setComponentValue(this.state.url)\n                  )\n                }\n              >\n                Open Article\n              </Button>\n            )}\n          </CardActions>\n        </Card>\n      </div>\n    )\n  }\n}\n\n// connection between component and Streamlit\nexport default withStreamlitConnection(CardComponent)\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport Postcard from \"./PostCard\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <Postcard />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js` & `st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map` & `st_blogpost_component-0.0.5/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.4/st_blogpost_component.egg-info/SOURCES.txt` & `st_blogpost_component-0.0.5/st_blogpost_component.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 st_blogpost_component.egg-info/top_level.txt
 st_blogpost_component/frontend/build/asset-manifest.json
 st_blogpost_component/frontend/build/bootstrap.min.css
 st_blogpost_component/frontend/build/index.html
 st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js
 st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt
 st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map
-st_blogpost_component/frontend/build/static/js/main.060e67f4.chunk.js
-st_blogpost_component/frontend/build/static/js/main.060e67f4.chunk.js.map
+st_blogpost_component/frontend/build/static/js/main.5833844e.chunk.js
+st_blogpost_component/frontend/build/static/js/main.5833844e.chunk.js.map
 st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
 st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
```

