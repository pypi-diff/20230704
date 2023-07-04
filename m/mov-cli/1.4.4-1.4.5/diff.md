# Comparing `tmp/mov_cli-1.4.4.tar.gz` & `tmp/mov_cli-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.4.4.tar", max compression
+gzip compressed data, was "mov_cli-1.4.5.tar", max compression
```

## Comparing `mov_cli-1.4.4.tar` & `mov_cli-1.4.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    35149 2023-06-23 09:33:09.736703 mov_cli-1.4.4/LICENSE
--rw-r--r--   0        0        0     7144 2023-06-23 09:33:09.736703 mov_cli-1.4.4/README.md
--rw-r--r--   0        0        0      235 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/__init__.py
--rw-r--r--   0        0        0     2617 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/__main__.py
--rw-r--r--   0        0        0        1 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      823 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      958 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      457 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      318 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0        0 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     2559 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/players/player.py
--rw-r--r--   0        0        0        0 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     1484 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/utils/dbs.py
--rw-r--r--   0        0        0     2731 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0     6133 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/utils/jsunpack.py
--rw-r--r--   0        0        0     2269 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1584 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/utils/player.py
--rw-r--r--   0        0        0      958 2023-06-23 09:33:09.736703 mov_cli-1.4.4/mov_cli/utils/provider.py
--rw-r--r--   0        0        0     8708 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0        0 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0    10970 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/actvid.py
--rw-r--r--   0        0        0     4177 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/animefox.py
--rw-r--r--   0        0        0     4208 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/dopebox.py
--rw-r--r--   0        0        0     1943 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/einthusan.py
--rw-r--r--   0        0        0     1724 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/eja.py
--rw-r--r--   0        0        0     3210 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/gogoanime.py
--rw-r--r--   0        0        0     3736 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/kisscartoon.py
--rw-r--r--   0        0        0     2509 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/openloadmov.py
--rw-r--r--   0        0        0     2563 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/redundant_kimcartoon.py
--rw-r--r--   0        0        0     4662 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/remotestream.py
--rw-r--r--   0        0        0     4422 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/scdn.py
--rw-r--r--   0        0        0     4217 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/sflix.py
--rw-r--r--   0        0        0     1644 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/solar.py
--rw-r--r--   0        0        0     2132 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/streamblasters.py
--rw-r--r--   0        0        0     1358 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/tamilyogi.py
--rw-r--r--   0        0        0     2895 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/turkish123.py
--rw-r--r--   0        0        0     4516 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/viewasian.py
--rw-r--r--   0        0        0     3395 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/watchasian.py
--rw-r--r--   0        0        0     3983 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/wlext.py
--rw-r--r--   0        0        0     3503 2023-06-23 09:33:09.740703 mov_cli-1.4.4/mov_cli/websites/yoturkish.py
--rw-r--r--   0        0        0      731 2023-06-23 09:33:09.740703 mov_cli-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     8127 1970-01-01 00:00:00.000000 mov_cli-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 17:42:07.620723 mov_cli-1.4.5/LICENSE
+-rw-r--r--   0        0        0     7112 2023-07-04 17:42:07.620723 mov_cli-1.4.5/README.md
+-rw-r--r--   0        0        0      235 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/__init__.py
+-rw-r--r--   0        0        0     2612 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/__main__.py
+-rw-r--r--   0        0        0        1 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      823 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      958 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      457 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      318 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     2559 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/players/player.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     1484 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/dbs.py
+-rw-r--r--   0        0        0     2715 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0     6133 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/jsunpack.py
+-rw-r--r--   0        0        0     2269 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1584 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/player.py
+-rw-r--r--   0        0        0      958 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/provider.py
+-rw-r--r--   0        0        0     8708 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0        0 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0    10970 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/actvid.py
+-rw-r--r--   0        0        0     4177 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/animefox.py
+-rw-r--r--   0        0        0     4208 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/dopebox.py
+-rw-r--r--   0        0        0     1943 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/einthusan.py
+-rw-r--r--   0        0        0     1724 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/eja.py
+-rw-r--r--   0        0        0     3210 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/gogoanime.py
+-rw-r--r--   0        0        0     3736 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/kisscartoon.py
+-rw-r--r--   0        0        0     2509 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/openloadmov.py
+-rw-r--r--   0        0        0     2563 2023-07-04 17:42:07.620723 mov_cli-1.4.5/mov_cli/websites/redundant_kimcartoon.py
+-rw-r--r--   0        0        0     4662 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/remotestream.py
+-rw-r--r--   0        0        0     4422 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/scdn.py
+-rw-r--r--   0        0        0     4217 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/sflix.py
+-rw-r--r--   0        0        0     1644 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/solar.py
+-rw-r--r--   0        0        0     2132 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/streamblasters.py
+-rw-r--r--   0        0        0     1358 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/tamilyogi.py
+-rw-r--r--   0        0        0     2895 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/turkish123.py
+-rw-r--r--   0        0        0     4516 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/viewasian.py
+-rw-r--r--   0        0        0     3395 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/watchasian.py
+-rw-r--r--   0        0        0     3983 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/wlext.py
+-rw-r--r--   0        0        0     3503 2023-07-04 17:42:07.624723 mov_cli-1.4.5/mov_cli/websites/yoturkish.py
+-rw-r--r--   0        0        0      731 2023-07-04 17:42:07.624723 mov_cli-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     8095 1970-01-01 00:00:00.000000 mov_cli-1.4.5/PKG-INFO
```

### Comparing `mov_cli-1.4.4/LICENSE` & `mov_cli-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/README.md` & `mov_cli-1.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,17 @@
   </li>
   <li>
     <a href="#getting-started">Getting Started</a>
     <ul>
       <li><a href="#prerequisites">Prerequisites</a></li>
       <li><a href="#installation">Installation</a></li>
       <ul>
