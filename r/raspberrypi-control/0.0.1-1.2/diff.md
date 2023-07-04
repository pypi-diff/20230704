# Comparing `tmp/raspberrypi_control-0.0.1.tar.gz` & `tmp/raspberrypi_control-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberrypi_control-0.0.1.tar", last modified: Tue Jul  4 18:17:10 2023, max compression
+gzip compressed data, was "raspberrypi_control-1.2.tar", last modified: Tue Jul  4 18:32:11 2023, max compression
```

## Comparing `raspberrypi_control-0.0.1.tar` & `raspberrypi_control-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:10.918026 raspberrypi_control-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 18:16:59.000000 raspberrypi_control-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-04 18:17:10.918026 raspberrypi_control-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-04 18:16:59.000000 raspberrypi_control-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-04 18:16:59.000000 raspberrypi_control-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:10.918026 raspberrypi_control-0.0.1/raspberrypi_control/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 18:16:59.000000 raspberrypi_control-0.0.1/raspberrypi_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57409 2023-07-04 18:16:59.000000 raspberrypi_control-0.0.1/raspberrypi_control/raspberrypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:10.918026 raspberrypi_control-0.0.1/raspberrypi_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-04 18:17:10.000000 raspberrypi_control-0.0.1/raspberrypi_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 18:17:10.000000 raspberrypi_control-0.0.1/raspberrypi_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:17:10.000000 raspberrypi_control-0.0.1/raspberrypi_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 18:17:10.000000 raspberrypi_control-0.0.1/raspberrypi_control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 18:17:10.000000 raspberrypi_control-0.0.1/raspberrypi_control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:17:10.918026 raspberrypi_control-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:32:11.488830 raspberrypi_control-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 18:31:59.000000 raspberrypi_control-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-04 18:32:11.488830 raspberrypi_control-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 18:31:59.000000 raspberrypi_control-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-04 18:31:59.000000 raspberrypi_control-1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:32:11.488830 raspberrypi_control-1.2/raspberrypi_control/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 18:31:59.000000 raspberrypi_control-1.2/raspberrypi_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57409 2023-07-04 18:31:59.000000 raspberrypi_control-1.2/raspberrypi_control/raspberrypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:32:11.488830 raspberrypi_control-1.2/raspberrypi_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-04 18:32:11.000000 raspberrypi_control-1.2/raspberrypi_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 18:32:11.000000 raspberrypi_control-1.2/raspberrypi_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:32:11.000000 raspberrypi_control-1.2/raspberrypi_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 18:32:11.000000 raspberrypi_control-1.2/raspberrypi_control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 18:32:11.000000 raspberrypi_control-1.2/raspberrypi_control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:32:11.488830 raspberrypi_control-1.2/setup.cfg
```

### Comparing `raspberrypi_control-0.0.1/LICENSE` & `raspberrypi_control-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberrypi_control-0.0.1/PKG-INFO` & `raspberrypi_control-1.2/raspberrypi_control.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: raspberrypi_control
-Version: 0.0.1
+Name: raspberrypi-control
+Version: 1.2
 Summary: Control Raspberrypi board with ssh and python
 Author-email: Geoloup Team <franckiebbb@gmail.com>
 Project-URL: Homepage, https://github.com/Geoloup/raspberry_control/
 Project-URL: Bug Tracker, https://github.com/Geoloup/raspberry_control/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,55 +13,55 @@
 License-File: LICENSE
 
 # **Raspberry Pi controller**
 ## Feature
 
  1. Connect in ssh to the Raspberry Pi
  2.  Module and Global call are supported
- 3. The function can be run on the Raspberry Pi  by calling `@raspberry.raspberry_command()` and get the result
+ 3. The function can be run on the Raspberry Pi  by calling `@raspberry_control.raspberry_command()` and get the result
  4. Get Output of a function that was run on the raspberry
  5. Real-time output
- 6. Run command on the Raspberry Pi with `raspberry.fun_command("command here")`
+ 6. Run command on the Raspberry Pi with `raspberry_control.run_command("command here")`
  7. You can do `@raspberrypi.timeout(time,default)` that will make the function stop after the time specified and stop if it's not finish
 ## Example
 
-    import raspberrypi # import package for raspberrypi controlling over ssh  
+    import raspberrypi_control # import package for raspberrypi controlling over ssh  
     import os # Put import here they are take and install to the raspberrypi file.  
     import time  
       
-    rp = raspberrypi # rp is for RaspBerryPi  
+    rp = raspberrypi_control # rp is for RaspBerryPi  
       
     i = 1234567890  
       
       
     @rp.raspberry_command() # run code and you're raspberrypi. If the raspberrypi was not find it's will be run in local.  
     def test():  
