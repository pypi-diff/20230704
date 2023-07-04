# Comparing `tmp/xgo-pythonlib-0.2.2.tar.gz` & `tmp/xgo-pythonlib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.2.2.tar", last modified: Mon Jul  3 08:00:16 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.2.3.tar", last modified: Tue Jul  4 13:34:53 2023, max compression
```

## Comparing `xgo-pythonlib-0.2.2.tar` & `xgo-pythonlib-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 08:00:16.830679 xgo-pythonlib-0.2.2/
--rw-rw-rw-   0        0        0     2337 2023-07-03 08:00:16.829679 xgo-pythonlib-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1710 2023-07-02 10:39:24.000000 xgo-pythonlib-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 08:00:16.830679 xgo-pythonlib-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     3744 2023-07-03 07:59:45.000000 xgo-pythonlib-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:00:16.819880 xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     2337 2023-07-03 08:00:16.000000 xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-03 08:00:16.000000 xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 08:00:16.000000 xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-03 08:00:16.000000 xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 08:00:16.820893 xgo-pythonlib-0.2.2/xgoedu/
--rw-rw-rw-   0        0        0    47784 2023-07-03 07:59:25.000000 xgo-pythonlib-0.2.2/xgoedu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:00:16.822894 xgo-pythonlib-0.2.2/xgolib/
--rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.2.2/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:00:16.828678 xgo-pythonlib-0.2.2/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.2.2/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.2.2/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.2.2/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:34:53.670424 xgo-pythonlib-0.2.3/
+-rw-rw-rw-   0        0        0     2490 2023-07-04 13:34:53.669424 xgo-pythonlib-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1863 2023-07-04 13:33:41.000000 xgo-pythonlib-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 13:34:53.670424 xgo-pythonlib-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     3744 2023-07-04 13:33:48.000000 xgo-pythonlib-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:34:53.660283 xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     2490 2023-07-04 13:34:53.000000 xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-04 13:34:53.000000 xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 13:34:53.000000 xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-04 13:34:53.000000 xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 13:34:53.661295 xgo-pythonlib-0.2.3/xgoedu/
+-rw-rw-rw-   0        0        0    49527 2023-07-04 13:31:39.000000 xgo-pythonlib-0.2.3/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:34:53.663295 xgo-pythonlib-0.2.3/xgolib/
+-rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.2.3/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:34:53.668424 xgo-pythonlib-0.2.3/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.2.3/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.2.3/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.2.3/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.2.2/PKG-INFO` & `xgo-pythonlib-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -56,15 +56,25 @@
 dog = XGO('xgomini')
 dog.action(1)
 ```
 ### 
 
 ## Change Log
 
-### [0.2.1] - 2023-07-02
+### [0.2.3] - 2023-07-04
+
+#### Added
+
+- Methods: cap_color_mask added.
+
+#### Fixed
+
+- CircleRecognition renamed BallRecognition and improved.
+
+### [0.2.2] - 2023-07-03
 
 #### Added
 
 - Five Methods: SpeechRecognition SpeechSynthesis QRRecognition CircleRecognition ColorRecognitio added.
 
 ### [0.2.0] - 2023-06-21
```

### Comparing `xgo-pythonlib-0.2.2/README.md` & `xgo-pythonlib-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,25 @@
 dog = XGO('xgomini')
 dog.action(1)
 ```
 ### 
 
 ## Change Log
 
-### [0.2.1] - 2023-07-02
+### [0.2.3] - 2023-07-04
+
+#### Added
+
+- Methods: cap_color_mask added.
+
+#### Fixed
+
+- CircleRecognition renamed BallRecognition and improved.
+
+### [0.2.2] - 2023-07-03
 
 #### Added
 
 - Five Methods: SpeechRecognition SpeechSynthesis QRRecognition CircleRecognition ColorRecognitio added.
 
 ### [0.2.0] - 2023-06-21
```

### Comparing `xgo-pythonlib-0.2.2/setup.py` & `xgo-pythonlib-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.2.2/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.2.3/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -56,15 +56,25 @@
 dog = XGO('xgomini')
 dog.action(1)
 ```
 ### 
 
 ## Change Log
 
-### [0.2.1] - 2023-07-02
+### [0.2.3] - 2023-07-04
+
+#### Added
+
+- Methods: cap_color_mask added.
+
+#### Fixed
+
+- CircleRecognition renamed BallRecognition and improved.
+
+### [0.2.2] - 2023-07-03
 
 #### Added
 
 - Five Methods: SpeechRecognition SpeechSynthesis QRRecognition CircleRecognition ColorRecognitio added.
 
 ### [0.2.0] - 2023-06-21
```

### Comparing `xgo-pythonlib-0.2.2/xgoedu/__init__.py` & `xgo-pythonlib-0.2.3/xgoedu/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import json
 import threading
 # from xgolib import XGO
 # from keras.preprocessing import image
 # import _thread  使用_thread会报错，坑！
 
 
