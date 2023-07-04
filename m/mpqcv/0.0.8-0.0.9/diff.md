# Comparing `tmp/mpqcv-0.0.8.tar.gz` & `tmp/mpqcv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpqcv-0.0.8.tar", last modified: Tue Mar 14 06:55:38 2023, max compression
+gzip compressed data, was "mpqcv-0.0.9.tar", last modified: Thu May 18 05:56:48 2023, max compression
```

## Comparing `mpqcv-0.0.8.tar` & `mpqcv-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 06:55:38.945562 mpqcv-0.0.8/
--rw-rw-rw-   0        0        0      210 2023-03-14 06:55:38.944628 mpqcv-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-14 06:55:38.935581 mpqcv-0.0.8/mpqcv/
--rw-rw-rw-   0        0        0   197632 2023-03-14 06:41:14.000000 mpqcv-0.0.8/mpqcv/My_CV.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0     4061 2022-12-16 07:02:44.000000 mpqcv-0.0.8/mpqcv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 06:55:38.944628 mpqcv-0.0.8/mpqcv.egg-info/
--rw-rw-rw-   0        0        0      210 2023-03-14 06:55:38.000000 mpqcv-0.0.8/mpqcv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-03-14 06:55:38.000000 mpqcv-0.0.8/mpqcv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 06:55:38.000000 mpqcv-0.0.8/mpqcv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-14 06:55:38.000000 mpqcv-0.0.8/mpqcv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-14 06:55:38.945562 mpqcv-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      459 2023-03-14 06:55:28.000000 mpqcv-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:56:48.699110 mpqcv-0.0.9/
+-rw-rw-rw-   0        0        0      210 2023-05-18 05:56:48.699110 mpqcv-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 05:56:48.689182 mpqcv-0.0.9/mpqcv/
+-rw-rw-rw-   0        0        0   198656 2023-05-18 05:54:25.000000 mpqcv-0.0.9/mpqcv/My_CV.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0     4100 2023-05-18 05:51:35.000000 mpqcv-0.0.9/mpqcv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:56:48.699110 mpqcv-0.0.9/mpqcv.egg-info/
+-rw-rw-rw-   0        0        0      210 2023-05-18 05:56:48.000000 mpqcv-0.0.9/mpqcv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-18 05:56:48.000000 mpqcv-0.0.9/mpqcv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 05:56:48.000000 mpqcv-0.0.9/mpqcv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 05:56:48.000000 mpqcv-0.0.9/mpqcv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 05:56:48.699110 mpqcv-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      414 2023-05-18 05:56:31.000000 mpqcv-0.0.9/setup.py
```

### Comparing `mpqcv-0.0.8/mpqcv/__init__.py` & `mpqcv-0.0.9/mpqcv/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import cv2
 import os
 lib_path = (os.path.split(os.path.realpath(__file__))[0])
 sys.path.append(lib_path)
 from My_CV import *
 # -*- coding utf-8 -*-
 """
-Created on Sept 2th 09:41 2020
+Created on May 18th 09:41 2023
 
 @auther: Peiqi Miao
 
 """
 def find_C_only(cnts,level):
     c = find_c_only(cnts,level)
     return c
@@ -32,39 +32,42 @@
 # Compute low order moments(1,2,3)
 def get_Color_moments(img):
     ####img为BGR格式,用opencv打开即可，或readPic（）方法
     color_feature = color_moments(img)
     return color_feature
 #########color moments(CMs)###################
 
-def cutPic(pic,gre_thre,kernel,thre1,thre2):
+def cutPic(pic,gre_thre=127,kernel=10,iter1=0,iter2=0):
     #gre_thre[0,255],kernel卷积核大小，thre1缩小程度，扩大程度
-    new_pic = cut_pic(pic,gre_thre,kernel,thre1,thre2)
+    new_pic = cut_pic(pic,gre_thre,kernel,iter1,iter2)
     return new_pic
 
 def readPic(name):
     img = read_pic(name)
     return img
 
 def readGraypic(name):
     img = readPic(name)
     gray_pic = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
     return gray_pic
 
-def showName(name,dely):
-    img = cv2.imread(name)
+def save_pic(savename):
+    cv2.imwrite(savename)
+
+def show_img(img,dely):
     cv2.namedWindow('show',0)
     cv2.imshow('show', img)
     cv2.waitKey(dely)
 
 def show_img(img,dely):
     cv2.namedWindow('show',0)
     cv2.imshow('show', img)
     cv2.waitKey(dely)
 
+
 def mkDir(path):
     mkdir(path)
 
 def rot90(img):
     img90 = rot_90(img)
     return img90
 
@@ -134,15 +137,15 @@
     out = tiaozheng234(img_list)
     return out
 
 def getGray(img1,channal):
     get_Gray(img1, channal)
 
 if __name__ == '__main__':
-    showName('./test2.jpg',0)
+    show_name('./test2.jpg',0)
     img = readGraypic('./test2.jpg')
     img = drawCircle(img,(100,100),30,255,-1,txt_key=0)
     show_img(img,0)
     # CMs = get_Color_oments(img)
     # print(CMs)
     # img = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
     # new_pic = cut_pic(img,100,10,1,1)
```

