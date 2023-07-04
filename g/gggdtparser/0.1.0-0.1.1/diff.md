# Comparing `tmp/gggdtparser-0.1.0.tar.gz` & `tmp/gggdtparser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gggdtparser-0.1.0.tar", last modified: Mon Jun 19 03:16:00 2023, max compression
+gzip compressed data, was "gggdtparser-0.1.1.tar", last modified: Tue Jul  4 07:37:37 2023, max compression
```

## Comparing `gggdtparser-0.1.0.tar` & `gggdtparser-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:16:00.253761 gggdtparser-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3404 2023-06-19 03:16:00.254760 gggdtparser-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 03:16:00.211414 gggdtparser-0.1.0/gggdtparser/
--rw-rw-rw-   0        0        0      227 2023-05-16 08:44:33.000000 gggdtparser-0.1.0/gggdtparser/__init__.py
--rw-rw-rw-   0        0        0     3260 2023-06-19 03:06:17.000000 gggdtparser-0.1.0/gggdtparser/dtconfigs.py
--rw-rw-rw-   0        0        0    17850 2023-06-19 03:07:20.000000 gggdtparser-0.1.0/gggdtparser/dtparser.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:16:00.238182 gggdtparser-0.1.0/gggdtparser/langs/
--rw-rw-rw-   0        0        0       88 2023-04-20 07:19:51.000000 gggdtparser-0.1.0/gggdtparser/langs/__init__.py
--rw-rw-rw-   0        0        0      235 2023-06-19 02:32:34.000000 gggdtparser-0.1.0/gggdtparser/langs/_id.py
--rw-rw-rw-   0        0        0      246 2023-06-19 02:32:40.000000 gggdtparser-0.1.0/gggdtparser/langs/az.py
--rw-rw-rw-   0        0        0      678 2023-06-19 02:44:22.000000 gggdtparser-0.1.0/gggdtparser/langs/de.py
--rw-rw-rw-   0        0        0     4773 2023-05-30 07:53:40.000000 gggdtparser-0.1.0/gggdtparser/langs/default.py
--rw-rw-rw-   0        0        0     3438 2023-06-19 01:52:13.000000 gggdtparser-0.1.0/gggdtparser/langs/en.py
--rw-rw-rw-   0        0        0      703 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/es.py
--rw-rw-rw-   0        0        0      943 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/fra.py
--rw-rw-rw-   0        0        0      223 2023-05-30 08:08:07.000000 gggdtparser-0.1.0/gggdtparser/langs/hi.py
--rw-rw-rw-   0        0        0      239 2023-05-30 06:33:25.000000 gggdtparser-0.1.0/gggdtparser/langs/ky.py
--rw-rw-rw-   0        0        0      345 2023-05-30 07:58:49.000000 gggdtparser-0.1.0/gggdtparser/langs/mr.py
--rw-rw-rw-   0        0        0      813 2023-06-19 02:00:07.000000 gggdtparser-0.1.0/gggdtparser/langs/ru.py
--rw-rw-rw-   0        0        0      249 2023-05-30 07:52:16.000000 gggdtparser-0.1.0/gggdtparser/langs/rw.py
--rw-rw-rw-   0        0        0      238 2023-05-30 08:00:58.000000 gggdtparser-0.1.0/gggdtparser/langs/si.py
--rw-rw-rw-   0        0        0      230 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/so.py
--rw-rw-rw-   0        0        0      329 2023-05-30 07:55:53.000000 gggdtparser-0.1.0/gggdtparser/langs/sw.py
--rw-rw-rw-   0        0        0      745 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/swe.py
--rw-rw-rw-   0        0        0      195 2023-05-30 08:05:09.000000 gggdtparser-0.1.0/gggdtparser/langs/tg.py
--rw-rw-rw-   0        0        0      300 2023-05-30 08:05:26.000000 gggdtparser-0.1.0/gggdtparser/langs/tr.py
--rw-rw-rw-   0        0        0      815 2023-06-19 02:54:06.000000 gggdtparser-0.1.0/gggdtparser/langs/uk.py
--rw-rw-rw-   0        0        0      231 2023-05-30 06:37:38.000000 gggdtparser-0.1.0/gggdtparser/langs/ur.py
--rw-rw-rw-   0        0        0      432 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/vie.py
--rw-rw-rw-   0        0        0      802 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/zh.py
--rw-rw-rw-   0        0        0      609 2023-05-25 03:05:13.000000 gggdtparser-0.1.0/gggdtparser/langs/zht.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:16:00.252781 gggdtparser-0.1.0/gggdtparser/test/
--rw-rw-rw-   0        0        0    43437 2023-05-25 04:15:16.000000 gggdtparser-0.1.0/gggdtparser/test/__init__.py
--rw-rw-rw-   0        0        0      112 2023-05-30 07:17:35.000000 gggdtparser-0.1.0/gggdtparser/test/_id.py
--rw-rw-rw-   0        0        0      829 2023-04-20 08:57:23.000000 gggdtparser-0.1.0/gggdtparser/test/az.py
--rw-rw-rw-   0        0        0      120 2023-05-30 08:08:48.000000 gggdtparser-0.1.0/gggdtparser/test/hi.py
--rw-rw-rw-   0        0        0      118 2023-05-30 06:34:41.000000 gggdtparser-0.1.0/gggdtparser/test/ky.py
--rw-rw-rw-   0        0        0      211 2023-05-30 07:59:04.000000 gggdtparser-0.1.0/gggdtparser/test/mr.py
--rw-rw-rw-   0        0        0      117 2023-05-30 07:52:38.000000 gggdtparser-0.1.0/gggdtparser/test/ru.py
--rw-rw-rw-   0        0        0      136 2023-05-30 07:52:38.000000 gggdtparser-0.1.0/gggdtparser/test/rw.py
--rw-rw-rw-   0        0        0      129 2023-05-30 08:01:52.000000 gggdtparser-0.1.0/gggdtparser/test/si.py
--rw-rw-rw-   0        0        0      158 2023-05-30 07:56:38.000000 gggdtparser-0.1.0/gggdtparser/test/sw.py
--rw-rw-rw-   0        0        0      129 2023-05-30 08:06:27.000000 gggdtparser-0.1.0/gggdtparser/test/tg.py
--rw-rw-rw-   0        0        0      127 2023-05-30 08:03:19.000000 gggdtparser-0.1.0/gggdtparser/test/tr.py
--rw-rw-rw-   0        0        0      178 2023-05-30 07:49:10.000000 gggdtparser-0.1.0/gggdtparser/test/uk.py
--rw-rw-rw-   0        0        0      140 2023-05-30 06:39:37.000000 gggdtparser-0.1.0/gggdtparser/test/ur.py
--rw-rw-rw-   0        0        0      570 2023-05-30 11:54:30.000000 gggdtparser-0.1.0/gggdtparser/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:16:00.215213 gggdtparser-0.1.0/gggdtparser.egg-info/
--rw-rw-rw-   0        0        0     3404 2023-06-19 03:16:00.000000 gggdtparser-0.1.0/gggdtparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2023-06-19 03:16:00.000000 gggdtparser-0.1.0/gggdtparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:16:00.000000 gggdtparser-0.1.0/gggdtparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-19 03:16:00.000000 gggdtparser-0.1.0/gggdtparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2023-06-19 03:16:00.255946 gggdtparser-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:37:37.704491 gggdtparser-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-07-04 07:37:37.704491 gggdtparser-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 07:37:37.665595 gggdtparser-0.1.1/gggdtparser/
+-rw-rw-rw-   0        0        0      227 2023-05-16 08:44:33.000000 gggdtparser-0.1.1/gggdtparser/__init__.py
+-rw-rw-rw-   0        0        0     3260 2023-06-19 03:06:17.000000 gggdtparser-0.1.1/gggdtparser/dtconfigs.py
+-rw-rw-rw-   0        0        0    17850 2023-06-19 03:07:20.000000 gggdtparser-0.1.1/gggdtparser/dtparser.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:37:37.691526 gggdtparser-0.1.1/gggdtparser/langs/
+-rw-rw-rw-   0        0        0       88 2023-04-20 07:19:51.000000 gggdtparser-0.1.1/gggdtparser/langs/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-06-19 02:32:34.000000 gggdtparser-0.1.1/gggdtparser/langs/_id.py
+-rw-rw-rw-   0        0        0      246 2023-06-19 02:32:40.000000 gggdtparser-0.1.1/gggdtparser/langs/az.py
+-rw-rw-rw-   0        0        0      678 2023-06-19 02:44:22.000000 gggdtparser-0.1.1/gggdtparser/langs/de.py
+-rw-rw-rw-   0        0        0     4783 2023-07-04 07:25:34.000000 gggdtparser-0.1.1/gggdtparser/langs/default.py
+-rw-rw-rw-   0        0        0     3438 2023-06-19 01:52:13.000000 gggdtparser-0.1.1/gggdtparser/langs/en.py
+-rw-rw-rw-   0        0        0      703 2023-05-25 03:05:13.000000 gggdtparser-0.1.1/gggdtparser/langs/es.py
+-rw-rw-rw-   0        0        0      950 2023-07-04 07:27:57.000000 gggdtparser-0.1.1/gggdtparser/langs/fra.py
+-rw-rw-rw-   0        0        0      223 2023-05-30 08:08:07.000000 gggdtparser-0.1.1/gggdtparser/langs/hi.py
+-rw-rw-rw-   0        0        0      239 2023-05-30 06:33:25.000000 gggdtparser-0.1.1/gggdtparser/langs/ky.py
+-rw-rw-rw-   0        0        0      345 2023-05-30 07:58:49.000000 gggdtparser-0.1.1/gggdtparser/langs/mr.py
+-rw-rw-rw-   0        0        0      813 2023-06-19 02:00:07.000000 gggdtparser-0.1.1/gggdtparser/langs/ru.py
+-rw-rw-rw-   0        0        0      249 2023-05-30 07:52:16.000000 gggdtparser-0.1.1/gggdtparser/langs/rw.py
+-rw-rw-rw-   0        0        0      238 2023-05-30 08:00:58.000000 gggdtparser-0.1.1/gggdtparser/langs/si.py
+-rw-rw-rw-   0        0        0      230 2023-05-25 03:05:13.000000 gggdtparser-0.1.1/gggdtparser/langs/so.py
+-rw-rw-rw-   0        0        0      329 2023-05-30 07:55:53.000000 gggdtparser-0.1.1/gggdtparser/langs/sw.py
+-rw-rw-rw-   0        0        0      745 2023-05-25 03:05:13.000000 gggdtparser-0.1.1/gggdtparser/langs/swe.py
+-rw-rw-rw-   0        0        0      195 2023-05-30 08:05:09.000000 gggdtparser-0.1.1/gggdtparser/langs/tg.py
+-rw-rw-rw-   0        0        0      300 2023-05-30 08:05:26.000000 gggdtparser-0.1.1/gggdtparser/langs/tr.py
+-rw-rw-rw-   0        0        0      815 2023-06-19 02:54:06.000000 gggdtparser-0.1.1/gggdtparser/langs/uk.py
+-rw-rw-rw-   0        0        0      231 2023-05-30 06:37:38.000000 gggdtparser-0.1.1/gggdtparser/langs/ur.py
+-rw-rw-rw-   0        0        0      432 2023-05-25 03:05:13.000000 gggdtparser-0.1.1/gggdtparser/langs/vie.py
+-rw-rw-rw-   0        0        0      802 2023-05-25 03:05:13.000000 gggdtparser-0.1.1/gggdtparser/langs/zh.py
+-rw-rw-rw-   0        0        0      631 2023-07-04 07:26:09.000000 gggdtparser-0.1.1/gggdtparser/langs/zht.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:37:37.703493 gggdtparser-0.1.1/gggdtparser/test/
+-rw-rw-rw-   0        0        0    43437 2023-05-25 04:15:16.000000 gggdtparser-0.1.1/gggdtparser/test/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-05-30 07:17:35.000000 gggdtparser-0.1.1/gggdtparser/test/_id.py
+-rw-rw-rw-   0        0        0      829 2023-04-20 08:57:23.000000 gggdtparser-0.1.1/gggdtparser/test/az.py
+-rw-rw-rw-   0        0        0      120 2023-05-30 08:08:48.000000 gggdtparser-0.1.1/gggdtparser/test/hi.py
+-rw-rw-rw-   0        0        0      118 2023-05-30 06:34:41.000000 gggdtparser-0.1.1/gggdtparser/test/ky.py
+-rw-rw-rw-   0        0        0      211 2023-05-30 07:59:04.000000 gggdtparser-0.1.1/gggdtparser/test/mr.py
+-rw-rw-rw-   0        0        0      117 2023-05-30 07:52:38.000000 gggdtparser-0.1.1/gggdtparser/test/ru.py
+-rw-rw-rw-   0        0        0      136 2023-05-30 07:52:38.000000 gggdtparser-0.1.1/gggdtparser/test/rw.py
+-rw-rw-rw-   0        0        0      129 2023-05-30 08:01:52.000000 gggdtparser-0.1.1/gggdtparser/test/si.py
+-rw-rw-rw-   0        0        0      158 2023-05-30 07:56:38.000000 gggdtparser-0.1.1/gggdtparser/test/sw.py
+-rw-rw-rw-   0        0        0      129 2023-05-30 08:06:27.000000 gggdtparser-0.1.1/gggdtparser/test/tg.py
+-rw-rw-rw-   0        0        0      127 2023-05-30 08:03:19.000000 gggdtparser-0.1.1/gggdtparser/test/tr.py
+-rw-rw-rw-   0        0        0      178 2023-05-30 07:49:10.000000 gggdtparser-0.1.1/gggdtparser/test/uk.py
+-rw-rw-rw-   0        0        0      140 2023-05-30 06:39:37.000000 gggdtparser-0.1.1/gggdtparser/test/ur.py
+-rw-rw-rw-   0        0        0      570 2023-05-30 11:54:30.000000 gggdtparser-0.1.1/gggdtparser/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:37:37.669584 gggdtparser-0.1.1/gggdtparser.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-07-04 07:37:37.000000 gggdtparser-0.1.1/gggdtparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2023-07-04 07:37:37.000000 gggdtparser-0.1.1/gggdtparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 07:37:37.000000 gggdtparser-0.1.1/gggdtparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 07:37:37.000000 gggdtparser-0.1.1/gggdtparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-07-04 07:37:37.705488 gggdtparser-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.1.1/setup.py
```

### Comparing `gggdtparser-0.1.0/LICENSE` & `gggdtparser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/PKG-INFO` & `gggdtparser-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.1.0
+Version: 0.1.1
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.1.0/README.md` & `gggdtparser-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/dtconfigs.py` & `gggdtparser-0.1.1/gggdtparser/dtconfigs.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/dtparser.py` & `gggdtparser-0.1.1/gggdtparser/dtparser.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/langs/de.py` & `gggdtparser-0.1.1/gggdtparser/langs/de.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/langs/default.py` & `gggdtparser-0.1.1/gggdtparser/langs/default.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<apm>am|pm)?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[分]?",
     r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<apm>am|pm)?\s*(?P<H>\d{1,2})\s*[时]?",
     r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?",
     r"^(?P<ts>\d{13})$",
     r"^(?P<ts>\d{10})$",
 
     # before
