# Comparing `tmp/acdh_xml_pyutils-0.4.0.tar.gz` & `tmp/acdh_xml_pyutils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdh_xml_pyutils-0.4.0.tar", last modified: Mon Apr 12 09:05:12 2021, max compression
+gzip compressed data, was "acdh_xml_pyutils-0.4.1.tar", last modified: Tue Jul  4 13:36:13 2023, max compression
```

## Comparing `acdh_xml_pyutils-0.4.0.tar` & `acdh_xml_pyutils-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 09:05:12.578831 acdh_xml_pyutils-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2021-04-12 09:05:12.578831 acdh_xml_pyutils-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 09:05:12.574830 acdh_xml_pyutils-0.4.0/acdh_xml_pyutils/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/acdh_xml_pyutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3540 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/acdh_xml_pyutils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 09:05:12.574830 acdh_xml_pyutils-0.4.0/acdh_xml_pyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2021-04-12 09:05:12.000000 acdh_xml_pyutils-0.4.0/acdh_xml_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-04-12 09:05:12.000000 acdh_xml_pyutils-0.4.0/acdh_xml_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-12 09:05:12.000000 acdh_xml_pyutils-0.4.0/acdh_xml_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-12 09:05:12.000000 acdh_xml_pyutils-0.4.0/acdh_xml_pyutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-04-12 09:05:12.000000 acdh_xml_pyutils-0.4.0/acdh_xml_pyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-04-12 09:05:12.000000 acdh_xml_pyutils-0.4.0/acdh_xml_pyutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 09:05:12.574830 acdh_xml_pyutils-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      351 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/acdh_xml_pyutils.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4815 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      324 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-04-12 09:05:12.578831 acdh_xml_pyutils-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 09:05:12.578831 acdh_xml_pyutils-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/tests/test.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     3926 2021-04-12 09:05:02.000000 acdh_xml_pyutils-0.4.0/tests/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:36:13.527229 acdh_xml_pyutils-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-04 13:36:13.527229 acdh_xml_pyutils-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:36:13.523229 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:36:13.527229 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils/files/tei _no_xml_decl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils/files/tei.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils/files/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:36:13.527229 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-04 13:36:13.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-04 13:36:13.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:36:13.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:36:13.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 13:36:13.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 13:36:13.000000 acdh_xml_pyutils-0.4.1/acdh_xml_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:36:13.527229 acdh_xml_pyutils-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:36:13.527229 acdh_xml_pyutils-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/tests/test.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-04 13:36:02.000000 acdh_xml_pyutils-0.4.1/tests/test_xml.py
```

### Comparing `acdh_xml_pyutils-0.4.0/LICENSE` & `acdh_xml_pyutils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acdh_xml_pyutils-0.4.0/acdh_xml_pyutils/xml.py` & `acdh_xml_pyutils-0.4.1/acdh_xml_pyutils/xml.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,109 +2,107 @@
 import datetime
 import requests
 import lxml.etree as ET
 
 from collections import Counter
 
 
-class XMLReader():
+class XMLReader:
 
-    """ Class to parse, preprocess and save XML/TEI
+    """Class to parse, preprocess and save XML/TEI
 
     :param xml: An XML Document, either a File Path, an URL to an XML or an XML string
     :type xml: str
 
     :return: A XMLReader instance
     :rtype: `xml.XMLReader`
 
     """
 
     def __init__(self, xml=None, xsl=None):
-
-        """ initializes the class
+        """initializes the class
 
         :param xml: An XML Document, either a File Path, an URL to an XML or an XML string
         :type xml: str
 
         :param xsl: Path to an XSL Stylesheet
         :type xsl: str
 
         :return: A XMLReader instance
         :rtype: `xml.XMLReader`
 
         """
-        self.ns_tei = {'tei': "http://www.tei-c.org/ns/1.0"}
-        self.ns_xml = {'xml': "http://www.w3.org/XML/1998/namespace"}
-        self.ns_tcf = {'tcf': "http://www.dspin.de/data/textcorpus"}
+        self.ns_tei = {"tei": "http://www.tei-c.org/ns/1.0"}
+        self.ns_xml = {"xml": "http://www.w3.org/XML/1998/namespace"}
+        self.ns_tcf = {"tcf": "http://www.dspin.de/data/textcorpus"}
         self.nsmap = {
-            'tei': "http://www.tei-c.org/ns/1.0",
-            'xml': "http://www.w3.org/XML/1998/namespace",
-            'tcf': "http://www.dspin.de/data/textcorpus"
+            "tei": "http://www.tei-c.org/ns/1.0",
+            "xml": "http://www.w3.org/XML/1998/namespace",
+            "tcf": "http://www.dspin.de/data/textcorpus",
         }
         self.file = xml.strip()
         if xsl:
             self.xsl = ET.parse(xsl)
         else:
             self.xsl = None
