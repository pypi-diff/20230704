# Comparing `tmp/smartcrop-0.3.3.tar.gz` & `tmp/smartcrop-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smartcrop-0.3.3.tar", last modified: Mon Jul  5 10:15:28 2021, max compression
+gzip compressed data, was "smartcrop-0.3.4.tar", last modified: Tue Jul  4 16:03:43 2023, max compression
```

## Comparing `smartcrop-0.3.3.tar` & `smartcrop-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-05 10:15:28.000000 smartcrop-0.3.3/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-07-05 10:15:28.000000 smartcrop-0.3.3/smartcrop.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)       10 2021-07-05 10:15:28.000000 smartcrop-0.3.3/smartcrop.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2021-07-05 10:15:28.000000 smartcrop-0.3.3/smartcrop.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)     3153 2021-07-05 10:15:28.000000 smartcrop-0.3.3/smartcrop.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)        1 2020-04-12 23:12:09.000000 smartcrop-0.3.3/smartcrop.egg-info/not-zip-safe
--rw-r--r--   0 david     (1000) david     (1000)      264 2021-07-05 10:15:28.000000 smartcrop-0.3.3/smartcrop.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)       48 2021-07-05 10:15:28.000000 smartcrop-0.3.3/smartcrop.egg-info/entry_points.txt
--rw-r--r--   0 david     (1000) david     (1000)       20 2021-07-05 10:15:28.000000 smartcrop-0.3.3/smartcrop.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2021-07-05 10:15:28.000000 smartcrop-0.3.3/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)     1870 2020-04-16 21:57:05.000000 smartcrop-0.3.3/README.rst
--rw-r--r--   0 david     (1000) david     (1000)     1072 2021-07-05 10:09:47.000000 smartcrop-0.3.3/setup.py
--rw-rw-r--   0 david     (1000) david     (1000)     3153 2021-07-05 10:15:28.000000 smartcrop-0.3.3/PKG-INFO
--rwxrwxr-x   0 david     (1000) david     (1000)    14303 2021-07-05 10:05:22.000000 smartcrop-0.3.3/smartcrop.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 16:03:43.982387 smartcrop-0.3.4/
+-rw-r--r--   0 david     (1000) david     (1000)      139 2019-01-25 20:19:19.000000 smartcrop-0.3.4/AUTHORS
+-rw-r--r--   0 david     (1000) david     (1000)     1079 2019-01-25 20:19:19.000000 smartcrop-0.3.4/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)     2488 2023-07-04 16:03:43.982387 smartcrop-0.3.4/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1870 2023-07-04 15:38:23.000000 smartcrop-0.3.4/README.rst
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-07-04 16:03:43.982387 smartcrop-0.3.4/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1072 2023-07-04 16:03:16.000000 smartcrop-0.3.4/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 16:03:43.978387 smartcrop-0.3.4/smartcrop.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)     2488 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      304 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       47 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/entry_points.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2019-01-25 20:31:01.000000 smartcrop-0.3.4/smartcrop.egg-info/not-zip-safe
+-rw-r--r--   0 david     (1000) david     (1000)       20 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       10 2023-07-04 16:03:43.000000 smartcrop-0.3.4/smartcrop.egg-info/top_level.txt
+-rwxrwxr-x   0 david     (1000) david     (1000)    14330 2023-07-04 15:39:37.000000 smartcrop-0.3.4/smartcrop.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 16:03:43.982387 smartcrop-0.3.4/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)      941 2023-07-04 15:39:37.000000 smartcrop-0.3.4/tests/test_smartcrop.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `smartcrop-0.3.3/README.rst` & `smartcrop-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `smartcrop-0.3.3/setup.py` & `smartcrop-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,9 +32,9 @@
     ],
     description='smartcrop implementation in Python',
     keywords=['image', 'crop', 'PIL', 'Pillow'],
     license='MIT',
     long_description=open('README.rst').read(),
     platforms='any',
     url='https://github.com/smartcrop/smartcrop.py',
-    version='0.3.3'
+    version='0.3.4'
 )
```

### Comparing `smartcrop-0.3.3/smartcrop.py` & `smartcrop-0.3.4/smartcrop.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
         score_image = analyse_image.copy()
         score_image.thumbnail(
             (
                 int(math.ceil(image.size[0] / self.score_down_sample)),
                 int(math.ceil(image.size[1] / self.score_down_sample))
             ),
-            Image.ANTIALIAS)
+            Image.Resampling.LANCZOS)
 
         top_crop = None
         top_score = -sys.maxsize
 
         crops = self.crops(
             image,
             crop_width,
@@ -153,15 +153,15 @@
         prescale_size = 1
         if prescale:
             prescale_size = 1 / scale / min_scale
             if prescale_size < 1:
                 image = image.copy()
                 image.thumbnail(
                     (int(image.size[0] * prescale_size), int(image.size[1] * prescale_size)),
-                    Image.ANTIALIAS)
+                    Image.Resampling.LANCZOS)
                 crop_width = int(math.floor(crop_width * prescale_size))
                 crop_height = int(math.floor(crop_height * prescale_size))
             else:
                 prescale_size = 1
 
         result = self.analyse(
             image,
@@ -391,13 +391,13 @@
 
     if options.debug_file:
         analyse_image = result.pop('analyse_image')
         cropper.debug_crop(analyse_image, result['top_crop']).save(options.debug_file)
         print(json.dumps(result))
 
     cropped_image = image.crop(box)
-    cropped_image.thumbnail((options.width, options.height), Image.ANTIALIAS)
+    cropped_image.thumbnail((options.width, options.height), Image.Resampling.LANCZOS)
     cropped_image.save(options.outputfile, 'JPEG', quality=90)
 
 
 if __name__ == '__main__':
     main()
```