-    r"(?P<bd>\d+)\s*天\s*(前|ago)",
+    r"(?P<bd>\d+)\s*(天|日)\s*(前|ago)",
     r"(?P<bM>\d+)\s*分钟\s*(前|ago)",
     r"(?P<bH>\d+)\s*小时\s*(前|ago)",
-    r"(?P<bm>\d+)\s*(个)?月\s*(前|ago)",
+    r"(?P<bm>\d+)\s*(个|個)?月\s*(前|ago)",
     r"(?P<bY>\d+)\s*年\s*(前|ago)",
     r"(?P<bS>\d+)\s*秒\s*(前|ago)",
     r"(?P<ba>\d+)\s*周\s*(前|ago)",
     r"(?P<ba>\d+)\s*星期\s*(前|ago)",
     # in
     r"(?P<wd>\d+)\s*天内",
     r"(?P<wM>\d+)\s*分钟内",
```

### Comparing `gggdtparser-0.1.0/gggdtparser/langs/en.py` & `gggdtparser-0.1.1/gggdtparser/langs/en.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/langs/es.py` & `gggdtparser-0.1.1/gggdtparser/langs/es.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/langs/fra.py` & `gggdtparser-0.1.1/gggdtparser/langs/fra.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 SUB_TRANSLATE = [
     (r"janvier|jan\.", "1月"),
     (r"février|fev\.", "2月"),
     (r"mars\.|mars", "3月"),
     (r"avril|avr\.", "4月"),
     (r"mai\.|mai", "5月"),
     (r"juin\.|juin", "6月"),
-    (r"juillet\.|juillet", "7月"),
+    (r"juillet\.|juil\.|juillet", "7月"),
     (r"aout\.|août", "8月"),
     (r"septembre|sept\.", "9月"),
     (r"octobre|oct\.", "10月"),
     (r"novembre|nov\.", "11月"),
     (r"décembre|dec\.", "12月"),
     (r"aujourd’hui à", ""),
     (r"à l’instant", "刚刚"),
```

### Comparing `gggdtparser-0.1.0/gggdtparser/langs/ru.py` & `gggdtparser-0.1.1/gggdtparser/langs/ru.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/langs/swe.py` & `gggdtparser-0.1.1/gggdtparser/langs/swe.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/langs/uk.py` & `gggdtparser-0.1.1/gggdtparser/langs/uk.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/langs/zh.py` & `gggdtparser-0.1.1/gggdtparser/langs/zh.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/langs/zht.py` & `gggdtparser-0.1.1/gggdtparser/langs/zht.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 ]
 
 SUB_TRANSLATE = [
     (r'時', '时'),
     (r'間', '间'),
     (r'國', '国'),
     (r'鐘', '钟'),
+    (r'個', '个'),
 ]
 FUZZY_REGEX_LIST = []
