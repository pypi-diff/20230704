# Comparing `tmp/spacename-1.0.0.tar.gz` & `tmp/spacename-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacename-1.0.0.tar", max compression
+gzip compressed data, was "spacename-1.0.1.tar", max compression
```

## Comparing `spacename-1.0.0.tar` & `spacename-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1098 2023-01-30 02:55:32.000000 spacename-1.0.0/LICENSE
--rw-r--r--   0        0        0      492 2023-02-01 05:43:40.000000 spacename-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2508 2023-02-12 03:32:34.000000 spacename-1.0.0/README.md
--rw-r--r--   0        0        0     2170 2023-01-31 05:27:36.000000 spacename-1.0.0/src/spacename/__init__.py
--rw-r--r--   0        0        0     2848 1970-01-01 00:00:00.000000 spacename-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-01-30 02:55:32.000000 spacename-1.0.1/LICENSE
+-rw-r--r--   0        0        0      942 2023-07-04 18:12:00.000000 spacename-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2535 2023-02-13 01:12:56.000000 spacename-1.0.1/README.md
+-rw-r--r--   0        0        0     2257 2023-07-04 17:44:28.000000 spacename-1.0.1/src/spacename/__init__.py
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 spacename-1.0.1/PKG-INFO
```

### Comparing `spacename-1.0.0/LICENSE` & `spacename-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spacename-1.0.0/README.md` & `spacename-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from spacename import Namespace
 
 ns = Namespace(key="val")
 print(ns.key)
 ```
 Output:
 ```py
-"val"
+val
 ```
 
 ### Adding/modifying keys and values to the Namespace
 
 ```py
 from spacename import Namespace
 
@@ -75,15 +75,15 @@
 
 # OR
 
 print(ns.to_dict())
 ```
 Output:
 ```py
-{'spam':'foo', 'eggs':'bar', 'bacon': 'baz'}
+{'spam': 'foo', 'eggs': 'bar', 'bacon': 'baz'}
 ```
 
 ### Converting to list
 
 ```py
 from spacename import Namespace
 
@@ -133,9 +133,13 @@
 ```py
 from spacename import Namespace
 
 ns = Namespace(spam="foo", eggs="bar", bacon="baz")
 
 print("spam" in ns)
 ```
+Output:
+```py
+True
+```
 
 [^1]: Supported package managers include, but are not limited to, pip, poetry, and any other package manager that supports the PyPI repository.
```

### Comparing `spacename-1.0.0/src/spacename/__init__.py` & `spacename-1.0.1/src/spacename/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,50 @@
+###################
+# IMPORTS & SETUP #
+###################
+
+from typing import List, Tuple
 __version__ = "1.0.0"
 
+
 class Namespace(object):
 	def __init__(self, **kwargs) -> None:
 		"""Initialize namespace object.
 
 		Args:
 			**kwargs (any, optional): Attributes to populate namespace with.
 		"""
 
 		self.fill_from_dict(kwargs)
-	
+
 	def fill_from_dict(self, dictionary: dict) -> None:
 		"""Populate Namespace using dict.
 
 		Args:
 			dictionary (dict): Dict to populate namespace with.
 		"""
 
 		for key in dictionary:
 			setattr(self, key, dictionary[key])
-	
+
 	def to_dict(self) -> dict:
 		"""Return dict of self.
 
 		Returns:
 			dict: Dict of self
 		"""
 		return self.__dict__
 
 	def __repr__(self) -> str:
 		"""Return string representation of self.
 
 		Returns:
 			str: String representation of self.
 		"""
-		
+
 		type_name = type(self).__name__
 		arg_strings = []
 		star_args = {}
 		for arg in self._get_args():
 			arg_strings.append(repr(arg))
 		for name, value in self._get_kwargs():
 			if name.isidentifier():
@@ -53,44 +59,44 @@
 		"""Check that self is equal to other.
 
 		Args:
 			other (Namespace): Object to check against
 
 		Returns:
 			bool: Is self equal to other?
-		"""		
+		"""
 		return vars(self) == vars(other) if isinstance(other, type(self)) else NotImplemented
 
-	def __contains__(self, key)-> bool:
+	def __contains__(self, key) -> bool:
 		"""Check if self contains given key.
 
 		Args:
 			key (str): Key to look for
 
 		Returns:
 			bool: Is key in self?
-		"""			
+		"""
 		return key in self.__dict__
 
 	def __iter__(self):
 		"""Return iterator of self.
 
 		Returns:
 			list_iterator: Iterator of self
 		"""
 		return iter(self._get_kwargs())
 
-	def _get_kwargs(self) -> list[tuple[str]]:
+	def _get_kwargs(self) -> List[Tuple[str]]:
 		"""Return keyword arguments of self in a list of tuples.
 
 		Returns:
-			list[tuple[str]]: List of self's keyword arguments.
-		"""		
+			List[Tuple[str]]: List of self's keyword arguments.
+		"""
 		return list(self.__dict__.items())
 
 	def _get_args(self) -> list:
 		"""Return arguments of self in  list.
 
 		Returns:
 			list: List of self's arguments
-		"""		
+		"""
 		return []
```

### Comparing `spacename-1.0.0/PKG-INFO` & `spacename-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 Metadata-Version: 2.1
 Name: spacename
-Version: 1.0.0
+Version: 1.0.1
 Summary: An alternative to dictionaries, built on the argparse Namespace class.
+Home-page: https://github.com/tinkering-townsperson/spacename
 License: MIT
 Author: AfterNoonPM
 Author-email: h2o.Drop2010+pypi@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Project-URL: Bug Tracker, https://github.com/tinkering-townsperson/spacename/issues
+Project-URL: Repository, https://github.com/tinkering-townsperson/spacename
 Description-Content-Type: text/markdown
 
 # Spacename
 ###### *An alternative to dictionaries, built on the argparse Namespace class.*
 
 ### Table of contents
 [Back to Top](#spacename)
@@ -54,15 +61,15 @@
 from spacename import Namespace
 
 ns = Namespace(key="val")
 print(ns.key)
 ```
 Output:
 ```py
-"val"
+val
 ```
 
 ### Adding/modifying keys and values to the Namespace
 
 ```py
 from spacename import Namespace
 
@@ -89,15 +96,15 @@
 
 # OR
 
 print(ns.to_dict())
 ```
 Output:
 ```py
-{'spam':'foo', 'eggs':'bar', 'bacon': 'baz'}
+{'spam': 'foo', 'eggs': 'bar', 'bacon': 'baz'}
 ```
 
 ### Converting to list
 
 ```py
 from spacename import Namespace
 
@@ -147,9 +154,13 @@
 ```py
 from spacename import Namespace
 
 ns = Namespace(spam="foo", eggs="bar", bacon="baz")
 
 print("spam" in ns)
 ```
+Output:
+```py
+True
+```
 
 [^1]: Supported package managers include, but are not limited to, pip, poetry, and any other package manager that supports the PyPI repository.
```

