# Comparing `tmp/sunidea-0.0.2.tar.gz` & `tmp/sunidea-0.0.3.tar.gz`

## Comparing `sunidea-0.0.2.tar` & `sunidea-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,13 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 sunidea-0.0.2/notes
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/.pypirc
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/LICENSE.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/README.md
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/__init__.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/pyproject.toml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_config/__init__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_config/sun_idea_config.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_module/__init__.py
--rw-r--r--   0        0        0   417998 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_module/origin_text.xlsx
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_module/task_doc.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_module/task_elasticsearch.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_module/task_multi.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_module/tmp_search
--rw-r--r--   0        0        0   121470 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_module/╓╨╣·│м╓╪_╖╩┼╓╥╜╤з╙к╤°╓╬┴╞╓╕─╧(2021).xlsx
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_module/╓╨╣·│м╓╪_╖╩┼╓╥╜╤з╙к╤°╓╬┴╞╓╕─╧(2021)2.xlsx
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/__init__.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/sun_idea_utils.py
--rw-r--r--   0        0        0    59257 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114646_683355.jpg
--rw-r--r--   0        0        0    58357 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114647_065113.jpg
--rw-r--r--   0        0        0    64107 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114647_230473.jpg
--rw-r--r--   0        0        0    48331 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114647_368826.jpg
--rw-r--r--   0        0        0    24630 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114647_821042.jpg
--rw-r--r--   0        0        0    34950 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114648_084066.jpg
--rw-r--r--   0        0        0    35174 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114648_890310.jpg
--rw-r--r--   0        0        0    58541 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114649_211963.jpg
--rw-r--r--   0        0        0    16563 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114649_566225.jpg
--rw-r--r--   0        0        0    42153 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114649_741567.jpg
--rw-r--r--   0        0        0    59257 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114703_360071.jpg
--rw-r--r--   0        0        0    58357 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114703_495397.jpg
--rw-r--r--   0        0        0    64107 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114703_633832.jpg
--rw-r--r--   0        0        0    48331 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114703_769865.jpg
--rw-r--r--   0        0        0    24630 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114703_879944.jpg
--rw-r--r--   0        0        0    34950 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114704_244859.jpg
--rw-r--r--   0        0        0    35174 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114704_520552.jpg
--rw-r--r--   0        0        0    58541 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114704_869510.jpg
--rw-r--r--   0        0        0    16563 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114705_073117.jpg
--rw-r--r--   0        0        0    42153 2020-02-02 00:00:00.000000 sunidea-0.0.2/SunIdea/sun_utils/cats_xiamu/20230630_114705_254518.jpg
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 sunidea-0.0.2/LICENSE
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 sunidea-0.0.2/README.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 sunidea-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sunidea-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sunidea-0.0.3/.pypirc
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 sunidea-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sunidea-0.0.3/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 sunidea-0.0.3/sun_config/__init__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sunidea-0.0.3/sun_config/sun_idea_config.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 sunidea-0.0.3/sun_module/__init__.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 sunidea-0.0.3/sun_module/multi_task.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sunidea-0.0.3/sun_utils/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sunidea-0.0.3/sun_utils/sun_idea_utils.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 sunidea-0.0.3/LICENSE
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 sunidea-0.0.3/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 sunidea-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 sunidea-0.0.3/PKG-INFO
```

### Comparing `sunidea-0.0.2/SunIdea/LICENSE.txt` & `sunidea-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sunidea-0.0.2/SunIdea/pyproject.toml` & `sunidea-0.0.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 5375 6e49 6465 6122 0d0a 7665 7273   "SunIdea"..vers
-00000070: 696f 6e20 3d20 2230 2e30 2e31 220d 0a61  ion = "0.0.1"..a
+00000070: 696f 6e20 3d20 2230 2e30 2e33 220d 0a61  ion = "0.0.3"..a
 00000080: 7574 686f 7273 203d 205b 0d0a 2020 7b20  uthors = [..  { 
 00000090: 6e61 6d65 3d22 e5ad 99e5 b08f e4ba 9422  name="........."
 000000a0: 2c20 656d 6169 6c3d 2273 756e 7368 7561  , email="sunshua
 000000b0: 6e67 6c6f 6e67 6466 4067 6d61 696c 2e63  nglongdf@gmail.c
 000000c0: 6f6d 227d 2c0d 0a5d 0d0a 6465 7363 7269  om"},..]..descri
 000000d0: 7074 696f 6e20 3d20 2273 756e 5f69 6465  ption = "sun_ide
 000000e0: 6120 6973 2061 2070 6163 6b61 6765 2066  a is a package f
@@ -27,19 +27,13 @@
 000001a0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
 000001b0: 7365 222c 0d0a 2020 2020 224f 7065 7261  se",..    "Opera
 000001c0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
 000001d0: 5320 496e 6465 7065 6e64 656e 7422 2c0d  S Independent",.
 000001e0: 0a5d 0d0a 6465 7065 6e64 656e 6369 6573  .]..dependencies
 000001f0: 203d 205b 0d0a 2020 2020 2020 2020 2274   = [..        "t
 00000200: 7164 6d3e 3d34 2e36 342e 3022 2c0d 0a20  qdm>=4.64.0",.. 
-00000210: 2020 2020 2020 2022 656c 6173 7469 6373         "elastics
-00000220: 6561 7263 683e 3d38 2e38 2e30 222c 0d0a  earch>=8.8.0",..
-00000230: 2020 2020 2020 2020 2274 6f72 6368 6b65          "torchke
-00000240: 7261 733e 3d33 2e38 2e39 222c 0d0a 2020  ras>=3.8.9",..  
-00000250: 2020 2020 2020 2266 616b 655f 7573 6572        "fake_user
-00000260: 6167 656e 743e 3d31 2e31 2e33 220d 0a20  agent>=1.1.3".. 
-00000270: 2020 205d 0d0a 0d0a 5b70 726f 6a65 6374     ]....[project
-00000280: 2e75 726c 735d 0d0a 2248 6f6d 6570 6167  .urls].."Homepag
-00000290: 6522 203d 2022 6874 7470 733a 2f2f 6769  e" = "https://gi
-000002a0: 7468 7562 2e63 6f6d 2f73 756e 7869 616f  thub.com/sunxiao
-000002b0: 7775 3f74 6162 3d70 726f 6a65 6374 7322  wu?tab=projects"
-000002c0: 0d0a                                     ..
+00000210: 2020 205d 0d0a 0d0a 5b70 726f 6a65 6374     ]....[project
+00000220: 2e75 726c 735d 0d0a 2248 6f6d 6570 6167  .urls].."Homepag
+00000230: 6522 203d 2022 6874 7470 733a 2f2f 6769  e" = "https://gi
+00000240: 7468 7562 2e63 6f6d 2f73 756e 7869 616f  thub.com/sunxiao
+00000250: 7775 3f74 6162 3d70 726f 6a65 6374 7322  wu?tab=projects"
+00000260: 0d0a                                     ..
```

### Comparing `sunidea-0.0.2/SunIdea/sun_module/task_multi.py` & `sunidea-0.0.3/sun_module/multi_task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 # -*- coding: utf-8 -*-
 # @Time : 2023/6/14 14:37
 # @Author : sunshuanglong
 # @File : multi_task.py
