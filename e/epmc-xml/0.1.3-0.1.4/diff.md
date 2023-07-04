# Comparing `tmp/epmc_xml-0.1.3.tar.gz` & `tmp/epmc_xml-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epmc_xml-0.1.3.tar", max compression
+gzip compressed data, was "epmc_xml-0.1.4.tar", max compression
```

## Comparing `epmc_xml-0.1.3.tar` & `epmc_xml-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-06-30 15:04:36.154342 epmc_xml-0.1.3/LICENSE
--rw-r--r--   0        0        0      334 2023-05-30 19:07:41.122842 epmc_xml-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-30 18:58:25.315802 epmc_xml-0.1.3/epmc_xml/__init__.py
--rw-r--r--   0        0        0     1175 2023-05-30 19:15:50.996869 epmc_xml-0.1.3/epmc_xml/article.py
--rw-r--r--   0        0        0     2936 2023-07-04 14:51:19.872921 epmc_xml-0.1.3/epmc_xml/fetch.py
--rw-r--r--   0        0        0      428 2023-07-04 14:52:12.755608 epmc_xml-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 epmc_xml-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-30 15:04:36.154342 epmc_xml-0.1.4/LICENSE
+-rw-r--r--   0        0        0      334 2023-05-30 19:07:41.122842 epmc_xml-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 18:58:25.315802 epmc_xml-0.1.4/epmc_xml/__init__.py
+-rw-r--r--   0        0        0     1175 2023-05-30 19:15:50.996869 epmc_xml-0.1.4/epmc_xml/article.py
+-rw-r--r--   0        0        0     2932 2023-07-04 15:05:21.020991 epmc_xml-0.1.4/epmc_xml/fetch.py
+-rw-r--r--   0        0        0      428 2023-07-04 15:08:26.342211 epmc_xml-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 epmc_xml-0.1.4/PKG-INFO
```

### Comparing `epmc_xml-0.1.3/LICENSE` & `epmc_xml-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `epmc_xml-0.1.3/epmc_xml/article.py` & `epmc_xml-0.1.4/epmc_xml/article.py`

 * *Files identical despite different names*

### Comparing `epmc_xml-0.1.3/epmc_xml/fetch.py` & `epmc_xml-0.1.4/epmc_xml/fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,25 +48,25 @@
         title = "".join(sec.find("./title").itertext())
         paras = sec.findall("./p")
         section_text = f"{title}\n"
         if len(paras) == 0:
             section_text += "".join(sec.itertext())
         for p in paras:
             section_text += "".join(p.itertext())
-            section_text += "\n\n"
+            section_text += "\n"
         ## find all subsections
         for subsec in sec.findall("./sec"):
             subsection_heading = subsec.find("./title")
             subsection_paras = subsec.findall("./p")
             if subsection_heading is not None:
                 section_text += "".join(subsection_heading.itertext())
             section_text += "".join(
                 ["".join(para.itertext()) for para in subsection_paras]
             )
-            section_text += "\n\n"
+            section_text += "\n"
 
         section_dict[title] = section_text
 
     return section_dict
 
 
 def get_author_list(xml_article):
```

### Comparing `epmc_xml-0.1.3/PKG-INFO` & `epmc_xml-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epmc-xml
-Version: 0.1.3
+Version: 0.1.4
 Summary: Get articles from Europe PMC as xml for further processing
 License: MIT
 Author: Andrew Green
 Author-email: a.f.green1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

