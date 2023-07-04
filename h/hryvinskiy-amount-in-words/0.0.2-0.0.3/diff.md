# Comparing `tmp/hryvinskiy_amount_in_words-0.0.2.tar.gz` & `tmp/hryvinskiy_amount_in_words-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hryvinskiy_amount_in_words-0.0.2.tar", last modified: Tue Jul  4 08:53:03 2023, max compression
+gzip compressed data, was "hryvinskiy_amount_in_words-0.0.3.tar", last modified: Tue Jul  4 08:59:13 2023, max compression
```

## Comparing `hryvinskiy_amount_in_words-0.0.2.tar` & `hryvinskiy_amount_in_words-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 08:53:03.413364 hryvinskiy_amount_in_words-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-04 07:57:32.000000 hryvinskiy_amount_in_words-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      707 2023-07-04 08:53:03.412820 hryvinskiy_amount_in_words-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-07-04 07:56:25.000000 hryvinskiy_amount_in_words-0.0.2/README.md
--rw-rw-rw-   0        0        0      519 2023-07-04 08:52:30.000000 hryvinskiy_amount_in_words-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 08:53:03.414341 hryvinskiy_amount_in_words-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 08:53:03.383982 hryvinskiy_amount_in_words-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 08:53:03.403461 hryvinskiy_amount_in_words-0.0.2/src/hryvinskiy_amount_in_words/
--rw-rw-rw-   0        0        0       14 2023-07-04 08:52:24.000000 hryvinskiy_amount_in_words-0.0.2/src/hryvinskiy_amount_in_words/__init__.py
--rw-rw-rw-   0        0        0     4737 2023-07-04 08:52:17.000000 hryvinskiy_amount_in_words-0.0.2/src/hryvinskiy_amount_in_words/example.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:53:03.410730 hryvinskiy_amount_in_words-0.0.2/src/hryvinskiy_amount_in_words.egg-info/
--rw-rw-rw-   0        0        0      707 2023-07-04 08:53:03.000000 hryvinskiy_amount_in_words-0.0.2/src/hryvinskiy_amount_in_words.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-07-04 08:53:03.000000 hryvinskiy_amount_in_words-0.0.2/src/hryvinskiy_amount_in_words.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 08:53:03.000000 hryvinskiy_amount_in_words-0.0.2/src/hryvinskiy_amount_in_words.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-04 08:53:03.000000 hryvinskiy_amount_in_words-0.0.2/src/hryvinskiy_amount_in_words.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 08:59:13.105507 hryvinskiy_amount_in_words-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-04 07:57:32.000000 hryvinskiy_amount_in_words-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      707 2023-07-04 08:59:13.103733 hryvinskiy_amount_in_words-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-07-04 07:56:25.000000 hryvinskiy_amount_in_words-0.0.3/README.md
+-rw-rw-rw-   0        0        0      519 2023-07-04 08:58:40.000000 hryvinskiy_amount_in_words-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 08:59:13.105507 hryvinskiy_amount_in_words-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 08:59:13.070157 hryvinskiy_amount_in_words-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:59:13.091127 hryvinskiy_amount_in_words-0.0.3/src/hryvinskiy_amount_in_words/
+-rw-rw-rw-   0        0        0       14 2023-07-04 08:52:24.000000 hryvinskiy_amount_in_words-0.0.3/src/hryvinskiy_amount_in_words/__init__.py
+-rw-rw-rw-   0        0        0     4112 2023-07-04 08:58:30.000000 hryvinskiy_amount_in_words-0.0.3/src/hryvinskiy_amount_in_words/example.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:59:13.101735 hryvinskiy_amount_in_words-0.0.3/src/hryvinskiy_amount_in_words.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-07-04 08:59:13.000000 hryvinskiy_amount_in_words-0.0.3/src/hryvinskiy_amount_in_words.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-07-04 08:59:13.000000 hryvinskiy_amount_in_words-0.0.3/src/hryvinskiy_amount_in_words.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 08:59:13.000000 hryvinskiy_amount_in_words-0.0.3/src/hryvinskiy_amount_in_words.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-04 08:59:13.000000 hryvinskiy_amount_in_words-0.0.3/src/hryvinskiy_amount_in_words.egg-info/top_level.txt
```

### Comparing `hryvinskiy_amount_in_words-0.0.2/LICENSE` & `hryvinskiy_amount_in_words-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hryvinskiy_amount_in_words-0.0.2/PKG-INFO` & `hryvinskiy_amount_in_words-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hryvinskiy_amount_in_words
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hryvinskiy_amount_in_words-0.0.2/pyproject.toml` & `hryvinskiy_amount_in_words-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hryvinskiy_amount_in_words"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hryvinskiy_amount_in_words-0.0.2/src/hryvinskiy_amount_in_words/example.py` & `hryvinskiy_amount_in_words-0.0.3/src/hryvinskiy_amount_in_words/example.py`

 * *Files 18% similar despite different names*

```diff
@@ -89,18 +89,10 @@
 		return hundreds[number_0]
 	elif number_1 == 1 and number_2 != 0:
 		return f"{hundreds[number_0]} {get_tens(number_1, number_2)}"
 	else:
 		return f"{hundreds[number_0]} {tens[number_1]} {units[number_2]}"
 
 
-if __name__ == "__main__":
-	print("Привіт,я програма що перетворює числове представлення грошової суми в суму прописом.\nМаксимальне дозволене число '999999.99'\n")
-	assert number_to_text(decimal.Decimal("1234.56")) == "Одна тисяча двiстi тридцять чотири гривні 56 копійок"
-	while True:
-		try:
-			number = decimal.Decimal(input("Введіть суму: "))
-			print("Результат:", number_to_text(number),"\n")
-		except:
-			print("Введіть суму числом\n")
+
```

### Comparing `hryvinskiy_amount_in_words-0.0.2/src/hryvinskiy_amount_in_words.egg-info/PKG-INFO` & `hryvinskiy_amount_in_words-0.0.3/src/hryvinskiy_amount_in_words.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hryvinskiy-amount-in-words
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

