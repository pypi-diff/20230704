# Comparing `tmp/hydrorollcore-0.1.0.tar.gz` & `tmp/hydrorollcore-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrorollcore-0.1.0.tar", last modified: Fri Jun 23 04:54:30 2023, max compression
+gzip compressed data, was "hydrorollcore-0.1.1.tar", max compression
```

## Comparing `hydrorollcore-0.1.0.tar` & `hydrorollcore-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:54:30.849954 hydrorollcore-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:54:30.849954 hydrorollcore-0.1.0/HydroRollCore/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 04:54:11.000000 hydrorollcore-0.1.0/HydroRollCore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-23 04:54:11.000000 hydrorollcore-0.1.0/HydroRollCore/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-23 04:54:11.000000 hydrorollcore-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-23 04:54:30.849954 hydrorollcore-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-23 04:54:11.000000 hydrorollcore-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:54:30.849954 hydrorollcore-0.1.0/hydrorollcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-23 04:54:30.000000 hydrorollcore-0.1.0/hydrorollcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-23 04:54:30.000000 hydrorollcore-0.1.0/hydrorollcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 04:54:30.000000 hydrorollcore-0.1.0/hydrorollcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 04:54:30.000000 hydrorollcore-0.1.0/hydrorollcore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 04:54:11.000000 hydrorollcore-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-23 04:54:30.849954 hydrorollcore-0.1.0/setup.cfg
+-rw-r--r--   0        0        0     1066 2023-07-04 05:53:34.695080 hydrorollcore-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3591 2023-07-04 05:53:34.695080 hydrorollcore-0.1.1/README.md
+-rw-r--r--   0        0        0       60 2023-07-04 05:53:34.695080 hydrorollcore-0.1.1/core/__init__.py
+-rw-r--r--   0        0        0      597 2023-07-04 05:53:34.695080 hydrorollcore-0.1.1/core/main.py
+-rw-r--r--   0        0        0      937 2023-07-04 05:53:34.695080 hydrorollcore-0.1.1/core/rule.py
+-rw-r--r--   0        0        0     1469 2023-07-04 05:53:34.695080 hydrorollcore-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 hydrorollcore-0.1.1/PKG-INFO
```

### Comparing `hydrorollcore-0.1.0/HydroRollCore/rule.py` & `hydrorollcore-0.1.1/core/rule.py`

 * *Files identical despite different names*

### Comparing `hydrorollcore-0.1.0/LICENSE` & `hydrorollcore-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrorollcore-0.1.0/PKG-INFO` & `hydrorollcore-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,51 @@
-Metadata-Version: 2.1
-Name: hydrorollcore
-Version: 0.1.0
-Summary: Core of HydroRoll.
-Home-page: https://github.com/HydoRoll-Team/HydroRollCore
-Author: 简律纯
-Author-email: i@jyunko.cn
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="right">HydroRollCore'水系核心</h1>
 
 <p align="right">
   <a aria-label="Join the community on GitHub" href="https://github.com/HydroRoll-Team/hydroroll/discussions" target="blank">
     <img alt="" src="https://img.shields.io/badge/Join%20the%20community-blueviolet.svg?logo=data:image/x-icon;base64,AAABAAEAEBAAAAEAIABoBAAAFgAAACgAAAAQAAAAIAAAAAEAIAAAAAAAAAQAAAAAAAAAAAAAAAAAAAAAAAAAAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8CAgL/CgoK/woKCv8GBgb/BgYG/woKCv8KCgr/AgIC/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/BgYG/0ZGRv9MTEz/JiYm/ygoKP9MTEz/RkZG/wYGBv8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP9ycnL/Li4u/1xcXP9eXl7/Li4u/3Jycv8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP88PDz/cnJy/05OTv9OTk7/UFBQ/05OTv9wcHD/Pj4+/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/Kioq/3Jycv9cXFz/TExM/05OTv9aWlr/cHBw/yoqKv8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/Pj4+/zg4OP+AgID/Pj4+/2ZmZv9oaGj/PDw8/4CAgP86Ojr/Pj4+/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/ywsLP9iYmL/enp6/zIyMv90dHT/dHR0/zAwMP98fHz/YmJi/ywsLP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP9SUlL/PDw8/3Jycv9CQkL/UlJS/1RUVP9CQkL/cnJy/zw8PP9SUlL/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/VFRU/yIiIv9aWlr/PDw8/zw8PP8+Pj7/PDw8/1hYWP8iIiL/VFRU/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/zQ0NP9CQkL/ZmZm/yIiIv9WVlb/WFhY/yIiIv9mZmb/QkJC/zY2Nv8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP9QUFD/BgYG/0RERP9KSkr/JCQk/yYmJv9KSkr/RERE/wgICP9QUFD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/CgoK/wICAv8KCgr/CgoK/wYGBv8GBgb/CgoK/woKCv8CAgL/CgoK/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA==&labelColor=000000&logoWidth=20&logoColor=white">
   </a>
+  <a href="https://pypi.org/project/HydroRollCore">
+    <img src="https://img.shields.io/pypi/v/hydrorollcore?labelColor=000000">
+  </a>
+  <a href="https://github.com/HydroRoll-Team/HydroRollCore/blob/master/LICENSE">
+    <img alt="" src="https://img.shields.io/pypi/l/hydrorollcore.svg?labelColor=000000&color=">
+  </a>
+   
+  [![.github/workflows/python-publish.yml](https://github.com/HydroRoll-Team/HydroRollCore/actions/workflows/python-publish.yml/badge.svg)](https://github.com/HydroRoll-Team/HydroRollCore/actions/workflows/python-publish.yml)
+  [![CodeQL](https://github.com/HydroRoll-Team/HydroRollCore/actions/workflows/codeql.yml/badge.svg)](https://github.com/HydroRoll-Team/HydroRollCore/actions/workflows/codeql.yml)
+  
 </p>
 
-## 🎁 Getting <img align="right" src="https://hydroroll.retrofor.space/HydroRollBlue.png" height="220">
+## 🎁 Getting <img align="right" src="https://hydroroll.retrofor.space/HydroRollBlue.png" height="120">
 
 1. 安装库
 
 在命令行输入。
 
 ``` shell
-pip install HydroRollCore
+poetry install --no-dev HydroRollCore # 推荐
+pnpm install HydroRollCore # 不推荐
+pip install HydroRollCore # 不推荐
 ```
 
 2. 创建规则包实例
 
 ``` shell
 mkdir myrules && cd myrules && mkdir rule1
 echo.> config.toml && echo.> __init__.py :: 创建空的配置文件和python运行脚本
 ```
 
 在 `__init__.py` 创建一个 `rule` 实例并继承 `Rule` 基类, 通过编写合适的相关方法与类注册规则包实现规则的自定义。
 
 ``` python
-from hydrorollcore import Rule
-
-class rule(Rule):
-  ...
+from HydroRollCore import Rules
 
-class Wiki(rule):
-  ...
+class Myrule(Rules):
+  """自设规则包，继承 Rules 基类"""
 ```
 
 3. 合理修改你的 `config.toml` 配置文件，完成注册!
 
 ## 📄 License
 
-[GPL 3.0](https://github.com/HydroRoll-Team/HydroRollCore/blob/main/LICENSE) © 2023-PRESENT [简律纯](https://github.com/HsiangNianian)
+[MIT](https://github.com/HydroRoll-Team/HydroRollCore/blob/master/LICENSE) © 2023-PRESENT [简律纯](https://github.com/HsiangNianian)
```

