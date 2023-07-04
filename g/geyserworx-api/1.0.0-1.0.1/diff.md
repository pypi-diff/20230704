# Comparing `tmp/geyserworx_api-1.0.0.tar.gz` & `tmp/geyserworx_api-1.0.1.tar.gz`

## Comparing `geyserworx_api-1.0.0.tar` & `geyserworx_api-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 geyserworx_api-1.0.0/src/geyserworx_api/__init__.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 geyserworx_api-1.0.0/src/geyserworx_api/geyserworx_api.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geyserworx_api-1.0.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 geyserworx_api-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geyserworx_api-1.0.0/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 geyserworx_api-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 geyserworx_api-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/src/geyserworx_api/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/src/geyserworx_api/geyserworx_api.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/PKG-INFO
```

### Comparing `geyserworx_api-1.0.0/src/geyserworx_api/geyserworx_api.py` & `geyserworx_api-1.0.1/src/geyserworx_api/geyserworx_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 class TemperatureType(Enum):
     AC = 'ACT'
     AC_BOOST = 'ACOT'
     PV = 'PVT'
 
 
 class GeyserworxAPI:
-    __API_BASE__ = 'gwa/'
+    __API_BASE__ = 'gwa'
     __TOPIC_BASE_GET__ = 'GWA'
     __TOPIC_BASE_SET__ = 'GWR'
 
     def __init__(
             self,
             session: ClientSession,
             geyser_serial_number: str,
             geyser_number: int = 1,
             base_url: str = "http://192.168.4.1"
     ):
         self.geyser_serial_number = geyser_serial_number
         self.geyser_number = geyser_number
-        self.base_url_get = f'{base_url}{self.__API_BASE__}?topic={self.__TOPIC_BASE_GET__}/{self.geyser_serial_number}/{self.geyser_number}/'
-        self.base_url_set = f'{base_url}{self.__API_BASE__}?topic={self.__TOPIC_BASE_SET__}/{self.geyser_serial_number}/{self.geyser_number}/'
+        self.base_url_get = f'{base_url}/{self.__API_BASE__}?topic={self.__TOPIC_BASE_GET__}/{self.geyser_serial_number}/{self.geyser_number}/'
+        self.base_url_set = f'{base_url}/{self.__API_BASE__}?topic={self.__TOPIC_BASE_SET__}/{self.geyser_serial_number}/{self.geyser_number}/'
         self.session = session
 
     async def get_current_temperature(self) -> float:
         url = f'{self.base_url_get}A'
         response = await self.session.get(url)
         response_json: dict = await response.json()
         return response_json['T']['G']
```

### Comparing `geyserworx_api-1.0.0/LICENSE` & `geyserworx_api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geyserworx_api-1.0.0/pyproject.toml` & `geyserworx_api-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geyserworx_api"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Dovi Joel", email="dovi@debuggingmadejoyful.tech" },
 ]
 description = "An SDK interface to read and set Geyserworx geysers without using the app."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `geyserworx_api-1.0.0/PKG-INFO` & `geyserworx_api-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geyserworx_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: An SDK interface to read and set Geyserworx geysers without using the app.
 Project-URL: Homepage, https://github.com/dovijoel/GeyserworxAPI
 Project-URL: Bug Tracker, https://github.com/dovijoel/GeyserworxAPI/issues
 Author-email: Dovi Joel <dovi@debuggingmadejoyful.tech>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

