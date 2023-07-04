# Comparing `tmp/linkedin_scraper-2.9.1.tar.gz` & `tmp/linkedin_scraper-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linkedin_scraper-2.9.1.tar", last modified: Wed Nov  2 09:13:11 2022, max compression
+gzip compressed data, was "dist/linkedin_scraper-2.9.2.tar", last modified: Mon Feb 13 11:36:19 2023, max compression
```

## Comparing `linkedin_scraper-2.9.1.tar` & `linkedin_scraper-2.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 joey      (1001) joey      (1001)        0 2022-11-02 09:13:11.000000 linkedin_scraper-2.9.1/
--rw-rw-r--   0 joey      (1001) joey      (1001)     7326 2022-11-02 09:13:11.000000 linkedin_scraper-2.9.1/PKG-INFO
--rw-rw-r--   0 joey      (1001) joey      (1001)     1175 2022-11-01 15:03:45.000000 linkedin_scraper-2.9.1/setup.py
--rw-rw-r--   0 joey      (1001) joey      (1001)    35149 2022-11-01 15:03:45.000000 linkedin_scraper-2.9.1/LICENSE
--rw-rw-r--   0 joey      (1001) joey      (1001)     7912 2022-11-01 15:03:45.000000 linkedin_scraper-2.9.1/README.rst
-drwxrwxr-x   0 joey      (1001) joey      (1001)        0 2022-11-02 09:13:11.000000 linkedin_scraper-2.9.1/linkedin_scraper.egg-info/
--rw-rw-r--   0 joey      (1001) joey      (1001)        1 2022-11-02 09:13:11.000000 linkedin_scraper-2.9.1/linkedin_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 joey      (1001) joey      (1001)     7326 2022-11-02 09:13:11.000000 linkedin_scraper-2.9.1/linkedin_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 joey      (1001) joey      (1001)      436 2022-11-02 09:13:11.000000 linkedin_scraper-2.9.1/linkedin_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 joey      (1001) joey      (1001)       17 2022-11-02 09:13:11.000000 linkedin_scraper-2.9.1/linkedin_scraper.egg-info/top_level.txt
--rw-rw-r--   0 joey      (1001) joey      (1001)       23 2022-11-02 09:13:11.000000 linkedin_scraper-2.9.1/linkedin_scraper.egg-info/requires.txt
--rw-rw-r--   0 joey      (1001) joey      (1001)       80 2022-11-02 09:13:11.000000 linkedin_scraper-2.9.1/setup.cfg
-drwxrwxr-x   0 joey      (1001) joey      (1001)        0 2022-11-02 09:13:11.000000 linkedin_scraper-2.9.1/linkedin_scraper/
--rw-rw-r--   0 joey      (1001) joey      (1001)       91 2022-11-01 15:03:45.000000 linkedin_scraper-2.9.1/linkedin_scraper/constants.py
--rw-rw-r--   0 joey      (1001) joey      (1001)     1509 2022-11-01 15:07:03.000000 linkedin_scraper-2.9.1/linkedin_scraper/actions.py
--rw-rw-r--   0 joey      (1001) joey      (1001)       29 2022-11-01 15:03:45.000000 linkedin_scraper-2.9.1/linkedin_scraper/selectors.py
--rw-rw-r--   0 joey      (1001) joey      (1001)    15709 2022-11-01 15:07:03.000000 linkedin_scraper-2.9.1/linkedin_scraper/company.py
--rw-rw-r--   0 joey      (1001) joey      (1001)      344 2022-11-02 09:12:06.000000 linkedin_scraper-2.9.1/linkedin_scraper/__init__.py
--rw-rw-r--   0 joey      (1001) joey      (1001)    16621 2022-11-01 15:17:06.000000 linkedin_scraper-2.9.1/linkedin_scraper/person.py
--rw-rw-r--   0 joey      (1001) joey      (1001)     1977 2022-11-01 15:07:03.000000 linkedin_scraper-2.9.1/linkedin_scraper/objects.py
+drwxrwxr-x   0 joey      (1001) joey      (1001)        0 2023-02-13 11:36:19.000000 linkedin_scraper-2.9.2/
+-rw-rw-r--   0 joey      (1001) joey      (1001)     7326 2023-02-13 11:36:19.000000 linkedin_scraper-2.9.2/PKG-INFO
+-rw-rw-r--   0 joey      (1001) joey      (1001)     1175 2022-11-01 15:03:45.000000 linkedin_scraper-2.9.2/setup.py
+-rw-rw-r--   0 joey      (1001) joey      (1001)    35149 2022-11-01 15:03:45.000000 linkedin_scraper-2.9.2/LICENSE
+-rw-rw-r--   0 joey      (1001) joey      (1001)     7912 2022-11-01 15:03:45.000000 linkedin_scraper-2.9.2/README.rst
+drwxrwxr-x   0 joey      (1001) joey      (1001)        0 2023-02-13 11:36:19.000000 linkedin_scraper-2.9.2/linkedin_scraper.egg-info/
+-rw-rw-r--   0 joey      (1001) joey      (1001)        1 2023-02-13 11:36:19.000000 linkedin_scraper-2.9.2/linkedin_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 joey      (1001) joey      (1001)     7326 2023-02-13 11:36:19.000000 linkedin_scraper-2.9.2/linkedin_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 joey      (1001) joey      (1001)      436 2023-02-13 11:36:19.000000 linkedin_scraper-2.9.2/linkedin_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 joey      (1001) joey      (1001)       17 2023-02-13 11:36:19.000000 linkedin_scraper-2.9.2/linkedin_scraper.egg-info/top_level.txt
+-rw-rw-r--   0 joey      (1001) joey      (1001)       23 2023-02-13 11:36:19.000000 linkedin_scraper-2.9.2/linkedin_scraper.egg-info/requires.txt
+-rw-rw-r--   0 joey      (1001) joey      (1001)       80 2023-02-13 11:36:19.000000 linkedin_scraper-2.9.2/setup.cfg
+drwxrwxr-x   0 joey      (1001) joey      (1001)        0 2023-02-13 11:36:19.000000 linkedin_scraper-2.9.2/linkedin_scraper/
+-rw-rw-r--   0 joey      (1001) joey      (1001)       98 2023-02-13 11:22:47.000000 linkedin_scraper-2.9.2/linkedin_scraper/constants.py
+-rw-rw-r--   0 joey      (1001) joey      (1001)     1509 2022-11-01 15:07:03.000000 linkedin_scraper-2.9.2/linkedin_scraper/actions.py
+-rw-rw-r--   0 joey      (1001) joey      (1001)       29 2022-11-01 15:03:45.000000 linkedin_scraper-2.9.2/linkedin_scraper/selectors.py
+-rw-rw-r--   0 joey      (1001) joey      (1001)    15709 2022-11-01 15:07:03.000000 linkedin_scraper-2.9.2/linkedin_scraper/company.py
+-rw-rw-r--   0 joey      (1001) joey      (1001)      344 2023-02-13 11:36:07.000000 linkedin_scraper-2.9.2/linkedin_scraper/__init__.py
+-rw-rw-r--   0 joey      (1001) joey      (1001)    16657 2022-11-15 17:43:04.000000 linkedin_scraper-2.9.2/linkedin_scraper/person.py
+-rw-rw-r--   0 joey      (1001) joey      (1001)     1986 2023-02-13 11:35:15.000000 linkedin_scraper-2.9.2/linkedin_scraper/objects.py
```

### Comparing `linkedin_scraper-2.9.1/PKG-INFO` & `linkedin_scraper-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: linkedin_scraper
-Version: 2.9.1
+Version: 2.9.2
 Summary: Scrapes user data from Linkedin
 Home-page: https://github.com/joeyism/linkedin_scraper
 Author: Joey Sham
 Author-email: sham.joey@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/joeyism/linkedin_scraper/dist/2.9.1.tar.gz