-        <li><a href="#win-and-linux">Windows / Linux</a></li>
-        <ul>
-          <li><a href="#linux">Linux</a></li>
-        </ul>
+        <li><a href="#windows--linux">Windows / Linux</a></li>
         <li><a href="#android">Android</a></li>
+        <li><a href="#ios">iOS</a></li>
       </ul>
     </ul>
   </li>
   <li><a href="#usage">Usage</a></li>
   <li><a href="#disclaimer">Disclaimer</a></li>
   <li><a href="#contributing">Contributing</a></li>
   <li><a href="#add-a-language">Adding Languages</a></li>
```

#### html2text {}

```diff
@@ -6,16 +6,16 @@
                          Report_Bug Â· Request_Feature
  ### Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Prerequisites
           o Installation
                 # Windows_/_Linux
-                      # Linux
                 # Android
+                # iOS
    3. Usage
    4. Disclaimer
    5. Contributing
    6. Adding_Languages
    7. License
    8. Contact
    9. inspiration
```

### Comparing `mov_cli-1.4.4/mov_cli/__main__.py` & `mov_cli-1.4.5/mov_cli/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # "kimcartoon": [kimcartoon, "https://kimcartoon.li"],
     "actvid": [actvid, "https://www.actvid.com"],
     "sflix": [sflix, "https://sflix.se"],
     "solar": [solar, "https://solarmovie.pe"],
     "dopebox": [dopebox, "https://dopebox.to"],
     "viewasian": [viewasian, "https://viewasian.co"],
     "gogoanime": [gogoanime, "https://gogoanime.hu"],
-    "watchasian": [watchasian, "https://www1.watchasian.id"],
+    "watchasian": [watchasian, "https://watchasian.mx"],
     "wlext": [wlext, "https://wlext.is"],
     "streamblasters": [streamblasters, "https://streamblasters.pro"],
     "tamilyogi": [tamilyogi, "https://tamilyogi.bike"],
     "einthusan": [einthusan, "https://einthusan.tv"],
     "turkish123": [turkish123, "https://turkish123.ac"],
     "animefox": [animefox, "https://animefox.to"],
     "scdn": [scdn, ""],
```

### Comparing `mov_cli-1.4.4/mov_cli/extractors/doodstream.py` & `mov_cli-1.4.5/mov_cli/extractors/doodstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.4.5/mov_cli/extractors/scdn/cr7sports.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.4.5/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.4.5/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.4.5/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.4.5/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.4.5/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/players/player.py` & `mov_cli-1.4.5/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/utils/dbs.py` & `mov_cli-1.4.5/mov_cli/utils/dbs.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/utils/httpclient.py` & `mov_cli-1.4.5/mov_cli/utils/httpclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,53 +20,53 @@
         print(page)
         try:
             req = self.session.get(page, follow_redirects=redirects)
             self.session.headers["Referer"] = page
         except Exception as e:
             print(
                 f"Error: {e}",
-                "\n Please open an issue if this is not due due to your internet connection",
+                "\n Please open an issue if this is not due to your internet connection",
             )
             sys.exit(-1)
         return req
 
     def post(self, page: str, data: dict = None, json=None) -> httpx.Response:
         print(page)
         if json is None:
             try:
                 req = self.session.post(page, data=data)
                 self.session.headers["Referer"] = page
             except Exception as e:
                 print(
                     f"Error: {e}",
-                    "\n Please open an issue if this is not due due to your internet connection",
+                    "\n Please open an issue if this is not due to your internet connection",
                 )
                 sys.exit(-1)
             return req
         else:
             try:
                 req = self.session.post(page, json=json)
                 self.session.headers["Referer"] = page
             except Exception as e:
                 print(
                     f"Error: {e}",
-                    "\n Please open an issue if this is not due due to your internet connection",
+                    "\n Please open an issue if this is not due to your internet connection",
                 )
                 sys.exit(-1)
             return req
 
     def head(self, page: str, redirects: False) -> httpx.Response:
         print(page)
         try:
             req = self.session.head(page, follow_redirects=redirects)
             self.session.headers["Referer"] = page
         except Exception as e:
             print(
                 f"Error: {e}",
-                "\n Please open an issue if this is not due due to your internet connection",
+                "\n Please open an issue if this is not due to your internet connection",
             )
             sys.exit(-1)
         return req
 
     def set_headers(self, header: dict) -> None:
         self.session.headers = header
         # do not use this!w