-__versinon__ = '1.2.8'
-__last_modified__ = '2023/7/3'
+__versinon__ = '1.3.0'
+__last_modified__ = '2023/7/4'
 
 GPIO.setwarnings(False)
 GPIO.setmode(GPIO.BCM)
 
 camera_still=False
 
 
@@ -840,39 +840,82 @@
         b,g,r = cv2.split(frame)
         img = cv2.merge((r,g,b))
         imgok = Image.fromarray(img)
         self.display.ShowImage(imgok)
 
         return ((color_x,color_y),color_radius)
 
-    def CircleRecognition(self,target="camera"):
+    def cap_color_mask(self,position=None, scale=25, h_error=20, s_limit=[90, 255], v_limit=[90, 230]):
+        if position is None:
+            position = [160, 100]
+        count = 0
+        self.open_camera()
+        while True:
+            if self.xgoButton("c"):   
+                break
+            success,frame = self.cap.read()
+            b,g,r = cv2.split(frame)
+            frame_bgr = cv2.merge((r,g,b))
+            hsv = cv2.cvtColor(frame_bgr, cv2.COLOR_BGR2HSV)
+            h, s, v = cv2.split(hsv)
+            color = np.mean(h[position[1]:position[1] + scale, position[0]:position[0] + scale])
+            if self.xgoButton("b") and count == 0:
+                count += 1
+                color = np.mean(h[position[1]:position[1] + scale, position[0]:position[0] + scale])
+                color_lower = [max(color - h_error, 0), s_limit[0], v_limit[0]]
+                color_upper = [min(color + h_error, 255), s_limit[1], v_limit[1]]
+                return [color_lower, color_upper]
+
+            if count == 0:
+                cv2.rectangle(frame, (position[0], position[1]), (position[0] + scale, position[1] + scale),
+                            (255, 255, 255), 2)
+                cv2.putText(frame, 'press button B', (40, 40), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (0, 0, 255), 2)
+            b,g,r = cv2.split(frame)
+            img = cv2.merge((r,g,b))
+            imgok = Image.fromarray(img)
+            self.display.ShowImage(imgok)
+    
+    def filter_img(self,frame,color):
+        b,g,r = cv2.split(frame)
+        frame_bgr = cv2.merge((r,g,b))
+        hsv = cv2.cvtColor(frame_bgr, cv2.COLOR_BGR2HSV)
+        if isinstance(color, list):
+            color_lower = np.array(color[0])
+            color_upper = np.array(color[1])
+        else:
+            color_upper, color_lower = get_color_mask(color)
+        mask = cv2.inRange(hsv, color_lower, color_upper)
+        img_mask = cv2.bitwise_and(frame, frame, mask=mask)
+        return img_mask
+
+    def BallRecognition(self,color_mask,target="camera",p1=36, p2=15, minR=6, maxR=35):
+        x=y=ra=0
         if target=="camera":
             self.open_camera()
             success,image = self.cap.read()
         else:
             path="/home/pi/xgoPictures/"
             image=np.array(Image.open(path+target))
-        img = cv2.cvtColor(image,cv2.COLOR_BGR2GRAY)
+
+        frame_mask=self.filter_img(image, color_mask)
+        
+        img = cv2.medianBlur(frame_mask, 5)
+        img = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
         
-        numpy_img = cv2.adaptiveThreshold(img, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY, 11, 15)   # 自动阈值二值化
-        #                                                      圆心距 canny阈值    投票数      最小半径       最大半径
-        circles = cv2.HoughCircles(img, cv2.HOUGH_GRADIENT, 1, 18,   param1=100, param2=80,  minRadius=40, maxRadius=150)
-        arr1 = np.zeros([0, 2], dtype=int)                      # 创建一个0行, 2列的空数组
-        re=[]
-        if circles is not None:
-            circles = np.uint16(np.around(circles))   
-            for i in circles[0, :]:
-                re.append(((i[0], i[1]), i[2]))
-                cv2.circle(image, (i[0], i[1]), i[2], (0, 0, 255), 3)  # 轮廓
-                cv2.circle(image, (i[0], i[1]), 2, (0, 0, 0), 6)     # 圆心
+        circles = cv2.HoughCircles(img, cv2.HOUGH_GRADIENT, 1, 20, param1=p1, param2=p2, minRadius=minR,maxRadius=maxR)
         b,g,r = cv2.split(image)
         image = cv2.merge((r,g,b))
+        if circles is not None and len(circles[0]) == 1:
+            param = circles[0][0]
+            x, y, ra = int(param[0]), int(param[1]), int(param[2])
+            cv2.circle(image, (x, y), ra, (255, 255, 255), 2)
+            cv2.circle(image, (x, y), 2, (255, 255, 255), 2)
         imgok = Image.fromarray(image)
         self.display.ShowImage(imgok)
-        return re
+        return x,y,ra
 
 
 
 
 
 class DemoError(Exception):
     pass
```

### Comparing `xgo-pythonlib-0.2.2/xgolib/__init__.py` & `xgo-pythonlib-0.2.3/xgolib/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.2/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.2.3/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.2/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.2.3/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