-    print("Hello RaspBerryPi")  
-    return "finished"  
+        print("Hello RaspBerryPi")  
+        return "finished"  
       
       
     @rp.raspberry_command() # run code and you're raspberrypi. If the raspberrypi was not find it's will be run in local  
     def other():  
-    global i  
-    print("Hello RaspBerryPi h")  
-    th = 0  
-    print(i)  
-    os.system("echo Hello World")  
-    while True:  
-    th = th + 1  
-    if th == 30:  
-    time.sleep(0.1)  
-    break  
-    return th  
+        global i  
+        print("Hello RaspBerryPi h")  
+        th = 0  
+        print(i)  
+        os.system("echo Hello World")  
+        while True:  
+            th = th + 1  
+            if th == 30:  
+                time.sleep(0.1)  
+                break  
+        return th  
       
       
     if __name__ == "__main__": # put all you're code to run at start here. Because if not the code will be run 2 time  
-    rp.raspberrypi().set_preparation("192.168.0.10", 8, 1) # config locator for the raspberrypi  
-    rp.raspberrypi().local("192.168.0.10") # set the start ip set in the line in the top  
-    rp.config("main") # file name if this file (no .py)  
-    print(test())  
-    print(other()) # you can get the output after
+        rp.raspberrypi().set_preparation("192.168.0.10", 8, 1) # config locator for the raspberrypi  
+        rp.raspberrypi().local("192.168.0.10") # set the start ip set in the line in the top  
+        rp.config("main") # file name if this file (no .py)  
+        print(test())  
+        print(other()) # you can get the output after
 
 ## How to install the package
-Do `Pip install raspberry-control`
+Do `pip install raspberry-control`
 Supported for python 3.10 and higher*
 *note not tested for lower version
```

### Comparing `raspberrypi_control-0.0.1/README.md` & `raspberrypi_control-1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # **Raspberry Pi controller**
 ## Feature
 
  1. Connect in ssh to the Raspberry Pi
  2.  Module and Global call are supported
- 3. The function can be run on the Raspberry Pi  by calling `@raspberry.raspberry_command()` and get the result
+ 3. The function can be run on the Raspberry Pi  by calling `@raspberry_control.raspberry_command()` and get the result
  4. Get Output of a function that was run on the raspberry
  5. Real-time output
- 6. Run command on the Raspberry Pi with `raspberry.fun_command("command here")`
+ 6. Run command on the Raspberry Pi with `raspberry_control.run_command("command here")`
  7. You can do `@raspberrypi.timeout(time,default)` that will make the function stop after the time specified and stop if it's not finish
 ## Example
 
-    import raspberrypi # import package for raspberrypi controlling over ssh  
+    import raspberrypi_control # import package for raspberrypi controlling over ssh  
     import os # Put import here they are take and install to the raspberrypi file.  
     import time  
       
-    rp = raspberrypi # rp is for RaspBerryPi  
+    rp = raspberrypi_control # rp is for RaspBerryPi  
       
     i = 1234567890  
       
       
     @rp.raspberry_command() # run code and you're raspberrypi. If the raspberrypi was not find it's will be run in local.  
     def test():  
-    print("Hello RaspBerryPi")  
-    return "finished"  
+        print("Hello RaspBerryPi")  
+        return "finished"  
       
       
     @rp.raspberry_command() # run code and you're raspberrypi. If the raspberrypi was not find it's will be run in local  
     def other():  
-    global i  
-    print("Hello RaspBerryPi h")  
-    th = 0  
-    print(i)  
-    os.system("echo Hello World")  
-    while True:  
-    th = th + 1  
-    if th == 30:  
-    time.sleep(0.1)  
-    break  
-    return th  
+        global i  
+        print("Hello RaspBerryPi h")  
+        th = 0  
+        print(i)  
+        os.system("echo Hello World")  
+        while True:  
+            th = th + 1  
+            if th == 30:  
+                time.sleep(0.1)  
+                break  
+        return th  
       
       
     if __name__ == "__main__": # put all you're code to run at start here. Because if not the code will be run 2 time  
-    rp.raspberrypi().set_preparation("192.168.0.10", 8, 1) # config locator for the raspberrypi  
-    rp.raspberrypi().local("192.168.0.10") # set the start ip set in the line in the top  
-    rp.config("main") # file name if this file (no .py)  
-    print(test())  
-    print(other()) # you can get the output after
+        rp.raspberrypi().set_preparation("192.168.0.10", 8, 1) # config locator for the raspberrypi  
+        rp.raspberrypi().local("192.168.0.10") # set the start ip set in the line in the top  
+        rp.config("main") # file name if this file (no .py)  
+        print(test())  
+        print(other()) # you can get the output after
 
 ## How to install the package
