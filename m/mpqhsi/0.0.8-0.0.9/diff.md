# Comparing `tmp/mpqhsi-0.0.8.tar.gz` & `tmp/mpqhsi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpqhsi-0.0.8.tar", last modified: Mon Jun  5 02:37:06 2023, max compression
+gzip compressed data, was "mpqhsi-0.0.9.tar", last modified: Tue Jul  4 01:58:53 2023, max compression
```

## Comparing `mpqhsi-0.0.8.tar` & `mpqhsi-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 02:37:06.113896 mpqhsi-0.0.8/
--rw-rw-rw-   0        0        0      217 2023-06-05 02:37:06.113896 mpqhsi-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 02:37:06.103892 mpqhsi-0.0.8/mpqhsi/
--rw-rw-rw-   0        0        0   133632 2023-05-18 05:29:38.000000 mpqhsi-0.0.8/mpqhsi/My_HSI.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0     5523 2023-05-18 06:05:00.000000 mpqhsi-0.0.8/mpqhsi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 02:37:06.113896 mpqhsi-0.0.8/mpqhsi.egg-info/
--rw-rw-rw-   0        0        0      217 2023-06-05 02:37:06.000000 mpqhsi-0.0.8/mpqhsi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-06-05 02:37:06.000000 mpqhsi-0.0.8/mpqhsi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 02:37:06.000000 mpqhsi-0.0.8/mpqhsi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-05 02:37:06.000000 mpqhsi-0.0.8/mpqhsi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 02:37:06.000000 mpqhsi-0.0.8/mpqhsi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 02:37:06.113896 mpqhsi-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      437 2023-06-05 02:35:30.000000 mpqhsi-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:58:53.709735 mpqhsi-0.0.9/
+-rw-rw-rw-   0        0        0      217 2023-07-04 01:58:53.709735 mpqhsi-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 01:58:53.700934 mpqhsi-0.0.9/mpqhsi/
+-rw-rw-rw-   0        0        0   134144 2023-07-04 01:58:13.000000 mpqhsi-0.0.9/mpqhsi/My_HSI.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0     5549 2023-07-04 01:57:07.000000 mpqhsi-0.0.9/mpqhsi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:58:53.707777 mpqhsi-0.0.9/mpqhsi.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-07-04 01:58:53.000000 mpqhsi-0.0.9/mpqhsi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-07-04 01:58:53.000000 mpqhsi-0.0.9/mpqhsi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 01:58:53.000000 mpqhsi-0.0.9/mpqhsi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-04 01:58:53.000000 mpqhsi-0.0.9/mpqhsi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 01:58:53.000000 mpqhsi-0.0.9/mpqhsi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 01:58:53.709735 mpqhsi-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      437 2023-07-04 01:52:18.000000 mpqhsi-0.0.9/setup.py
```

### Comparing `mpqhsi-0.0.8/mpqhsi/__init__.py` & `mpqhsi-0.0.9/mpqhsi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     return data_cube
 
 def read_Data_one_band(name1,name2,band=[80]):
     #####以灰度图像的形式读取高光谱数据，即单波段数据图像#####
     img_org = read_data_one_band(name1,name2,band)
     return img_org
 
-def read_Data_one_sp(name1,name2,band=80,gre_thre=100,kernel = 10,iter1 = 0,iter2 = 0,key=0):
+def read_Data_one_sp(name1,name2,band=80,gre_thre=100,kernel = 10,iter1 = 0,iter2 = 0,key=0,type=0):
     #####通过该方法生成二值化图像及二值化图像像素值为key处所有高光谱数据的光谱数据并以列表形式显示#####
-    bin_img, sp_list = read_data_one_sp(name1,name2,band,gre_thre,kernel,iter1,iter2,key)
+    bin_img, sp_list = read_data_one_sp(name1,name2,band,gre_thre,kernel,iter1,iter2,key,type)
     return bin_img,sp_list
 
 def HSI_Read_one_band(name1,name2,band=[80]):
     #####通过该方法读取某个波段下高光谱图像数据，返回标准化后的图像#####
     img = HSI_read_one_band(name1,name2,band)
     return img
 
@@ -63,18 +63,18 @@
 def HSI_Savedir_rgbpic(in_path,out_oath,bands=[64,35,14]):
     #####通过该方法将指定波段高光谱图像以伪彩色图像式保存到指定文件夹#####
     # 此处原始数据类型需为.hdr和.cube##
     #eg:../../data/HSI/test_data/,最后有'/'
     HSI_savedir_rgbpic(in_path,out_oath,bands)
 
 
-def HSI_Meandata_make(in_path,out_path,band=80,gre_thre=100):
+def HSI_Meandata_make(in_path,out_path,band=80,gre_thre=100,type = 0):
     #####通过该方法将指定波段高光谱图像中目标区域平均光谱计算出来#####
     # 此处原始数据类型需为.hdr和.cube##
-    result = HSI_meandata_make(in_path,out_path,band,gre_thre)
+    result = HSI_meandata_make(in_path,out_path,band,gre_thre,type)
     return result
 
 def HSI_get_splist_byclick(datacube, channal=3, bands=[10, 20, 30]):
     #####通过该方法可将鼠标点击位置光谱数据以dataframe的形式存在df中########
     df = get_splist_byclick(datacube, channal, bands)
     return df
```

