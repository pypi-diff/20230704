# Comparing `tmp/pyowletapi-2023.7.1.tar.gz` & `tmp/pyowletapi-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyowletapi-2023.7.1.tar", last modified: Mon Jul  3 13:35:46 2023, max compression
+gzip compressed data, was "pyowletapi-2023.7.2.tar", last modified: Tue Jul  4 14:18:47 2023, max compression
```

## Comparing `pyowletapi-2023.7.1.tar` & `pyowletapi-2023.7.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 13:35:46.285499 pyowletapi-2023.7.1/
--rw-rw-rw-   0        0        0     1869 2023-07-03 13:35:46.286498 pyowletapi-2023.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     1496 2023-05-09 08:51:20.000000 pyowletapi-2023.7.1/README.md
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-07-03 13:35:46.288498 pyowletapi-2023.7.1/setup.cfg
--rw-rw-rw-   0        0        0      819 2023-07-03 13:35:33.000000 pyowletapi-2023.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:35:46.190511 pyowletapi-2023.7.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 13:35:46.250498 pyowletapi-2023.7.1/src/pyowletapi/
--rw-rw-rw-   0        0        0       17 2023-05-02 10:29:46.000000 pyowletapi-2023.7.1/src/pyowletapi/__init__.py
--rw-rw-rw-   0        0        0    18256 2023-05-26 13:48:59.000000 pyowletapi-2023.7.1/src/pyowletapi/api.py
--rw-rw-rw-   0        0        0     2507 2023-07-03 09:18:19.000000 pyowletapi-2023.7.1/src/pyowletapi/const.py
--rw-rw-rw-   0        0        0      636 2023-05-26 13:37:20.000000 pyowletapi-2023.7.1/src/pyowletapi/exceptions.py
--rw-rw-rw-   0        0        0     4306 2023-05-09 08:46:26.000000 pyowletapi-2023.7.1/src/pyowletapi/owlet.py
--rw-rw-rw-   0        0        0     7388 2023-05-25 15:44:47.000000 pyowletapi-2023.7.1/src/pyowletapi/sock.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:35:46.283498 pyowletapi-2023.7.1/src/pyowletapi.egg-info/
--rw-rw-rw-   0        0        0     1869 2023-07-03 13:35:46.000000 pyowletapi-2023.7.1/src/pyowletapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-03 13:35:46.000000 pyowletapi-2023.7.1/src/pyowletapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 13:35:46.000000 pyowletapi-2023.7.1/src/pyowletapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 13:35:46.000000 pyowletapi-2023.7.1/src/pyowletapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-03 13:35:46.000000 pyowletapi-2023.7.1/src/pyowletapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 14:18:47.982435 pyowletapi-2023.7.2/
+-rw-rw-rw-   0        0        0     1982 2023-07-04 14:18:47.982435 pyowletapi-2023.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1609 2023-07-04 14:08:58.000000 pyowletapi-2023.7.2/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-04 14:18:47.985439 pyowletapi-2023.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-07-04 14:18:13.000000 pyowletapi-2023.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:18:47.917436 pyowletapi-2023.7.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 14:18:47.940439 pyowletapi-2023.7.2/src/pyowletapi/
+-rw-rw-rw-   0        0        0       17 2023-05-02 10:29:46.000000 pyowletapi-2023.7.2/src/pyowletapi/__init__.py
+-rw-rw-rw-   0        0        0    18255 2023-07-03 15:45:42.000000 pyowletapi-2023.7.2/src/pyowletapi/api.py
+-rw-rw-rw-   0        0        0     2464 2023-07-04 14:06:51.000000 pyowletapi-2023.7.2/src/pyowletapi/const.py
+-rw-rw-rw-   0        0        0      636 2023-05-26 13:37:20.000000 pyowletapi-2023.7.2/src/pyowletapi/exceptions.py
+-rw-rw-rw-   0        0        0     7493 2023-07-04 13:57:59.000000 pyowletapi-2023.7.2/src/pyowletapi/sock.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:18:47.980436 pyowletapi-2023.7.2/src/pyowletapi.egg-info/
+-rw-rw-rw-   0        0        0     1982 2023-07-04 14:18:47.000000 pyowletapi-2023.7.2/src/pyowletapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-04 14:18:47.000000 pyowletapi-2023.7.2/src/pyowletapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 14:18:47.000000 pyowletapi-2023.7.2/src/pyowletapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 14:18:47.000000 pyowletapi-2023.7.2/src/pyowletapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-04 14:18:47.000000 pyowletapi-2023.7.2/src/pyowletapi.egg-info/top_level.txt
```

### Comparing `pyowletapi-2023.7.1/PKG-INFO` & `pyowletapi-2023.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Owlet baby montior API wrapper
-Home-page: https://github.com/RyanClark123/pyowletapi
+Home-page: https://github.com/ryanbdclark/pyowletapi
 Author: Ryan Clark
 Keywords: owlet,api,baby
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Introduction
 
 First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
 
