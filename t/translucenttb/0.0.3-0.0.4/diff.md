# Comparing `tmp/translucenttb-0.0.3.tar.gz` & `tmp/translucenttb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translucenttb-0.0.3.tar", last modified: Sat Jul  1 04:46:19 2023, max compression
+gzip compressed data, was "translucenttb-0.0.4.tar", last modified: Tue Jul  4 08:02:07 2023, max compression
```

## Comparing `translucenttb-0.0.3.tar` & `translucenttb-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 04:46:19.934819 translucenttb-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-01 04:46:19.934819 translucenttb-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-01 04:45:56.000000 translucenttb-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 04:45:56.000000 translucenttb-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 04:46:19.934819 translucenttb-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-01 04:45:56.000000 translucenttb-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 04:46:19.934819 translucenttb-0.0.3/translucenttb/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 04:45:56.000000 translucenttb-0.0.3/translucenttb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-01 04:45:56.000000 translucenttb-0.0.3/translucenttb/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-01 04:45:56.000000 translucenttb-0.0.3/translucenttb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 04:46:19.934819 translucenttb-0.0.3/translucenttb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-01 04:46:19.000000 translucenttb-0.0.3/translucenttb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-01 04:46:19.000000 translucenttb-0.0.3/translucenttb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 04:46:19.000000 translucenttb-0.0.3/translucenttb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 04:46:19.000000 translucenttb-0.0.3/translucenttb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:02:07.356603 translucenttb-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-04 08:02:07.356603 translucenttb-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-04 08:01:45.000000 translucenttb-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 08:01:45.000000 translucenttb-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:02:07.356603 translucenttb-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-04 08:01:45.000000 translucenttb-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:02:07.356603 translucenttb-0.0.4/translucenttb/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-04 08:01:45.000000 translucenttb-0.0.4/translucenttb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-04 08:01:45.000000 translucenttb-0.0.4/translucenttb/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-04 08:01:45.000000 translucenttb-0.0.4/translucenttb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:02:07.356603 translucenttb-0.0.4/translucenttb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-04 08:02:07.000000 translucenttb-0.0.4/translucenttb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 08:02:07.000000 translucenttb-0.0.4/translucenttb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:02:07.000000 translucenttb-0.0.4/translucenttb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 08:02:07.000000 translucenttb-0.0.4/translucenttb.egg-info/top_level.txt
```

### Comparing `translucenttb-0.0.3/PKG-INFO` & `translucenttb-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: translucenttb
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python version TranslucentTB
 Home-page: https://github.com/littlewhitecloud/TranslucentTB/
 Author: littlewhitecloud
 Description-Content-Type: text/markdown
 
 ### TranslucentTB
 #### This is a python version TranslucentTB maybe with tkinter and ctypes
-> Add gui later
-### Clear
+
+A lightweight utility that makes the Windows taskbar translucent/transparent on Windows 10 and Windows11.
+
+### Screenshots
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/97763cac-2b58-4208-b98b-36d031c86880)
-### Noeffect
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/761f84b4-5367-40a2-81ec-e9e97b2f19f5)
-### Blur
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/78b2a579-4c5f-4d95-8b68-4fe2b4f2ba29)
-### Acrylic
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/211f4147-ce5d-4f04-9126-e274369abdfd)
 
 ### Usage
 ```python
 from translucenttb import blur # import the blur function
 blur(blurtype="acrylic") # for example acrylic
 # choose one type from ("clear", "noeffect", "blur", "acrylic")
@@ -28,15 +27,17 @@
 ### UI
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/0a9ecdd5-f5ae-4fa9-b124-09a1e9ed849a)
 ```python
 from translucenttb import Settings
 example = Settings()
 example.mainloop()
 ```
-### Fun Example:
+### Example:
+<details>
+    
 ```python
 from time import sleep
 
 from translucenttb import blur
 
 
 def colorful():
@@ -86,7 +87,9 @@
         blur("noeffect", hexcolor)
         sleep(0.1)
 
 
 colorful()
 ```
 https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/a2d0b4cc-0698-46c0-b050-e3d89c788964
+
+</details>
```

### Comparing `translucenttb-0.0.3/README.md` & `translucenttb-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 ### TranslucentTB
 #### This is a python version TranslucentTB maybe with tkinter and ctypes
-> Add gui later
-### Clear
+
+A lightweight utility that makes the Windows taskbar translucent/transparent on Windows 10 and Windows11.
+
+### Screenshots
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/97763cac-2b58-4208-b98b-36d031c86880)
-### Noeffect
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/761f84b4-5367-40a2-81ec-e9e97b2f19f5)
-### Blur
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/78b2a579-4c5f-4d95-8b68-4fe2b4f2ba29)
-### Acrylic
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/211f4147-ce5d-4f04-9126-e274369abdfd)
 
 ### Usage
 ```python
 from translucenttb import blur # import the blur function
 blur(blurtype="acrylic") # for example acrylic
 # choose one type from ("clear", "noeffect", "blur", "acrylic")
@@ -20,15 +19,17 @@
 ### UI
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/0a9ecdd5-f5ae-4fa9-b124-09a1e9ed849a)
 ```python
 from translucenttb import Settings
 example = Settings()
 example.mainloop()
 ```
-### Fun Example:
+### Example:
+<details>
+    
 ```python
 from time import sleep
 
 from translucenttb import blur
 
 
 def colorful():