-        if self.file.startswith('http'):
+        if self.file.startswith("http"):
             r = requests.get(
                 self.file,
                 headers={
-                    'Content-type': 'application/xml; charset=utf-8',
-                    'Accept-Charset': 'utf-8'
-                    }
-                )
+                    "Content-type": "application/xml; charset=utf-8",
+                    "Accept-Charset": "utf-8",
+                },
+            )
             try:
-                self.original = ET.fromstring(r.content.decode('utf-8'))
+                self.original = ET.fromstring(r.content.decode("utf-8"))
             except ValueError:
-                self.original = ET.fromstring(r.content.decode('utf-8').encode('utf-8'))
-        elif self.file.startswith('<'):
+                self.original = ET.fromstring(r.content.decode("utf-8").encode("utf-8"))
+        elif self.file.startswith("<"):
             try:
                 self.original = ET.parse(self.file)
             except OSError:
-                self.original = ET.fromstring(self.file.encode('utf8'))
+                self.original = ET.fromstring(self.file.encode("utf8"))
         else:
             self.original = ET.parse(self.file)
         self.tree = self.original
         if self.xsl:
             transform = ET.XSLT(self.xsl)
             self.tree = transform(self.tree)
 
     def get_elements(self):
-        """ returns a list of all element names of the current tree
+        """returns a list of all element names of the current tree
 
         :return: A list of all element names
         :rtype: list
 
         """
         all_elements = [element.tag for element in self.tree.iter()]
         return all_elements
 
     def get_element_stats(self):
-        """ returns a `collections.Counter` object holding element count
+        """returns a `collections.Counter` object holding element count
 
         :return: A list of all element names
         :rtype: `collections.Counter`
         """
         return Counter(self.get_elements())
 
     def return_byte_like_object(self):
-        """ returns current doc as byte like object"""
+        """returns current doc as byte like object"""
 
         return ET.tostring(self.tree, encoding="utf-8")
 
     def return_string(self):
-
         """
         returns current doc as string
 
         :rtype: str
 
         """
-        return self.return_byte_like_object().decode('utf-8')
+        return self.return_byte_like_object().decode("utf-8")
 
     def tree_to_file(self, file=None):
         """
         saves current tree to file
 
         :param file: A filename/location to save the current doc
         :type file: str
@@ -112,13 +110,15 @@
         :return: The save-location
         :rtype: str
 
         """
         if file:
             pass
         else:
-            timestamp = datetime.datetime.fromtimestamp(time.time()).strftime('%Y-%m-%d-%H-%M-%S')
+            timestamp = datetime.datetime.fromtimestamp(time.time()).strftime(
+                "%Y-%m-%d-%H-%M-%S"
+            )
             file = "{}.xml".format(timestamp)
 
-        with open(file, 'wb') as f:
+        with open(file, "wb") as f:
             f.write(ET.tostring(self.tree, encoding="UTF-8"))
         return file
```

### Comparing `acdh_xml_pyutils-0.4.0/setup.py` & `acdh_xml_pyutils-0.4.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,27 +19,20 @@
                     file_list.add(os.path.join(dname, f))
     finally:
         os.chdir(cur_dir)
 
     return list(file_list)
 
 
-with open('README.rst') as readme_file:
+with open('README.md') as readme_file:
     readme = readme_file.read()
 
-with open('CHANGELOG.rst') as history_file:
-    history = history_file.read()
-
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
-setup_requirements = ['pytest-runner', ]
-
-test_requirements = ['pytest>=3', ]
-
 setup(
     author="Peter Andorfer",
     author_email='peter.andorfer@oeaw.ac.at',
     python_requires='>=3.7',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
@@ -48,25 +41,23 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     description="Utility functions to work with XML",
     install_requires=requirements,
     license="MIT",
-    long_description=readme + '\n\n' + history,
+    long_description=readme,
+    long_description_content_type="text/markdown",
     include_package_data=True,
     keywords='acdh_xml_pyutils',
     name='acdh_xml_pyutils',
     packages=find_packages(include=['acdh_xml_pyutils', 'acdh_xml_pyutils.*']),
     package_data={
         module.__name__: walker(
             os.path.dirname(module.__file__),
             'files'
         ),
     },
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
     url='https://github.com/acdh-oeaw/acdh_xml_pyutils',
-    version='0.4.0',
+    version='0.4.1',
     zip_safe=False,
 )
```

### Comparing `acdh_xml_pyutils-0.4.0/tests/test_xml.py` & `acdh_xml_pyutils-0.4.1/tests/test_xml.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,26 @@
 import os
 import unittest
 
 import collections
 
 from acdh_xml_pyutils.xml import XMLReader
 
