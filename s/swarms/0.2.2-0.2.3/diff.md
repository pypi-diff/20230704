# Comparing `tmp/swarms-0.2.2.tar.gz` & `tmp/swarms-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.2.2.tar", last modified: Tue Jul  4 01:36:47 2023, max compression
+gzip compressed data, was "swarms-0.2.3.tar", last modified: Tue Jul  4 02:03:47 2023, max compression
```

## Comparing `swarms-0.2.2.tar` & `swarms-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:36:47.971172 swarms-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 01:36:31.000000 swarms-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 01:36:47.971172 swarms-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-04 01:36:31.000000 swarms-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:36:47.971172 swarms-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-04 01:36:31.000000 swarms-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:36:47.967172 swarms-0.2.2/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 01:36:31.000000 swarms-0.2.2/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:36:47.971172 swarms-0.2.2/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 01:36:31.000000 swarms-0.2.2/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 01:36:31.000000 swarms-0.2.2/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:36:47.971172 swarms-0.2.2/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 01:36:31.000000 swarms-0.2.2/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 01:36:31.000000 swarms-0.2.2/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 01:36:31.000000 swarms-0.2.2/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 01:36:31.000000 swarms-0.2.2/swarms/agents/workers/metaprompt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    79059 2023-07-04 01:36:31.000000 swarms-0.2.2/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 01:36:31.000000 swarms-0.2.2/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:36:47.967172 swarms-0.2.2/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 01:36:47.000000 swarms-0.2.2/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 01:36:47.000000 swarms-0.2.2/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:36:47.000000 swarms-0.2.2/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-04 01:36:47.000000 swarms-0.2.2/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 01:36:47.000000 swarms-0.2.2/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:47.626384 swarms-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 02:03:35.000000 swarms-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 02:03:47.626384 swarms-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-04 02:03:35.000000 swarms-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 02:03:47.626384 swarms-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-04 02:03:35.000000 swarms-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:47.622384 swarms-0.2.3/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:47.626384 swarms-0.2.3/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:47.626384 swarms-0.2.3/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/metaprompt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79319 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:47.622384 swarms-0.2.3/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 02:03:47.000000 swarms-0.2.3/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 02:03:47.000000 swarms-0.2.3/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 02:03:47.000000 swarms-0.2.3/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 02:03:47.000000 swarms-0.2.3/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 02:03:47.000000 swarms-0.2.3/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.2.2/LICENSE` & `swarms-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.2.2/PKG-INFO` & `swarms-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.2.2
+Version: 0.2.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.2.2/README.md` & `swarms-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.2.2/setup.py` & `swarms-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.2.2',
+  version = '0.2.3',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
@@ -49,15 +49,15 @@
         "safetensors",
         "streamlit",
         "test-tube",
         "timm",
         "torchmetrics",
         "webdataset",
         "yapf",
-        'GroundingDINO'
+        # 'GroundingDINO'
         "wolframalpha",
         "wikipedia",
         "httpx",
         "ggl",
         "gradio_tools",
         "arxiv",
         "google-api-python-client",
```

### Comparing `swarms-0.2.2/swarms/agents/swarms.py` & `swarms-0.2.3/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.2/swarms/agents/workers/agents.py` & `swarms-0.2.3/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.2/swarms/agents/workers/auto_agent.py` & `swarms-0.2.3/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.2/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.2.3/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.2/swarms/agents/workers/multi_modal.py` & `swarms-0.2.3/swarms/agents/workers/multi_modal.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 
 from langchain.agents.initialize import initialize_agent
 from langchain.agents.tools import Tool
 from langchain.chains.conversation.memory import ConversationBufferMemory
 from langchain.llms.openai import OpenAI
 
 # Grounding DINO
-import groundingdino.datasets.transforms as T
-from groundingdino.models import build_model
-from groundingdino.util import box_ops
-from groundingdino.util.slconfig import SLConfig
-from groundingdino.util.utils import clean_state_dict, get_phrases_from_posmap
+# import groundingdino.datasets.transforms as T
+# from groundingdino.models import build_model
+# from groundingdino.util import box_ops
+# from groundingdino.util.slconfig import SLConfig
+# from groundingdino.util.utils import clean_state_dict, get_phrases_from_posmap
 
