# Comparing `tmp/deface-1.3.0.tar.gz` & `tmp/deface-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deface-1.3.0.tar", last modified: Mon May  1 20:24:19 2023, max compression
+gzip compressed data, was "deface-1.4.0.tar", last modified: Tue Jul  4 15:16:46 2023, max compression
```

## Comparing `deface-1.3.0.tar` & `deface-1.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.761496 deface-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-01 20:24:05.000000 deface-1.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.749496 deface-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.749496 deface-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-01 20:24:05.000000 deface-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-01 20:24:05.000000 deface-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-01 20:24:05.000000 deface-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-05-01 20:24:19.761496 deface-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-01 20:24:05.000000 deface-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.757496 deface-1.3.0/deface/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-01 20:24:05.000000 deface-1.3.0/deface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 20:24:19.000000 deface-1.3.0/deface/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)  7532772 2023-05-01 20:24:05.000000 deface-1.3.0/deface/centerface.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-01 20:24:05.000000 deface-1.3.0/deface/centerface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14681 2023-05-01 20:24:05.000000 deface-1.3.0/deface/deface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.757496 deface-1.3.0/deface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-01 20:24:05.000000 deface-1.3.0/deface.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.761496 deface-1.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    83046 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    82598 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city_anonymized.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    80240 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city_anonymized_boxes.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    86879 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city_anonymized_scores.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    78648 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city_anonymized_thresh0.02.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    83369 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city_anonymized_thresh0.7.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-01 20:24:05.000000 deface-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-01 20:24:05.000000 deface-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:24:19.761496 deface-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:16:46.648390 deface-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-04 15:16:36.000000 deface-1.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:16:46.636390 deface-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:16:46.636390 deface-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-04 15:16:36.000000 deface-1.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-04 15:16:36.000000 deface-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-04 15:16:36.000000 deface-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15877 2023-07-04 15:16:46.648390 deface-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-07-04 15:16:36.000000 deface-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:16:46.644390 deface-1.4.0/deface/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 15:16:36.000000 deface-1.4.0/deface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 15:16:46.000000 deface-1.4.0/deface/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7304518 2023-07-04 15:16:36.000000 deface-1.4.0/deface/centerface.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-04 15:16:36.000000 deface-1.4.0/deface/centerface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15011 2023-07-04 15:16:36.000000 deface-1.4.0/deface/deface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:16:46.644390 deface-1.4.0/deface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15877 2023-07-04 15:16:46.000000 deface-1.4.0/deface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-04 15:16:46.000000 deface-1.4.0/deface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:16:46.000000 deface-1.4.0/deface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-04 15:16:46.000000 deface-1.4.0/deface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-04 15:16:46.000000 deface-1.4.0/deface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 15:16:46.000000 deface-1.4.0/deface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-04 15:16:36.000000 deface-1.4.0/deface.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:16:46.648390 deface-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    83046 2023-07-04 15:16:36.000000 deface-1.4.0/examples/city.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    82598 2023-07-04 15:16:36.000000 deface-1.4.0/examples/city_anonymized.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    80240 2023-07-04 15:16:36.000000 deface-1.4.0/examples/city_anonymized_boxes.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    86879 2023-07-04 15:16:36.000000 deface-1.4.0/examples/city_anonymized_scores.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    78648 2023-07-04 15:16:36.000000 deface-1.4.0/examples/city_anonymized_thresh0.02.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    83369 2023-07-04 15:16:36.000000 deface-1.4.0/examples/city_anonymized_thresh0.7.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-04 15:16:36.000000 deface-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 15:16:36.000000 deface-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:16:46.648390 deface-1.4.0/setup.cfg
```

### Comparing `deface-1.3.0/.github/workflows/python-publish.yml` & `deface-1.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/.gitignore` & `deface-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/LICENSE` & `deface-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/PKG-INFO` & `deface-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deface
-Version: 1.3.0
+Version: 1.4.0
 Summary: Video anonymization by face detection
 License: MIT License
         
         Copyright (c) 2020 Martin Drawitsch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -27,17 +27,21 @@
 Project-URL: repository, https://github.com/ORB-HD/deface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: gpu
+Provides-Extra: cuda
+Provides-Extra: directml
+Provides-Extra: openvino
 License-File: LICENSE
 