```

### Comparing `gggdtparser-0.1.0/gggdtparser/test/__init__.py` & `gggdtparser-0.1.1/gggdtparser/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/test/az.py` & `gggdtparser-0.1.1/gggdtparser/test/az.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser/utils.py` & `gggdtparser-0.1.1/gggdtparser/utils.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/gggdtparser.egg-info/PKG-INFO` & `gggdtparser-0.1.1/gggdtparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.1.0
+Version: 0.1.1
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.1.0/gggdtparser.egg-info/SOURCES.txt` & `gggdtparser-0.1.1/gggdtparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.0/setup.cfg` & `gggdtparser-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6767 6474 7061 7273 6572 0d0a   = gggdtparser..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 300d  version = 0.1.0.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 310d  version = 0.1.1.
 00000030: 0a61 7574 686f 7220 3d20 6b75 7365 6e0d  .author = kusen.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6875 3131 3934 3534 3231 3936 4071 712e  hu1194542196@qq.
 00000060: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000070: 203d 20cd a8d3 c3a1 a2b1 e3bd dda1 a2d7   = .............
 00000080: bcc8 b7b5 c4d7 d6b7 fbb4 aeca b1bc e4bd  ................
 00000090: e2ce f6b9 a4be df0d 0a6c 6f6e 675f 6465  .........long_de
```

