# Comparing `tmp/tflite_runtime_nightly-2.14.0.dev20230701-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.14.0.dev20230702-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2404757 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-Jul-02 05:02 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6832592 b- defN 23-Jul-02 05:04 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-Jul-02 05:02 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-Jul-02 05:02 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-Jul-02 05:02 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1441 b- defN 23-Jul-02 05:04 tflite_runtime_nightly-2.14.0.dev20230701.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-Jul-02 05:04 tflite_runtime_nightly-2.14.0.dev20230701.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jul-02 05:04 tflite_runtime_nightly-2.14.0.dev20230701.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Jul-02 05:04 tflite_runtime_nightly-2.14.0.dev20230701.dist-info/RECORD
-9 files, 6877482 bytes uncompressed, 2403211 bytes compressed:  65.1%
+Zip file size: 2404758 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-03 05:00 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6832592 b- defN 23-Jul-03 05:02 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-Jul-03 05:00 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-Jul-03 05:00 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Jul-03 05:00 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1441 b- defN 23-Jul-03 05:02 tflite_runtime_nightly-2.14.0.dev20230702.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-Jul-03 05:02 tflite_runtime_nightly-2.14.0.dev20230702.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jul-03 05:02 tflite_runtime_nightly-2.14.0.dev20230702.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Jul-03 05:02 tflite_runtime_nightly-2.14.0.dev20230702.dist-info/RECORD
+9 files, 6877482 bytes uncompressed, 2403212 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230701.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.14.0.dev20230702.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230701.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.14.0.dev20230702.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230701.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.14.0.dev20230702.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230701.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.14.0.dev20230702.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.14.0dev20230701'
-__git_version__ = '0.6.0-150074-g2a5fbc57749'
+__version__ = '2.14.0dev20230702'
+__git_version__ = '0.6.0-150079-gd73b955e04f'
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230701.dist-info/METADATA` & `tflite_runtime_nightly-2.14.0.dev20230702.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.14.0.dev20230701
+Version: 2.14.0.dev20230702
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230701.dist-info/RECORD` & `tflite_runtime_nightly-2.14.0.dev20230702.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tflite_runtime/__init__.py,sha256=yhsk1zc9nkHNbNsu7tqYO9Sv8f7mJLbxG1qNmYen8m0,80
+tflite_runtime/__init__.py,sha256=jO_Wxf8cl9yX4wuCRGHLFppZjmxe_WlhWewvHUyPYuA,80
 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so,sha256=7fwaoTUV8Zbv85HV-ImljprVdaRZm7Jwi85DIogjEGI,6832592
 tflite_runtime/interpreter.py,sha256=WdMKqxuFdoGPyOKoCsZsHbvsVQXs_81OrG7VUE8p5JU,38775
 tflite_runtime/metrics_interface.py,sha256=dVu6SmbnQUntPgE5o6BxHVMyemwli-7F6tDfVMGrlYI,1542
 tflite_runtime/metrics_portable.py,sha256=YBiMNokP9JtoQaUcCRRY1T_iFSZGeWCjr6L0iUR6eY8,2048
-tflite_runtime_nightly-2.14.0.dev20230701.dist-info/METADATA,sha256=OXr3Bm6RWhtla3dPw6K9heO0-LNHb5z0DMfFEhrInOk,1441
-tflite_runtime_nightly-2.14.0.dev20230701.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
-tflite_runtime_nightly-2.14.0.dev20230701.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
-tflite_runtime_nightly-2.14.0.dev20230701.dist-info/RECORD,,
+tflite_runtime_nightly-2.14.0.dev20230702.dist-info/METADATA,sha256=xSSzAeRBh9dUfs3kcGn6AkDk7NTee3plxISLT1OvTOQ,1441
+tflite_runtime_nightly-2.14.0.dev20230702.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
+tflite_runtime_nightly-2.14.0.dev20230702.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
+tflite_runtime_nightly-2.14.0.dev20230702.dist-info/RECORD,,
```