```

### Comparing `mov_cli-1.4.4/mov_cli/utils/jsunpack.py` & `mov_cli-1.4.5/mov_cli/utils/jsunpack.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/utils/lang.py` & `mov_cli-1.4.5/mov_cli/utils/lang.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/utils/player.py` & `mov_cli-1.4.5/mov_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/utils/provider.py` & `mov_cli-1.4.5/mov_cli/utils/provider.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/utils/scraper.py` & `mov_cli-1.4.5/mov_cli/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/actvid.py` & `mov_cli-1.4.5/mov_cli/websites/actvid.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/animefox.py` & `mov_cli-1.4.5/mov_cli/websites/animefox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/dopebox.py` & `mov_cli-1.4.5/mov_cli/websites/dopebox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/einthusan.py` & `mov_cli-1.4.5/mov_cli/websites/einthusan.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/eja.py` & `mov_cli-1.4.5/mov_cli/websites/eja.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/gogoanime.py` & `mov_cli-1.4.5/mov_cli/websites/gogoanime.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/kisscartoon.py` & `mov_cli-1.4.5/mov_cli/websites/kisscartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/openloadmov.py` & `mov_cli-1.4.5/mov_cli/websites/openloadmov.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/redundant_kimcartoon.py` & `mov_cli-1.4.5/mov_cli/websites/redundant_kimcartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/remotestream.py` & `mov_cli-1.4.5/mov_cli/websites/remotestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/scdn.py` & `mov_cli-1.4.5/mov_cli/websites/scdn.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/sflix.py` & `mov_cli-1.4.5/mov_cli/websites/sflix.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/solar.py` & `mov_cli-1.4.5/mov_cli/websites/solar.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/streamblasters.py` & `mov_cli-1.4.5/mov_cli/websites/streamblasters.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/tamilyogi.py` & `mov_cli-1.4.5/mov_cli/websites/tamilyogi.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/turkish123.py` & `mov_cli-1.4.5/mov_cli/websites/turkish123.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/viewasian.py` & `mov_cli-1.4.5/mov_cli/websites/viewasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/watchasian.py` & `mov_cli-1.4.5/mov_cli/websites/watchasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/wlext.py` & `mov_cli-1.4.5/mov_cli/websites/wlext.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/mov_cli/websites/yoturkish.py` & `mov_cli-1.4.5/mov_cli/websites/yoturkish.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.4/pyproject.toml` & `mov_cli-1.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.4.4"
+version = "1.4.5"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports."
 authors = ["Pain <painedposeidon444@gmail.com>"]
 maintainers = ["Ananas <ananas@ad1hl.xyz>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
```

### Comparing `mov_cli-1.4.4/PKG-INFO` & `mov_cli-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 1.4.4
+Version: 1.4.5
 Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
 Home-page: https://github.com/mov-cli/mov-cli
 License: GPLv3
 Author: Pain
 Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas
 Maintainer-email: ananas@ad1hl.xyz
@@ -75,19 +75,17 @@
   </li>
   <li>
     <a href="#getting-started">Getting Started</a>
     <ul>
       <li><a href="#prerequisites">Prerequisites</a></li>
       <li><a href="#installation">Installation</a></li>
       <ul>
-        <li><a href="#win-and-linux">Windows / Linux</a></li>
-        <ul>
-          <li><a href="#linux">Linux</a></li>
-        </ul>
+        <li><a href="#windows--linux">Windows / Linux</a></li>
         <li><a href="#android">Android</a></li>
+        <li><a href="#ios">iOS</a></li>
       </ul>
     </ul>
   </li>
   <li><a href="#usage">Usage</a></li>
   <li><a href="#disclaimer">Disclaimer</a></li>
   <li><a href="#contributing">Contributing</a></li>
   <li><a href="#add-a-language">Adding Languages</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.4.4 Summary: A cli tool to
+Metadata-Version: 2.1 Name: mov-cli Version: 1.4.5 Summary: A cli tool to
 browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
 mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas Maintainer-email: ananas@ad1hl.xyz Requires-Python:
 >=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
@@ -19,16 +19,16 @@
                          Report_Bug Â· Request_Feature
  ### Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Prerequisites
           o Installation
                 # Windows_/_Linux
-                      # Linux
                 # Android
+                # iOS
    3. Usage
    4. Disclaimer
    5. Contributing
    6. Adding_Languages
    7. License
    8. Contact
    9. inspiration
```

