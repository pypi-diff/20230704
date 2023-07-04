# Comparing `tmp/mailx-0.0.6.tar.gz` & `tmp/mailx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mailx-0.0.6.tar", last modified: Fri Apr 29 13:45:13 2022, max compression
+gzip compressed data, was "mailx-0.0.7.tar", last modified: Tue Jul  4 08:40:33 2023, max compression
```

## Comparing `mailx-0.0.6.tar` & `mailx-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2022-04-29 13:45:13.108994 mailx-0.0.6/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2022-03-20 07:33:29.000000 mailx-0.0.6/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1147 2022-04-29 13:45:13.108583 mailx-0.0.6/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      716 2022-03-21 04:11:22.000000 mailx-0.0.6/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2022-04-29 13:45:13.106008 mailx-0.0.6/mailx/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      204 2022-03-21 04:11:22.000000 mailx-0.0.6/mailx/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4825 2022-04-29 13:43:48.000000 mailx-0.0.6/mailx/mailx.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2022-04-29 13:45:13.108162 mailx-0.0.6/mailx.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1147 2022-04-29 13:45:13.000000 mailx-0.0.6/mailx.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      203 2022-04-29 13:45:13.000000 mailx-0.0.6/mailx.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2022-04-29 13:45:13.000000 mailx-0.0.6/mailx.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       12 2022-04-29 13:45:13.000000 mailx-0.0.6/mailx.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        6 2022-04-29 13:45:13.000000 mailx-0.0.6/mailx.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2022-04-29 13:45:13.109111 mailx-0.0.6/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      857 2022-04-29 13:43:48.000000 mailx-0.0.6/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-04 08:40:33.036955 mailx-0.0.7/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2023-07-04 08:38:31.000000 mailx-0.0.7/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1059 2023-07-04 08:40:33.036864 mailx-0.0.7/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      716 2023-07-04 08:38:31.000000 mailx-0.0.7/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-04 08:40:33.036123 mailx-0.0.7/mailx/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      204 2023-07-04 08:38:31.000000 mailx-0.0.7/mailx/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4825 2023-07-04 08:38:31.000000 mailx-0.0.7/mailx/mailx.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-04 08:40:33.036730 mailx-0.0.7/mailx.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1059 2023-07-04 08:40:33.000000 mailx-0.0.7/mailx.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      203 2023-07-04 08:40:33.000000 mailx-0.0.7/mailx.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-04 08:40:33.000000 mailx-0.0.7/mailx.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       12 2023-07-04 08:40:33.000000 mailx-0.0.7/mailx.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        6 2023-07-04 08:40:33.000000 mailx-0.0.7/mailx.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-04 08:40:33.036992 mailx-0.0.7/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      859 2023-07-04 08:39:54.000000 mailx-0.0.7/setup.py
```

### Comparing `mailx-0.0.6/LICENSE` & `mailx-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mailx-0.0.6/PKG-INFO` & `mailx-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: mailx
-Version: 0.0.6
+Version: 0.0.7
 Summary: make it easy to use mail
 Home-page: https://gitee.com/ZeroSeeker/mailx
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mailx
 
 #### 介绍
@@ -49,9 +46,7 @@
 smtp_port={your smtp_port}
 from_name={your from_name}
 smtp_username={your smtp_username}
 smtp_password={your_smtp_username}
 to_addrs={your smtp_username, split by ","}
 ```
 - SMTP服务端口号：25或80或465(SSL加密)
-
-
```

### Comparing `mailx-0.0.6/README.md` & `mailx-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mailx-0.0.6/mailx/mailx.py` & `mailx-0.0.7/mailx/mailx.py`

 * *Files identical despite different names*

### Comparing `mailx-0.0.6/mailx.egg-info/PKG-INFO` & `mailx-0.0.7/mailx.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: mailx
-Version: 0.0.6
+Version: 0.0.7
 Summary: make it easy to use mail
 Home-page: https://gitee.com/ZeroSeeker/mailx
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mailx
 
 #### 介绍
@@ -49,9 +46,7 @@
 smtp_port={your smtp_port}
 from_name={your from_name}
 smtp_username={your smtp_username}
 smtp_password={your_smtp_username}
 to_addrs={your smtp_username, split by ","}
 ```
 - SMTP服务端口号：25或80或465(SSL加密)
-
-
```

### Comparing `mailx-0.0.6/setup.py` & `mailx-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mailx",
-    version="0.0.6",
+    version="0.0.7",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use mail",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/mailx",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        # "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'envx==0.0.5',
+        'envx>=1.0.1',
     ]
 )
```