+Download-URL: https://github.com/joeyism/linkedin_scraper/dist/2.9.2.tar.gz
 Keywords: linkedin,scraping,scraper
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Linkedin Scraper
```

### Comparing `linkedin_scraper-2.9.1/setup.py` & `linkedin_scraper-2.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `linkedin_scraper-2.9.1/LICENSE` & `linkedin_scraper-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linkedin_scraper-2.9.1/README.rst` & `linkedin_scraper-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `linkedin_scraper-2.9.1/linkedin_scraper.egg-info/PKG-INFO` & `linkedin_scraper-2.9.2/linkedin_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: linkedin-scraper
-Version: 2.9.1
+Version: 2.9.2
 Summary: Scrapes user data from Linkedin
 Home-page: https://github.com/joeyism/linkedin_scraper
 Author: Joey Sham
 Author-email: sham.joey@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/joeyism/linkedin_scraper/dist/2.9.1.tar.gz
+Download-URL: https://github.com/joeyism/linkedin_scraper/dist/2.9.2.tar.gz
 Keywords: linkedin,scraping,scraper
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Linkedin Scraper
```

### Comparing `linkedin_scraper-2.9.1/linkedin_scraper/actions.py` & `linkedin_scraper-2.9.2/linkedin_scraper/actions.py`

 * *Files identical despite different names*

### Comparing `linkedin_scraper-2.9.1/linkedin_scraper/company.py` & `linkedin_scraper-2.9.2/linkedin_scraper/company.py`

 * *Files identical despite different names*

### Comparing `linkedin_scraper-2.9.1/linkedin_scraper/person.py` & `linkedin_scraper-2.9.2/linkedin_scraper/person.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         company=None,
         job_title=None,
         contacts=None,
         driver=None,
         get=True,
         scrape=True,
         close_on_complete=True,
+        time_to_wait_after_login=0,
     ):
         self.linkedin_url = linkedin_url
         self.name = name
         self.about = about or []
         self.experiences = experiences or []
         self.educations = educations or []
         self.interests = interests or []
```

### Comparing `linkedin_scraper-2.9.1/linkedin_scraper/objects.py` & `linkedin_scraper-2.9.2/linkedin_scraper/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 @dataclass
 class Scraper:
     driver: Chrome = None
 
     def is_signed_in(self):
         try:
-            self.driver.find_element(By.ID,c.VERIFY_LOGIN_ID)
+            self.driver.find_element(By.CLASS_NAME, c.VERIFY_LOGIN_ID)
             return True
         except:
             pass
         return False
 
     def __find_element_by_class_name__(self, class_name):
         try:
```

