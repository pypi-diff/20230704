# Comparing `tmp/apidriver-0.7.0.tar.gz` & `tmp/apidriver-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidriver-0.7.0.tar", last modified: Tue Apr  4 01:22:11 2023, max compression
+gzip compressed data, was "apidriver-0.8.0.tar", last modified: Tue Jul  4 01:40:20 2023, max compression
```

## Comparing `apidriver-0.7.0.tar` & `apidriver-0.8.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 01:22:11.233089 apidriver-0.7.0/
--rw-rw-rw-   0        0        0     1088 2023-03-16 03:56:05.000000 apidriver-0.7.0/LICENSE.txt
--rw-rw-rw-   0        0        0       87 2023-03-16 03:56:05.000000 apidriver-0.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0      249 2023-04-04 01:22:11.233089 apidriver-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3453 2023-03-17 08:46:28.000000 apidriver-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 01:22:11.154980 apidriver-0.7.0/api_driver/
--rw-rw-rw-   0        0        0       66 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/__init__.py
--rw-rw-rw-   0        0        0      127 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/__main__.py
--rw-rw-rw-   0        0        0      131 2023-04-04 01:21:25.000000 apidriver-0.7.0/api_driver/_version.py
--rw-rw-rw-   0        0        0     2812 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/ad_utils.py
--rw-rw-rw-   0        0        0     3073 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/command.py
--rw-rw-rw-   0        0        0    15136 2023-03-23 01:23:50.000000 apidriver-0.7.0/api_driver/har_parser.py
--rw-rw-rw-   0        0        0     2278 2023-03-22 09:36:36.000000 apidriver-0.7.0/api_driver/loader_swagger.py
--rw-rw-rw-   0        0        0     4587 2023-03-23 01:23:50.000000 apidriver-0.7.0/api_driver/project_generator.py
--rw-rw-rw-   0        0        0     8018 2023-03-30 11:20:25.000000 apidriver-0.7.0/api_driver/swagger_generate.py
--rw-rw-rw-   0        0        0      503 2023-03-23 01:23:50.000000 apidriver-0.7.0/api_driver/template.py
-drwxrwxrwx   0        0        0        0 2023-04-04 01:22:11.186224 apidriver-0.7.0/api_driver/templates/
--rw-rw-rw-   0        0        0     2179 2023-03-22 06:14:06.000000 apidriver-0.7.0/api_driver/templates/api.tpl
--rw-rw-rw-   0        0        0      389 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/templates/api_demo.tpl
--rw-rw-rw-   0        0        0      413 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/templates/base_testcase.tpl
--rw-rw-rw-   0        0        0     2962 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/templates/har2api_case.tpl
--rw-rw-rw-   0        0        0     2308 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/templates/har2case.tpl
--rw-rw-rw-   0        0        0     5338 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/templates/http.tpl
--rw-rw-rw-   0        0        0      367 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/templates/testcase_demo.tpl
--rw-rw-rw-   0        0        0     2933 2023-03-23 01:28:38.000000 apidriver-0.7.0/api_driver/testcase_mixin.py
-drwxrwxrwx   0        0        0        0 2023-04-04 01:22:11.217498 apidriver-0.7.0/api_driver/utils/
--rw-rw-rw-   0        0        0        0 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/utils/__init__.py
--rw-rw-rw-   0        0        0     1076 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/utils/custom_str_utils.py
--rw-rw-rw-   0        0        0     1945 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/utils/database_conn.py
--rw-rw-rw-   0        0        0     3448 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/utils/fake.py
--rw-rw-rw-   0        0        0     2226 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/utils/placeholder.py
--rw-rw-rw-   0        0        0     1326 2023-03-16 03:56:05.000000 apidriver-0.7.0/api_driver/utils/service_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-04 01:22:11.233089 apidriver-0.7.0/apidriver.egg-info/
--rw-rw-rw-   0        0        0      249 2023-04-04 01:22:10.000000 apidriver-0.7.0/apidriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1012 2023-04-04 01:22:11.000000 apidriver-0.7.0/apidriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 01:22:10.000000 apidriver-0.7.0/apidriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-04 01:22:10.000000 apidriver-0.7.0/apidriver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      171 2023-04-04 01:22:10.000000 apidriver-0.7.0/apidriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-04 01:22:10.000000 apidriver-0.7.0/apidriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      180 2023-03-17 08:44:35.000000 apidriver-0.7.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 01:22:11.233089 apidriver-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-03-17 07:12:37.000000 apidriver-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 01:22:11.233089 apidriver-0.7.0/test/
--rw-rw-rw-   0        0        0     1154 2023-03-31 09:28:07.000000 apidriver-0.7.0/test/test_cli.py
--rw-rw-rw-   0        0        0      148 2023-03-31 09:20:56.000000 apidriver-0.7.0/test/test_main.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.070278 apidriver-0.8.0/
+-rw-r--r--   0 chnjx      (501) staff       (20)     1068 2023-02-07 12:22:16.000000 apidriver-0.8.0/LICENSE.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       84 2023-03-15 15:32:00.000000 apidriver-0.8.0/MANIFEST.in
+-rw-r--r--   0 chnjx      (501) staff       (20)      239 2023-07-04 01:40:20.069604 apidriver-0.8.0/PKG-INFO
+-rw-r--r--   0 chnjx      (501) staff       (20)     3340 2023-04-13 12:44:49.000000 apidriver-0.8.0/README.md
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.057227 apidriver-0.8.0/api_driver/
+-rw-r--r--   0 chnjx      (501) staff       (20)       64 2023-03-14 14:16:04.000000 apidriver-0.8.0/api_driver/__init__.py
+-rw-r--r--   0 chnjx      (501) staff       (20)      120 2023-03-15 15:01:02.000000 apidriver-0.8.0/api_driver/__main__.py
+-rw-r--r--   0 chnjx      (501) staff       (20)      127 2023-07-04 01:38:12.000000 apidriver-0.8.0/api_driver/_version.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2712 2023-07-04 01:36:23.000000 apidriver-0.8.0/api_driver/ad_utils.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2971 2023-03-15 15:08:27.000000 apidriver-0.8.0/api_driver/command.py
+-rw-r--r--   0 chnjx      (501) staff       (20)    14714 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/har_parser.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2278 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/loader_swagger.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     4417 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/project_generator.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     8018 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/swagger_generate.py
+-rw-r--r--   0 chnjx      (501) staff       (20)      485 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/template.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.060954 apidriver-0.8.0/api_driver/templates/
+-rw-r--r--   0 chnjx      (501) staff       (20)     2121 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/templates/api.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)      374 2023-03-15 15:46:44.000000 apidriver-0.8.0/api_driver/templates/api_demo.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)      398 2023-03-15 15:08:27.000000 apidriver-0.8.0/api_driver/templates/base_testcase.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     2879 2023-03-15 15:12:01.000000 apidriver-0.8.0/api_driver/templates/har2api_case.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     2242 2023-03-15 15:12:01.000000 apidriver-0.8.0/api_driver/templates/har2case.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     5224 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/templates/http.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)      355 2023-03-15 13:14:27.000000 apidriver-0.8.0/api_driver/templates/testcase_demo.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     2933 2023-04-13 12:44:49.000000 apidriver-0.8.0/api_driver/testcase_mixin.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.064374 apidriver-0.8.0/api_driver/utils/
+-rw-r--r--   0 chnjx      (501) staff       (20)        0 2023-02-07 12:22:16.000000 apidriver-0.8.0/api_driver/utils/__init__.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     1043 2023-03-15 15:08:27.000000 apidriver-0.8.0/api_driver/utils/custom_str_utils.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     1882 2023-03-14 13:52:12.000000 apidriver-0.8.0/api_driver/utils/database_conn.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     3322 2023-03-14 13:52:12.000000 apidriver-0.8.0/api_driver/utils/fake.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2172 2023-03-15 15:08:27.000000 apidriver-0.8.0/api_driver/utils/placeholder.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     1283 2023-02-17 12:48:23.000000 apidriver-0.8.0/api_driver/utils/service_logger.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.068155 apidriver-0.8.0/apidriver.egg-info/
+-rw-r--r--   0 chnjx      (501) staff       (20)      239 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/PKG-INFO
+-rw-r--r--   0 chnjx      (501) staff       (20)      994 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/SOURCES.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)        1 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/dependency_links.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       40 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/entry_points.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)      171 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/requires.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       11 2023-07-04 01:40:20.000000 apidriver-0.8.0/apidriver.egg-info/top_level.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)      170 2023-04-13 12:44:49.000000 apidriver-0.8.0/requirements.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       38 2023-07-04 01:40:20.070571 apidriver-0.8.0/setup.cfg
+-rw-r--r--   0 chnjx      (501) staff       (20)      903 2023-04-13 12:44:49.000000 apidriver-0.8.0/setup.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-04 01:40:20.068739 apidriver-0.8.0/test/
+-rw-r--r--   0 chnjx      (501) staff       (20)     1105 2023-04-13 12:44:49.000000 apidriver-0.8.0/test/test_cli.py
```

### Comparing `apidriver-0.7.0/LICENSE.txt` & `apidriver-0.8.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `apidriver-0.7.0/README.md` & `apidriver-0.8.0/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-# api-driver
-### 项目介绍
-  - api-driver是一个的接口测试框架，项目架构采取了api-object设计模式，将用例和接口定义进行分离
-  - 设计初衷：
-      1. 统一的项目架构可以更好地支持团队协作以及日后的维护
-      2. 提供便捷的功能让用例编写更加简单和高效
-  - 目前实现：
-      1. 一建生成接口测试项目
-      2. swagger接口文档
-      3. har生成测试用例
-      4. 快速运行并集成测试报告
-      
-### 安装
-  ```shell
-  pip install apidriver
-  ```
-
-### 使用
-安装完成后会得到一个命令行工具：adf
-具体使用方法：
-```
-# 获取帮助
-adf --help:
-Usage: adf [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  har2case       将har转换成用例
-  run            运行用例并集成allure报告
-  start_project  创建项目
-  swagger2api    swagger文档转换成api-object
-
-
-# 生成接口测试项目
-Usage: adf start_project [OPTIONS]
-
-  创建项目 :param project_name: 项目名称
-
-Options:
-  -n, --project-name TEXT  project name  [required]
-  --help                   Show this message and exit.
-  
-示例：
-adf start_project -n "project_name"
-会在当前目录下生成一个项目：
-project_name:.
-├───api_object
-├───har
-├───swagger
-└───testcase
-
-# swagger 生成 api-object
-Usage: adf swagger2api [OPTIONS]
-
-  swagger文档转换成api-object :param swagger_doc: swagger.json 文件 :param api_dir:
-  api存放路径 非必填
-
-Options:
-  -s, --swagger-doc TEXT  Swagger doc file.  [required]
-  -d, --api-dir TEXT      api save dir.
-  --help                  Show this message and exit.
-
-示例：
-adf swagger2api -s swagger.json
-会在api-object路径下生成对应的api模块
-
-# har转测试用例
-Usage: adf har2case [OPTIONS]
-
-  将har转换成用例 :param har: har文件路径 :param api: har对应api-object文件 :param testcase:
-  用例路径 :param exclude:  过来的url :return:
-
-Options:
-  -h, --har TEXT       har file path  [required]
-  -a, --api TEXT       api object dir
-  -t, --testcase TEXT  testcase dir
-  -e, --exclude TEXT   exclude url
-  --help               Show this message and exit.
-
-示例
-adf har2case -h har_file_dir -e "png|js|css"
-会将har转成测试用例放在testcase目录下 并将 png/js/css结尾的路径给剔除
-adf har2case -h har_file_dir -a api_object
-api_object目录下查找是否存在har对应api类并生成api-object模式的测试用例
-```
-api使用
-```python
-# 占位符替换
-# 占位符使用${random(num)} 或 ${random(num1,num2)} 前面是生成字符串，后面的是生成范围内的数字
-from api_driver.testcase_mixin import TestcaseMixin
-# 替换字典中的占位符
-TestcaseMixin().replace_formal_dict_2_actual(data_dict)
-# 替换列表中的占位符
-TestcaseMixin().replace_formal_list_2_actual(data_list)
-# 替换字符串的占位符
-TestcaseMixin().replace_formal_str_2_actual(data)
-
-# 进行json_schema的校验
-TestcaseMixin().assert_schema(res,schema_file_dir,schema_file)
-
-# 假数据生成
-from api_driver.utils.fake import Fake
-Fake # 提供了丰富的假数据生成方法 
-```
-
-### 后续优化
-1. 往基于模型测试的设计模式方向优化
-2. 实现swagger导入生成基本测试用例
-3. 提供更丰富的api
-4. 集成mock功能
-
+# api-driver
+### 项目介绍
+  - api-driver是一个的接口测试框架，项目架构采取了api-object设计模式，将用例和接口定义进行分离
+  - 设计初衷：
+      1. 统一的项目架构可以更好地支持团队协作以及日后的维护
+      2. 提供便捷的功能让用例编写更加简单和高效
+  - 目前实现：
+      1. 一建生成接口测试项目
+      2. swagger接口文档
+      3. har生成测试用例
+      4. 快速运行并集成测试报告
+      
+### 安装
+  ```shell
+  pip install apidriver
+  ```
+
+### 使用
+安装完成后会得到一个命令行工具：adf
+具体使用方法：
+```
+# 获取帮助
+adf --help:
+Usage: adf [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  har2case       将har转换成用例
+  run            运行用例并集成allure报告
+  start_project  创建项目
+  swagger2api    swagger文档转换成api-object
+
+
+# 生成接口测试项目
+Usage: adf start_project [OPTIONS]
+
+  创建项目 :param project_name: 项目名称
+
+Options:
+  -n, --project-name TEXT  project name  [required]
+  --help                   Show this message and exit.
+  
+示例：
+adf start_project -n "project_name"
+会在当前目录下生成一个项目：
+project_name:.
+├───api_object
+├───har
+├───swagger
+└───testcase
+
+# swagger 生成 api-object
+Usage: adf swagger2api [OPTIONS]
+
+  swagger文档转换成api-object :param swagger_doc: swagger.json 文件 :param api_dir:
+  api存放路径 非必填
+
+Options:
+  -s, --swagger-doc TEXT  Swagger doc file.  [required]
+  -d, --api-dir TEXT      api save dir.
+  --help                  Show this message and exit.
+
+示例：
+adf swagger2api -s swagger.json
+会在api-object路径下生成对应的api模块
+
+# har转测试用例
+Usage: adf har2case [OPTIONS]
+
+  将har转换成用例 :param har: har文件路径 :param api: har对应api-object文件 :param testcase:
+  用例路径 :param exclude:  过来的url :return:
+
+Options:
+  -h, --har TEXT       har file path  [required]
+  -a, --api TEXT       api object dir
+  -t, --testcase TEXT  testcase dir
+  -e, --exclude TEXT   exclude url
+  --help               Show this message and exit.
+
+示例
+adf har2case -h har_file_dir -e "png|js|css"
+会将har转成测试用例放在testcase目录下 并将 png/js/css结尾的路径给剔除
+adf har2case -h har_file_dir -a api_object
+api_object目录下查找是否存在har对应api类并生成api-object模式的测试用例
+```
+api使用
+```python
+# 占位符替换
+# 占位符使用${random(num)} 或 ${random(num1,num2)} 前面是生成字符串，后面的是生成范围内的数字
+from api_driver.testcase_mixin import TestcaseMixin
+# 替换字典中的占位符
+TestcaseMixin().replace_formal_dict_2_actual(data_dict)
+# 替换列表中的占位符
+TestcaseMixin().replace_formal_list_2_actual(data_list)
+# 替换字符串的占位符
+TestcaseMixin().replace_formal_str_2_actual(data)
+
+# 进行json_schema的校验
+TestcaseMixin().assert_schema(res,schema_file_dir,schema_file)
+
+# 假数据生成
+from api_driver.utils.fake import Fake
+Fake # 提供了丰富的假数据生成方法 
+```
+
+### 后续优化
+1. 往基于模型测试的设计模式方向优化
+2. 实现swagger导入生成基本测试用例
+3. 提供更丰富的api
+4. 集成mock功能
+
```

### Comparing `apidriver-0.7.0/api_driver/ad_utils.py` & `apidriver-0.8.0/api_driver/ad_utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-# -*- coding:utf-8 -*-
-# @Time     :2023/3/1 11:08
-# @Author   :CHNJX
-# @File     :ad_utils.py
-# @Desc     :public utils
-import ast
-from os import makedirs
-import os
-from urllib.parse import unquote
-import re
-
-
-def covert_list_to_dict(list_data):
-    """
-    将har list data 转换成dict
-    :param list_data
-        list_data (list)
-            [
-                {"name": "v", "value": "1"},
-                {"name": "w", "value": "2"}
-            ]
-
-    :return:
-        dict:
-            {"v": "1", "w": "2"}
-    """
-    return {item['name']: item.get('value') for item in list_data}
-
-
-def convert_x_www_form_to_dict(form_data: str):
-    """
-    将form表单数据装换成dict字典数据
-    :param form_data:  (str): a=1&b=2
-    :return: (dict) {"a":1, "b":2}
-    """
-    if isinstance(form_data, str):
-        res_dict = {}
-        for kev_value in form_data.split('&'):
-            try:
-                key, value = kev_value.split('=')
-            except ValueError:
-                raise Exception(f"错误的 x_www_form_urlencoded 数据: {form_data}")
-            # unquote('abc%20def') -> 'abc def'.
-            res_dict[key] = unquote(value)
-        return res_dict
-    else:
-        return form_data
-
-
-def get_class_and_func(api_file, url, method) -> tuple:
-    """
-    获取到类名和方法名
-    :param api_file: 对应api文件
-    :param url:     对应请求url
-    :param method:  请求方式
-    :return:
-    """
-    api_class = ''
-    func_name = ''
-    with open(api_file, 'r', encoding='utf-8') as f:
-        cd = ast.parse(f.read())
-        for item in cd.body:
-            if isinstance(item, ast.ClassDef) and item.body:
-                for func in item.body:
-                    if isinstance(func, ast.FunctionDef):
-                        func_str = ast.dump(func)
-                        if url in func_str and method.lower() in func_str:
-                            pattern = "name='(.*?)'"
-                            api_class = re.search(pattern, ast.dump(item)).group(1)
-                            func_name = re.search(pattern, ast.dump(func)).group(1)
-                            break
-    return api_class, func_name
-
-
-def write(content, file_path):
-    """
-    将内容写入文档中
-    :param content:  要写入的内容
-    :param file_path: 文件路径（不存在则会进行创建）
-    :return: None
-    """
-    dir_ = os.path.dirname(file_path)
-    if not os.path.exists(dir_):
-        os.makedirs(dir_)
-    with open(file_path, 'w', encoding='utf-8') as f:
-        f.write(content)
-
-
-def create_folder(path):
-    """
-    创建目录
-    :param path: 目录路径
-    :return: None
-    """
-    makedirs(path)
-    print(f'create folder {path}')
-
-
-
-
+# -*- coding:utf-8 -*-
+# @Time     :2023/3/1 11:08
+# @Author   :CHNJX
+# @File     :ad_utils.py
+# @Desc     :public utils
+import ast
+from os import makedirs
+import os
+from urllib.parse import unquote
+import re
+
+
+def covert_list_to_dict(list_data):
+    """
+    将har list data 转换成dict
+    :param list_data
+        list_data (list)
+            [
+                {"name": "v", "value": "1"},
+                {"name": "w", "value": "2"}
+            ]
+
+    :return:
+        dict:
+            {"v": "1", "w": "2"}
+    """
+    return {item['name']: item.get('value') for item in list_data}
+
+
+def convert_x_www_form_to_dict(form_data: str):
+    """
+    将form表单数据装换成dict字典数据
+    :param form_data:  (str): a=1&b=2
+    :return: (dict) {"a":1, "b":2}
+    """
+    if isinstance(form_data, str):
+        res_dict = {}
+        for kev_value in form_data.split('&'):
+            try:
+                key, value = kev_value.split('=')
+            except ValueError:
+                raise Exception(f"错误的 x_www_form_urlencoded 数据: {form_data}")
+            # unquote('abc%20def') -> 'abc def'.
+            res_dict[key] = unquote(value)
+        return res_dict
+    else:
+        return form_data
+
+
+def get_class_and_func(api_file, url, method) -> tuple:
+    """
+    获取到类名和方法名
+    :param api_file: 对应api文件
+    :param url:     对应请求url
+    :param method:  请求方式
+    :return:
+    """
+    api_class = ''
+    func_name = ''
+    with open(api_file, 'r', encoding='utf-8') as f:
+        cd = ast.parse(f.read())
+        for item in cd.body:
+            if isinstance(item, ast.ClassDef) and item.body:
+                for func in item.body:
+                    if isinstance(func, ast.FunctionDef):
+                        func_str = ast.dump(func)
+                        if url in func_str and method.lower() in func_str:
+                            pattern = "name='(.*?)'"
+                            api_class = re.search(pattern, ast.dump(item)).group(1)
+                            func_name = re.search(pattern, ast.dump(func)).group(1)
+                            break
+    return api_class, func_name
+
+
+def write(content, file_path):
+    """
+    将内容写入文档中
+    :param content:  要写入的内容
+    :param file_path: 文件路径（不存在则会进行创建）
+    :return: None
+    """
+    dir_ = os.path.dirname(file_path)
+    if not os.path.exists(dir_):
+        os.makedirs(dir_)
+    with open(file_path, 'w', encoding='utf-8') as f:
+        f.write(content)
+
+
+def create_folder(path):
+    """
+    创建目录
+    :param path: 目录路径
+    :return: None
+    """
+    makedirs(path)
+    print(f'create folder {path}')
+
+
+
+
```

### Comparing `apidriver-0.7.0/api_driver/command.py` & `apidriver-0.8.0/api_driver/command.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-# -*- coding:utf-8 -*-
-# @Time     :2023/2/7 12:38
-# @Author   :CHNJX
-# @File     :command.py
-# @Desc     :命令工具
-import subprocess
-import sys
-from os.path import dirname, exists
-import click as click
-
-from api_driver.har_parser import HarParser
-
-sys.path.append(dirname(sys.path[0]))
-
-from api_driver.project_generator import ProjectGenerator
-from api_driver.swagger_generate import SwaggerGenerator
-
-group = click.Group()
-
-
-@click.command('start_project')
-@click.option('-n', '--project-name', required=True, help='project name')
-def start_project(project_name):
-    """
-    创建项目
-    :param project_name: 项目名称
-    """
-    ProjectGenerator().project_generate(project_name)
-
-
-@click.command('swagger2api')
-@click.option('-s', '--swagger-doc',
-              required=True, help='Swagger doc file.')
-@click.option('-d', '--api-dir',
-              required=False, help='api save dir.')
-def swagger2api(swagger_doc, api_dir):
-    """
-    swagger文档转换成api-object
-    :param swagger_doc: swagger.json 文件
-    :param api_dir:  api存放路径 非必填
-    """
-    SwaggerGenerator().generate(swagger_doc, api_dir)
-
-
-@click.command('run')
-@click.option('-c', '--testcase',
-              required=True, help='testcase')
-@click.option('-t', '--tag',
-              required=False, help='testcase')
-@click.option('-r', '--reset', help='auto clear report', required=False, default='false',
-              type=click.Choice(['true', 'false']))
-def run(testcase, tag, reset):
-    """
-    运行用例并集成allure报告
-    :param testcase: 用例路径
-    :param tag: 用例标签
-    :param reset: 是否重置allure报告
-    :return: 
-    """""
-    command = f'pytest -v -s {testcase}'
-    if reset == 'true':
-        if 'win' in sys.platform:
-            subprocess.call(f'rmdir /Q /S allure-results', shell=True)
-        else:
-            subprocess.call(f'rmdir -rf allure-results', shell=True)
-    if tag:
-        command += f' -m {tag}'
-    subprocess.call(command + ' --alluredir=./allure-results', shell=True)
-
-
-@click.command('har2case')
-@click.option('-h', '--har',
-              required=True, help='har file path')
-@click.option('-a', '--api',
-              required=False, help='api object dir', default=None)
-@click.option('-t', '--testcase', help='testcase dir', required=False, default='testcase')
-@click.option('-e', '--exclude', help='exclude url', required=False, default='')
-def har2case(har, api, testcase, exclude):
-    """
-    将har转换成用例
-    :param har: har文件路径
-    :param api: har对应api-object文件
-    :param testcase:  用例路径
-    :param exclude:  过来的url
-    :return:
-    """
-    hp = HarParser(har_file_path=har, api_object=api, exclude_url=exclude)
-    hp.generate_testcase(testcase_path=testcase)
-
-
-group.add_command(start_project)
-group.add_command(swagger2api)
-group.add_command(run)
-group.add_command(har2case)
-
-
-def cmd():
-    group.main()
-
-
-if __name__ == '__main__':
-    cmd()
+# -*- coding:utf-8 -*-
+# @Time     :2023/2/7 12:38
+# @Author   :CHNJX
+# @File     :command.py
+# @Desc     :命令工具
+import subprocess
+import sys
+from os.path import dirname, exists
+import click as click
+
+from api_driver.har_parser import HarParser
+
+sys.path.append(dirname(sys.path[0]))
+
+from api_driver.project_generator import ProjectGenerator
+from api_driver.swagger_generate import SwaggerGenerator
+
+group = click.Group()
+
+
+@click.command('start_project')
+@click.option('-n', '--project-name', required=True, help='project name')
+def start_project(project_name):
+    """
+    创建项目
+    :param project_name: 项目名称
+    """
+    ProjectGenerator().project_generate(project_name)
+
+
+@click.command('swagger2api')
+@click.option('-s', '--swagger-doc',
+              required=True, help='Swagger doc file.')
+@click.option('-d', '--api-dir',
+              required=False, help='api save dir.')
+def swagger2api(swagger_doc, api_dir):
+    """
+    swagger文档转换成api-object
+    :param swagger_doc: swagger.json 文件
+    :param api_dir:  api存放路径 非必填
+    """
+    SwaggerGenerator().generate(swagger_doc, api_dir)
+
+
+@click.command('run')
+@click.option('-c', '--testcase',
+              required=True, help='testcase')
+@click.option('-t', '--tag',
+              required=False, help='testcase')
+@click.option('-r', '--reset', help='auto clear report', required=False, default='false',
+              type=click.Choice(['true', 'false']))
+def run(testcase, tag, reset):
+    """
+    运行用例并集成allure报告
+    :param testcase: 用例路径
+    :param tag: 用例标签
+    :param reset: 是否重置allure报告
+    :return: 
+    """""
+    command = f'pytest -v -s {testcase}'
+    if reset == 'true':
+        if 'win' in sys.platform:
+            subprocess.call(f'rmdir /Q /S allure-results', shell=True)
+        else:
+            subprocess.call(f'rmdir -rf allure-results', shell=True)
+    if tag:
+        command += f' -m {tag}'
+    subprocess.call(command + ' --alluredir=./allure-results', shell=True)
+
+
+@click.command('har2case')
+@click.option('-h', '--har',
+              required=True, help='har file path')
+@click.option('-a', '--api',
+              required=False, help='api object dir', default=None)
+@click.option('-t', '--testcase', help='testcase dir', required=False, default='testcase')
+@click.option('-e', '--exclude', help='exclude url', required=False, default='')
+def har2case(har, api, testcase, exclude):
+    """
+    将har转换成用例
+    :param har: har文件路径
+    :param api: har对应api-object文件
+    :param testcase:  用例路径
+    :param exclude:  过来的url
+    :return:
+    """
+    hp = HarParser(har_file_path=har, api_object=api, exclude_url=exclude)
+    hp.generate_testcase(testcase_path=testcase)
+
+
+group.add_command(start_project)
+group.add_command(swagger2api)
+group.add_command(run)
+group.add_command(har2case)
+
+
+def cmd():
+    group.main()
+
+
+if __name__ == '__main__':
+    cmd()
```

### Comparing `apidriver-0.7.0/api_driver/loader_swagger.py` & `apidriver-0.8.0/api_driver/loader_swagger.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.7.0/api_driver/swagger_generate.py` & `apidriver-0.8.0/api_driver/swagger_generate.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.7.0/api_driver/templates/api.tpl` & `apidriver-0.8.0/api_driver/templates/api.tpl`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from api_object.http import Http
-
-
-class {{ tag }}(Http):
-
-    {%- for key,path in paths.items() %}
-
-    def {{ path["name"] }}(self{{ path["params_list"].__len__() and ", " or "" }}{{ path["params_list"] | join(", ") }}):
-        """
-        {{path["desc"]}}
-        {%- for param in path["parameters"] %}
-        :param {{param["name"]}}: {{param["description"]}} {% if param["required"] -%}*{% endif %}
-        {%- if loop.last %}
-        {% endif %}
-        {%- endfor -%}
-
-        {%- for param_name in path["json"] %}
-        :param {{param_name}}:
-        {%- if loop.last %}
-        {% endif %}
-        {%- endfor %}
-        """
-
-        req_data = {
-            "url": {% if path["url_param"] %}f"{{path["url"]}}/{ {{path["url_param"]}} }"{% else %}f"{{key}}"{% endif %},
-            {%- if path["parameters"] %}
-            "params": {
-                {%- for param in path["parameters"] %}
-                "{{param["name"]}}": {{param["name"]}}{%- if not loop.last %},{% else %}
-                {% endif %}
-                {%- endfor -%}
-            },
-            {% endif -%}
-            {%- if path["data"] %}
-            "data": {
-                {%- for param_name in path["data"] %}
-                "{{param_name}}": {{param_name}}{%- if not loop.last %},{% else %}
-                {% endif %}
-                {%- endfor -%}
-            },
-            {% endif -%}
-            {%- if path["files"] %}
-            "files": [
-                {%- for file_name in path["files"] %}
-                ('{{file_name}}', (file.split('/')[-1] if '/' in file else file.split('\\')[-1],
-                          open({{file_name}}, 'rb'),
-                          'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'))
-                {%- if not loop.last %},{% else %}
-                {% endif %}
-                {%- endfor -%}
-            ],
-            {% endif -%}
-            {%- if path["content-type"] %}
-            "headers": {"content-type": "{{path["content-type"]}}"}
-            {% endif -%}
-        }
-        return self.req(method="{{path["method"]}}", **req_data)
-
+from api_object.http import Http
+
+
+class {{ tag }}(Http):
+
+    {%- for key,path in paths.items() %}
+
+    def {{ path["name"] }}(self{{ path["params_list"].__len__() and ", " or "" }}{{ path["params_list"] | join(", ") }}):
+        """
+        {{path["desc"]}}
+        {%- for param in path["parameters"] %}
+        :param {{param["name"]}}: {{param["description"]}} {% if param["required"] -%}*{% endif %}
+        {%- if loop.last %}
+        {% endif %}
+        {%- endfor -%}
+
+        {%- for param_name in path["json"] %}
+        :param {{param_name}}:
+        {%- if loop.last %}
+        {% endif %}
+        {%- endfor %}
+        """
+
+        req_data = {
+            "url": {% if path["url_param"] %}f"{{path["url"]}}/{ {{path["url_param"]}} }"{% else %}f"{{key}}"{% endif %},
+            {%- if path["parameters"] %}
+            "params": {
+                {%- for param in path["parameters"] %}
+                "{{param["name"]}}": {{param["name"]}}{%- if not loop.last %},{% else %}
+                {% endif %}
+                {%- endfor -%}
+            },
+            {% endif -%}
+            {%- if path["data"] %}
+            "data": {
+                {%- for param_name in path["data"] %}
+                "{{param_name}}": {{param_name}}{%- if not loop.last %},{% else %}
+                {% endif %}
+                {%- endfor -%}
+            },
+            {% endif -%}
+            {%- if path["files"] %}
+            "files": [
+                {%- for file_name in path["files"] %}
+                ('{{file_name}}', (file.split('/')[-1] if '/' in file else file.split('\\')[-1],
+                          open({{file_name}}, 'rb'),
+                          'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'))
+                {%- if not loop.last %},{% else %}
+                {% endif %}
+                {%- endfor -%}
+            ],
+            {% endif -%}
+            {%- if path["content-type"] %}
+            "headers": {"content-type": "{{path["content-type"]}}"}
+            {% endif -%}
+        }
+        return self.req(method="{{path["method"]}}", **req_data)
+
     {%- endfor -%}
```

### Comparing `apidriver-0.7.0/api_driver/templates/har2api_case.tpl` & `apidriver-0.8.0/api_driver/templates/har2api_case.tpl`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from api_object.http import Http
-from jsonpath import jsonpath
-from testcase.test_base import TestBase
-{%- for module in module_dir_list %}
-from {{module}} import *
-{%- endfor %}
-
-
-class Test{{model_name}}(TestBase):
-
-    def setup_class(self):
-        self.http = Http()
-
-    def test_{{case_name}}(self):
-        self.logger.info('用例名称：{{case_name}}')
-        {%- for step in testcase_steps %}
-        self.logger.info('测试步骤：{{step['name']}}')
-        {% if step['api_class'] and step['func_name'] %}
-        request_data = {}
-        {%- if step['request']['params'] %}
-        request_data.update({{step['request']['params']}})
-        {% endif %}
-        {%- if step['request']['data'] %}
-        request_data.update({{step['request']['data']}})
-        {% endif %}
-        {%- if step['request']['json'] %}
-        request_data.update({{step['request']['json']}})
-        {% endif %}
-        resp = {{step['api_class']}}().{{step['func_name']}}(**request_data)
-        {% else %}
-        req_data = {
-            "url": "{{step['request']['url']}}",
-            "method": "{{step['request']['method']}}",
-            {%- if step['request']['params'] %}
-            'params': {{step['request']['params']}},
-            {% endif %}
-            {%- if step['request']['data'] %}
-            'data': {{step['request']['data']}},
-            {% endif %}
-            {%- if step['request']['json'] %}
-            'json': {{step['request']['json']}},
-            {% endif %}
-            {%- if step['request']['headers'] -%}
-            'headers': {{step['request']['headers']}},
-            {% endif -%}
-        }
-        resp = self.http.req(**req_data)
-        {%- endif %}
-
-        # 断言
-        {% for valid in step['validate'] %}
-        {%- for key,value in valid.items() -%}
-        {%- if key=='equals' -%}
-        assert resp['{{value[0]}}'] == {{value[1]}}
-        {% else %}
-        assert {{value[0]}} in "{{value[1]}}"
-        {% endif %}
-        {%- endfor -%}
-        {%- endfor -%}
-
-        {%- if step['header_validate'] -%}
-        {% for valid in step['header_validate'] %}
-        {%- for key,value in valid.items() -%}
-        {%- if key=='equals' -%}
-        assert resp['headers']['{{value[0]}}'] == "{{value[1]}}"
-        {% else %}
-        assert resp['headers']['{{value[0]}}'] == "{{value[1]}}"
-        {% endif %}
-        {%- endfor -%}
-        {%- endfor -%}
-        {% endif %}
-
-        {%- if step['json_validate'] -%}
-        {% for valid in step['json_validate'] %}
-        {%- for key,value in valid.items() -%}
-        {%- if key=='equals' -%}
-        assert str(jsonpath(resp, '$..{{value[0]}}')[0]) == "{{value[1]}}"
-        {% else %}
-        assert str(jsonpath(resp, '$..{{value[0]}}')[0]) in "{{value[1]}}"
-        {% endif %}
-        {%- endfor -%}
-        {%- endfor -%}
-        {% endif %}
+from api_object.http import Http
+from jsonpath import jsonpath
+from testcase.test_base import TestBase
+{%- for module in module_dir_list %}
+from {{module}} import *
+{%- endfor %}
+
+
+class Test{{model_name}}(TestBase):
+
+    def setup_class(self):
+        self.http = Http()
+
+    def test_{{case_name}}(self):
+        self.logger.info('用例名称：{{case_name}}')
+        {%- for step in testcase_steps %}
+        self.logger.info('测试步骤：{{step['name']}}')
+        {% if step['api_class'] and step['func_name'] %}
+        request_data = {}
+        {%- if step['request']['params'] %}
+        request_data.update({{step['request']['params']}})
+        {% endif %}
+        {%- if step['request']['data'] %}
+        request_data.update({{step['request']['data']}})
+        {% endif %}
+        {%- if step['request']['json'] %}
+        request_data.update({{step['request']['json']}})
+        {% endif %}
+        resp = {{step['api_class']}}().{{step['func_name']}}(**request_data)
+        {% else %}
+        req_data = {
+            "url": "{{step['request']['url']}}",
+            "method": "{{step['request']['method']}}",
+            {%- if step['request']['params'] %}
+            'params': {{step['request']['params']}},
+            {% endif %}
+            {%- if step['request']['data'] %}
+            'data': {{step['request']['data']}},
+            {% endif %}
+            {%- if step['request']['json'] %}
+            'json': {{step['request']['json']}},
+            {% endif %}
+            {%- if step['request']['headers'] -%}
+            'headers': {{step['request']['headers']}},
+            {% endif -%}
+        }
+        resp = self.http.req(**req_data)
+        {%- endif %}
+
+        # 断言
+        {% for valid in step['validate'] %}
+        {%- for key,value in valid.items() -%}
+        {%- if key=='equals' -%}
+        assert resp['{{value[0]}}'] == {{value[1]}}
+        {% else %}
+        assert {{value[0]}} in "{{value[1]}}"
+        {% endif %}
+        {%- endfor -%}
+        {%- endfor -%}
+
+        {%- if step['header_validate'] -%}
+        {% for valid in step['header_validate'] %}
+        {%- for key,value in valid.items() -%}
+        {%- if key=='equals' -%}
+        assert resp['headers']['{{value[0]}}'] == "{{value[1]}}"
+        {% else %}
+        assert resp['headers']['{{value[0]}}'] == "{{value[1]}}"
+        {% endif %}
+        {%- endfor -%}
+        {%- endfor -%}
+        {% endif %}
+
+        {%- if step['json_validate'] -%}
+        {% for valid in step['json_validate'] %}
+        {%- for key,value in valid.items() -%}
+        {%- if key=='equals' -%}
+        assert str(jsonpath(resp, '$..{{value[0]}}')[0]) == "{{value[1]}}"
+        {% else %}
+        assert str(jsonpath(resp, '$..{{value[0]}}')[0]) in "{{value[1]}}"
+        {% endif %}
+        {%- endfor -%}
+        {%- endfor -%}
+        {% endif %}
         {%- endfor -%}
```

### Comparing `apidriver-0.7.0/api_driver/templates/har2case.tpl` & `apidriver-0.8.0/api_driver/templates/har2case.tpl`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from api_object.http import Http
-from jsonpath import jsonpath
-from testcase.test_base import TestBase
-
-
-class Test{{model_name}}(TestBase):
-
-    def setup_class(self):
-        self.http = Http()
-
-    def test_{{case_name}}(self):
-        self.logger.info('用例名称：{{case_name}}')
-        {%- for step in testcase_steps %}
-        self.logger.info('测试步骤：{{step['name']}}')
-        req_data = {
-            "url": "{{step['request']['url']}}",
-            "method": "{{step['request']['method']}}",
-            {%- if step['request']['params'] %}
-            'params': {{step['request']['params']}},
-            {% endif %}
-            {%- if step['request']['data'] %}
-            'data': {{step['request']['data']}},
-            {% endif %}
-            {%- if step['request']['json'] %}
-            'json': {{step['request']['json']}},
-            {% endif %}
-            {%- if step['request']['headers'] -%}
-            'headers': {{step['request']['headers']}},
-            {% endif -%}
-        }
-
-        resp = self.http.req(**req_data)
-        # 断言
-        {% for valid in step['validate'] %}
-        {%- for key,value in valid.items() -%}
-        {%- if key=='equals' -%}
-        assert resp['{{value[0]}}'] == {{value[1]}}
-        {% else %}
-        assert {{value[0]}} in "{{value[1]}}"
-        {% endif %}
-        {%- endfor -%}
-        {%- endfor -%}
-
-        {%- if step['header_validate'] -%}
-        {% for valid in step['header_validate'] %}
-        {%- for key,value in valid.items() -%}
-        {%- if key=='equals' -%}
-        assert resp['headers']['{{value[0]}}'] == "{{value[1]}}"
-        {% else %}
-        assert resp['headers']['{{value[0]}}'] == "{{value[1]}}"
-        {% endif %}
-        {%- endfor -%}
-        {%- endfor -%}
-        {% endif %}
-
-        {%- if step['json_validate'] -%}
-        {% for valid in step['json_validate'] %}
-        {%- for key,value in valid.items() -%}
-        {%- if key=='equals' -%}
-        assert str(jsonpath(resp, '$..{{value[0]}}')[0]) == "{{value[1]}}"
-        {% else %}
-        assert str(jsonpath(resp, '$..{{value[0]}}')[0]) in "{{value[1]}}"
-        {% endif %}
-        {%- endfor -%}
-        {%- endfor -%}
-        {% endif %}
+from api_object.http import Http
+from jsonpath import jsonpath
+from testcase.test_base import TestBase
+
+
+class Test{{model_name}}(TestBase):
+
+    def setup_class(self):
+        self.http = Http()
+
+    def test_{{case_name}}(self):
+        self.logger.info('用例名称：{{case_name}}')
+        {%- for step in testcase_steps %}
+        self.logger.info('测试步骤：{{step['name']}}')
+        req_data = {
+            "url": "{{step['request']['url']}}",
+            "method": "{{step['request']['method']}}",
+            {%- if step['request']['params'] %}
+            'params': {{step['request']['params']}},
+            {% endif %}
+            {%- if step['request']['data'] %}
+            'data': {{step['request']['data']}},
+            {% endif %}
+            {%- if step['request']['json'] %}
+            'json': {{step['request']['json']}},
+            {% endif %}
+            {%- if step['request']['headers'] -%}
+            'headers': {{step['request']['headers']}},
+            {% endif -%}
+        }
+
+        resp = self.http.req(**req_data)
+        # 断言
+        {% for valid in step['validate'] %}
+        {%- for key,value in valid.items() -%}
+        {%- if key=='equals' -%}
+        assert resp['{{value[0]}}'] == {{value[1]}}
+        {% else %}
+        assert {{value[0]}} in "{{value[1]}}"
+        {% endif %}
+        {%- endfor -%}
+        {%- endfor -%}
+
+        {%- if step['header_validate'] -%}
+        {% for valid in step['header_validate'] %}
+        {%- for key,value in valid.items() -%}
+        {%- if key=='equals' -%}
+        assert resp['headers']['{{value[0]}}'] == "{{value[1]}}"
+        {% else %}
+        assert resp['headers']['{{value[0]}}'] == "{{value[1]}}"
+        {% endif %}
+        {%- endfor -%}
+        {%- endfor -%}
+        {% endif %}
+
+        {%- if step['json_validate'] -%}
+        {% for valid in step['json_validate'] %}
+        {%- for key,value in valid.items() -%}
+        {%- if key=='equals' -%}
+        assert str(jsonpath(resp, '$..{{value[0]}}')[0]) == "{{value[1]}}"
+        {% else %}
+        assert str(jsonpath(resp, '$..{{value[0]}}')[0]) in "{{value[1]}}"
+        {% endif %}
+        {%- endfor -%}
+        {%- endfor -%}
+        {% endif %}
         {%- endfor -%}
```

### Comparing `apidriver-0.7.0/api_driver/templates/http.tpl` & `apidriver-0.8.0/api_driver/templates/http.tpl`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-import requests
-
-import os
-
-from api_driver.utils.service_logger import Logger
-
-
-class Http:
-    def __init__(self, base_url=''):
-        self.base_uri = base_url
-        self.headers = {}
-
-        self.base_dir = os.path.join(os.path.dirname(__file__), '..')
-        self.logger = Logger.getLogger("api", self.base_dir)
-
-    def req(self, method, url, headers=None, return_json=True, **kwargs):
-        """
-        发送请求
-        :param return_json: 响应数据是否以json格式返回
-        :param json: json格式参数
-        :param params: url携带参数
-        :param data: 表单参数
-        :param method: method for the new :class:`Request` object: ``GET``, ``OPTIONS``, ``HEAD``, ``POST``, ``PUT``, ``PATCH``, or ``DELETE``.
-        :param url: URL for the new :class:`Request` object.
-            in the query string for the :class:`Request`.
-            object to send in the body of the :class:`Request`.
-        :param headers: (optional) Dictionary of HTTP Headers to send with the :class:`Request`.
-        :param cookies: (optional) Dict or CookieJar object to send with the :class:`Request`.
-        :param files: (optional) Dictionary of ``'name': file-like-objects`` (or ``{'name': file-tuple}``) for multipart encoding upload.
-            ``file-tuple`` can be a 2-tuple ``('filename', fileobj)``, 3-tuple ``('filename', fileobj, 'content_type')``
-            or a 4-tuple ``('filename', fileobj, 'content_type', custom_headers)``, where ``'content-type'`` is a string
-            defining the content type of the given file and ``custom_headers`` a dict-like object containing additional headers
-            to add for the file.
-        :param auth: (optional) Auth tuple to enable Basic/Digest/Custom HTTP Auth.
-        :param timeout: (optional) How many seconds to wait for the server to send data
-            before giving up, as a float, or a :ref:`(connect timeout, read
-            timeout) <timeouts>` tuple.
-        :type timeout: float or tuple
-        :param allow_redirects: (optional) Boolean. Enable/disable GET/OPTIONS/POST/PUT/PATCH/DELETE/HEAD redirection. Defaults to ``True``.
-        :type allow_redirects: bool
-        :param proxies: (optional) Dictionary mapping protocol to the URL of the proxy.
-        :param verify: (optional) Either a boolean, in which case it controls whether we verify
-                the server's TLS certificate, or a string, in which case it must be a path
-                to a CA bundle to use. Defaults to ``True``.
-        :param stream: (optional) if ``False``, the response content will be immediately downloaded.
-        :param cert: (optional) if String, path to ssl client cert file (.pem). If Tuple, ('cert', 'key') pair.
-
-        """
-        self.logger.info(f"======请求接口地址：{url}======请求方式：{method}======请求数据{kwargs.__str__()}")
-        if headers:
-            self.headers.update(headers)
-        try:
-            resp = requests.request(method=method, url=self.base_uri + url, headers=self.headers, **kwargs)
-            self.logger.info(f'请求结果：{resp.text}')
-        except requests.exceptions.RequestException as e:
-            self.logger.error("请求接口错误: " + e.__str__())
-            raise e
-        try:
-            if return_json:
-                json_data: dict = resp.json()
-            else:
-                return resp
-        except ValueError:
-            json_data = {}
-        json_data.update({'status_code': resp.status_code,
-                          'text': resp.text,
-                          'resp_time': resp.elapsed.total_seconds(),
-                          'headers': resp.headers})
-        return json_data
-
-    def get_req(self, url, headers=None, return_json=True, **kwargs):
-        """
-        get请求
-        :param url: 请求路径
-        :param headers: 请求头
-        :param return_json: 是否返回json格式响应
-        :param kwargs: request的所有请求参数
-        :return: Response
-        """
-        return self.req("get", url, headers, return_json, **kwargs)
-
-    def post_req(self, url, headers=None, return_json=True, **kwargs):
-        """
-        get请求
-        :param url: 请求路径
-        :param headers: 请求头
-        :param return_json: 是否返回json格式响应
-        :param kwargs: request的所有请求参数
-        :return: Response
-        """
-        return self.req("post", url, headers, return_json, **kwargs)
-
-    def put_req(self, url, headers=None, return_json=True, **kwargs):
-        """
-        put请求
-        :param url: 请求路径
-        :param headers: 请求头
-        :param return_json: 是否返回json格式响应
-        :param kwargs: request的所有请求参数
-        :return: Response
-        """
-        return self.req("put", url, headers, return_json, **kwargs)
-
-    def delete_req(self, url, headers=None, return_json=True, **kwargs):
-        """
-        put请求
-        :param url: 请求路径
-        :param headers: 请求头
-        :param return_json: 是否返回json格式响应
-        :param kwargs: request的所有请求参数
-        :return: Response
-        """
-        return self.req("delete", url, headers, return_json, **kwargs)
-
+import requests
+
+import os
+
+from api_driver.utils.service_logger import Logger
+
+
+class Http:
+    def __init__(self, base_url=''):
+        self.base_uri = base_url
+        self.headers = {}
+
+        self.base_dir = os.path.join(os.path.dirname(__file__), '..')
+        self.logger = Logger.getLogger("api", self.base_dir)
+
+    def req(self, method, url, headers=None, return_json=True, **kwargs):
+        """
+        发送请求
+        :param return_json: 响应数据是否以json格式返回
+        :param json: json格式参数
+        :param params: url携带参数
+        :param data: 表单参数
+        :param method: method for the new :class:`Request` object: ``GET``, ``OPTIONS``, ``HEAD``, ``POST``, ``PUT``, ``PATCH``, or ``DELETE``.
+        :param url: URL for the new :class:`Request` object.
+            in the query string for the :class:`Request`.
+            object to send in the body of the :class:`Request`.
+        :param headers: (optional) Dictionary of HTTP Headers to send with the :class:`Request`.
+        :param cookies: (optional) Dict or CookieJar object to send with the :class:`Request`.
+        :param files: (optional) Dictionary of ``'name': file-like-objects`` (or ``{'name': file-tuple}``) for multipart encoding upload.
+            ``file-tuple`` can be a 2-tuple ``('filename', fileobj)``, 3-tuple ``('filename', fileobj, 'content_type')``
+            or a 4-tuple ``('filename', fileobj, 'content_type', custom_headers)``, where ``'content-type'`` is a string
+            defining the content type of the given file and ``custom_headers`` a dict-like object containing additional headers
+            to add for the file.
+        :param auth: (optional) Auth tuple to enable Basic/Digest/Custom HTTP Auth.
+        :param timeout: (optional) How many seconds to wait for the server to send data
+            before giving up, as a float, or a :ref:`(connect timeout, read
+            timeout) <timeouts>` tuple.
+        :type timeout: float or tuple
+        :param allow_redirects: (optional) Boolean. Enable/disable GET/OPTIONS/POST/PUT/PATCH/DELETE/HEAD redirection. Defaults to ``True``.
+        :type allow_redirects: bool
+        :param proxies: (optional) Dictionary mapping protocol to the URL of the proxy.
+        :param verify: (optional) Either a boolean, in which case it controls whether we verify
+                the server's TLS certificate, or a string, in which case it must be a path
+                to a CA bundle to use. Defaults to ``True``.
+        :param stream: (optional) if ``False``, the response content will be immediately downloaded.
+        :param cert: (optional) if String, path to ssl client cert file (.pem). If Tuple, ('cert', 'key') pair.
+
+        """
+        self.logger.info(f"======请求接口地址：{url}======请求方式：{method}======请求数据{kwargs.__str__()}")
+        if headers:
+            self.headers.update(headers)
+        try:
+            resp = requests.request(method=method, url=self.base_uri + url, headers=self.headers, **kwargs)
+            self.logger.info(f'请求结果：{resp.text}')
+        except requests.exceptions.RequestException as e:
+            self.logger.error("请求接口错误: " + e.__str__())
+            raise e
+        try:
+            if return_json:
+                json_data: dict = resp.json()
+            else:
+                return resp
+        except ValueError:
+            json_data = {}
+        json_data.update({'status_code': resp.status_code,
+                          'text': resp.text,
+                          'resp_time': resp.elapsed.total_seconds(),
+                          'headers': resp.headers})
+        return json_data
+
+    def get_req(self, url, headers=None, return_json=True, **kwargs):
+        """
+        get请求
+        :param url: 请求路径
+        :param headers: 请求头
+        :param return_json: 是否返回json格式响应
+        :param kwargs: request的所有请求参数
+        :return: Response
+        """
+        return self.req("get", url, headers, return_json, **kwargs)
+
+    def post_req(self, url, headers=None, return_json=True, **kwargs):
+        """
+        get请求
+        :param url: 请求路径
+        :param headers: 请求头
+        :param return_json: 是否返回json格式响应
+        :param kwargs: request的所有请求参数
+        :return: Response
+        """
+        return self.req("post", url, headers, return_json, **kwargs)
+
+    def put_req(self, url, headers=None, return_json=True, **kwargs):
+        """
+        put请求
+        :param url: 请求路径
+        :param headers: 请求头
+        :param return_json: 是否返回json格式响应
+        :param kwargs: request的所有请求参数
+        :return: Response
+        """
+        return self.req("put", url, headers, return_json, **kwargs)
+
+    def delete_req(self, url, headers=None, return_json=True, **kwargs):
+        """
+        put请求
+        :param url: 请求路径
+        :param headers: 请求头
+        :param return_json: 是否返回json格式响应
+        :param kwargs: request的所有请求参数
+        :return: Response
+        """
+        return self.req("delete", url, headers, return_json, **kwargs)
+
```

### Comparing `apidriver-0.7.0/api_driver/testcase_mixin.py` & `apidriver-0.8.0/api_driver/testcase_mixin.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.7.0/api_driver/utils/database_conn.py` & `apidriver-0.8.0/api_driver/utils/database_conn.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# -*- coding:utf-8 -*-
-# @Time     :2022/7/1 11:20
-# @Author   :CHNJX
-# @File     :database_conn.py
-# @Desc     :获取数据库链接
-
-import pymysql
-
-
-class DatabaseConn:
-    conn = None
-    cursor = None
-
-    def __init__(self, database_config):
-        """
-        :param database_config:
-            example:
-            database_config = {
-                'host': 'xxx.cn',
-                'port': 3306,
-                'user': 'root',
-                'password': '123456',
-                'database': 'test',
-                'autocommit': True
-            }
-        """
-        self.create_conn(database_config)
-
-    def create_conn(self, database_config):
-        if not self.conn:
-            self.conn = pymysql.connect(charset='utf8', **database_config)
-            self.cursor = self.conn.cursor()
-
-    def close_conn(self):
-        if self.conn:
-            self.conn.close()
-
-    def excuse_sql(self, sql_str, params=None):
-        self.conn.ping(reconnect=True)
-        self.cursor.execute(sql_str, params)
-        # 判断是否为查询语句
-        try:
-            self.conn.ping(reconnect=True)
-            self.cursor.execute(sql_str, params)
-            # 判断是否为查询语句
-            if 'select' in sql_str.lower():
-                return self.cursor.fetchone()
-            else:
-                self.conn.commit()
-                return self.cursor.rowcount
-        except Exception as e:
-            print(f"Error in executing sql: {str(e)}")
-            self.conn.rollback()
-
-    def excuse_sql_with_all(self, sql_str, params=None):
-        """查询语句获取全量数据"""
-        try:
-            self.conn.ping(reconnect=True)
-            self.cursor.execute(sql_str, params)
-            return self.cursor.fetchall()
-        except Exception as e:
-            print(f"Error in executing sql: {str(e)}")
-            self.conn.rollback()
+# -*- coding:utf-8 -*-
+# @Time     :2022/7/1 11:20
+# @Author   :CHNJX
+# @File     :database_conn.py
+# @Desc     :获取数据库链接
+
+import pymysql
+
+
+class DatabaseConn:
+    conn = None
+    cursor = None
+
+    def __init__(self, database_config):
+        """
+        :param database_config:
+            example:
+            database_config = {
+                'host': 'xxx.cn',
+                'port': 3306,
+                'user': 'root',
+                'password': '123456',
+                'database': 'test',
+                'autocommit': True
+            }
+        """
+        self.create_conn(database_config)
+
+    def create_conn(self, database_config):
+        if not self.conn:
+            self.conn = pymysql.connect(charset='utf8', **database_config)
+            self.cursor = self.conn.cursor()
+
+    def close_conn(self):
+        if self.conn:
+            self.conn.close()
+
+    def excuse_sql(self, sql_str, params=None):
+        self.conn.ping(reconnect=True)
+        self.cursor.execute(sql_str, params)
+        # 判断是否为查询语句
+        try:
+            self.conn.ping(reconnect=True)
+            self.cursor.execute(sql_str, params)
+            # 判断是否为查询语句
+            if 'select' in sql_str.lower():
+                return self.cursor.fetchone()
+            else:
+                self.conn.commit()
+                return self.cursor.rowcount
+        except Exception as e:
+            print(f"Error in executing sql: {str(e)}")
+            self.conn.rollback()
+
+    def excuse_sql_with_all(self, sql_str, params=None):
+        """查询语句获取全量数据"""
+        try:
+            self.conn.ping(reconnect=True)
+            self.cursor.execute(sql_str, params)
+            return self.cursor.fetchall()
+        except Exception as e:
+            print(f"Error in executing sql: {str(e)}")
+            self.conn.rollback()
```

### Comparing `apidriver-0.7.0/api_driver/utils/service_logger.py` & `apidriver-0.8.0/api_driver/utils/service_logger.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# -*- coding:utf-8 -*-
-# @Time     :2023/2/3 7:48 上午
-# @Author   :CHNJX
-# @File     :service_logger.py
-# @Desc     :日志构造器
-
-import logging
-import os
-import sys
-import time
-from datetime import datetime
-
-
-class Logger:
-
-    @classmethod
-    def getLogger(cls, name, root_path, package_name="log") -> logging:
-        logger = logging.getLogger(name)
-        if logger.handlers:
-            return logger
-        logger.setLevel(logging.DEBUG)
-        now_string = datetime.now().strftime('%Y%m%d')
-        file_name = f'{now_string}_log.log'
-        logger_dir = os.path.join(root_path, package_name)
-        if not os.path.exists(logger_dir):
-            os.mkdir(logger_dir)
-        file_path = os.path.join(logger_dir, file_name)
-        t = int(time.time())
-
-        # FileHandler
-        fh = logging.FileHandler(file_path, mode='a', encoding='utf-8')
-        fh.setLevel(logging.DEBUG)
-        formatter = logging.Formatter(
-            '******%(asctime)s - %(name)s - %(filename)s,line %(lineno)s - %(levelname)s: %(message)s')
-        fh.setFormatter(formatter)
-
-        sh = logging.StreamHandler(sys.stdout)
-        sh.setFormatter(formatter)
-        sh.setLevel(logging.DEBUG)
-        logger.addHandler(fh)
-        logger.addHandler(sh)
-
-        return logger
+# -*- coding:utf-8 -*-
+# @Time     :2023/2/3 7:48 上午
+# @Author   :CHNJX
+# @File     :service_logger.py
+# @Desc     :日志构造器
+
+import logging
+import os
+import sys
+import time
+from datetime import datetime
+
+
+class Logger:
+
+    @classmethod
+    def getLogger(cls, name, root_path, package_name="log") -> logging:
+        logger = logging.getLogger(name)
+        if logger.handlers:
+            return logger
+        logger.setLevel(logging.DEBUG)
+        now_string = datetime.now().strftime('%Y%m%d')
+        file_name = f'{now_string}_log.log'
+        logger_dir = os.path.join(root_path, package_name)
+        if not os.path.exists(logger_dir):
+            os.mkdir(logger_dir)
+        file_path = os.path.join(logger_dir, file_name)
+        t = int(time.time())
+
+        # FileHandler
+        fh = logging.FileHandler(file_path, mode='a', encoding='utf-8')
+        fh.setLevel(logging.DEBUG)
+        formatter = logging.Formatter(
+            '******%(asctime)s - %(name)s - %(filename)s,line %(lineno)s - %(levelname)s: %(message)s')
+        fh.setFormatter(formatter)
+
+        sh = logging.StreamHandler(sys.stdout)
+        sh.setFormatter(formatter)
+        sh.setLevel(logging.DEBUG)
+        logger.addHandler(fh)
+        logger.addHandler(sh)
+
+        return logger
```

### Comparing `apidriver-0.7.0/apidriver.egg-info/SOURCES.txt` & `apidriver-0.8.0/apidriver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,8 @@
 api_driver/utils/service_logger.py
 apidriver.egg-info/PKG-INFO
 apidriver.egg-info/SOURCES.txt
 apidriver.egg-info/dependency_links.txt
 apidriver.egg-info/entry_points.txt
 apidriver.egg-info/requires.txt
 apidriver.egg-info/top_level.txt
-test/test_cli.py
-test/test_main.py
+test/test_cli.py
```

### Comparing `apidriver-0.7.0/setup.py` & `apidriver-0.8.0/setup.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from __future__ import absolute_import
-import re
-import ast
-from setuptools import setup
-
-_version_re = re.compile(r'__version__\s+=\s+(.*)')
-
-with open('api_driver/_version.py', 'rb') as f:
-    version = str(ast.literal_eval(_version_re.search(
-        f.read().decode('utf-8')).group(1)))
-
-with open('requirements.txt') as f:
-    requirements = [line for line in f.read().splitlines() if line]
-
-setup(
-    name='apidriver',
-    description='api test framework cli',
-    version=version,
-    author='CHNJX',
-    author_email='chaozhourose@gmail.com',
-    url='https://github.com/CHNJX/api-driver',
-    packages=['api_driver','api_driver.utils'],
-    package_data={'templates': ['api_driver/templates/*']},
-    include_package_data=True,
-    entry_points={
-        'console_scripts': [
-            'adf=api_driver:cmd'
-        ]
-    },
-    install_requires=requirements,
-    tests_require=['pytest'],
-)
+from __future__ import absolute_import
+import re
+import ast
+from setuptools import setup
+
+_version_re = re.compile(r'__version__\s+=\s+(.*)')
+
+with open('api_driver/_version.py', 'rb') as f:
+    version = str(ast.literal_eval(_version_re.search(
+        f.read().decode('utf-8')).group(1)))
+
+with open('requirements.txt') as f:
+    requirements = [line for line in f.read().splitlines() if line]
+
+setup(
+    name='apidriver',
+    description='api test framework cli',
+    version=version,
+    author='CHNJX',
+    author_email='chaozhourose@gmail.com',
+    url='https://github.com/CHNJX/api-driver',
+    packages=['api_driver','api_driver.utils'],
+    package_data={'templates': ['api_driver/templates/*']},
+    include_package_data=True,
+    entry_points={
+        'console_scripts': [
+            'adf=api_driver:cmd'
+        ]
+    },
+    install_requires=requirements,
+    tests_require=['pytest'],
+)
```

### Comparing `apidriver-0.7.0/test/test_cli.py` & `apidriver-0.8.0/test/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-import os
-from os.path import join, dirname
-
-import pytest
-
-from api_driver.har_parser import HarParser
-from api_driver.project_generator import ProjectGenerator
-from api_driver.swagger_generate import SwaggerGenerator
-
-
-class TestCommand:
-    def test_start_project(self):
-        ProjectGenerator().project_generate('new_project')
-        assert os.path.isdir(os.path.join('new_project', "api_object"))
-        assert os.path.isdir(os.path.join('new_project', "testcase"))
-
-    def test_swagger_generate(self):
-        SwaggerGenerator().generate(join(dirname(__file__), 'swagger/swagger.json'),
-                                    join(dirname(__file__), 'api_object'))
-        assert os.path.exists(os.path.join(dirname(__file__) + "/api_object", "users.py"))
-
-    def test_har2case_generate(self):
-        har_file = join(dirname(__file__), 'data/demo.har')
-        testcase_dir = join(dirname(__file__), 'testcase')
-        har = HarParser(har_file_path=har_file)
-        har.generate_testcase(testcase_path=testcase_dir)
-        assert os.path.exists(os.path.join(dirname(__file__) + "/testcase", "test_demo.py"))
-
-
-
+import os
+from os.path import join, dirname
+
+from api_driver.har_parser import HarParser
+from api_driver.project_generator import ProjectGenerator
+from api_driver.swagger_generate import SwaggerGenerator
+
+
+class TestCommand:
+    def test_start_project(self):
+        ProjectGenerator().project_generate('new_project')
+        assert os.path.isdir(os.path.join('new_project', "api_object"))
+        assert os.path.isdir(os.path.join('new_project', "testcase"))
+
+    def test_swagger_generate(self):
+        SwaggerGenerator().generate(join(dirname(__file__), 'swagger/swagger.json'),
+                                    join(dirname(__file__), 'api_object'))
+        assert os.path.exists(os.path.join(dirname(__file__) + "/api_object", "users.py"))
+
+    def test_har2case_generate(self):
+        har_file = join(dirname(__file__), 'data/demo.har')
+        testcase_dir = join(dirname(__file__), 'testcase')
+        har = HarParser(har_file_path=har_file)
+        har.generate_testcase(testcase_path=testcase_dir)
+        assert os.path.exists(os.path.join(dirname(__file__) + "/testcase", "test_demo.py"))
```

