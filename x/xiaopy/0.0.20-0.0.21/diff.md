# Comparing `tmp/xiaopy-0.0.20.tar.gz` & `tmp/xiaopy-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaopy-0.0.20.tar", last modified: Mon May  8 07:17:42 2023, max compression
+gzip compressed data, was "xiaopy-0.0.21.tar", last modified: Tue Jul  4 01:15:11 2023, max compression
```

## Comparing `xiaopy-0.0.20.tar` & `xiaopy-0.0.21.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 07:17:42.253083 xiaopy-0.0.20/
--rw-rw-rw-   0        0        0      262 2023-05-08 07:17:42.253083 xiaopy-0.0.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 07:17:42.236128 xiaopy-0.0.20/PyGameAutoAndroid/
--rw-rw-rw-   0        0        0    10028 2023-04-25 10:19:41.000000 xiaopy-0.0.20/PyGameAutoAndroid/PyGameAutoAndroid.py
--rw-rw-rw-   0        0        0      261 2023-02-15 16:25:44.000000 xiaopy-0.0.20/PyGameAutoAndroid/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-08 07:17:42.254080 xiaopy-0.0.20/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 07:17:42.240117 xiaopy-0.0.20/xiaopy/
--rw-rw-rw-   0        0        0      250 2023-02-15 16:25:49.000000 xiaopy-0.0.20/xiaopy/__init__.py
--rw-rw-rw-   0        0        0    10028 2023-04-25 10:20:08.000000 xiaopy-0.0.20/xiaopy/xiaopy.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:17:42.250093 xiaopy-0.0.20/xiaopy.egg-info/
--rw-rw-rw-   0        0        0      262 2023-05-08 07:17:42.000000 xiaopy-0.0.20/xiaopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-05-08 07:17:42.000000 xiaopy-0.0.20/xiaopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 07:17:42.000000 xiaopy-0.0.20/xiaopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-08 07:17:42.000000 xiaopy-0.0.20/xiaopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      631 2023-05-08 07:09:14.000000 xiaopy-0.0.20/xiaopy_setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:15:11.833469 xiaopy-0.0.21/
+-rw-rw-rw-   0        0        0      262 2023-07-04 01:15:11.832492 xiaopy-0.0.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 01:15:11.821757 xiaopy-0.0.21/PyGameAutoAndroid/
+-rw-rw-rw-   0        0        0    11623 2023-07-04 01:03:28.000000 xiaopy-0.0.21/PyGameAutoAndroid/PyGameAutoAndroid.py
+-rw-rw-rw-   0        0        0      261 2023-02-15 16:25:44.000000 xiaopy-0.0.21/PyGameAutoAndroid/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-04 01:15:11.833469 xiaopy-0.0.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 01:15:11.824684 xiaopy-0.0.21/xiaopy/
+-rw-rw-rw-   0        0        0      250 2023-02-15 16:25:49.000000 xiaopy-0.0.21/xiaopy/__init__.py
+-rw-rw-rw-   0        0        0    11623 2023-07-04 01:03:28.000000 xiaopy-0.0.21/xiaopy/xiaopy.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:15:11.831516 xiaopy-0.0.21/xiaopy.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-07-04 01:15:11.000000 xiaopy-0.0.21/xiaopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-04 01:15:11.000000 xiaopy-0.0.21/xiaopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 01:15:11.000000 xiaopy-0.0.21/xiaopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-04 01:15:11.000000 xiaopy-0.0.21/xiaopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      631 2023-07-04 01:10:00.000000 xiaopy-0.0.21/xiaopy_setup.py
```

### Comparing `xiaopy-0.0.20/PyGameAutoAndroid/PyGameAutoAndroid.py` & `xiaopy-0.0.21/PyGameAutoAndroid/PyGameAutoAndroid.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,14 +91,63 @@
     def inputTextAndEnter(self, text: str):
         pass
 
     def clearText(self):
         pass
 
 