-Do `Pip install raspberry-control`
+Do `pip install raspberry-control`
 Supported for python 3.10 and higher*
 *note not tested for lower version
```

### Comparing `raspberrypi_control-0.0.1/pyproject.toml` & `raspberrypi_control-1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raspberrypi_control"
-version = "0.0.1"
+version = "1.2"
 authors = [
   { name="Geoloup Team", email="franckiebbb@gmail.com"},
 ]
 description = "Control Raspberrypi board with ssh and python"
 readme = "README.md"
 dependencies = [
     "requests",
```

### Comparing `raspberrypi_control-0.0.1/raspberrypi_control/raspberrypi.py` & `raspberrypi_control-1.2/raspberrypi_control/raspberrypi.py`

 * *Files identical despite different names*

### Comparing `raspberrypi_control-0.0.1/raspberrypi_control.egg-info/PKG-INFO` & `raspberrypi_control-1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: raspberrypi-control
-Version: 0.0.1
+Name: raspberrypi_control
+Version: 1.2
 Summary: Control Raspberrypi board with ssh and python
 Author-email: Geoloup Team <franckiebbb@gmail.com>
 Project-URL: Homepage, https://github.com/Geoloup/raspberry_control/
 Project-URL: Bug Tracker, https://github.com/Geoloup/raspberry_control/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,55 +13,55 @@
 License-File: LICENSE
 
 # **Raspberry Pi controller**
 ## Feature
 
  1. Connect in ssh to the Raspberry Pi
  2.  Module and Global call are supported
- 3. The function can be run on the Raspberry Pi  by calling `@raspberry.raspberry_command()` and get the result
+ 3. The function can be run on the Raspberry Pi  by calling `@raspberry_control.raspberry_command()` and get the result
  4. Get Output of a function that was run on the raspberry
  5. Real-time output
- 6. Run command on the Raspberry Pi with `raspberry.fun_command("command here")`
+ 6. Run command on the Raspberry Pi with `raspberry_control.run_command("command here")`
  7. You can do `@raspberrypi.timeout(time,default)` that will make the function stop after the time specified and stop if it's not finish
 ## Example
 
-    import raspberrypi # import package for raspberrypi controlling over ssh  
+    import raspberrypi_control # import package for raspberrypi controlling over ssh  
     import os # Put import here they are take and install to the raspberrypi file.  
     import time  
       
-    rp = raspberrypi # rp is for RaspBerryPi  
+    rp = raspberrypi_control # rp is for RaspBerryPi  
       
     i = 1234567890  
       
       
     @rp.raspberry_command() # run code and you're raspberrypi. If the raspberrypi was not find it's will be run in local.  
     def test():  
-    print("Hello RaspBerryPi")  
-    return "finished"  
+        print("Hello RaspBerryPi")  
+        return "finished"  
       
       
     @rp.raspberry_command() # run code and you're raspberrypi. If the raspberrypi was not find it's will be run in local  
     def other():  
-    global i  
-    print("Hello RaspBerryPi h")  
-    th = 0  
-    print(i)  
-    os.system("echo Hello World")  
-    while True:  
-    th = th + 1  
-    if th == 30:  
-    time.sleep(0.1)  
-    break  
-    return th  
+        global i  
+        print("Hello RaspBerryPi h")  
+        th = 0  
+        print(i)  
+        os.system("echo Hello World")  
+        while True:  
+            th = th + 1  
+            if th == 30:  
+                time.sleep(0.1)  
+                break  
+        return th  
       
       
     if __name__ == "__main__": # put all you're code to run at start here. Because if not the code will be run 2 time  
-    rp.raspberrypi().set_preparation("192.168.0.10", 8, 1) # config locator for the raspberrypi  
-    rp.raspberrypi().local("192.168.0.10") # set the start ip set in the line in the top  
-    rp.config("main") # file name if this file (no .py)  
-    print(test())  
-    print(other()) # you can get the output after
+        rp.raspberrypi().set_preparation("192.168.0.10", 8, 1) # config locator for the raspberrypi  
+        rp.raspberrypi().local("192.168.0.10") # set the start ip set in the line in the top  
+        rp.config("main") # file name if this file (no .py)  
+        print(test())  
+        print(other()) # you can get the output after
 
 ## How to install the package
-Do `Pip install raspberry-control`
+Do `pip install raspberry-control`
 Supported for python 3.10 and higher*
 *note not tested for lower version
```

