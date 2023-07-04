# Comparing `tmp/hayloft-0.4.0a0.tar.gz` & `tmp/hayloft-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.4.0a0.tar", max compression
+gzip compressed data, was "hayloft-0.4.1.tar", max compression
```

## Comparing `hayloft-0.4.0a0.tar` & `hayloft-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.4.0a0/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.4.0a0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.4.0a0/hayloft/__init__.py
--rw-r--r--   0        0        0     5048 2023-07-03 08:43:15.676287 hayloft-0.4.0a0/hayloft/app.py
--rw-r--r--   0        0        0     1660 2023-07-03 08:42:36.775929 hayloft-0.4.0a0/hayloft/llama_index.py
--rw-r--r--   0        0        0      922 2023-07-02 09:44:38.522358 hayloft-0.4.0a0/hayloft/logger.py
--rw-r--r--   0        0        0    28209 2023-07-03 08:44:28.656963 hayloft-0.4.0a0/hayloft/public/assets/index-883c7b1f.css
--rw-r--r--   0        0        0   184324 2023-07-03 08:44:28.656963 hayloft-0.4.0a0/hayloft/public/assets/index-889253f9.js
--rw-r--r--   0        0        0      384 2023-07-03 08:44:28.656963 hayloft-0.4.0a0/hayloft/public/index.html
--rw-r--r--   0        0        0      575 2023-06-26 15:43:07.772960 hayloft-0.4.0a0/hayloft/schema.py
--rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.4.0a0/hayloft/sse.py
--rw-r--r--   0        0        0      573 2023-07-03 08:45:50.574393 hayloft-0.4.0a0/pyproject.toml
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 hayloft-0.4.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2275 2023-07-04 09:48:24.845305 hayloft-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.4.1/hayloft/__init__.py
+-rw-r--r--   0        0        0     5048 2023-07-03 09:02:58.696438 hayloft-0.4.1/hayloft/app.py
+-rw-r--r--   0        0        0     1660 2023-07-03 09:02:58.696438 hayloft-0.4.1/hayloft/llama_index.py
+-rw-r--r--   0        0        0      922 2023-07-03 09:02:58.696438 hayloft-0.4.1/hayloft/logger.py
+-rw-r--r--   0        0        0    28209 2023-07-03 09:02:58.696438 hayloft-0.4.1/hayloft/public/assets/index-883c7b1f.css
+-rw-r--r--   0        0        0   184324 2023-07-03 09:02:58.699772 hayloft-0.4.1/hayloft/public/assets/index-889253f9.js
+-rw-r--r--   0        0        0      384 2023-07-03 09:02:58.699772 hayloft-0.4.1/hayloft/public/index.html
+-rw-r--r--   0        0        0      575 2023-06-26 15:43:07.772960 hayloft-0.4.1/hayloft/schema.py
+-rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.4.1/hayloft/sse.py
+-rw-r--r--   0        0        0      579 2023-07-04 09:54:32.844157 hayloft-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3174 1970-01-01 00:00:00.000000 hayloft-0.4.1/PKG-INFO
```

### Comparing `hayloft-0.4.0a0/LICENSE` & `hayloft-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0a0/hayloft/app.py` & `hayloft-0.4.1/hayloft/app.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0a0/hayloft/llama_index.py` & `hayloft-0.4.1/hayloft/llama_index.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0a0/hayloft/logger.py` & `hayloft-0.4.1/hayloft/logger.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0a0/hayloft/public/assets/index-883c7b1f.css` & `hayloft-0.4.1/hayloft/public/assets/index-883c7b1f.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0a0/hayloft/public/assets/index-889253f9.js` & `hayloft-0.4.1/hayloft/public/assets/index-889253f9.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0a0/hayloft/schema.py` & `hayloft-0.4.1/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0a0/hayloft/sse.py` & `hayloft-0.4.1/hayloft/sse.py`

 * *Files identical despite different names*