+[![PyPI](https://img.shields.io/pypi/v/deface)](https://pypi.org/project/deface/) [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ORB-HD/deface/python-publish.yml)](https://github.com/ORB-HD/deface/actions)
+
 # `deface`: Video anonymization by face detection
 
 `deface` is a simple command-line tool for automatic anonymization of faces in videos or photos.
 It works by first detecting all human faces in each video frame and then applying an anonymization filter (blurring or black boxes) on each detected face region.
 By default all audio tracks are discarded as well.
 
 
@@ -134,14 +138,20 @@
                         FFMPEG config arguments for encoding output videos.
                         This argument is expected in JSON notation. For a list
                         of possible options, refer to the ffmpeg-imageio docs.
                         Default: '{"codec": "libx264"}'.
   --backend {auto,onnxrt,opencv}
                         Backend for ONNX model execution. Default: "auto"
                         (prefer onnxrt if available).
+  --execution-provider EP, --ep EP
+                        Override onnxrt execution provider (see
+                        https://onnxruntime.ai/docs/execution-providers/). If
+                        not specified, the presumably fastest available one
+                        will be automatically selected. Only used if backend is
+                        onnxrt.
   --version             Print version number and exit.
   --help, -h            Show this help message and exit.
 ```
 
 ## Usage examples
 
 In most use cases the default configuration should be sufficient, but depending on individual requirements and type of media to be processed, some of the options might need to be adjusted. In this section, some common example scenarios that require option changes are presented. All of the examples use the photo [examples/city.jpg](examples/city.jpg), but they work the same on any video or photo file.
@@ -193,37 +203,53 @@
 
 For example, if your inputs have the common aspect ratio 16:9, you can instruct the detector to run in 360p resolution by specifying `--scale 640x360`.
 If the results at this fairly low resolution are not good enough, detection at 720p input resolution (`--scale 1280x720`) may work better.
 
 
 ## Hardware acceleration
 
-Depending on your available hardware, you can often speed up neural network inference by enabling the optional [ONNX Runtime](https://microsoft.github.io/onnxruntime/) backend of `deface`.
+Depending on your available hardware, you can speed up neural network inference by enabling the optional [ONNX Runtime](https://microsoft.github.io/onnxruntime/) backend of `deface`. For optimal performance you should install it with appropriate [Execution Providers](https://onnxruntime.ai/docs/execution-providers) for your system. If you have multiple Execution Providers installed, ONNX Runtime will try to automatically use the fastest one available.
+
+Here are some recommendations for common setups:
 
-### CUDA (on Nvidia GPUs)
+### CUDA (only for Nvidia GPUs)
 
 If you have a CUDA-capable GPU, you can enable GPU acceleration by installing the relevant packages:
 
     $ python3 -m pip install onnx onnxruntime-gpu
 
 If the `onnxruntime-gpu` package is found and a GPU is available, the face detection network is automatically offloaded to the GPU.
 This can significantly improve the overall processing speed.
 
+### DirectML (only for Windows)
+
+Windows users with capable non-Nvidia GPUs can enable GPU-accelerated inference with DirectML by installing:
+
+    $ python3 -m pip install onnx onnxruntime-directml
+
+### OpenVINO
+
+OpenVINO can accelerate inference even on CPU-only systems by a few percent, compared to the default OpenCV and ONNX Runtime implementations. It works on Linux and Windows, but not yet on Python 3.11 as of July 2023. Install the backend with:
+
+    $ python3 -m pip install onnx onnxruntime-openvino
+
+
 ### Other platforms
 
-If your machine doesn't have a CUDA-capable GPU but you want to accelerate computation on another hardware platform (e.g. Intel CPUs), you can look into the available options in the [ONNX Runtime build matrix](https://microsoft.github.io/onnxruntime/).
+If you your setup doesn't fit with these recommendations, look into the available options at the [Execution Provider](https://onnxruntime.ai/docs/execution-providers/#summary-of-supported-execution-providers) documentation and find the respective installation instructions in the [ONNX Runtime build matrix](https://microsoft.github.io/onnxruntime/).
 
 
 ## How it works
 
 The included face detection system is based on CenterFace ([code](https://github.com/Star-Clouds/centerface), [paper](https://arxiv.org/abs/1911.03599)), a deep neural network optimized for fast but reliable detection of human faces in photos.
 The network was trained on the [WIDER FACE](http://shuoyang1213.me/WIDERFACE/) dataset, which contains annotated photos showing faces in a wide variety of scales, poses and occlusions.
 
 Although the face detector is originally intended to be used for normal 2D images, `deface` can also use it to detect faces in video data by analyzing each video frame independently.
 The face bounding boxes predicted by the CenterFace detector are then used as masks to determine where to apply anonymization filters.
 
 
 ## Credits
 
-- `centerface.onnx` (original) and `centerface.py` (modified) are based on https://github.com/Star-Clouds/centerface (revision [8c39a49](https://github.com/Star-Clouds/CenterFace/tree/8c39a497afb78fb2c064eb84bf010c273bb7d3ce)),
-  [released under MIT license](https://github.com/Star-Clouds/CenterFace/blob/36afed/LICENSE).
-- The original source of the example images in the `examples` directory can be found [here](https://www.pexels.com/de-de/foto/stadt-kreuzung-strasse-menschen-109919/) (released under the [Pexels photo license](https://www.pexels.com/photo-license/)).
+- `centerface.py` is based on https://github.com/Star-Clouds/centerface (revision [8c39a49](https://github.com/Star-Clouds/CenterFace/tree/8c39a497afb78fb2c064eb84bf010c273bb7d3ce)),
+  [released under MIT license](https://github.com/Star-Clouds/CenterFace/blob/36afed/LICENSE)
+- The included model file `centerface.onnx` is an unmodified copy of the [`centerface_bnmerged.onnx`](https://github.com/Star-Clouds/CenterFace/blob/b82ec0c4844e89fd5a0305986aed9bdf33c72585/models/onnx/centerface_bnmerged.onnx) from https://github.com/Star-Clouds/centerface
+- The original source of the example images in the `examples` directory can be found [here](https://www.pexels.com/de-de/foto/stadt-kreuzung-strasse-menschen-109919/) (released under the [Pexels photo license](https://www.pexels.com/photo-license/))
```

### Comparing `deface-1.3.0/README.md` & `deface-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI](https://img.shields.io/pypi/v/deface)](https://pypi.org/project/deface/) [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ORB-HD/deface/python-publish.yml)](https://github.com/ORB-HD/deface/actions)
+
 # `deface`: Video anonymization by face detection
 
 `deface` is a simple command-line tool for automatic anonymization of faces in videos or photos.
 It works by first detecting all human faces in each video frame and then applying an anonymization filter (blurring or black boxes) on each detected face region.
 By default all audio tracks are discarded as well.
 
 
@@ -98,14 +100,20 @@
                         FFMPEG config arguments for encoding output videos.
                         This argument is expected in JSON notation. For a list
                         of possible options, refer to the ffmpeg-imageio docs.
                         Default: '{"codec": "libx264"}'.
   --backend {auto,onnxrt,opencv}
                         Backend for ONNX model execution. Default: "auto"
                         (prefer onnxrt if available).
+  --execution-provider EP, --ep EP
+                        Override onnxrt execution provider (see
+                        https://onnxruntime.ai/docs/execution-providers/). If
+                        not specified, the presumably fastest available one
+                        will be automatically selected. Only used if backend is
+                        onnxrt.
   --version             Print version number and exit.
   --help, -h            Show this help message and exit.
 ```
 
 ## Usage examples
 
 In most use cases the default configuration should be sufficient, but depending on individual requirements and type of media to be processed, some of the options might need to be adjusted. In this section, some common example scenarios that require option changes are presented. All of the examples use the photo [examples/city.jpg](examples/city.jpg), but they work the same on any video or photo file.
@@ -157,37 +165,53 @@
 
 For example, if your inputs have the common aspect ratio 16:9, you can instruct the detector to run in 360p resolution by specifying `--scale 640x360`.
 If the results at this fairly low resolution are not good enough, detection at 720p input resolution (`--scale 1280x720`) may work better.
 
 
 ## Hardware acceleration
 
-Depending on your available hardware, you can often speed up neural network inference by enabling the optional [ONNX Runtime](https://microsoft.github.io/onnxruntime/) backend of `deface`.
+Depending on your available hardware, you can speed up neural network inference by enabling the optional [ONNX Runtime](https://microsoft.github.io/onnxruntime/) backend of `deface`. For optimal performance you should install it with appropriate [Execution Providers](https://onnxruntime.ai/docs/execution-providers) for your system. If you have multiple Execution Providers installed, ONNX Runtime will try to automatically use the fastest one available.
+
+Here are some recommendations for common setups:
 
-### CUDA (on Nvidia GPUs)
+### CUDA (only for Nvidia GPUs)
 
 If you have a CUDA-capable GPU, you can enable GPU acceleration by installing the relevant packages:
 
     $ python3 -m pip install onnx onnxruntime-gpu
 
 If the `onnxruntime-gpu` package is found and a GPU is available, the face detection network is automatically offloaded to the GPU.
 This can significantly improve the overall processing speed.
 
+### DirectML (only for Windows)
+
+Windows users with capable non-Nvidia GPUs can enable GPU-accelerated inference with DirectML by installing:
+
+    $ python3 -m pip install onnx onnxruntime-directml
+
+### OpenVINO
+
+OpenVINO can accelerate inference even on CPU-only systems by a few percent, compared to the default OpenCV and ONNX Runtime implementations. It works on Linux and Windows, but not yet on Python 3.11 as of July 2023. Install the backend with:
+
+    $ python3 -m pip install onnx onnxruntime-openvino
+
+
 ### Other platforms
 
-If your machine doesn't have a CUDA-capable GPU but you want to accelerate computation on another hardware platform (e.g. Intel CPUs), you can look into the available options in the [ONNX Runtime build matrix](https://microsoft.github.io/onnxruntime/).
+If you your setup doesn't fit with these recommendations, look into the available options at the [Execution Provider](https://onnxruntime.ai/docs/execution-providers/#summary-of-supported-execution-providers) documentation and find the respective installation instructions in the [ONNX Runtime build matrix](https://microsoft.github.io/onnxruntime/).
 
 
 ## How it works
 
 The included face detection system is based on CenterFace ([code](https://github.com/Star-Clouds/centerface), [paper](https://arxiv.org/abs/1911.03599)), a deep neural network optimized for fast but reliable detection of human faces in photos.
 The network was trained on the [WIDER FACE](http://shuoyang1213.me/WIDERFACE/) dataset, which contains annotated photos showing faces in a wide variety of scales, poses and occlusions.
 
 Although the face detector is originally intended to be used for normal 2D images, `deface` can also use it to detect faces in video data by analyzing each video frame independently.
 The face bounding boxes predicted by the CenterFace detector are then used as masks to determine where to apply anonymization filters.
 
 
 ## Credits
 
-- `centerface.onnx` (original) and `centerface.py` (modified) are based on https://github.com/Star-Clouds/centerface (revision [8c39a49](https://github.com/Star-Clouds/CenterFace/tree/8c39a497afb78fb2c064eb84bf010c273bb7d3ce)),
-  [released under MIT license](https://github.com/Star-Clouds/CenterFace/blob/36afed/LICENSE).
-- The original source of the example images in the `examples` directory can be found [here](https://www.pexels.com/de-de/foto/stadt-kreuzung-strasse-menschen-109919/) (released under the [Pexels photo license](https://www.pexels.com/photo-license/)).
+- `centerface.py` is based on https://github.com/Star-Clouds/centerface (revision [8c39a49](https://github.com/Star-Clouds/CenterFace/tree/8c39a497afb78fb2c064eb84bf010c273bb7d3ce)),
+  [released under MIT license](https://github.com/Star-Clouds/CenterFace/blob/36afed/LICENSE)
+- The included model file `centerface.onnx` is an unmodified copy of the [`centerface_bnmerged.onnx`](https://github.com/Star-Clouds/CenterFace/blob/b82ec0c4844e89fd5a0305986aed9bdf33c72585/models/onnx/centerface_bnmerged.onnx) from https://github.com/Star-Clouds/centerface
+- The original source of the example images in the `examples` directory can be found [here](https://www.pexels.com/de-de/foto/stadt-kreuzung-strasse-menschen-109919/) (released under the [Pexels photo license](https://www.pexels.com/photo-license/))
```

### Comparing `deface-1.3.0/deface/centerface.py` & `deface-1.4.0/deface/centerface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import datetime
 import os
 
+from functools import lru_cache
+
 import numpy as np
 import cv2
 
 
 # Find file relative to the location of this code files
 default_onnx_path = f'{os.path.dirname(__file__)}/centerface.onnx'
 
@@ -15,15 +16,15 @@
         img = cv2.cvtColor(img, cv2.COLOR_GRAY2RGB)
     elif img.shape[2] == 4:  # 4-channel RGBA -> RGB
         img = cv2.cvtColor(img, cv2.COLOR_RGBA2RGB)
     return img
 
 
 class CenterFace:
-    def __init__(self, onnx_path=None, in_shape=None, backend='auto'):
+    def __init__(self, onnx_path=None, in_shape=None, backend='auto', override_execution_provider=None):
         self.in_shape = in_shape
         self.onnx_input_name = 'input.1'
         self.onnx_output_names = ['537', '538', '539', '540']
 
         if onnx_path is None:
             onnx_path = default_onnx_path
 
@@ -46,19 +47,32 @@
             import onnxruntime
 
             # Silence warnings about unnecessary bn initializers
             onnxruntime.set_default_logger_severity(3)
 
             static_model = onnx.load(onnx_path)
             dyn_model = self.dynamicize_shapes(static_model)
-            self.sess = onnxruntime.InferenceSession(dyn_model.SerializeToString(), providers=['CUDAExecutionProvider', 'CPUExecutionProvider'])
+
+            # onnxruntime.get_available_providers() Returns a list of all
+            #  available providers in a reasonable ordering (GPU providers
+            #  first, then accelerated CPU providers like OpenVINO, then
+            #  CPUExecutionProvider as the last choice).
+            #  In normal conditions, overriding this choice won't be necessary.
+            available_providers = onnxruntime.get_available_providers()
+            if override_execution_provider is None:
+                ort_providers = available_providers
+            else:
+                if override_execution_provider not in available_providers:
+                    raise ValueError(f'{override_execution_provider=} not found. Available providers are: {available_providers}')
+                ort_providers = [override_execution_provider]
+
+            self.sess = onnxruntime.InferenceSession(dyn_model.SerializeToString(), providers=ort_providers)
 
             preferred_provider = self.sess.get_providers()[0]
-            preferred_device = 'GPU' if preferred_provider.startswith('CUDA') else 'CPU'
-            # print(f'Running on {preferred_device}.')
+            print(f'Running on {preferred_provider}.')
 
     @staticmethod
     def dynamicize_shapes(static_model):
         from onnx.tools.update_model_dims import update_inputs_outputs_dims
 
         input_dims, output_dims = {}, {}
         for node in static_model.graph.input:
@@ -77,43 +91,44 @@
             '540': ['B', 10, 'h', 'w']  # landmarks
         })
         dyn_model = update_inputs_outputs_dims(static_model, input_dims, output_dims)
         return dyn_model
 
     def __call__(self, img, threshold=0.5):
         img = ensure_rgb(img)
-        self.orig_shape = img.shape[:2]
-        if self.in_shape is None:
-            self.in_shape = self.orig_shape[::-1]
-        if not hasattr(self, 'h_new'):  # First call, need to compute sizes
-            self.w_new, self.h_new, self.scale_w, self.scale_h = self.transform(self.in_shape)
+        orig_shape = img.shape[:2]
+        in_shape = orig_shape[::-1] if self.in_shape is None else self.in_shape
+        # Compute sizes
+        w_new, h_new, scale_w, scale_h = self.shape_transform(in_shape, orig_shape)
 
         blob = cv2.dnn.blobFromImage(
-            img, scalefactor=1.0, size=(self.w_new, self.h_new),
+            img, scalefactor=1.0, size=(w_new, h_new),
             mean=(0, 0, 0), swapRB=False, crop=False
         )
         if self.backend == 'opencv':
             self.net.setInput(blob)
             heatmap, scale, offset, lms = self.net.forward(self.onnx_output_names)
         elif self.backend == 'onnxrt':
             heatmap, scale, offset, lms = self.sess.run(self.onnx_output_names, {self.onnx_input_name: blob})
         else:
             raise RuntimeError(f'Unknown backend {self.backend}')
-        dets, lms = self.decode(heatmap, scale, offset, lms, (self.h_new, self.w_new), threshold=threshold)
+        dets, lms = self.decode(heatmap, scale, offset, lms, (h_new, w_new), threshold=threshold)
         if len(dets) > 0:
-            dets[:, 0:4:2], dets[:, 1:4:2] = dets[:, 0:4:2] / self.scale_w, dets[:, 1:4:2] / self.scale_h
-            lms[:, 0:10:2], lms[:, 1:10:2] = lms[:, 0:10:2] / self.scale_w, lms[:, 1:10:2] / self.scale_h
+            dets[:, 0:4:2], dets[:, 1:4:2] = dets[:, 0:4:2] / scale_w, dets[:, 1:4:2] / scale_h
+            lms[:, 0:10:2], lms[:, 1:10:2] = lms[:, 0:10:2] / scale_w, lms[:, 1:10:2] / scale_h
         else:
             dets = np.empty(shape=[0, 5], dtype=np.float32)
             lms = np.empty(shape=[0, 10], dtype=np.float32)
 
         return dets, lms
 
-    def transform(self, in_shape):
-        h_orig, w_orig = self.orig_shape
+    @staticmethod
+    @lru_cache(maxsize=128)
+    def shape_transform(in_shape, orig_shape):
+        h_orig, w_orig = orig_shape
         w_new, h_new = in_shape
         # Make spatial dims divisible by 32
         w_new, h_new = int(np.ceil(w_new / 32) * 32), int(np.ceil(h_new / 32) * 32)
         scale_w, scale_h = w_new / w_orig, h_new / h_orig
         return w_new, h_new, scale_w, scale_h
 
     def decode(self, heatmap, scale, offset, landmark, size, threshold=0.1):
```

### Comparing `deface-1.3.0/deface/deface.py` & `deface-1.4.0/deface/deface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 #!/usr/bin/env python3
 
 import argparse
-import glob
 import json
 import mimetypes
 import os
-import sys
 from typing import Dict, Tuple
 
 import tqdm
 import skimage.draw
 import numpy as np
 import imageio
 import imageio.plugins.ffmpeg
 import cv2
 
 from deface import __version__
-# __version__ = 'a'
 from deface.centerface import CenterFace
 
 
-# TODO: Optionally preserve audio track?
-
-
 def scale_bb(x1, y1, x2, y2, mask_scale=1.0):
     s = mask_scale - 1.0
     h, w = y2 - y1, x2 - x1
     y1 -= h * s
     y2 += h * s
     x1 -= w * s
     x2 += w * s
@@ -288,14 +282,17 @@
         '--ffmpeg-config', default={"codec": "libx264"}, type=json.loads,
         help='FFMPEG config arguments for encoding output videos. This argument is expected in JSON notation. For a list of possible options, refer to the ffmpeg-imageio docs. Default: \'{"codec": "libx264"}\'.'
     )  # See https://imageio.readthedocs.io/en/stable/format_ffmpeg.html#parameters-for-saving
     parser.add_argument(
         '--backend', default='auto', choices=['auto', 'onnxrt', 'opencv'],
         help='Backend for ONNX model execution. Default: "auto" (prefer onnxrt if available).')
     parser.add_argument(
+        '--execution-provider', '--ep', default=None, metavar='EP',
+        help='Override onnxrt execution provider (see https://onnxruntime.ai/docs/execution-providers/). If not specified, the presumably fastest available one will be automatically selected. Only used if backend is onnxrt.')
+    parser.add_argument(
         '--version', action='version', version=__version__,
         help='Print version number and exit.')
     parser.add_argument('--help', '-h', action='help', help='Show this help message and exit.')
 
     args = parser.parse_args()
 
     if len(args.input) == 0:
@@ -331,25 +328,26 @@
     threshold = args.thresh
     ellipse = not args.boxes
     mask_scale = args.mask_scale
     keep_audio = args.keep_audio
     ffmpeg_config = args.ffmpeg_config
     backend = args.backend
     in_shape = args.scale
+    execution_provider = args.execution_provider
     replaceimg = None
     if in_shape is not None:
         w, h = in_shape.split('x')
         in_shape = int(w), int(h)
     if replacewith == "img":
         replaceimg = imageio.imread(args.replaceimg)
         print(f'After opening {args.replaceimg} shape: {replaceimg.shape}')
 
 
     # TODO: scalar downscaling setting (-> in_shape), preserving aspect ratio
-    centerface = CenterFace(in_shape=in_shape, backend=backend)
+    centerface = CenterFace(in_shape=in_shape, backend=backend, override_execution_provider=execution_provider)
 
     multi_file = len(ipaths) > 1
     if multi_file:
         ipaths = tqdm.tqdm(ipaths, position=0, dynamic_ncols=True, desc='Batch progress')
 
     for ipath in ipaths:
         opath = base_opath
```

### Comparing `deface-1.3.0/deface.egg-info/PKG-INFO` & `deface-1.4.0/deface.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deface
-Version: 1.3.0
+Version: 1.4.0
 Summary: Video anonymization by face detection
 License: MIT License
         
         Copyright (c) 2020 Martin Drawitsch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -27,17 +27,21 @@
 Project-URL: repository, https://github.com/ORB-HD/deface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: gpu
+Provides-Extra: cuda
+Provides-Extra: directml
+Provides-Extra: openvino
 License-File: LICENSE
 
+[![PyPI](https://img.shields.io/pypi/v/deface)](https://pypi.org/project/deface/) [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ORB-HD/deface/python-publish.yml)](https://github.com/ORB-HD/deface/actions)
+
 # `deface`: Video anonymization by face detection
 
 `deface` is a simple command-line tool for automatic anonymization of faces in videos or photos.
 It works by first detecting all human faces in each video frame and then applying an anonymization filter (blurring or black boxes) on each detected face region.
 By default all audio tracks are discarded as well.
 
 
@@ -134,14 +138,20 @@
                         FFMPEG config arguments for encoding output videos.
                         This argument is expected in JSON notation. For a list
                         of possible options, refer to the ffmpeg-imageio docs.
                         Default: '{"codec": "libx264"}'.
   --backend {auto,onnxrt,opencv}
                         Backend for ONNX model execution. Default: "auto"
                         (prefer onnxrt if available).
+  --execution-provider EP, --ep EP
+                        Override onnxrt execution provider (see
+                        https://onnxruntime.ai/docs/execution-providers/). If
+                        not specified, the presumably fastest available one
+                        will be automatically selected. Only used if backend is
+                        onnxrt.
   --version             Print version number and exit.
   --help, -h            Show this help message and exit.
 ```
 
 ## Usage examples
 
 In most use cases the default configuration should be sufficient, but depending on individual requirements and type of media to be processed, some of the options might need to be adjusted. In this section, some common example scenarios that require option changes are presented. All of the examples use the photo [examples/city.jpg](examples/city.jpg), but they work the same on any video or photo file.
@@ -193,37 +203,53 @@
 
 For example, if your inputs have the common aspect ratio 16:9, you can instruct the detector to run in 360p resolution by specifying `--scale 640x360`.
 If the results at this fairly low resolution are not good enough, detection at 720p input resolution (`--scale 1280x720`) may work better.
 
 
 ## Hardware acceleration
 
-Depending on your available hardware, you can often speed up neural network inference by enabling the optional [ONNX Runtime](https://microsoft.github.io/onnxruntime/) backend of `deface`.
+Depending on your available hardware, you can speed up neural network inference by enabling the optional [ONNX Runtime](https://microsoft.github.io/onnxruntime/) backend of `deface`. For optimal performance you should install it with appropriate [Execution Providers](https://onnxruntime.ai/docs/execution-providers) for your system. If you have multiple Execution Providers installed, ONNX Runtime will try to automatically use the fastest one available.
+
+Here are some recommendations for common setups:
 
-### CUDA (on Nvidia GPUs)
+### CUDA (only for Nvidia GPUs)
 
 If you have a CUDA-capable GPU, you can enable GPU acceleration by installing the relevant packages:
 
     $ python3 -m pip install onnx onnxruntime-gpu
 
 If the `onnxruntime-gpu` package is found and a GPU is available, the face detection network is automatically offloaded to the GPU.
 This can significantly improve the overall processing speed.
 
+### DirectML (only for Windows)
+
+Windows users with capable non-Nvidia GPUs can enable GPU-accelerated inference with DirectML by installing:
+
+    $ python3 -m pip install onnx onnxruntime-directml
+
+### OpenVINO
+
+OpenVINO can accelerate inference even on CPU-only systems by a few percent, compared to the default OpenCV and ONNX Runtime implementations. It works on Linux and Windows, but not yet on Python 3.11 as of July 2023. Install the backend with:
+
+    $ python3 -m pip install onnx onnxruntime-openvino
+
+
 ### Other platforms
 
-If your machine doesn't have a CUDA-capable GPU but you want to accelerate computation on another hardware platform (e.g. Intel CPUs), you can look into the available options in the [ONNX Runtime build matrix](https://microsoft.github.io/onnxruntime/).
+If you your setup doesn't fit with these recommendations, look into the available options at the [Execution Provider](https://onnxruntime.ai/docs/execution-providers/#summary-of-supported-execution-providers) documentation and find the respective installation instructions in the [ONNX Runtime build matrix](https://microsoft.github.io/onnxruntime/).
 
 
 ## How it works
 
 The included face detection system is based on CenterFace ([code](https://github.com/Star-Clouds/centerface), [paper](https://arxiv.org/abs/1911.03599)), a deep neural network optimized for fast but reliable detection of human faces in photos.
 The network was trained on the [WIDER FACE](http://shuoyang1213.me/WIDERFACE/) dataset, which contains annotated photos showing faces in a wide variety of scales, poses and occlusions.
 
 Although the face detector is originally intended to be used for normal 2D images, `deface` can also use it to detect faces in video data by analyzing each video frame independently.
 The face bounding boxes predicted by the CenterFace detector are then used as masks to determine where to apply anonymization filters.
 
 
 ## Credits
 
-- `centerface.onnx` (original) and `centerface.py` (modified) are based on https://github.com/Star-Clouds/centerface (revision [8c39a49](https://github.com/Star-Clouds/CenterFace/tree/8c39a497afb78fb2c064eb84bf010c273bb7d3ce)),
-  [released under MIT license](https://github.com/Star-Clouds/CenterFace/blob/36afed/LICENSE).
-- The original source of the example images in the `examples` directory can be found [here](https://www.pexels.com/de-de/foto/stadt-kreuzung-strasse-menschen-109919/) (released under the [Pexels photo license](https://www.pexels.com/photo-license/)).
+- `centerface.py` is based on https://github.com/Star-Clouds/centerface (revision [8c39a49](https://github.com/Star-Clouds/CenterFace/tree/8c39a497afb78fb2c064eb84bf010c273bb7d3ce)),
+  [released under MIT license](https://github.com/Star-Clouds/CenterFace/blob/36afed/LICENSE)
+- The included model file `centerface.onnx` is an unmodified copy of the [`centerface_bnmerged.onnx`](https://github.com/Star-Clouds/CenterFace/blob/b82ec0c4844e89fd5a0305986aed9bdf33c72585/models/onnx/centerface_bnmerged.onnx) from https://github.com/Star-Clouds/centerface
+- The original source of the example images in the `examples` directory can be found [here](https://www.pexels.com/de-de/foto/stadt-kreuzung-strasse-menschen-109919/) (released under the [Pexels photo license](https://www.pexels.com/photo-license/))
```

### Comparing `deface-1.3.0/deface.egg-info/SOURCES.txt` & `deface-1.4.0/deface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/deface.spec` & `deface-1.4.0/deface.spec`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/examples/city.jpg` & `deface-1.4.0/examples/city.jpg`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/examples/city_anonymized.jpg` & `deface-1.4.0/examples/city_anonymized.jpg`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/examples/city_anonymized_boxes.jpg` & `deface-1.4.0/examples/city_anonymized_boxes.jpg`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/examples/city_anonymized_scores.jpg` & `deface-1.4.0/examples/city_anonymized_scores.jpg`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/examples/city_anonymized_thresh0.02.jpg` & `deface-1.4.0/examples/city_anonymized_thresh0.02.jpg`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/examples/city_anonymized_thresh0.7.jpg` & `deface-1.4.0/examples/city_anonymized_thresh0.7.jpg`

 * *Files identical despite different names*

### Comparing `deface-1.3.0/pyproject.toml` & `deface-1.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     "numpy",
     "tqdm",
     "scikit-image",
     "opencv-python",
 ]
 
 [project.optional-dependencies]
-gpu = ["onnxruntime-gpu"]
+cuda = ["onnx", "onnxruntime-cuda"]
+directml = ["onnx", "onnxruntime-directml"]
+openvino = ["onnx", "onnxruntime-openvino"]
 
 [project.scripts]
 deface = "deface.deface:main"
 
 [tool.setuptools]
 packages = ["deface"]
```