@@ -56,8 +56,8 @@
 socks = {device['device']['dsn']: Sock(api, device['device']) for device in devices}
 ```
 
 to get current reading from sock call the update_properties function on each sock object
 ```python
 device.update_properties()
 ```
-This will return a tuple, the first element being the raw response as a dict and the second element is a more cut down dict version of the response showing only the most relevant data.
+This will return a dictionary, the key 'raw_properties' contains the raw response as a dict and the 'properties' key is a more cut down dict version of the response showing only the most relevant data and the 'tokens' key will return a dictionary if the api tokens have changed since the last call
```

### Comparing `pyowletapi-2023.7.1/README.md` & `pyowletapi-2023.7.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 socks = {device['device']['dsn']: Sock(api, device['device']) for device in devices}
 ```
 
 to get current reading from sock call the update_properties function on each sock object
 ```python
 device.update_properties()
 ```
-This will return a tuple, the first element being the raw response as a dict and the second element is a more cut down dict version of the response showing only the most relevant data.
+This will return a dictionary, the key 'raw_properties' contains the raw response as a dict and the 'properties' key is a more cut down dict version of the response showing only the most relevant data and the 'tokens' key will return a dictionary if the api tokens have changed since the last call
```

### Comparing `pyowletapi-2023.7.1/setup.py` & `pyowletapi-2023.7.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="pyowletapi",
-    version="2023.07.01",
+    version="2023.7.2",
     description="Owlet baby montior API wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/RyanClark123/pyowletapi",
+    url="https://github.com/ryanbdclark/pyowletapi",
     author="Ryan Clark",
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     keywords="owlet, api, baby",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.10",
     install_requires=["aiohttp"],
 )
```

### Comparing `pyowletapi-2023.7.1/src/pyowletapi/api.py` & `pyowletapi-2023.7.2/src/pyowletapi/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,19 +101,19 @@
         self._refresh: str = refresh
         self._tokens_changed: bool = False
         self._has_authenticated: bool = False
         self.session = session
         self.headers = {}
         self.devices = {}
 
-        self._api_url = REGION_INFO[self._region]["url_base"]
-
         if self._region not in ["europe", "world"]:
             raise OwletAuthenticationError("Supplied region not valid")
 
+        self._api_url = REGION_INFO[self._region]["url_base"]
+
         if self.session is None:
             self.session = aiohttp.ClientSession()
 
     @property
     def tokens(self) -> TokenDict:
         """Returns a TokenDict object with current auth token, expiry and refresh token"""
         return {
@@ -280,15 +280,15 @@
                     "X-Android-Cert": "2A3BC26DB0B8B0792DBE28E6FFDC2598F9B12B74",
                 },
             ) as response:
                 response_json = await response.json()
 
                 if response.status != 200:
                     match response.status:
-                        case 401:
+                        case 400:
                             raise OwletAuthenticationError("Refresh token not valid")
                         case _:
                             raise OwletError("Generic refresh error, contact dev")
 
                 self._refresh = response_json["refresh_token"]
 
                 mini_token = await self.get_mini_token(response_json["id_token"])
