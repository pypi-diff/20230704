# Comparing `tmp/cdcstream-0.2.2.tar.gz` & `tmp/cdcstream-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdcstream-0.2.2.tar", max compression
+gzip compressed data, was "cdcstream-0.2.3.tar", max compression
```

## Comparing `cdcstream-0.2.2.tar` & `cdcstream-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      916 2023-01-26 14:03:02.604195 cdcstream-0.2.2/cdcstream/__init__.py
--rw-r--r--   0        0        0    15633 2023-01-26 13:35:25.081624 cdcstream-0.2.2/cdcstream/cdcstream.py
--rw-r--r--   0        0        0    10944 2022-11-24 14:02:08.490795 cdcstream-0.2.2/cdcstream/dilca_wrapper.py
--rw-r--r--   0        0        0     3621 2022-11-24 13:45:13.607609 cdcstream-0.2.2/cdcstream/tools.py
--rw-r--r--   0        0        0     1372 2023-01-26 13:32:48.562181 cdcstream-0.2.2/DESCRIPTION.md
--rw-r--r--   0        0        0    35821 2022-08-24 12:32:04.521420 cdcstream-0.2.2/LICENSE
--rw-r--r--   0        0        0    92055 2022-07-29 16:26:34.835921 cdcstream-0.2.2/LICENSE_LIBRARIES
--rw-r--r--   0        0        0      915 2023-01-26 14:02:54.720705 cdcstream-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 cdcstream-0.2.2/setup.py
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 cdcstream-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      916 2023-07-04 15:34:27.177983 cdcstream-0.2.3/cdcstream/__init__.py
+-rw-r--r--   0        0        0    15633 2023-04-19 11:48:18.882039 cdcstream-0.2.3/cdcstream/cdcstream.py
+-rw-r--r--   0        0        0    10944 2023-04-19 11:48:18.883039 cdcstream-0.2.3/cdcstream/dilca_wrapper.py
+-rw-r--r--   0        0        0     3621 2023-04-19 11:48:18.884039 cdcstream-0.2.3/cdcstream/tools.py
+-rw-r--r--   0        0        0     1372 2023-04-19 11:48:18.878040 cdcstream-0.2.3/DESCRIPTION.md
+-rw-r--r--   0        0        0    35821 2023-04-19 11:48:18.879039 cdcstream-0.2.3/LICENSE
+-rw-r--r--   0        0        0    92055 2023-04-19 11:48:18.880039 cdcstream-0.2.3/LICENSE_LIBRARIES
+-rw-r--r--   0        0        0      915 2023-07-04 15:34:27.177983 cdcstream-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 cdcstream-0.2.3/setup.py
+-rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 cdcstream-0.2.3/PKG-INFO
```

### Comparing `cdcstream-0.2.2/cdcstream/__init__.py` & `cdcstream-0.2.3/cdcstream/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 __author__ = 'Martin Trat'
 __email__ = 'trat@fzi.de'
 __license__ = 'GNU General Public License v3.0'
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 
 from .cdcstream import DriftDetector, CDCStream
 from .dilca_wrapper import DilcaDistance, dilca_workflow
```

### Comparing `cdcstream-0.2.2/cdcstream/cdcstream.py` & `cdcstream-0.2.3/cdcstream/cdcstream.py`

 * *Files identical despite different names*

### Comparing `cdcstream-0.2.2/cdcstream/dilca_wrapper.py` & `cdcstream-0.2.3/cdcstream/dilca_wrapper.py`

 * *Files identical despite different names*

### Comparing `cdcstream-0.2.2/cdcstream/tools.py` & `cdcstream-0.2.3/cdcstream/tools.py`

 * *Files identical despite different names*

### Comparing `cdcstream-0.2.2/DESCRIPTION.md` & `cdcstream-0.2.3/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `cdcstream-0.2.2/LICENSE` & `cdcstream-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdcstream-0.2.2/LICENSE_LIBRARIES` & `cdcstream-0.2.3/LICENSE_LIBRARIES`

 * *Files identical despite different names*

### Comparing `cdcstream-0.2.2/pyproject.toml` & `cdcstream-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdcstream"
-version = "0.2.2"
+version = "0.2.3"
 description = "Implementation of Ienco's algorithm CDCStream"
 readme = "DESCRIPTION.md"
 authors = ["Martin Trat <trat@fzi.de>"]
 homepage = "https://github.com/fzi-forschungszentrum-informatik/cdcstream"
 repository = "https://github.com/fzi-forschungszentrum-informatik/cdcstream"
 license = "GNU General Public License v3.0"
 classifiers = [
@@ -12,15 +12,15 @@
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha"
 ]
 
 [tool.poetry.dependencies]
 packaging = "*"
-python = ">=3.7"
+python = ">=3.8"
 numpy = "*"
 pandas = "*"
 python-javabridge = "*"
 python-weka-wrapper3 = "^0.2"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `cdcstream-0.2.2/setup.py` & `cdcstream-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
  'packaging',
  'pandas',
  'python-javabridge',
  'python-weka-wrapper3>=0.2,<0.3']
 
 setup_kwargs = {
     'name': 'cdcstream',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': "Implementation of Ienco's algorithm CDCStream",
     'long_description': "Cite this work as (BibTex):\n```\n@techreport{TratBenderOvtcharova2023_1000155196,\n    author       = {Trat, Martin and Bender, Janek and Ovtcharova, Jivka},\n    year         = {2023},\n    title        = {Sensitivity-Based Optimization of Unsupervised Drift Detection for Categorical Data Streams},\n    doi          = {10.5445/IR/1000155196},\n    institution  = {{Karlsruher Institut für Technologie (KIT)}},\n    issn         = {2194-1629},\n    series       = {KIT Scientific Working Papers},\n    keywords     = {unsupervised conceptdriftdetection, data streammining, productiveartificialintelligence, categorical data processing},\n    pagetotal    = {10},\n    language     = {english},\n    volume       = {208}\n}\n```\n\nImplementation of an augmented version of Dino Ienco's algorithm **CDCStream** (Change Detection in Categorical Evolving Data Streams) ([https://doi.org/10.1145/2554850.2554864](https://doi.org/10.1145/2554850.2554864)).\n\n## Requirements\nPlease note that several requirements need to be fulfilled in order to run the software.\nSee repository readme for details.\n\n## Acknowledgements\nThis software was developed at the FZI Research Center for Information Technology.\nThe associated research was funded by the German Federal Ministry of Education and Research (grant number: 02K18D033) within the context of the project SEAMLESS.\n",
     'author': 'Martin Trat',
     'author_email': 'trat@fzi.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fzi-forschungszentrum-informatik/cdcstream',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7',
+    'python_requires': '>=3.8',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `cdcstream-0.2.2/PKG-INFO` & `cdcstream-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: cdcstream
-Version: 0.2.2
+Version: 0.2.3
 Summary: Implementation of Ienco's algorithm CDCStream
 Home-page: https://github.com/fzi-forschungszentrum-informatik/cdcstream
 License: GNU General Public License v3.0
 Author: Martin Trat
 Author-email: trat@fzi.de
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: numpy
```

