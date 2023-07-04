# Comparing `tmp/lfinancial-0.1.6.tar.gz` & `tmp/lfinancial-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.1.6.tar", last modified: Tue Jul  4 12:48:35 2023, max compression
+gzip compressed data, was "lfinancial-0.1.7.tar", last modified: Tue Jul  4 16:04:42 2023, max compression
```

## Comparing `lfinancial-0.1.6.tar` & `lfinancial-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:48:35.658787 lfinancial-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-04 12:48:14.000000 lfinancial-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-04 12:48:35.658787 lfinancial-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-04 12:48:14.000000 lfinancial-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:48:35.654787 lfinancial-0.1.6/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 12:48:14.000000 lfinancial-0.1.6/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-04 12:48:14.000000 lfinancial-0.1.6/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-04 12:48:14.000000 lfinancial-0.1.6/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:48:35.658787 lfinancial-0.1.6/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-04 12:48:35.000000 lfinancial-0.1.6/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-04 12:48:35.000000 lfinancial-0.1.6/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:48:35.000000 lfinancial-0.1.6/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 12:48:35.000000 lfinancial-0.1.6/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 12:48:35.658787 lfinancial-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-04 12:48:14.000000 lfinancial-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:48:35.658787 lfinancial-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-04 12:48:14.000000 lfinancial-0.1.6/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:04:42.435782 lfinancial-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-04 16:04:23.000000 lfinancial-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-04 16:04:42.435782 lfinancial-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-04 16:04:23.000000 lfinancial-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:04:42.435782 lfinancial-0.1.7/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 16:04:23.000000 lfinancial-0.1.7/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-04 16:04:23.000000 lfinancial-0.1.7/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-04 16:04:23.000000 lfinancial-0.1.7/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:04:42.435782 lfinancial-0.1.7/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-04 16:04:42.000000 lfinancial-0.1.7/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-04 16:04:42.000000 lfinancial-0.1.7/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:04:42.000000 lfinancial-0.1.7/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 16:04:42.000000 lfinancial-0.1.7/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 16:04:42.435782 lfinancial-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-04 16:04:23.000000 lfinancial-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:04:42.435782 lfinancial-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-04 16:04:23.000000 lfinancial-0.1.7/tests/test_document.py
```

### Comparing `lfinancial-0.1.6/LICENSE.txt` & `lfinancial-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.6/PKG-INFO` & `lfinancial-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lfinancial-0.1.6/README.md` & `lfinancial-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.6/lfinancial/factory.py` & `lfinancial-0.1.7/lfinancial/factory.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.6/lfinancial/financial.py` & `lfinancial-0.1.7/lfinancial/financial.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 from lfinancial.factory import GeneratorFactory
 
 
 class Financial:
     def __init__(self):
         self._generator_factory = GeneratorFactory()
 
-    def _generate(self, generator_name, country):
+    def __generate(self, generator_name, country):
         generator = self._generator_factory.create_generator(generator_name)
         return generator.gen(generator_name, country)
 
     def ssn(self, country=None):
-        return self._generate("SSN", country)
+        return self.__generate("SSN", country)
 
     def id_card(self, country=None):
-        return self._generate("IDCard", country)
+        return self.__generate("IDCard", country)
 
     def passport(self, country=None):
-        return self._generate("Passport", country)
+        return self.__generate("Passport", country)
 
     def nric(self, country=None):
-        return self._generate("NRIC", country)
+        return self.__generate("NRIC", country)
 
     def my_number(self, country=None):
-        return self._generate("MyNumber", country)
+        return self.__generate("MyNumber", country)
 
     def first_name(self, country=None):
-        return self._generate("first_name", country)
+        return self.__generate("first_name", country)
 
     def middle_name(self, country=None):
-        return self._generate("middle_name", country)
+        return self.__generate("middle_name", country)
 
     def last_name(self, country=None):
-        return self._generate("last_name", country)
+        return self.__generate("last_name", country)
 
     def cn_name(self, country=None):
-        return self._generate("cn_name", country)
+        return self.__generate("cn_name", country)
 
     def kana_name(self, country=None):
-        return self._generate("kana_name", country)
+        return self.__generate("kana_name", country)
 
     def cellphone(self, country=None):
-        return self._generate("cellphone", country)
+        return self.__generate("cellphone", country)
 
     def area_code(self, country=None):
-        return self._generate("area_code", country)
+        return self.__generate("area_code", country)
 
     def high_risk_country(self, country=None):
-        return self._generate("high_risk", country)
+        return self.__generate("high_risk", country)
 
     def email(self, suffix=None):
-        return self._generate("email", suffix)
+        return self.__generate("email", suffix)
 
     def bank(self, country=None):
-        return self._generate("bank", country)
+        return self.__generate("bank", country)
 
 
 if __name__ == '__main__':
     f = Financial()
     print(f.ssn())
     print(f.id_card())
     print(f.passport())
```

### Comparing `lfinancial-0.1.6/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.1.7/lfinancial.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lfinancial-0.1.6/setup.py` & `lfinancial-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='lfinancial',
-    version='0.1.6',
+    version='0.1.7',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=['lfinancial'],
```