+class Device:
+    def systemLanguage(self):
+        pass
+
+    def systemLanguageList(self):
+        pass
+
+    def systemVersion(self):
+        pass
+
+    def manufacturer(self):
+        pass
+
+    def product(self):
+        pass
+
+    def brand(self):
+        pass
+
+    def model(self):
+        pass
+
+    def board(self):
+        pass
+
+    def name(self):
+        pass
+
+    def hardware(self):
+        pass
+
+    def host(self):
+        pass
+
+    def display(self):
+        pass
+
+    def id(self):
+        pass
+
+    def user(self):
+        pass
+
+    def serial(self):
+        pass
+
+    def sdk(self):
+        pass
+
 class Size:
     width = None
     height = None
 
 
 class Selector:
     def join(self, selector):
@@ -147,15 +196,15 @@
         :param y2: 终点 y 坐标
         :param duration: 滑动时间
         :return:
         """
         pass
 
     @classmethod
-    def gesture(cls, path: Path):
+    def gesture(cls, path: Path, path2: Path=None):
         pass
 
     @classmethod
     def getColor(cls, x: int, y: int):
         """
         获取颜色
         :param x: x 坐标
@@ -192,23 +241,24 @@
         """
         多点比色
         :return:
         """
         return
 
     @classmethod
-    def findColor(cls, mainColorDesc: str, multiColorDesc: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0):
+    def findColor(cls, mainColorDesc: str, multiColorDesc: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, sim=1.0):
         """
         多点找色
         :param mainColorDesc: 主点颜色描述
         :param multiColorDesc: 多点颜色描述
         :param x1: 起点 x 坐标
         :param y1: 起点 y 坐标
         :param x2: 终点 x 坐标
         :param y2: 终点 y 坐标
+        :param sim: 相似度
         :return:
         """
         return Point
 
     @classmethod
     def findImage(cls, imgName: str, x1: object = 0, y1: object = 0, x2: object = 0, y2: object = 0, sim: float = 0.9):
         """
@@ -343,14 +393,24 @@
         长点击节点
         :param node:
         :return:
         """
         pass
 
     @classmethod
+    def setNodeText(cls, node: Node, text: str) -> bool:
+        """
+        节点输入
+        :param node:
+        :param text:
+        :return:
+        """
+        pass
+
+    @classmethod
     def log(cls, *msg: object):
         """
         日志框打印
         :param msg: 日志内容
         :return:
         """
         pass
@@ -405,14 +465,23 @@
         关闭APP
         :param packageName:
         :return:
         """
         pass
 
     @classmethod
+    def changeOrientation(cls, orientation: int):
+        """
+        设置屏幕方向
+        :param orientation:
+        :return:
+        """
+        pass
+
+    @classmethod
     def currentAppPackageName(cls):
         """
         获取当前APP包名
         :return:
         """
         pass
 
@@ -424,20 +493,40 @@
         """
         return Size
 
     @classmethod
     def screenshot(cls, fileName: str = None, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0):
         """
         截图
+        :param x1:
+        :param y1:
+        :param x2:
+        :param y2:
         :param fileName: 文件名
         :return:
         """
         pass
 
     @classmethod
+    def copy(cls, text: str):
+        """
+        设置剪切板内容
+        :return:
+        """
+        pass
+
+    @classmethod
+    def paste(cls):
+        """
+        获取剪切板内容
+        :return:
+        """
+        pass
+
+    @classmethod
     def inputText(cls, text: str):
         """
         输入文本
         :param text:
         :return:
         """
         pass
@@ -461,7 +550,15 @@
     @classmethod
     def keyboard(cls):
         """
         获取键盘对象
         :return:
         """
         return Keyboard()
+
+    @classmethod
+    def device(cls):
+        """
+        获取设备对象
+        :return:
+        """
+        return Device()
```

### Comparing `xiaopy-0.0.20/xiaopy/xiaopy.py` & `xiaopy-0.0.21/xiaopy/xiaopy.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,14 +91,63 @@
     def inputTextAndEnter(self, text: str):
         pass
 
     def clearText(self):
         pass
 
 
