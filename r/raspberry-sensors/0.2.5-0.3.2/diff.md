# Comparing `tmp/raspberry-sensors-0.2.5.tar.gz` & `tmp/raspberry-sensors-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberry-sensors-0.2.5.tar", last modified: Sat Jul  1 18:34:28 2023, max compression
+gzip compressed data, was "raspberry-sensors-0.3.2.tar", last modified: Tue Jul  4 14:46:37 2023, max compression
```

## Comparing `raspberry-sensors-0.2.5.tar` & `raspberry-sensors-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 18:34:28.617002 raspberry-sensors-0.2.5/
--rw-rw-rw-   0        0        0     1091 2023-06-28 10:47:29.000000 raspberry-sensors-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     1787 2023-07-01 18:34:28.617002 raspberry-sensors-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1362 2023-07-01 18:34:08.000000 raspberry-sensors-0.2.5/README.md
--rw-rw-rw-   0        0        0      501 2023-07-01 18:34:14.000000 raspberry-sensors-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 18:34:28.617002 raspberry-sensors-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 18:34:28.586895 raspberry-sensors-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 18:34:28.596843 raspberry-sensors-0.2.5/src/raspberry-sensors/
--rw-rw-rw-   0        0        0        0 2023-06-28 10:37:28.000000 raspberry-sensors-0.2.5/src/raspberry-sensors/__init__.py
--rw-rw-rw-   0        0        0     3315 2023-06-28 10:26:16.000000 raspberry-sensors-0.2.5/src/raspberry-sensors/sensors.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:34:28.608452 raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/
--rw-rw-rw-   0        0        0     1787 2023-07-01 18:34:28.000000 raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-07-01 18:34:28.000000 raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 18:34:28.000000 raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-01 18:34:28.000000 raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-01 18:34:28.608452 raspberry-sensors-0.2.5/src/raspberry_sensors_Develper/
--rw-rw-rw-   0        0        0     3400 2023-07-01 18:27:02.000000 raspberry-sensors-0.2.5/src/raspberry_sensors_Develper/sensors.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:46:37.114729 raspberry-sensors-0.3.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-28 10:47:29.000000 raspberry-sensors-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1787 2023-07-04 14:46:37.113590 raspberry-sensors-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1362 2023-07-01 18:34:08.000000 raspberry-sensors-0.3.2/README.md
+-rw-rw-rw-   0        0        0      501 2023-07-04 12:43:15.000000 raspberry-sensors-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 14:46:37.114729 raspberry-sensors-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 14:46:37.078592 raspberry-sensors-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 14:46:37.095686 raspberry-sensors-0.3.2/src/raspberry-sensors/
+-rw-rw-rw-   0        0        0        0 2023-06-28 10:37:28.000000 raspberry-sensors-0.3.2/src/raspberry-sensors/__init__.py
+-rw-rw-rw-   0        0        0     3820 2023-07-04 12:18:45.000000 raspberry-sensors-0.3.2/src/raspberry-sensors/sensors.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:46:37.108375 raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/
+-rw-rw-rw-   0        0        0     1787 2023-07-04 14:46:37.000000 raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-04 14:46:37.000000 raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 14:46:37.000000 raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-04 14:46:37.000000 raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/top_level.txt
```

### Comparing `raspberry-sensors-0.2.5/LICENSE` & `raspberry-sensors-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.2.5/PKG-INFO` & `raspberry-sensors-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberry-sensors
-Version: 0.2.5
+Version: 0.3.2
 Summary: This package for getting values from sensors mh_z19, DHT, ads1015
 Author-email: Develper <testerlzt@mail.ru>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `raspberry-sensors-0.2.5/README.md` & `raspberry-sensors-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.2.5/src/raspberry-sensors/sensors.py` & `raspberry-sensors-0.3.2/src/raspberry-sensors/sensors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-import busio, board
+try:
+    import busio, board
+except:
+    raise Exception("[raspberry_sensors] No standard modules 'busio', 'board'")
 
 dht, ads, mhz = 0, 0, 0
 try:
     from Adafruit_DHT import DHT22, DHT11, read
 except:
     dht = 1
-    print("DHT not available, library 'Adafruit-DHT' not installed")
+    print("[raspberry_sensors] DHT not available, library 'Adafruit-DHT' not installed")
 try:
     from adafruit_ads1x15 import analog_in, ads1015
 except:
     ads = 1
-    print("ADS not available, library 'adafruit_ads1x15' not installed")
+    print("[raspberry_sensors] ADS not available, library 'adafruit-circuitpython-ads1x15' not installed")
 try:
     from mh_z19 import read_from_pwm, read as mhz_read
 except:
     mhz = 1
-    print("MHZ19 not available, library 'mh_z19' not installed")
+    print("[raspberry_sensors] MHZ19 not available, library 'mh-z19' not installed")
 
 
 class Sensors:
     def __init__(self, loging_error=True):
         global ads
         self.loging_error = loging_error
         self.cache = {"humidity": 0.0, "temperature": 0.0, "chanels": [-0, -0, -0, -0], "co2": 0}
@@ -31,58 +34,66 @@
                 analog_in.AnalogIn(self.ads, 1),
                 analog_in.AnalogIn(self.ads, 2),
                 analog_in.AnalogIn(self.ads, 3)
             ]
         except Exception as ex:
             ads = 1
             if self.loging_error:
-                print(f"ADS init error -> {ex}")
+                self.logs(f"ADS init error -> {ex}", "e")
 
-    def get_dht(self, _type=22, pin=4):
+    def logs(self, text, _type="l"):
+        color = "\033[1m"
+        if _type == "w":
+            color = "\033[43m"
+        elif _type == "e":
+            color = "\033[41m"
+        print(f"[\033[30mraspberry_sensors\033[0m]{color}{text}\033[0m")
+
+    def get_dht(self, _type=22, gpio=4):
         if dht:
             if self.loging_error:
-                print("DHT not available")
+                self.logs("DHT not available")
             return {"humidity": self.cache["humidity"], "temperature": self.cache["temperature"]}
         try:
-            h, t = read(DHT22 if _type==22 else DHT11, pin)
+            h, t = read(DHT22 if _type==22 else DHT11, gpio)
             if h and t:
                 self.cache["humidity"], self.cache["temperature"] = round(h, 2), round(t, 2)
             else:
                 if self.loging_error:
-                    print(f"DHT error, used cache")
+                    self.logs(f"DHT error, used cache", "w")
         except Exception as ex:
             if self.loging_error:
-                print(f"DHT error ({ex}), used cache")
+                self.logs(f"DHT error ({ex}), used cache", "w")
         return {"humidity": self.cache["humidity"], "temperature": self.cache["temperature"]}
 
+    def get_mhz(self, gpio=12, pwm=False, _range=5000):
+        if mhz:
+            if self.loging_error:
+                self.logs("MHZ19 not available")
+            return self.cache["co2"]
+        try:
+            if pwm:
+                self.cache["co2"] = read_from_pwm(gpio=gpio, range=_range)["co2"]
+            else:
+                self.cache["co2"] = mhz_read()["co2"]
+        except Exception as ex:
+            if self.loging_error:
+                self.logs(f"MHZ19 error ({ex}), used cache", "w")
+        return {"co2": self.cache["co2"]}
+
     def get_ads(self, chanel, interpolate=False, interpolate_min=0, interpolate_max=0):
         if ads:
             if self.loging_error:
-                print("ADS not available")
+                self.logs("ADS not available")
             return 0.0
         if chanel > 3 or chanel < 0:
             if self.loging_error:
-                print("The wrong channel is selected, only 0, 1, 2, 3 can be used\nUse chanel 0")
+                self.logs("The wrong channel is selected, only 0, 1, 2, 3 can be used\nUse chanel 0")
             chanel = 0
         try:
             self.cache["chanels"][chanel] = self.ads_chanels[chanel].voltage
         except Exception as ex:
             if self.loging_error:
-                print(f"ADS error ({ex}), used cache")
+                self.logs(f"ADS error ({ex}), used cache", "w")
         if interpolate:
             return round(interpolate_min+(interpolate_max-interpolate_min)*(self.cache["chanels"][chanel]/5),2)
-        return self.cache["chanels"][chanel]
-
-    def get_mhz(self, gpio=12, pwm=False, _range=5000):
-        if mhz:
-            if self.loging_error:
-                print("MHZ19 not available")
-            return self.cache["co2"]
-        try:
-            if pwm:
-                self.cache["co2"] = read_from_pwm(gpio=gpio, range=_range)["co2"]
-            else:
-                self.cache["co2"] = mhz_read()["co2"]
-        except Exception as ex:
-            if self.loging_error:
-                print(f"MHZ19 error ({ex}), used cache")
-        return self.cache["co2"]
+        return self.cache["chanels"][chanel]
```

### Comparing `raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/PKG-INFO` & `raspberry-sensors-0.3.2/src/raspberry_sensors.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberry-sensors
-Version: 0.2.5
+Version: 0.3.2
 Summary: This package for getting values from sensors mh_z19, DHT, ads1015
 Author-email: Develper <testerlzt@mail.ru>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