-FILES = glob.glob(
-    "./acdh_xml_pyutils/files/*.xml",
-    recursive=False
-)
+FILES = glob.glob("./acdh_xml_pyutils/files/*.xml", recursive=False)
 
 # XML_URL = "https://id.acdh.oeaw.ac.at/thun/editions/szeberinyi-an-thun-1859-11-29-a3-xxi-d529.xml?format=raw"
 
 XML_URLS = [
     "https://id.acdh.oeaw.ac.at/thun/editions/szeberinyi-an-thun-1859-11-29-a3-xxi-d529.xml?format=raw",
-    "https://raw.githubusercontent.com/bleierr/NERDPool/main/RTA_1576/HStA_Dresden_Loc10199_4_fol265_1576-07-15.xml",
-    "https://raw.githubusercontent.com/KONDE-AT/thun-data/master/editions/ansichten-ueber-waisenvermoegen-von-walter-1857-08-22-a3-xxi-d430.xml",
+    "https://raw.githubusercontent.com/KONDE-AT/thun-data/master/editions/ansichten-ueber-waisenvermoegen-von-walter-1857-08-22-a3-xxi-d430.xml",  # noqa: E501
     "http://gams.uni-graz.at/o:aled.1/TEI_SOURCE",
 ]
 
-XML_STRINGS = ["""
+XML_STRINGS = [
+    """
 <?xml version="1.0" encoding="UTF-8"?>
 <TEI xmlns="http://www.tei-c.org/ns/1.0">
   <teiHeader>
       <fileDesc>
          <titleStmt>
             <title>Title</title>
          </titleStmt>
@@ -43,15 +40,15 @@
   <text>
       <body>
          <p>Some text here.</p>
       </body>
   </text>
 </TEI>
 """,
-"""<TEI xmlns="http://www.tei-c.org/ns/1.0">
+    """<TEI xmlns="http://www.tei-c.org/ns/1.0">
   <teiHeader>
       <fileDesc>
          <titleStmt>
             <title>Title</title>
          </titleStmt>
          <publicationStmt>
             <p>Publication Information</p>
@@ -63,20 +60,18 @@
   </teiHeader>
   <text>
       <body>
          <p>Some text here.</p>
       </body>
   </text>
 </TEI>
-"""]
+""",
+]
 
-DEFAULT_XSL = os.path.join(
-    os.path.dirname(__file__),
-    "test.xsl"
-)
+DEFAULT_XSL = os.path.join(os.path.dirname(__file__), "test.xsl")
 
 
 class TestAcdh_xml_pyutils(unittest.TestCase):
     """Tests for `acdh_xml_pyutils` package."""
 
     def setUp(self):
         """Set up test fixtures, if any."""
@@ -105,32 +100,32 @@
             doc = XMLReader(xml=x)
             self.assertIsInstance(doc.return_string(), str)
             self.assertIsInstance(doc.return_byte_like_object(), bytes)
 
     def test_004_write_to_file(self):
         doc = XMLReader(xml=XML_STRINGS[0])
         res = doc.tree_to_file()
-        self.assertTrue(res.startswith('2'))
-        self.assertTrue(res.endswith('.xml'))
+        self.assertTrue(res.startswith("2"))
+        self.assertTrue(res.endswith(".xml"))
         self.assertTrue(os.path.isfile(res))
         os.remove(res)
-        res = doc.tree_to_file(file='hansi.xml')
-        self.assertTrue(res.startswith('hansi'))
-        self.assertTrue(res.endswith('.xml'))
+        res = doc.tree_to_file(file="hansi.xml")
+        self.assertTrue(res.startswith("hansi"))
+        self.assertTrue(res.endswith(".xml"))
         self.assertTrue(os.path.isfile(res))
         os.remove(res)
 
     def test_005_get_elements(self):
         doc = XMLReader(xml=XML_STRINGS[0])
         els = doc.get_elements()
         self.assertIsInstance(els, list)
 
     def test_006_get_element_stats(self):
         doc = XMLReader(xml=XML_STRINGS[0])
         els = doc.get_element_stats()
         self.assertIsInstance(els, collections.Counter)
-        self.assertTrue('{http://www.tei-c.org/ns/1.0}TEI' in els.keys())
+        self.assertTrue("{http://www.tei-c.org/ns/1.0}TEI" in els.keys())
 
     def test_007_transform(self):
         doc = XMLReader(xml=XML_STRINGS[0], xsl=DEFAULT_XSL)
         els = doc.get_elements()
-        self.assertTrue('{http://www.tei-c.org/ns/1.0}hansi' in els)
+        self.assertTrue("{http://www.tei-c.org/ns/1.0}hansi" in els)
```

