# Comparing `tmp/sdqrcode-0.3.8.tar.gz` & `tmp/sdqrcode-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.3.8.tar", max compression
+gzip compressed data, was "sdqrcode-0.3.9.tar", max compression
```

## Comparing `sdqrcode-0.3.8.tar` & `sdqrcode-0.3.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-07-03 16:24:12.660349 sdqrcode-0.3.8/LICENSE
--rw-r--r--   0        0        0    10777 2023-07-03 16:24:12.660349 sdqrcode-0.3.8/README.md
--rw-r--r--   0        0        0      659 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     3458 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/Engines/AutoEngine.py
--rw-r--r--   0        0        0     8787 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/Engines/DiffusersEngine.py
--rw-r--r--   0        0        0      186 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/Engines/Engine.py
--rw-r--r--   0        0        0      599 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/Engines/engine_util.py
--rw-r--r--   0        0        0       32 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0      719 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/configs/brightness_auto.yaml
--rw-r--r--   0        0        0      610 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/brightness_diffusers.yaml
--rw-r--r--   0        0        0       22 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/custom.yaml
--rw-r--r--   0        0        0      737 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/default.yaml
--rw-r--r--   0        0        0      719 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/default_auto.yaml
--rw-r--r--   0        0        0      777 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/default_diffusers.yaml
--rw-r--r--   0        0        0      624 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/img2img_tile_auto.yaml
--rw-r--r--   0        0        0      644 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/img2img_tile_diffusers.yaml
--rw-r--r--   0        0        0    13545 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 sdqrcode-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-03 19:55:42.480190 sdqrcode-0.3.9/LICENSE
+-rw-r--r--   0        0        0    10777 2023-07-03 19:55:42.480190 sdqrcode-0.3.9/README.md
+-rw-r--r--   0        0        0      659 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3477 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     8814 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      599 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/configs/brightness_auto.yaml
+-rw-r--r--   0        0        0      610 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/configs/brightness_diffusers.yaml
+-rw-r--r--   0        0        0       22 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      752 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      777 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0      624 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/configs/img2img_tile_auto.yaml
+-rw-r--r--   0        0        0      644 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/configs/img2img_tile_diffusers.yaml
+-rw-r--r--   0        0        0    13506 2023-07-03 19:55:42.552190 sdqrcode-0.3.9/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 sdqrcode-0.3.9/PKG-INFO
```

### Comparing `sdqrcode-0.3.8/LICENSE` & `sdqrcode-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.8/README.md` & `sdqrcode-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.8/pyproject.toml` & `sdqrcode-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdqrcode"
-version = "0.3.8"
+version = "0.3.9"
 description = "Generate ai qr codes with stable diffusion and controlnet with standardised methods"
 authors = ["PhilSad <philippe.henri.saade@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `sdqrcode-0.3.8/src/sdqrcode/Engines/AutoEngine.py` & `sdqrcode-0.3.9/src/sdqrcode/Engines/AutoEngine.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         input_image: PIL.Image.Image = None,
         controlnet_input_images: PIL.Image.Image = None,
         return_cn_imgs=False,
     ) -> PIL.Image.Image:
         
         # set the model
         self.api.util_set_model(self.config["global"]["model_name_or_path"])