+class Device:
+    def systemLanguage(self):
+        pass
+
+    def systemLanguageList(self):
+        pass
+
+    def systemVersion(self):
+        pass
+
+    def manufacturer(self):
+        pass
+
+    def product(self):
+        pass
+
+    def brand(self):
+        pass
+
+    def model(self):
+        pass
+
+    def board(self):
+        pass
+
+    def name(self):
+        pass
+
+    def hardware(self):
+        pass
+
+    def host(self):
+        pass
+
+    def display(self):
+        pass
+
+    def id(self):
+        pass
+
+    def user(self):
+        pass
+
+    def serial(self):
+        pass
+
+    def sdk(self):
+        pass
+
 class Size:
     width = None
     height = None
 
 
 class Selector:
     def join(self, selector):
@@ -147,15 +196,15 @@
         :param y2: 终点 y 坐标
         :param duration: 滑动时间
         :return:
         """
         pass
 
     @classmethod
-    def gesture(cls, path: Path):
+    def gesture(cls, path: Path, path2: Path=None):
         pass
 
     @classmethod
     def getColor(cls, x: int, y: int):
         """
         获取颜色
         :param x: x 坐标
@@ -192,23 +241,24 @@
         """
         多点比色
         :return:
         """
         return
 
     @classmethod
-    def findColor(cls, mainColorDesc: str, multiColorDesc: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0):
+    def findColor(cls, mainColorDesc: str, multiColorDesc: str, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0, sim=1.0):
         """
         多点找色
         :param mainColorDesc: 主点颜色描述
         :param multiColorDesc: 多点颜色描述
         :param x1: 起点 x 坐标
         :param y1: 起点 y 坐标
         :param x2: 终点 x 坐标
         :param y2: 终点 y 坐标
+        :param sim: 相似度
         :return:
         """
         return Point
 
     @classmethod
     def findImage(cls, imgName: str, x1: object = 0, y1: object = 0, x2: object = 0, y2: object = 0, sim: float = 0.9):
         """
@@ -343,14 +393,24 @@
         长点击节点
         :param node:
         :return:
         """
         pass
 
     @classmethod
+    def setNodeText(cls, node: Node, text: str) -> bool:
+        """
+        节点输入
+        :param node:
+        :param text:
+        :return:
+        """
+        pass
+
+    @classmethod
     def log(cls, *msg: object):
         """
         日志框打印
         :param msg: 日志内容
         :return:
         """
         pass
@@ -405,14 +465,23 @@
         关闭APP
         :param packageName:
         :return:
         """
         pass
 
     @classmethod
+    def changeOrientation(cls, orientation: int):
+        """
+        设置屏幕方向
+        :param orientation:
+        :return:
+        """
+        pass
+
+    @classmethod
     def currentAppPackageName(cls):
         """
         获取当前APP包名
         :return:
         """
         pass
 
@@ -424,20 +493,40 @@
         """
         return Size
 
     @classmethod
     def screenshot(cls, fileName: str = None, x1: int = 0, y1: int = 0, x2: int = 0, y2: int = 0):
         """
         截图
+        :param x1:
+        :param y1:
+        :param x2:
+        :param y2:
         :param fileName: 文件名
         :return:
         """
         pass
 
     @classmethod
+    def copy(cls, text: str):
+        """
+        设置剪切板内容
+        :return:
+        """
+        pass
+
+    @classmethod
+    def paste(cls):
+        """
+        获取剪切板内容
+        :return:
+        """
+        pass
+
+    @classmethod
     def inputText(cls, text: str):
         """
         输入文本
         :param text:
         :return:
         """
         pass
@@ -461,7 +550,15 @@
     @classmethod
     def keyboard(cls):
         """
         获取键盘对象
         :return:
         """
         return Keyboard()
+
+    @classmethod
+    def device(cls):
+        """
+        获取设备对象
+        :return:
+        """
+        return Device()
```

### Comparing `xiaopy-0.0.20/xiaopy_setup.py` & `xiaopy-0.0.21/xiaopy_setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Description：
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='xiaopy',
-    version='0.0.20',
+    version='0.0.21',
     packages=find_packages(),
     license='MIT',
     author='小派精灵',
     author_email='3383716176@qq.com',
     description='小派精灵手机自动化',
     classifiers=[
         "Programming Language :: Python :: 3",
```

