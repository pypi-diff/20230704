# Comparing `tmp/blosc2_btune-1.0.0rc1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/blosc2_btune-1.0.0rc2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 2881541 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 16:01 blosc2_btune.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 16:01 blosc2_btune/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 16:01 blosc2_btune-1.0.0rc1.dist-info/
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-06 16:01 blosc2_btune/__init__.py
--rwxr-xr-x  2.0 unx  7749768 b- defN 23-Jun-06 16:01 blosc2_btune/libblosc2_btune.so
--rw-r--r--  2.0 unx    13506 b- defN 23-Jun-06 16:01 blosc2_btune-1.0.0rc1.dist-info/METADATA
--rw-rw-r--  2.0 unx      611 b- defN 23-Jun-06 16:01 blosc2_btune-1.0.0rc1.dist-info/RECORD
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-06 16:01 blosc2_btune-1.0.0rc1.dist-info/top_level.txt
--rw-r--r--  2.0 unx      142 b- defN 23-Jun-06 16:01 blosc2_btune-1.0.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx    34689 b- defN 23-Jun-06 16:01 blosc2_btune-1.0.0rc1.dist-info/LICENSE.txt
-10 files, 7799516 bytes uncompressed, 2880117 bytes compressed:  63.1%
+Zip file size: 2881567 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-07 08:33 blosc2_btune.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-07 08:33 blosc2_btune/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-07 08:33 blosc2_btune-1.0.0rc2.dist-info/
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-07 08:33 blosc2_btune/__init__.py
+-rwxr-xr-x  2.0 unx  7749768 b- defN 23-Jun-07 08:33 blosc2_btune/libblosc2_btune.so
+-rw-r--r--  2.0 unx    13558 b- defN 23-Jun-07 08:33 blosc2_btune-1.0.0rc2.dist-info/METADATA
+-rw-rw-r--  2.0 unx      611 b- defN 23-Jun-07 08:33 blosc2_btune-1.0.0rc2.dist-info/RECORD
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-07 08:33 blosc2_btune-1.0.0rc2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-07 08:33 blosc2_btune-1.0.0rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx    34689 b- defN 23-Jun-07 08:33 blosc2_btune-1.0.0rc2.dist-info/LICENSE.txt
+10 files, 7799568 bytes uncompressed, 2880143 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
 Filename: blosc2_btune.libs/
 Comment: 
 
 Filename: blosc2_btune/
 Comment: 
 
-Filename: blosc2_btune-1.0.0rc1.dist-info/
+Filename: blosc2_btune-1.0.0rc2.dist-info/
 Comment: 
 
 Filename: blosc2_btune/__init__.py
 Comment: 
 
 Filename: blosc2_btune/libblosc2_btune.so
 Comment: 
 
-Filename: blosc2_btune-1.0.0rc1.dist-info/METADATA
+Filename: blosc2_btune-1.0.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: blosc2_btune-1.0.0rc1.dist-info/RECORD
+Filename: blosc2_btune-1.0.0rc2.dist-info/RECORD
 Comment: 
 
-Filename: blosc2_btune-1.0.0rc1.dist-info/top_level.txt
+Filename: blosc2_btune-1.0.0rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: blosc2_btune-1.0.0rc1.dist-info/WHEEL
+Filename: blosc2_btune-1.0.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: blosc2_btune-1.0.0rc1.dist-info/LICENSE.txt
+Filename: blosc2_btune-1.0.0rc2.dist-info/LICENSE.txt
 Comment: 
 
 Zip file comment:
```

## blosc2_btune/__init__.py

```diff
@@ -2,15 +2,15 @@
 #
 # Copyright (C) 2021  The Blosc Developers <blosc@blosc.org>
 # https://blosc.org
 # License: BSD 3-Clause (see LICENSE.txt)
 #
 # See LICENSE.txt for details about copyright and rights to use.
 
-VERSION = "1.0.0-rc.1"
+VERSION = "1.0.0-rc.2"
 
 import os
 import platform
 from pathlib import Path
 
 def print_libpath():
     system = platform.system()
