# Comparing `tmp/bohrium-sdk-0.2.3.tar.gz` & `tmp/bohrium-sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.2.3.tar", last modified: Sun Jun 25 03:32:34 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.3.0.tar", last modified: Tue Jul  4 08:46:59 2023, max compression
```

## Comparing `bohrium-sdk-0.2.3.tar` & `bohrium-sdk-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-25 03:32:34.274164 bohrium-sdk-0.2.3/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-25 03:32:34.273884 bohrium-sdk-0.2.3/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.2.3/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-25 03:32:34.261433 bohrium-sdk-0.2.3/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-25 03:32:34.000000 bohrium-sdk-0.2.3/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      444 2023-06-25 03:32:34.000000 bohrium-sdk-0.2.3/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-25 03:32:34.000000 bohrium-sdk-0.2.3/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-25 03:32:34.000000 bohrium-sdk-0.2.3/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-25 03:32:34.272144 bohrium-sdk-0.2.3/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.2.3/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.2.3/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     7164 2023-06-15 01:18:06.000000 bohrium-sdk-0.2.3/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-08 02:50:49.000000 bohrium-sdk-0.2.3/bohriumsdk/database.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-12 09:26:10.000000 bohrium-sdk-0.2.3/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4121 2023-06-14 13:34:07.000000 bohrium-sdk-0.2.3/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.2.3/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-12 09:26:00.000000 bohrium-sdk-0.2.3/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     8511 2023-06-15 00:55:51.000000 bohrium-sdk-0.2.3/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-25 03:32:34.273276 bohrium-sdk-0.2.3/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.2.3/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.2.3/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4649 2023-06-25 03:27:49.000000 bohrium-sdk-0.2.3/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-07 01:28:13.000000 bohrium-sdk-0.2.3/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-25 03:32:34.274288 bohrium-sdk-0.2.3/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      366 2023-06-25 03:31:44.000000 bohrium-sdk-0.2.3/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 08:46:59.495921 bohrium-sdk-0.3.0/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-07-04 08:46:59.495668 bohrium-sdk-0.3.0/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 08:46:59.490716 bohrium-sdk-0.3.0/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-07-04 08:46:59.000000 bohrium-sdk-0.3.0/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      444 2023-07-04 08:46:59.000000 bohrium-sdk-0.3.0/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-07-04 08:46:59.000000 bohrium-sdk-0.3.0/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-07-04 08:46:59.000000 bohrium-sdk-0.3.0/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 08:46:59.494688 bohrium-sdk-0.3.0/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     7031 2023-07-04 03:12:10.000000 bohrium-sdk-0.3.0/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/database.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4121 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     8428 2023-07-04 03:26:27.000000 bohrium-sdk-0.3.0/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 08:46:59.495379 bohrium-sdk-0.3.0/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4649 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-07-04 08:46:59.495970 bohrium-sdk-0.3.0/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      366 2023-07-04 08:46:38.000000 bohrium-sdk-0.3.0/setup.py
```

### Comparing `bohrium-sdk-0.2.3/bohriumsdk/client.py` & `bohrium-sdk-0.3.0/bohriumsdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,29 +44,26 @@
                 self.config['password'] = password
                 self.base_url = base_url_v1
             if token is not None:
                 self.token = token
             else:
                 self._login()
         elif api_version == "v2":
-            self.env = os.getenv("ENV", "prod")
-
+            self.openapi_host = os.getenv("OPENAPI_HOST", "https://openapi.dp.tech")
             self.config_file_location_expand = os.path.expanduser(config_file_location_v2)
             if not os.path.exists(self.config_file_location_expand):
-                print("Config File ~/.brmconfig not found! Please visit https://bohrium.dp.tech/personal/setting and click AccessKey create button to generate it !")
+                weburl = self.openapi_host.replace("openapi", "bohrium")
+                print(f"Config File ~/.brmconfig not found! Please visit {weburl}/personal/setting and click AccessKey create button to generate it !")
                 self.access_key = input("Please enter AccessKey: ")
-                if self.env == "test":
-                    data = f"[Credentials]\nbaseUrl=https://openapi.test.dp.tech\naccessKey={self.access_key}"
-                else:
-                    data = f"[Credentials]\nbaseUrl=https://openapi.dp.tech\naccessKey={self.access_key}"
+                data = f"[Credentials]\naccessKey={self.access_key}"
                 with open(self.config_file_location_expand, 'w') as f:
                     f.write(data)
             config = configparser.ConfigParser()
             config.read(self.config_file_location_expand)
-            self.base_url = config.get('Credentials', 'baseUrl')
+            self.base_url = self.openapi_host
             self.access_key = config.get('Credentials', 'accessKey')
             self.params = {"accessKey": self.access_key}
             self.token = ""
             self.check_ak()
             
 
     def post(self, url, host="", json=None, data=None, headers=None, params=None, stream=False, retry=5):
```

### Comparing `bohrium-sdk-0.2.3/bohriumsdk/database.py` & `bohrium-sdk-0.3.0/bohriumsdk/database.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.3/bohriumsdk/image.py` & `bohrium-sdk-0.3.0/bohriumsdk/image.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.3/bohriumsdk/job.py` & `bohrium-sdk-0.3.0/bohriumsdk/job.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.3/bohriumsdk/node.py` & `bohrium-sdk-0.3.0/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.3/bohriumsdk/project.py` & `bohrium-sdk-0.3.0/bohriumsdk/project.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.3/bohriumsdk/storage.py` & `bohrium-sdk-0.3.0/bohriumsdk/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,15 @@
     def __init__(
             self,
             base_url: str = "https://openapi.dp.tech",
             client: Client = None,
         ) -> None:
         
         self.base_url = base_url
-        if client.env == "test":
-            self.host = "https://tiefblue.test.dp.tech"
-        else:
-            self.host = "https://tiefblue.dp.tech"
+        self.host = client.openapi_host.replace("openapi", "tiefblue")
         self.client = client
 
     
     def encode_base64(
             self, 
             parameter: dict = {}
         ) -> str:
```

### Comparing `bohrium-sdk-0.2.3/bohriumsdk/test.py` & `bohrium-sdk-0.3.0/bohriumsdk/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,11 +154,11 @@
     c = Client()
     prompt = "你好"
     res = c.chat(prompt)
     print(res)
 
 
 if __name__ == "__main__":
-    test_chat()
-    # test_job_detail()
+    # test_chat()
+    test_job_detail()
     # test_base64()
     # test_db()
```

### Comparing `bohrium-sdk-0.2.3/bohriumsdk/util.py` & `bohrium-sdk-0.3.0/bohriumsdk/util.py`

 * *Files identical despite different names*

