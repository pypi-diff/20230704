# Comparing `tmp/baysalt_christmas-0.1.8.1.tar.gz` & `tmp/baysalt_christmas-0.1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.8.1.tar", last modified: Mon Jul  3 03:03:27 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.8.2.tar", last modified: Tue Jul  4 08:31:54 2023, max compression
```

## Comparing `baysalt_christmas-0.1.8.1.tar` & `baysalt_christmas-0.1.8.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 03:03:27.197772 baysalt_christmas-0.1.8.1/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.8.1/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.8.1/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-03 03:03:27.197635 baysalt_christmas-0.1.8.1/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.8.1/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 03:03:27.193443 baysalt_christmas-0.1.8.1/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-03 03:03:27.000000 baysalt_christmas-0.1.8.1/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-03 03:03:27.000000 baysalt_christmas-0.1.8.1/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-03 03:03:27.000000 baysalt_christmas-0.1.8.1/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-03 03:03:27.000000 baysalt_christmas-0.1.8.1/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-03 03:03:27.000000 baysalt_christmas-0.1.8.1/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 03:03:27.195108 baysalt_christmas-0.1.8.1/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.8.1/christmas/Blogging.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 03:03:27.195404 baysalt_christmas-0.1.8.1/christmas/Pyshell/
--rw-r--r--   0 christmas   (501) staff       (20)     5975 2023-07-03 03:03:25.000000 baysalt_christmas-0.1.8.1/christmas/Pyshell/RS_File.py
--rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.8.1/christmas/Pyshell/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.8.1/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-03 02:25:27.000000 baysalt_christmas-0.1.8.1/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.8.1/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.8.1/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 03:03:27.196206 baysalt_christmas-0.1.8.1/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.1/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.1/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.8.1/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-03 03:03:27.197298 baysalt_christmas-0.1.8.1/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.8.1/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.1/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.1/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.8.1/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.8.1/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     9042 2023-06-28 02:50:13.000000 baysalt_christmas-0.1.8.1/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.8.1/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.8.1/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.8.1/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-03 03:03:27.197826 baysalt_christmas-0.1.8.1/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-03 03:03:25.000000 baysalt_christmas-0.1.8.1/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:31:54.861039 baysalt_christmas-0.1.8.2/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.8.2/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.8.2/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-04 08:31:54.860899 baysalt_christmas-0.1.8.2/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.8.2/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:31:54.852611 baysalt_christmas-0.1.8.2/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-04 08:31:54.000000 baysalt_christmas-0.1.8.2/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-04 08:31:54.000000 baysalt_christmas-0.1.8.2/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-04 08:31:54.000000 baysalt_christmas-0.1.8.2/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-04 08:31:54.000000 baysalt_christmas-0.1.8.2/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-04 08:31:54.000000 baysalt_christmas-0.1.8.2/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:31:54.855112 baysalt_christmas-0.1.8.2/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.8.2/christmas/Blogging.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:31:54.855560 baysalt_christmas-0.1.8.2/christmas/Pyshell/
+-rw-r--r--   0 christmas   (501) staff       (20)     5969 2023-07-04 08:31:53.000000 baysalt_christmas-0.1.8.2/christmas/Pyshell/RS_File.py
+-rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.8.2/christmas/Pyshell/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.8.2/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-03 02:25:27.000000 baysalt_christmas-0.1.8.2/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.8.2/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.8.2/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:31:54.859194 baysalt_christmas-0.1.8.2/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.2/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.2/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.8.2/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:31:54.860533 baysalt_christmas-0.1.8.2/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.8.2/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.2/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.2/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.8.2/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.8.2/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     9042 2023-06-28 02:50:13.000000 baysalt_christmas-0.1.8.2/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.8.2/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.8.2/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.8.2/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-04 08:31:54.861094 baysalt_christmas-0.1.8.2/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-04 08:31:53.000000 baysalt_christmas-0.1.8.2/setup.py
```

### Comparing `baysalt_christmas-0.1.8.1/.DS_Store` & `baysalt_christmas-0.1.8.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/PKG-INFO` & `baysalt_christmas-0.1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.8.1/README.md` & `baysalt_christmas-0.1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.8.2/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.8.1/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.8.2/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/Blogging.py` & `baysalt_christmas-0.1.8.2/christmas/Blogging.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/Pyshell/RS_File.py` & `baysalt_christmas-0.1.8.2/christmas/Pyshell/RS_File.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             _rekey = _al.strip(_char)
             if _rekey in _dict.keys():
                 vvalue = vvalue.replace(_al, _dict[_rekey])
                 _dict[kkey] = vvalue
     return _dict
 
 
-def read_source_sh(_Sfile, _logger=logger_RS):  # sourcery skip: low-code-quality
+def read_env_sh(_Sfile, _logger=logger_RS):  # sourcery skip: low-code-quality
     """
     读取bash.oneapi文件中的加载环境变量的行，并写入os.environ里，
     以 #, if, source开头的行不读取
     非export开头的行不加入os.environ
     """
     # 获取基本路径, 非export开头的行
     path_dict = {}
@@ -136,15 +136,15 @@
 
 def RS_file_os(_Sfile, _logger=logger_RS):
     """
     :param _Sfile: bash.oneapi文件的路径
     :param _logger: 日志记录器
     :return: None
     """
-    source_env_os(read_source_sh(_Sfile, _logger))
+    source_env_os(read_env_sh(_Sfile, _logger))
 
 
 def RS_example():
     """
     :return: None
     """
     _Sfile = r'D:\Graduate_1\new_grid\move_file\bash.oneapi'
```

### Comparing `baysalt_christmas-0.1.8.1/christmas/S_DateTime.py` & `baysalt_christmas-0.1.8.2/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/commonCode.py` & `baysalt_christmas-0.1.8.2/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/cprintf.py` & `baysalt_christmas-0.1.8.2/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.8.2/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.8.2/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.8.2/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.8.2/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/mncPy/common.py` & `baysalt_christmas-0.1.8.2/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.8.2/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/processBar.py` & `baysalt_christmas-0.1.8.2/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/read_conf.py` & `baysalt_christmas-0.1.8.2/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/christmas/server_info.py` & `baysalt_christmas-0.1.8.2/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.1/setup.py` & `baysalt_christmas-0.1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.8.1",
+    version="0.1.8.2",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

