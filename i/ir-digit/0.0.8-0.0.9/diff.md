# Comparing `tmp/ir_digit-0.0.8.tar.gz` & `tmp/ir_digit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ir_digit-0.0.8.tar", last modified: Mon Mar 27 12:14:11 2023, max compression
+gzip compressed data, was "ir_digit-0.0.9.tar", last modified: Mon Mar 27 13:56:32 2023, max compression
```

## Comparing `ir_digit-0.0.8.tar` & `ir_digit-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 12:14:11.896505 ir_digit-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-03-24 06:34:05.000000 ir_digit-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      414 2023-03-27 12:14:11.895505 ir_digit-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-03-27 07:07:49.000000 ir_digit-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 12:14:11.891503 ir_digit-0.0.8/digit/
--rw-rw-rw-   0        0        0      144 2023-03-27 12:13:29.000000 ir_digit-0.0.8/digit/__init__.py
--rw-rw-rw-   0        0        0      910 2023-03-27 09:02:10.000000 ir_digit-0.0.8/digit/code.py
--rw-rw-rw-   0        0        0      502 2023-03-27 11:09:42.000000 ir_digit-0.0.8/digit/data_access.py
--rw-rw-rw-   0        0        0     1088 2023-03-27 11:52:00.000000 ir_digit-0.0.8/digit/download_repo.py
--rw-rw-rw-   0        0        0      428 2023-03-27 11:09:42.000000 ir_digit-0.0.8/digit/load_config.py
-drwxrwxrwx   0        0        0        0 2023-03-27 12:14:11.894505 ir_digit-0.0.8/ir_digit.egg-info/
--rw-rw-rw-   0        0        0      414 2023-03-27 12:14:11.000000 ir_digit-0.0.8/ir_digit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-03-27 12:14:11.000000 ir_digit-0.0.8/ir_digit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 12:14:11.000000 ir_digit-0.0.8/ir_digit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-27 12:14:11.000000 ir_digit-0.0.8/ir_digit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 12:14:11.896505 ir_digit-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      550 2023-03-27 12:13:37.000000 ir_digit-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-27 13:56:32.418610 ir_digit-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-03-24 06:34:05.000000 ir_digit-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      414 2023-03-27 13:56:32.418610 ir_digit-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-03-27 07:07:49.000000 ir_digit-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-27 13:56:32.412085 ir_digit-0.0.9/digit/
+-rw-rw-rw-   0        0        0      144 2023-03-27 12:13:29.000000 ir_digit-0.0.9/digit/__init__.py
+-rw-rw-rw-   0        0        0     1042 2023-03-27 13:54:45.000000 ir_digit-0.0.9/digit/code.py
+-rw-rw-rw-   0        0        0      550 2023-03-27 13:54:36.000000 ir_digit-0.0.9/digit/data_access.py
+-rw-rw-rw-   0        0        0     1117 2023-03-27 13:54:36.000000 ir_digit-0.0.9/digit/download_repo.py
+-rw-rw-rw-   0        0        0      468 2023-03-27 13:52:53.000000 ir_digit-0.0.9/digit/load_config.py
+drwxrwxrwx   0        0        0        0 2023-03-27 13:56:32.417610 ir_digit-0.0.9/ir_digit.egg-info/
+-rw-rw-rw-   0        0        0      414 2023-03-27 13:56:32.000000 ir_digit-0.0.9/ir_digit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-03-27 13:56:32.000000 ir_digit-0.0.9/ir_digit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-27 13:56:32.000000 ir_digit-0.0.9/ir_digit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-03-27 13:56:32.000000 ir_digit-0.0.9/ir_digit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-27 13:56:32.418610 ir_digit-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      550 2023-03-27 13:56:19.000000 ir_digit-0.0.9/setup.py
```

### Comparing `ir_digit-0.0.8/LICENSE` & `ir_digit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ir_digit-0.0.8/digit/code.py` & `ir_digit-0.0.9/digit/code.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # -*- coding:utf-8 -*-
 import pandas
 
+"""
+Code接口，本地集成Code实现MyCode类。
+将数据预处理等方封装在MyCode类中，方便后续调用。
+"""
+
 
 class Code(object):
     """
     Code 类是一个接口，用于定义 Code 类的基本属性和方法，建议继承 Code类的类名设为 MyCode
     """
 
     def __init__(self, data: pandas.DataFrame):
```

### Comparing `ir_digit-0.0.8/digit/download_repo.py` & `ir_digit-0.0.9/digit/download_repo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
 
 import git
 
+"""
+下载git仓库
+"""
+
 
 def download_repo_git(url, path):
     print('Download start...')
     if not os.path.exists(path):  # 不存在该路径，创建该路径
         os.mkdir(path)
         # 下载git仓库
         git.Repo.clone_from(url, path)
```

### Comparing `ir_digit-0.0.8/setup.py` & `ir_digit-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="ir_digit",
-    version="0.0.8",
+    version="0.0.9",
     author="FKLiu",
     author_email="fkliu001@outlook.com",
     description="digit package",
     long_description="digit package ……",
     long_description_content_type="text",
     url="https://example.com",
     packages=setuptools.find_packages(),
```