-        
+        print("model set")
+
         # define controlnet units
         cn_units = []
         for cn_input_img, (name, unit) in zip(
             controlnet_input_images, self.config["controlnet_units"].items()
         ):
             print("unit", unit)
             cn_unit = webuiapi.ControlNetUnit(
```

### Comparing `sdqrcode-0.3.8/src/sdqrcode/Engines/DiffusersEngine.py` & `sdqrcode-0.3.9/src/sdqrcode/Engines/DiffusersEngine.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,17 @@
     def __init__(self, config, torch_dtype):
         super().__init__(config)
 
         self.controlnet_units = []
         for name, unit in self.config["controlnet_units"].items():
             cn_unit = ControlNetModel.from_pretrained(unit["model"], torch_dtype=torch_dtype)
             self.controlnet_units.append(cn_unit)
+        
+        
+        
         if len(self.controlnet_units) == 1:
             self.controlnet_units = self.controlnet_units[0]
             
         if self.config["global"]["mode"] == "txt2img":  
             self.pipeline = StableDiffusionControlNetPipeline.from_pretrained(
                 self.config["global"]["model_name_or_path"],
                 controlnet=self.controlnet_units,
```

### Comparing `sdqrcode-0.3.8/src/sdqrcode/Engines/engine_util.py` & `sdqrcode-0.3.9/src/sdqrcode/Engines/engine_util.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.8/src/sdqrcode/configs/brightness_auto.yaml` & `sdqrcode-0.3.9/src/sdqrcode/configs/brightness_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.8/src/sdqrcode/configs/brightness_diffusers.yaml` & `sdqrcode-0.3.9/src/sdqrcode/configs/brightness_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.8/src/sdqrcode/configs/default.yaml` & `sdqrcode-0.3.9/src/sdqrcode/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.8/src/sdqrcode/configs/default_auto.yaml` & `sdqrcode-0.3.9/src/sdqrcode/configs/img2img_tile_auto.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 global:
-  mode: txt2img
-  prompt: a beautiful dalmatian portrait, front shot
-  negative_prompt: ""
-  model_name_or_path: 6ce0161689
+  mode: img2img
+  input_image: qrcode
+  prompt: "a beautiful minecraft landscape, lights and shadows"
+  negative_prompt: "ugly"
+  model_name_or_path: "6ce0161689"
+  denoising_strength: 0.7
   steps: 20
-  scheduler_name: DPM++ 2M Karras
+  scheduler_name: Euler a
   cfg_scale: 7
   width: 768
   height: 768
   seed: -1
   batch_size: 1
 
 controlnet_units:
-  brightness:
-    model: control_v1p_sd15_brightness [5f6aa6ed]
-    cn_input_image: qrcode
-    module: none
-    weight: 0.35
-    start: 0.0
-    end: 1.0
-
   tile:
     model: control_v11f1e_sd15_tile [a371b31b]
     cn_input_image: qrcode
     module: none
     weight: 0.5
     start: 0.35
     end: 0.70
 
 qrcode:
-  text: https://koll.ai
+  text: "https://koll.ai"
   error_correction: high # [low, medium, quart, high]
   box_size: 10
   border: 4
   fill_color: black
   back_color: white
```

### Comparing `sdqrcode-0.3.8/src/sdqrcode/configs/default_diffusers.yaml` & `sdqrcode-0.3.9/src/sdqrcode/configs/default_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.8/src/sdqrcode/configs/img2img_tile_auto.yaml` & `sdqrcode-0.3.9/src/sdqrcode/configs/img2img_tile_diffusers.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 global:
   mode: img2img
-  input_image: qrcode
   prompt: "a beautiful minecraft landscape, lights and shadows"
   negative_prompt: "ugly"
-  model_name_or_path: "6ce0161689"
-  denoising_strength: 0.7
+  model_name_or_path: "SG161222/Realistic_Vision_V2.0"
   steps: 20
   scheduler_name: Euler a
   cfg_scale: 7
   width: 768
   height: 768
   seed: -1
   batch_size: 1
+  input_image: qrcode
+  denoising_strength: 0.7
 
 controlnet_units:
   tile:
-    model: control_v11f1e_sd15_tile [a371b31b]
+    model: lllyasviel/control_v11f1e_sd15_tile
     cn_input_image: qrcode
     module: none
     weight: 0.5
     start: 0.35
     end: 0.70
 
 qrcode:
```

### Comparing `sdqrcode-0.3.8/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.3.9/src/sdqrcode/sdqrcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import os
 import urllib.request
 from pathlib import Path
 import requests
 from io import BytesIO
 import sdqrcode.Engines.engine_util as engine_util
 from typing import Union
-import torch
+
+try:
+    import torch
+except:
+    pass
 
 CONFIGS = {
     "default_auto":           Path(__file__).parent / "configs" / "default_auto.yaml",
     "default_diffusers":      Path(__file__).parent / "configs" / "default_diffusers.yaml",
     "brightness_auto":        Path(__file__).parent / "configs" / "brightness_auto.yaml",
     "brightness_diffusers":   Path(__file__).parent / "configs" / "brightness_diffusers.yaml",
     "img2img_tile_auto":      Path(__file__).parent / "configs" / "img2img_tile_auto.yaml",
@@ -32,15 +36,15 @@
         self,
         config_name_or_path_or_dict: str,
         auto_api_hostname: str = None,
         auto_api_port: int = None,
         auto_api_https: bool = None,
         auto_api_username: str = None,
         auto_api_password: str = None,
-        torch_dtype: torch.dtype = torch.float32,
+        torch_dtype = None,
     ):
         """
         Args:
             backend: Backend enum, one of auto_api, diffusers
             model: Model name or path to a pretrained model
             config_name_or_path: Pretrained config name or path if not the same as model_name
             auto_api_hostname: Hostname of the Automatic1111 server
@@ -245,15 +249,15 @@
 def init(
     config: str = "default_diffusers",
     auto_api_hostname: str = None,
     auto_api_port: int = None,
     auto_api_https: bool = None,
     auto_api_username: str = None,
     auto_api_password: str = None,
-    torch_dtype: torch.dtype = torch.float32,
+    torch_dtype = None,
     **config_kwargs,
 ):
     """
     config_kwargs:
         model_name_or_path: str = None,
         steps: int = None,
         cfg_scale: float = None,
@@ -293,15 +297,15 @@
 def init_and_generate_sd_qrcode(
     config_name_or_path: str = "default_diffusers",
     auto_api_hostname: str = "",
     auto_api_port: int = 7860,
     auto_api_https: bool = True,
     auto_api_username: str = "",
     auto_api_password: str = "",
-    torch_dtype: torch.dtype = torch.float32,
+    torch_dtype = None,
     **config_kwargs,
 ) -> tuple[PIL.Image.Image, Sdqrcode]:
     # check if variables are set in env
     auto_api_hostname = (
         os.getenv("AUTO_API_HOSTNAME", "")
         if auto_api_hostname == ""
         else auto_api_hostname
```

### Comparing `sdqrcode-0.3.8/PKG-INFO` & `sdqrcode-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.3.8
+Version: 0.3.9
 Summary: Generate ai qr codes with stable diffusion and controlnet with standardised methods
 License: MIT
 Author: PhilSad
 Author-email: philippe.henri.saade@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