@@ -305,15 +305,15 @@
         Returns
         -------
         None: if auth_token and expiry in object are ok then returns none
         dict: If auth token generated then dict with the new token returned
         """
         if self._auth_token is None and self._refresh is None:
             if self._user is None or self._password is None:
-                return OwletAuthenticationError("Username or password not supplied")
+                raise OwletAuthenticationError("Username or password not supplied")
 
             await self.password_verification()
 
         if self._auth_token is None or self._expiry <= time.time():
             return await self.refresh_authentication()
 
         self.headers["Authorization"] = "auth_token " + self._auth_token
```

### Comparing `pyowletapi-2023.7.1/src/pyowletapi/const.py` & `pyowletapi-2023.7.2/src/pyowletapi/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,39 +10,42 @@
         "lost_power_alert": "LOST_POWER_ALRT",
         "sock_disconnected": "SOCK_DISCON_ALRT",
         "sock_off": "SOCK_OFF",
     }
 }
 
 VITALS = {
-    # Additional attributes not implemented
-    # Current alerts mask - "alrt" int
-    # Firmware update status - "ota" int
-    # Sock readings flag - "srf" int
-    # Soft brick status - "sb" int
-    # Movement bucket - "mvb" int
-    # Wellness alert - "onm" int
-    # Hardware version - "hw" String
-    # Monitoring start time - "mst" int
-    # Base station battery status - "bsb" int
     float: {
         "oxygen_saturation": "ox",
         "heart_rate": "hr",
         "battery_percentage": "bat",
         "battery_minutes": "btt",
         "signal_strength": "rsi",
         "oxygen_10_av": "oxta",
     },
     bool: {
-        "moving": "mv",
+        "base_station_on": "bso",
+    },
+    int: {
+        "sock_connection": "sc",
+        "skin_temperature": "st",
+        "sleep_state": "ss",
+        "movement": "mv",
+        "movement_bucket": "mvb",
         "alert_paused_status": "aps",
         "charging": "chg",
-        "base_station_on": "bso",
+        "alerts_mask": "alrt",
+        "update_status": "ota",
+        "readings_flag": "srf",
+        "brick_status": "sb",
+        "wellness_alert": "onm",
+        "monitoring_start_time": "mst",
+        "base_battery_status": "bsb",
     },
-    int: {"sock_connection": "sc", "skin_temperature": "st", "sleep_state": "ss"},
+    str: {"hardware_version": "hw"},
     "other": {"last_updated": "data_updated_at"},
 }
 
 REGION_INFO = {
     "world": {
         "url_mini": "https://ayla-sso.owletdata.com/mini/",
         "url_signin": "https://user-field-1a2039d9.aylanetworks.com/api/v1/token_sign_in",
```

### Comparing `pyowletapi-2023.7.1/src/pyowletapi/exceptions.py` & `pyowletapi-2023.7.2/src/pyowletapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyowletapi-2023.7.1/src/pyowletapi/sock.py` & `pyowletapi-2023.7.2/src/pyowletapi/sock.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 class PropertiesDict(TypedDict):
     raw_properties: dict
     properties: dict
     tokens: Union[None, TokenDict]
 
+
 class Sock:
     """
     Class representing a Owlet sock device
 
     Attributes
     ----------
     name : str
@@ -175,28 +176,30 @@
                 key: type(self._raw_properties[property]["value"])
                 for key, property in properties_tmp.items()
             }
 
         if self._version == 3:
             vitals = json.loads(self._raw_properties["REAL_TIME_VITALS"]["value"])
 
-            for type, vitals_tmp in VITALS.items():
-                for key, property in vitals_tmp.items():
-                    match key:
+            for type, vitals_list in VITALS.items():
+                for vital_desc, vital_key in vitals_list.items():
+                    match vital_desc:
                         case "base_station_on":
-                            properties[key] = bool(vitals["bso"]) or bool(vitals["chg"])
+                            properties[vital_desc] = bool(vitals["bso"]) or bool(
+                                vitals["chg"]
+                            )
                         case "last_updated":
-                            properties[key] = datetime.datetime.strptime(
+                            properties[vital_desc] = datetime.datetime.strptime(
                                 self._raw_properties["REAL_TIME_VITALS"][
                                     "data_updated_at"
                                 ],
                                 "%Y-%m-%dT%H:%M:%SZ",
                             ).strftime("%Y/%m/%d %H:%M:%S")
                         case _:
-                            properties[key] = type(vitals[property])
+                            properties[vital_desc] = type(vitals[vital_key])
 
         return properties
 
     async def _check_version(self) -> None:
         version = 0
         if "REAL_TIME_VITALS" in self._raw_properties:
             version = 3
```

### Comparing `pyowletapi-2023.7.1/src/pyowletapi.egg-info/PKG-INFO` & `pyowletapi-2023.7.2/src/pyowletapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Owlet baby montior API wrapper
-Home-page: https://github.com/RyanClark123/pyowletapi
+Home-page: https://github.com/ryanbdclark/pyowletapi
 Author: Ryan Clark
 Keywords: owlet,api,baby
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Introduction
 
 First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
 
@@ -56,8 +56,8 @@
 socks = {device['device']['dsn']: Sock(api, device['device']) for device in devices}
 ```
 
 to get current reading from sock call the update_properties function on each sock object
 ```python
 device.update_properties()
 ```
-This will return a tuple, the first element being the raw response as a dict and the second element is a more cut down dict version of the response showing only the most relevant data.
+This will return a dictionary, the key 'raw_properties' contains the raw response as a dict and the 'properties' key is a more cut down dict version of the response showing only the most relevant data and the 'tokens' key will return a dictionary if the api tokens have changed since the last call
```