+from concurrent.futures import ProcessPoolExecutor, wait
 from ..sun_config import sun_idea_config
 from tqdm import tqdm
 import json
-from concurrent.futures import ProcessPoolExecutor, wait
 
-class MngrMulti(object):
+
+class MultiTask(object):
     def __init__(self, process_num=None):
         self.config = sun_idea_config.config_all["multi_task"]
         if process_num is None:
             self.process_num = self.config["process_num"]
         else:
             self.process_num = process_num
         self.__executor = ProcessPoolExecutor(max_workers=self.process_num)
 
-    def multi_task_processing(self, data_list, fun_job):
+    def multi_task_processing(self, data_list, fun_job, **kwargs):
         process_list = list()
         res_list = list()
         data_sub_sum = len(data_list) // self.process_num
         for idx in range(0, len(data_list), data_sub_sum):
             item = data_list[idx: idx + data_sub_sum]
-            process_list.append(self.__executor.submit(fun_job, item))
+            process_list.append(self.__executor.submit(fun_job, item, **kwargs))
         wait(process_list)
         for _ in process_list:
             res_list.extend(_.result())
         return res_list
 
     def load_jsonl(self, file_path):
         data_list = open(file_path, "r", encoding="utf-8").read().strip().split("\n")
-        return self.multi_task_processing(data_list, self.parse_jsonls_to_str_list)
-
-    def close(self):
-        self.__executor.shutdown()
+        data_args = dict()
+        return self.multi_task_processing(data_list, self.parse_jsonls_to_str_list, **data_args)
 
     @staticmethod
-    def parse_jsonls_to_str_list(data_list):
+    def parse_jsonls_to_str_list(data_list, **kwargs):
         res_list = list()
         for item in tqdm(data_list, desc="to_json..."):
             res_list.append(json.loads(item))
         return res_list
 
+    def close(self):
+        self.__executor.shutdown()
+
 
-def fun_job(data_list):
+def fun_job(data_list, **kwargs):
+    a = kwargs
     for item in tqdm(data_list, desc="processing..."):
         for i in range(1000):
             item[f"add_{i}"] = "made by sunxiaowu"
 
     return data_list
 
 
 if __name__ == "__main__":
-    task_obj = MngrMulti(process_num=32)
-    data_list = task_obj.load_jsonl("test.jsonl")
-    res_list = task_obj.multi_task_processing(data_list, fun_job)
+    task_obj = MultiTask(process_num=32)
+    # data_list = task_obj.load_jsonl("test.jsonl")
+    data_list = {"key1": "你好", "key2": "好的"}
+    res_list = task_obj.multi_task_processing(data_list, fun_job, **data_list)
     print(len(res_list))
     print(res_list[0])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sunidea-0.0.2/PKG-INFO` & `sunidea-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunIdea
-Version: 0.0.2
+Version: 0.0.3
 Summary: sun_idea is a package for tools
 Project-URL: Homepage, https://github.com/sunxiaowu?tab=projects
 Author-email: 孙小五 <sunshuanglongdf@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Othneil Drew
         
@@ -29,13 +29,8 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: tqdm>=4.64.0
 Description-Content-Type: text/markdown
 
-description = "sun_idea is a package for multiprocess"
-# 写完自己的模块后 修改pyproject.toml，然后执行以下命令制作包及上传pypi
-# python3 -m build
-# twine upload dist/*
-
-multi_task_processing 添加可变参数传参
+description = "sun_idea is a package for multiprocess"
```