@@ -78,7 +79,9 @@
         blur("noeffect", hexcolor)
         sleep(0.1)
 
 
 colorful()
 ```
 https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/a2d0b4cc-0698-46c0-b050-e3d89c788964
+
+</details>
```

### Comparing `translucenttb-0.0.3/translucenttb/blur.py` & `translucenttb-0.0.4/translucenttb/blur.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,39 +58,40 @@
     blue = HEX[5:7]
     green = HEX[3:5]
     red = HEX[1:3]
     gradientColor = alpha + blue + green + red
     return int(gradientColor, base=16)
 
 
-def blur(blurtype: str = "acrylic", hexColor: str = ""):
-    hwnd = windll.user32.FindWindowW("Shell_TrayWnd", None)
+def blur(blurtype: str = "acrylic", hexColor: str = "", spechwnd: int = None):
+    hwnd = spechwnd if spechwnd else windll.user32.FindWindowW("Shell_TrayWnd", None)
+
     accent = ACCENTPOLICY()
     accent.AccentState = 3
-
     gradientColor = 0
-
-    accent.AccentFlags = 2
-    gradientColor = (
-        HEXtoRGBAint("#0000000000") if not hexColor else HEXtoRGBAint(hexColor)
-    )
+	
+    if hexColor:
+        accent.AccentFlags = 2
+        gradientColor = (
+            HEXtoRGBAint(hexColor)
+        )
 
     if blurtype == "clear":
         accent.AccentState = 2
     elif blurtype == "noeffect":
         accent.AccentState = 1
     elif blurtype == "blur":
         DWM_BB_ENABLE = 0x01
         bb = DWM_BLURBEHIND()
         bb.dwFlags = DWM_BB_ENABLE
         bb.fEnable = 1
         bb.hRgnBlur = 1
         windll.dwmapi.DwmEnableBlurBehindWindow(hwnd, byref(bb))
     elif blurtype == "acrylic":
-        accent.AccentState = 3
+        accent.AccentState = 4
     accent.GradientColor = gradientColor
 
     data = WINDOWCOMPOSITIONATTRIBDATA()
     data.Attribute = 19
     data.SizeOfData = sizeof(accent)
     data.Data = cast(pointer(accent), POINTER(c_int))
```

### Comparing `translucenttb-0.0.3/translucenttb/main.py` & `translucenttb-0.0.4/translucenttb/main.py`

 * *Files identical despite different names*

### Comparing `translucenttb-0.0.3/translucenttb.egg-info/PKG-INFO` & `translucenttb-0.0.4/translucenttb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: translucenttb
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python version TranslucentTB
 Home-page: https://github.com/littlewhitecloud/TranslucentTB/
 Author: littlewhitecloud
 Description-Content-Type: text/markdown
 
 ### TranslucentTB
 #### This is a python version TranslucentTB maybe with tkinter and ctypes
-> Add gui later
-### Clear
+
+A lightweight utility that makes the Windows taskbar translucent/transparent on Windows 10 and Windows11.
+
+### Screenshots
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/97763cac-2b58-4208-b98b-36d031c86880)
-### Noeffect
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/761f84b4-5367-40a2-81ec-e9e97b2f19f5)
-### Blur
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/78b2a579-4c5f-4d95-8b68-4fe2b4f2ba29)
-### Acrylic
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/211f4147-ce5d-4f04-9126-e274369abdfd)
 
 ### Usage
 ```python
 from translucenttb import blur # import the blur function
 blur(blurtype="acrylic") # for example acrylic
 # choose one type from ("clear", "noeffect", "blur", "acrylic")
@@ -28,15 +27,17 @@
 ### UI
 ![image](https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/0a9ecdd5-f5ae-4fa9-b124-09a1e9ed849a)
 ```python
 from translucenttb import Settings
 example = Settings()
 example.mainloop()
 ```
-### Fun Example:
+### Example:
+<details>
+    
 ```python
 from time import sleep
 
 from translucenttb import blur
 
 
 def colorful():
@@ -86,7 +87,9 @@
         blur("noeffect", hexcolor)
         sleep(0.1)
 
 
 colorful()
 ```
 https://github.com/littlewhitecloud/TranslucentTB/assets/71159641/a2d0b4cc-0698-46c0-b050-e3d89c788964
+
+</details>
```