```

## blosc2_btune/libblosc2_btune.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 5c44c24d47ae673173de3f86de98d7650d7cdfef
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: c1567d64e3dfbeb8d5246ddf9cca4b944d2051f5
```

### strings --all --bytes=8 {}

```diff
@@ -10873,15 +10873,15 @@
 rhs_data->params.zero_point
 NumDimensions(lhs_data) >= 2
 NumDimensions(lhs_data) <= 5
 NumDimensions(rhs_data) >= 2
 NumDimensions(rhs_data) <= 5
 accum_dim_rhs
 accum_dim_lhs
-/project/_skbuild/linux-x86_64-3.8/cmake-build/ruy/ruy/kernel_common.h
+/project/_skbuild/linux-x86_64-3.9/cmake-build/ruy/ruy/kernel_common.h
 %s:%d: %s condition not satisfied: %s
 /project/tensorflow_src/tensorflow/lite/kernels/batch_matmul.cc
 lhs_data->type == kTfLiteFloat32 || lhs_data->type == kTfLiteInt8 || lhs_data->type == kTfLiteInt16
 rhs_data->type == kTfLiteFloat32 || rhs_data->type == kTfLiteInt8 || rhs_data->type == kTfLiteInt16
 (lhs_data->type == kTfLiteFloat32 && rhs_data->type == kTfLiteInt8) || lhs_data->type == rhs_data->type
 Can only transpose tensors with float, int8 or int16 type.
 mul_params.multiplier_exponent_perchannel()
@@ -12175,24 +12175,24 @@
 N6tflite8resource8internal15StaticHashtableISslEE
 :deque::_M_new_elements_at_front
 deque::_M_new_elements_at_back
 fft2d memory allocation error
 WARNING: Converting from kKeep case.
 residual_rows
 RUY_CHECK_LT
-/project/_skbuild/linux-x86_64-3.8/cmake-build/ruy/ruy/kernel_x86.h
+/project/_skbuild/linux-x86_64-3.9/cmake-build/ruy/ruy/kernel_x86.h
 %s:%d: %s condition not satisfied:   [ %s %s %s ]   with values   [ %s %s %s ].
-/project/_skbuild/linux-x86_64-3.8/cmake-build/ruy/ruy/kernel_avx512.cc
+/project/_skbuild/linux-x86_64-3.9/cmake-build/ruy/ruy/kernel_avx512.cc
 RUY_CHECK_GE
-/project/_skbuild/linux-x86_64-3.8/cmake-build/ruy/ruy/apply_multiplier.cc
+/project/_skbuild/linux-x86_64-3.9/cmake-build/ruy/ruy/apply_multiplier.cc
 (enum value %d)
 ctx->num_threads_strategy()
 RUY_CHECK_EQ
 NumThreadsStrategy::kDefault
-/project/_skbuild/linux-x86_64-3.8/cmake-build/ruy/ruy/trmul.cc
+/project/_skbuild/linux-x86_64-3.9/cmake-build/ruy/ruy/trmul.cc
 N3ruy4TaskE
 *N3ruy12_GLOBAL__N_19TrMulTaskE
 RUY_PATHS
 *ZN3ruy12_GLOBAL__N_127DetectRuntimeSupportedPathsENS_4PathEPNS_7CpuInfoEEUlvE0_
 *ZN3ruy12_GLOBAL__N_127DetectRuntimeSupportedPathsENS_4PathEPNS_7CpuInfoEEUlvE1_
 *ZN3ruy12_GLOBAL__N_127DetectRuntimeSupportedPathsENS_4PathEPNS_7CpuInfoEEUlvE2_
 NSt6thread11_State_implINS_8_InvokerISt5tupleIJPFvPN3ruy6ThreadEES5_EEEEEE
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -4380,15 +4380,15 @@
   0x005fb190 73696f6e 73287268 735f6461 74612920 sions(rhs_data) 
   0x005fb1a0 3e3d2032 004e756d 44696d65 6e73696f >= 2.NumDimensio
   0x005fb1b0 6e732872 68735f64 61746129 203c3d20 ns(rhs_data) <= 
   0x005fb1c0 35007268 735f6469 6d006163 63756d5f 5.rhs_dim.accum_
   0x005fb1d0 64696d5f 72687300 61636375 6d5f6469 dim_rhs.accum_di
   0x005fb1e0 6d5f6c68 73000000 2f70726f 6a656374 m_lhs.../project
   0x005fb1f0 2f5f736b 6275696c 642f6c69 6e75782d /_skbuild/linux-
-  0x005fb200 7838365f 36342d33 2e382f63 6d616b65 x86_64-3.8/cmake
+  0x005fb200 7838365f 36342d33 2e392f63 6d616b65 x86_64-3.9/cmake
   0x005fb210 2d627569 6c642f72 75792f72 75792f6b -build/ruy/ruy/k
   0x005fb220 65726e65 6c5f636f 6d6d6f6e 2e680000 ernel_common.h..
   0x005fb230 25733a25 643a2025 7320636f 6e646974 %s:%d: %s condit
   0x005fb240 696f6e20 6e6f7420 73617469 73666965 ion not satisfie
   0x005fb250 643a2025 730a0000 2f70726f 6a656374 d: %s.../project
   0x005fb260 2f74656e 736f7266 6c6f775f 7372632f /tensorflow_src/
   0x005fb270 74656e73 6f72666c 6f772f6c 6974652f tensorflow/lite/
@@ -9643,15 +9643,15 @@
   0x0060fa80 c865eeff f05feeff 7063eeff 1865eeff .e..._..pc...e..
   0x0060fa90 7065eeff e065eeff f05feeff d861eeff pe...e..._...a..
   0x0060faa0 46636345 00504663 63450025 6c6c6400 FccE.PFccE.%lld.
   0x0060fab0 72657369 6475616c 5f726f77 73005255 residual_rows.RU
   0x0060fac0 595f4348 45434b5f 4c54003c 00000000 Y_CHECK_LT.<....
   0x0060fad0 2f70726f 6a656374 2f5f736b 6275696c /project/_skbuil
   0x0060fae0 642f6c69 6e75782d 7838365f 36342d33 d/linux-x86_64-3
-  0x0060faf0 2e382f63 6d616b65 2d627569 6c642f72 .8/cmake-build/r
+  0x0060faf0 2e392f63 6d616b65 2d627569 6c642f72 .9/cmake-build/r
   0x0060fb00 75792f72 75792f6b 65726e65 6c5f7838 uy/ruy/kernel_x8
   0x0060fb10 362e6800 00000000 25733a25 643a2025 6.h.....%s:%d: %
   0x0060fb20 7320636f 6e646974 696f6e20 6e6f7420 s condition not 
   0x0060fb30 73617469 73666965 643a2020 205b2025 satisfied:   [ %
   0x0060fb40 73202573 20257320 5d202020 77697468 s %s %s ]   with
   0x0060fb50 2076616c 75657320 20205b20 25732025  values   [ %s %
   0x0060fb60 73202573 205d2e0a 00000000 a491eeff s %s ]..........
@@ -9724,21 +9724,21 @@
   0x0060ff90 07000000 07000000 07000000 07000000 ................
   0x0060ffa0 00000040 00000080 00000040 00000080 ...@.......@....
   0x0060ffb0 00000040 00000080 00000040 00000080 ...@.......@....
   0x0060ffc0 00000000 02000000 04000000 06000000 ................
   0x0060ffd0 01000000 03000000 05000000 07000000 ................
   0x0060ffe0 2f70726f 6a656374 2f5f736b 6275696c /project/_skbuil
   0x0060fff0 642f6c69 6e75782d 7838365f 36342d33 d/linux-x86_64-3
-  0x00610000 2e382f63 6d616b65 2d627569 6c642f72 .8/cmake-build/r
+  0x00610000 2e392f63 6d616b65 2d627569 6c642f72 .9/cmake-build/r
   0x00610010 75792f72 75792f6b 65726e65 6c5f6176 uy/ruy/kernel_av
   0x00610020 78353132 2e636300 73686966 74005255 x512.cc.shift.RU
   0x00610030 595f4348 45434b5f 4745003e 3d002d33 Y_CHECK_GE.>=.-3
   0x00610040 31000000 00000000 2f70726f 6a656374 1......./project
   0x00610050 2f5f736b 6275696c 642f6c69 6e75782d /_skbuild/linux-
-  0x00610060 7838365f 36342d33 2e382f63 6d616b65 x86_64-3.8/cmake
+  0x00610060 7838365f 36342d33 2e392f63 6d616b65 x86_64-3.9/cmake
   0x00610070 2d627569 6c642f72 75792f72 75792f61 -build/ruy/ruy/a
   0x00610080 70706c79 5f6d756c 7469706c 6965722e pply_multiplier.
   0x00610090 63630000 00000000 00000000 00000000 cc..............
   0x006100a0 01000100 01000100 01000100 01000100 ................
   0x006100b0 01000100 01000100 01000100 01000100 ................
   0x006100c0 00000000 01000000 02000000 03000000 ................
   0x006100d0 04000000 05000000 06000000 07000000 ................
@@ -9758,15 +9758,15 @@
   0x006101b0 6374782d 3e6e756d 5f746872 65616473 ctx->num_threads
   0x006101c0 5f737472 61746567 79282900 5255595f _strategy().RUY_
   0x006101d0 43484543 4b5f4551 003d3d00 4e756d54 CHECK_EQ.==.NumT
   0x006101e0 68726561 64735374 72617465 67793a3a hreadsStrategy::
   0x006101f0 6b446566 61756c74 00000000 00000000 kDefault........
   0x00610200 2f70726f 6a656374 2f5f736b 6275696c /project/_skbuil
   0x00610210 642f6c69 6e75782d 7838365f 36342d33 d/linux-x86_64-3
-  0x00610220 2e382f63 6d616b65 2d627569 6c642f72 .8/cmake-build/r
+  0x00610220 2e392f63 6d616b65 2d627569 6c642f72 .9/cmake-build/r
   0x00610230 75792f72 75792f74 726d756c 2e636300 uy/ruy/trmul.cc.
   0x00610240 4e337275 79345461 736b4500 00000000 N3ruy4TaskE.....
   0x00610250 00000000 00000000 00000000 00000000 ................
   0x00610260 2a4e3372 75793132 5f474c4f 42414c5f *N3ruy12_GLOBAL_
   0x00610270 5f4e5f31 3954724d 756c5461 736b4500 _N_19TrMulTaskE.
   0x00610280 5255595f 50415448 53007374 6f690000 RUY_PATHS.stoi..
   0x00610290 00000000 00000000 00000000 00000000 ................
```

## Comparing `blosc2_btune-1.0.0rc1.dist-info/METADATA` & `blosc2_btune-1.0.0rc2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: blosc2-btune
-Version: 1.0.0rc1
-Summary: My package description
-Author-email: Blosc Development Team <blosc@blosc.org>
-License: BSD-3-Clause
+Version: 1.0.0rc2
+Summary: BTUNE plugin for Blosc2. Automatically choose the best codec/filter for your data.
+Author-email: Blosc Development Team <contact@blosc.org>
+License: GNU Affero General Public License version 3
 Keywords: plugin,blosc2
 Platform: any
-Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: C
+Classifier: Programming Language :: C++
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: C
-Classifier: Programming Language :: C++
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Blosc2 BTune
 
 BTune is a dynamic plugin for Blosc2 that helps you find the optimal combination of compression parameters by training a neural network on your most representative datasets.
```

## Comparing `blosc2_btune-1.0.0rc1.dist-info/LICENSE.txt` & `blosc2_btune-1.0.0rc2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

