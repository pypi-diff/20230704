# Comparing `tmp/fast_align_audio-0.1.1-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/fast_align_audio-0.1.2-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10768 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat    11776 b- defN 23-Jun-30 12:53 _fast_align_audio.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-30 12:49 fast_align_audio/__init__.py
--rw-rw-rw-  2.0 fat      618 b- defN 23-Jun-30 12:49 fast_align_audio/_fast_align_audio_cffi.py
--rw-rw-rw-  2.0 fat     3379 b- defN 23-Jun-30 12:49 fast_align_audio/fast_align_audio.py
--rw-rw-rw-  2.0 fat      761 b- defN 23-Jun-30 12:53 fast_align_audio-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2510 b- defN 23-Jun-30 12:53 fast_align_audio-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jun-30 12:53 fast_align_audio-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       35 b- defN 23-Jun-30 12:53 fast_align_audio-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      806 b- defN 23-Jun-30 12:53 fast_align_audio-0.1.1.dist-info/RECORD
-9 files, 20065 bytes uncompressed, 9356 bytes compressed:  53.4%
+Zip file size: 10739 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat    11776 b- defN 23-Jul-04 08:43 _fast_align_audio.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       68 b- defN 23-Jul-04 08:37 fast_align_audio/__init__.py
+-rw-rw-rw-  2.0 fat      618 b- defN 23-Jul-04 08:37 fast_align_audio/_alignment_cffi.py
+-rw-rw-rw-  2.0 fat     3379 b- defN 23-Jul-04 08:37 fast_align_audio/alignment.py
+-rw-rw-rw-  2.0 fat      761 b- defN 23-Jul-04 08:43 fast_align_audio-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2510 b- defN 23-Jul-04 08:43 fast_align_audio-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-04 08:43 fast_align_audio-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       35 b- defN 23-Jul-04 08:43 fast_align_audio-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      792 b- defN 23-Jul-04 08:43 fast_align_audio-0.1.2.dist-info/RECORD
+9 files, 20046 bytes uncompressed, 9355 bytes compressed:  53.3%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: _fast_align_audio.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: fast_align_audio/__init__.py
 Comment: 
 
-Filename: fast_align_audio/_fast_align_audio_cffi.py
+Filename: fast_align_audio/_alignment_cffi.py
 Comment: 
 
-Filename: fast_align_audio/fast_align_audio.py
+Filename: fast_align_audio/alignment.py
 Comment: 
 
-Filename: fast_align_audio-0.1.1.dist-info/LICENSE
+Filename: fast_align_audio-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: fast_align_audio-0.1.1.dist-info/METADATA
+Filename: fast_align_audio-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: fast_align_audio-0.1.1.dist-info/WHEEL
+Filename: fast_align_audio-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: fast_align_audio-0.1.1.dist-info/top_level.txt
+Filename: fast_align_audio-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fast_align_audio-0.1.1.dist-info/RECORD
+Filename: fast_align_audio-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fast_align_audio/__init__.py

```diff
@@ -1,3 +1,3 @@
-from .fast_align_audio import best_offset, align
+from .alignment import best_offset, align
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `fast_align_audio/_fast_align_audio_cffi.py` & `fast_align_audio/_alignment_cffi.py`

 * *Files identical despite different names*

## Comparing `fast_align_audio/fast_align_audio.py` & `fast_align_audio/alignment.py`

 * *Files identical despite different names*

## Comparing `fast_align_audio-0.1.1.dist-info/LICENSE` & `fast_align_audio-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fast_align_audio-0.1.1.dist-info/METADATA` & `fast_align_audio-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-align-audio
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fast python library for aligning similar audio snippets passed in as NumPy arrays.
 License: ISC
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Multimedia :: Sound/Audio
```