-# segment anything
+# segment anything #
 from segment_anything import build_sam, SamPredictor, SamAutomaticMaskGenerator
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 import wget
 
 VISUAL_CHATGPT_PREFIX = """Visual ChatGPT is designed to be able to assist with a wide range of text and visual related tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. Visual ChatGPT is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
@@ -1019,157 +1019,157 @@
         plt.axis('off')
         plt.savefig(
             updated_image_path, 
             bbox_inches="tight", dpi=300, pad_inches=0.0
         )
         return updated_image_path
     
-class Text2Box:
-    def __init__(self, device):
-        print(f"Initializing ObjectDetection to {device}")
-        self.device = device
-        self.torch_dtype = torch.float16 if 'cuda' in device else torch.float32
-        self.model_checkpoint_path = os.path.join("checkpoints","groundingdino")
-        self.model_config_path = os.path.join("checkpoints","grounding_config.py")
-        self.download_parameters()
-        self.box_threshold = 0.3
-        self.text_threshold = 0.25
-        self.grounding = (self.load_model()).to(self.device)
-
-    def download_parameters(self):
-        url = "https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth"
-        if not os.path.exists(self.model_checkpoint_path):
-            wget.download(url,out=self.model_checkpoint_path)
-        config_url = "https://raw.githubusercontent.com/IDEA-Research/GroundingDINO/main/groundingdino/config/GroundingDINO_SwinT_OGC.py"
-        if not os.path.exists(self.model_config_path):
-            wget.download(config_url,out=self.model_config_path)
-    def load_image(self,image_path):
-         # load image
-        image_pil = Image.open(image_path).convert("RGB")  # load image
-
-        transform = T.Compose(
-            [
-                T.RandomResize([512], max_size=1333),
-                T.ToTensor(),
-                T.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225]),
-            ]
-        )
-        image, _ = transform(image_pil, None)  # 3, h, w
-        return image_pil, image
+# class Text2Box:
+#     def __init__(self, device):
+#         print(f"Initializing ObjectDetection to {device}")
+#         self.device = device
+#         self.torch_dtype = torch.float16 if 'cuda' in device else torch.float32
+#         self.model_checkpoint_path = os.path.join("checkpoints","groundingdino")
+#         self.model_config_path = os.path.join("checkpoints","grounding_config.py")
+#         self.download_parameters()
+#         self.box_threshold = 0.3
+#         self.text_threshold = 0.25
+#         self.grounding = (self.load_model()).to(self.device)
+
+#     def download_parameters(self):
+#         url = "https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth"
+#         if not os.path.exists(self.model_checkpoint_path):
+#             wget.download(url,out=self.model_checkpoint_path)
+#         config_url = "https://raw.githubusercontent.com/IDEA-Research/GroundingDINO/main/groundingdino/config/GroundingDINO_SwinT_OGC.py"
+#         if not os.path.exists(self.model_config_path):
+#             wget.download(config_url,out=self.model_config_path)
+#     def load_image(self,image_path):
+#          # load image
+#         image_pil = Image.open(image_path).convert("RGB")  # load image
+
+#         transform = T.Compose(
+#             [
+#                 T.RandomResize([512], max_size=1333),
+#                 T.ToTensor(),
+#                 T.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225]),
+#             ]
+#         )
+#         image, _ = transform(image_pil, None)  # 3, h, w
+#         return image_pil, image
+
+#     def load_model(self):
+#         args = SLConfig.fromfile(self.model_config_path)
+#         args.device = self.device
+#         model = build_model(args)
+#         checkpoint = torch.load(self.model_checkpoint_path, map_location="cpu")
+#         load_res = model.load_state_dict(clean_state_dict(checkpoint["model"]), strict=False)
+#         print(load_res)
+#         _ = model.eval()
+#         return model
+
+#     def get_grounding_boxes(self, image, caption, with_logits=True):
+#         caption = caption.lower()
+#         caption = caption.strip()
+#         if not caption.endswith("."):
+#             caption = caption + "."
+#         image = image.to(self.device)
+#         with torch.no_grad():
+#             outputs = self.grounding(image[None], captions=[caption])
+#         logits = outputs["pred_logits"].cpu().sigmoid()[0]  # (nq, 256)
+#         boxes = outputs["pred_boxes"].cpu()[0]  # (nq, 4)
+#         logits.shape[0]
+
+#         # filter output
+#         logits_filt = logits.clone()
+#         boxes_filt = boxes.clone()
+#         filt_mask = logits_filt.max(dim=1)[0] > self.box_threshold
+#         logits_filt = logits_filt[filt_mask]  # num_filt, 256
+#         boxes_filt = boxes_filt[filt_mask]  # num_filt, 4
+#         logits_filt.shape[0]
+
+#         # get phrase
+#         tokenlizer = self.grounding.tokenizer
+#         tokenized = tokenlizer(caption)
+#         # build pred
+#         pred_phrases = []
+#         for logit, box in zip(logits_filt, boxes_filt):
+#             pred_phrase = get_phrases_from_posmap(logit > self.text_threshold, tokenized, tokenlizer)
+#             if with_logits:
+#                 pred_phrases.append(pred_phrase + f"({str(logit.max().item())[:4]})")
+#             else:
+#                 pred_phrases.append(pred_phrase)
 
-    def load_model(self):
-        args = SLConfig.fromfile(self.model_config_path)
-        args.device = self.device
-        model = build_model(args)
-        checkpoint = torch.load(self.model_checkpoint_path, map_location="cpu")
-        load_res = model.load_state_dict(clean_state_dict(checkpoint["model"]), strict=False)
-        print(load_res)
-        _ = model.eval()
-        return model
-
-    def get_grounding_boxes(self, image, caption, with_logits=True):
-        caption = caption.lower()
-        caption = caption.strip()
-        if not caption.endswith("."):
-            caption = caption + "."
-        image = image.to(self.device)
-        with torch.no_grad():
-            outputs = self.grounding(image[None], captions=[caption])
-        logits = outputs["pred_logits"].cpu().sigmoid()[0]  # (nq, 256)
-        boxes = outputs["pred_boxes"].cpu()[0]  # (nq, 4)
-        logits.shape[0]
-
-        # filter output
-        logits_filt = logits.clone()
-        boxes_filt = boxes.clone()
-        filt_mask = logits_filt.max(dim=1)[0] > self.box_threshold
-        logits_filt = logits_filt[filt_mask]  # num_filt, 256
-        boxes_filt = boxes_filt[filt_mask]  # num_filt, 4
-        logits_filt.shape[0]
-
-        # get phrase
-        tokenlizer = self.grounding.tokenizer
-        tokenized = tokenlizer(caption)
-        # build pred
-        pred_phrases = []
-        for logit, box in zip(logits_filt, boxes_filt):
-            pred_phrase = get_phrases_from_posmap(logit > self.text_threshold, tokenized, tokenlizer)
-            if with_logits:
-                pred_phrases.append(pred_phrase + f"({str(logit.max().item())[:4]})")
-            else:
-                pred_phrases.append(pred_phrase)
-
-        return boxes_filt, pred_phrases
+#         return boxes_filt, pred_phrases
     
-    def plot_boxes_to_image(self, image_pil, tgt):
-        H, W = tgt["size"]
-        boxes = tgt["boxes"]
-        labels = tgt["labels"]
-        assert len(boxes) == len(labels), "boxes and labels must have same length"
-
-        draw = ImageDraw.Draw(image_pil)
-        mask = Image.new("L", image_pil.size, 0)
-        mask_draw = ImageDraw.Draw(mask)
-
-        # draw boxes and masks
-        for box, label in zip(boxes, labels):
-            # from 0..1 to 0..W, 0..H
-            box = box * torch.Tensor([W, H, W, H])
-            # from xywh to xyxy
-            box[:2] -= box[2:] / 2
-            box[2:] += box[:2]
-            # random color
-            color = tuple(np.random.randint(0, 255, size=3).tolist())
-            # draw
-            x0, y0, x1, y1 = box
-            x0, y0, x1, y1 = int(x0), int(y0), int(x1), int(y1)
-
-            draw.rectangle([x0, y0, x1, y1], outline=color, width=6)
-            # draw.text((x0, y0), str(label), fill=color)
-
-            font = ImageFont.load_default()
-            if hasattr(font, "getbbox"):
-                bbox = draw.textbbox((x0, y0), str(label), font)
-            else:
-                w, h = draw.textsize(str(label), font)
-                bbox = (x0, y0, w + x0, y0 + h)
-            # bbox = draw.textbbox((x0, y0), str(label))
-            draw.rectangle(bbox, fill=color)
-            draw.text((x0, y0), str(label), fill="white")
+#     def plot_boxes_to_image(self, image_pil, tgt):
+#         H, W = tgt["size"]
+#         boxes = tgt["boxes"]
+#         labels = tgt["labels"]
+#         assert len(boxes) == len(labels), "boxes and labels must have same length"
+
+#         draw = ImageDraw.Draw(image_pil)
+#         mask = Image.new("L", image_pil.size, 0)
+#         mask_draw = ImageDraw.Draw(mask)
+
+#         # draw boxes and masks
+#         for box, label in zip(boxes, labels):
+#             # from 0..1 to 0..W, 0..H
+#             box = box * torch.Tensor([W, H, W, H])
+#             # from xywh to xyxy
+#             box[:2] -= box[2:] / 2
+#             box[2:] += box[:2]
+#             # random color
+#             color = tuple(np.random.randint(0, 255, size=3).tolist())
+#             # draw
+#             x0, y0, x1, y1 = box
+#             x0, y0, x1, y1 = int(x0), int(y0), int(x1), int(y1)
+
+#             draw.rectangle([x0, y0, x1, y1], outline=color, width=6)
+#             # draw.text((x0, y0), str(label), fill=color)
+
+#             font = ImageFont.load_default()
+#             if hasattr(font, "getbbox"):
+#                 bbox = draw.textbbox((x0, y0), str(label), font)
+#             else:
+#                 w, h = draw.textsize(str(label), font)
+#                 bbox = (x0, y0, w + x0, y0 + h)
+#             # bbox = draw.textbbox((x0, y0), str(label))
+#             draw.rectangle(bbox, fill=color)
+#             draw.text((x0, y0), str(label), fill="white")
 
-            mask_draw.rectangle([x0, y0, x1, y1], fill=255, width=2)
+#             mask_draw.rectangle([x0, y0, x1, y1], fill=255, width=2)
 
-        return image_pil, mask
+#         return image_pil, mask
     
-    @prompts(name="Detect the Give Object",
-             description="useful when you only want to detect or find out given objects in the picture"  
-                         "The input to this tool should be a comma separated string of two, "
-                         "representing the image_path, the text description of the object to be found")
-    def inference(self, inputs):
-        image_path, det_prompt = inputs.split(",")
-        print(f"image_path={image_path}, text_prompt={det_prompt}")
-        image_pil, image = self.load_image(image_path)
-
-        boxes_filt, pred_phrases = self.get_grounding_boxes(image, det_prompt)
-
-        size = image_pil.size
-        pred_dict = {
-        "boxes": boxes_filt,
-        "size": [size[1], size[0]],  # H,W
-        "labels": pred_phrases,}
-
-        image_with_box = self.plot_boxes_to_image(image_pil, pred_dict)[0]
-
-        updated_image_path = get_new_image_name(image_path, func_name="detect-something")
-        updated_image = image_with_box.resize(size)
-        updated_image.save(updated_image_path)
-        print(
-            f"\nProcessed ObejectDetecting, Input Image: {image_path}, Object to be Detect {det_prompt}, "
-            f"Output Image: {updated_image_path}")
-        return updated_image_path
+#     @prompts(name="Detect the Give Object",
+#              description="useful when you only want to detect or find out given objects in the picture"  
+#                          "The input to this tool should be a comma separated string of two, "
+#                          "representing the image_path, the text description of the object to be found")
+#     def inference(self, inputs):
+#         image_path, det_prompt = inputs.split(",")
+#         print(f"image_path={image_path}, text_prompt={det_prompt}")
+#         image_pil, image = self.load_image(image_path)
+
+#         boxes_filt, pred_phrases = self.get_grounding_boxes(image, det_prompt)
+
+#         size = image_pil.size
+#         pred_dict = {
+#         "boxes": boxes_filt,
+#         "size": [size[1], size[0]],  # H,W
+#         "labels": pred_phrases,}
+
+#         image_with_box = self.plot_boxes_to_image(image_pil, pred_dict)[0]
+
+#         updated_image_path = get_new_image_name(image_path, func_name="detect-something")
+#         updated_image = image_with_box.resize(size)
+#         updated_image.save(updated_image_path)
+#         print(
+#             f"\nProcessed ObejectDetecting, Input Image: {image_path}, Object to be Detect {det_prompt}, "
+#             f"Output Image: {updated_image_path}")
+#         return updated_image_path
 
 
 class Inpainting:
     def __init__(self, device):
         self.device = device
         self.revision = 'fp16' if 'cuda' in self.device else None
         self.torch_dtype = torch.float16 if 'cuda' in self.device else torch.float32
```

### Comparing `swarms-0.2.2/swarms/agents/workers/omni_agent.py` & `swarms-0.2.3/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.2/swarms.egg-info/PKG-INFO` & `swarms-0.2.3/swarms.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.2.2
+Version: 0.2.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.2.2/swarms.egg-info/requires.txt` & `swarms-0.2.3/swarms.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 safetensors
 streamlit
 test-tube
 timm
 torchmetrics
 webdataset
 yapf
-GroundingDINOwolframalpha
+wolframalpha
 wikipedia
 httpx
 ggl
 gradio_tools
 arxiv
 google-api-python-client
 google-auth-oauthlib
```

