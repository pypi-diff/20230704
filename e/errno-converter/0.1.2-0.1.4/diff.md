# Comparing `tmp/errno_converter-0.1.2.tar.gz` & `tmp/errno_converter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "errno_converter-0.1.2.tar", last modified: Wed Aug 24 23:11:33 2022, max compression
+gzip compressed data, was "errno_converter-0.1.4.tar", last modified: Tue Jul  4 20:48:17 2023, max compression
```

## Comparing `errno_converter-0.1.2.tar` & `errno_converter-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2022-08-24 23:11:33.044391 errno_converter-0.1.2/
--rw-r--r--   0 poku      (1000) poku      (1000)     7048 2021-10-29 23:27:48.000000 errno_converter-0.1.2/LICENSE
--rw-r--r--   0 poku      (1000) poku      (1000)    11081 2022-08-24 23:11:33.044391 errno_converter-0.1.2/PKG-INFO
--rw-r--r--   0 poku      (1000) poku      (1000)     2381 2022-08-24 23:08:46.000000 errno_converter-0.1.2/README.md
--rw-r--r--   0 poku      (1000) poku      (1000)      838 2022-08-24 23:08:46.000000 errno_converter-0.1.2/pyproject.toml
--rw-r--r--   0 poku      (1000) poku      (1000)       38 2022-08-24 23:11:33.044391 errno_converter-0.1.2/setup.cfg
-drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2022-08-24 23:11:33.041058 errno_converter-0.1.2/src/
--rw-r--r--   0 poku      (1000) poku      (1000)        0 2022-08-24 23:08:46.000000 errno_converter-0.1.2/src/__init__.py
--rwxr-xr-x   0 poku      (1000) poku      (1000)     4325 2022-08-24 23:08:46.000000 errno_converter-0.1.2/src/converter_lib.py
-drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2022-08-24 23:11:33.041058 errno_converter-0.1.2/src/errno_converter.egg-info/
--rw-r--r--   0 poku      (1000) poku      (1000)    11081 2022-08-24 23:11:33.000000 errno_converter-0.1.2/src/errno_converter.egg-info/PKG-INFO
--rw-r--r--   0 poku      (1000) poku      (1000)      356 2022-08-24 23:11:33.000000 errno_converter-0.1.2/src/errno_converter.egg-info/SOURCES.txt
--rw-r--r--   0 poku      (1000) poku      (1000)        1 2022-08-24 23:11:33.000000 errno_converter-0.1.2/src/errno_converter.egg-info/dependency_links.txt
--rw-r--r--   0 poku      (1000) poku      (1000)      135 2022-08-24 23:11:33.000000 errno_converter-0.1.2/src/errno_converter.egg-info/entry_points.txt
--rw-r--r--   0 poku      (1000) poku      (1000)       71 2022-08-24 23:11:33.000000 errno_converter-0.1.2/src/errno_converter.egg-info/top_level.txt
--rwxr-xr-x   0 poku      (1000) poku      (1000)      566 2022-08-24 23:08:46.000000 errno_converter-0.1.2/src/errno_converter.py
--rwxr-xr-x   0 poku      (1000) poku      (1000)      610 2022-08-24 23:08:46.000000 errno_converter-0.1.2/src/http_converter.py
--rwxr-xr-x   0 poku      (1000) poku      (1000)      611 2022-08-24 23:08:46.000000 errno_converter-0.1.2/src/signal_converter.py
+drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-04 20:48:17.293100 errno_converter-0.1.4/
+-rw-r--r--   0 poku      (1000) poku      (1000)     7048 2021-10-29 23:27:48.000000 errno_converter-0.1.4/LICENSE
+-rw-r--r--   0 poku      (1000) poku      (1000)    11081 2023-07-04 20:48:17.293100 errno_converter-0.1.4/PKG-INFO
+-rw-r--r--   0 poku      (1000) poku      (1000)     2381 2022-08-24 23:08:46.000000 errno_converter-0.1.4/README.md
+-rw-r--r--   0 poku      (1000) poku      (1000)      838 2023-07-04 20:38:56.000000 errno_converter-0.1.4/pyproject.toml
+-rw-r--r--   0 poku      (1000) poku      (1000)       38 2023-07-04 20:48:17.293100 errno_converter-0.1.4/setup.cfg
+drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-04 20:48:17.289767 errno_converter-0.1.4/src/
+-rw-r--r--   0 poku      (1000) poku      (1000)        0 2022-08-24 23:08:46.000000 errno_converter-0.1.4/src/__init__.py
+-rwxr-xr-x   0 poku      (1000) poku      (1000)     5005 2023-07-04 20:08:00.000000 errno_converter-0.1.4/src/converter_lib.py
+drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-04 20:48:17.293100 errno_converter-0.1.4/src/errno_converter.egg-info/
+-rw-r--r--   0 poku      (1000) poku      (1000)    11081 2023-07-04 20:48:17.000000 errno_converter-0.1.4/src/errno_converter.egg-info/PKG-INFO
+-rw-r--r--   0 poku      (1000) poku      (1000)      356 2023-07-04 20:48:17.000000 errno_converter-0.1.4/src/errno_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 poku      (1000) poku      (1000)        1 2023-07-04 20:48:17.000000 errno_converter-0.1.4/src/errno_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 poku      (1000) poku      (1000)      135 2023-07-04 20:48:17.000000 errno_converter-0.1.4/src/errno_converter.egg-info/entry_points.txt
+-rw-r--r--   0 poku      (1000) poku      (1000)       71 2023-07-04 20:48:17.000000 errno_converter-0.1.4/src/errno_converter.egg-info/top_level.txt
+-rwxr-xr-x   0 poku      (1000) poku      (1000)      567 2023-07-04 20:08:00.000000 errno_converter-0.1.4/src/errno_converter.py
+-rwxr-xr-x   0 poku      (1000) poku      (1000)      610 2023-07-04 20:08:00.000000 errno_converter-0.1.4/src/http_converter.py
+-rwxr-xr-x   0 poku      (1000) poku      (1000)      611 2023-07-04 20:08:00.000000 errno_converter-0.1.4/src/signal_converter.py
```

### Comparing `errno_converter-0.1.2/LICENSE` & `errno_converter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `errno_converter-0.1.2/PKG-INFO` & `errno_converter-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: errno_converter
-Version: 0.1.2
+Version: 0.1.4
 Summary: As simple command line tool to convert error numbers (of C errno.h), http status codes and signal numbers to human readable strings or back zu numbers.
 Author-email: Heinrich Kießling <heinrich@kiess.link>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
```

### Comparing `errno_converter-0.1.2/README.md` & `errno_converter-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `errno_converter-0.1.2/pyproject.toml` & `errno_converter-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "errno_converter"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
   { name="Heinrich Kießling", email="heinrich@kiess.link" },
 ]
 description = "As simple command line tool to convert error numbers (of C errno.h), http status codes and signal numbers to human readable strings or back zu numbers."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `errno_converter-0.1.2/src/converter_lib.py` & `errno_converter-0.1.4/src/converter_lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,30 +35,36 @@
     @classmethod
     def print_version(cls):
         """
         Print Git project version by running ``git describe --tags`` in this project.
         """
 
         project_dir = os.path.dirname(__file__)
-        with open(os.devnull, 'wb') as devnull:
-            version = subprocess.check_output(['git', 'describe', '--tags'], stderr=devnull, cwd=project_dir)
+        with open(os.devnull, "wb") as devnull:
+            version = subprocess.check_output(
+                ["git", "describe", "--tags"], stderr=devnull, cwd=project_dir
+            )
             version = version.rstrip()
-        if hasattr(version, 'decode'):
-            version = version.decode('utf-8')
+        if hasattr(version, "decode"):
+            version = version.decode("utf-8")
         print(f"{sys.argv[0]} version {version}")
 
     @classmethod
     def print_help(cls):
-        print("{cmd} [-v] list|<{name}-number>|<{name}-name>".format(cmd=sys.argv[0], name=cls.NAME))
+        print(
+            "{cmd} [-v] list|<{name}-number>|<{name}-name>".format(
+                cmd=sys.argv[0], name=cls.NAME
+            )
+        )
 
     @classmethod
     def convert(cls, number=None, code=None, verbose=False):
         """
-        :param int number: 
-        :param str code: 
+        :param int number:
+        :param str code:
         :param bool verbose:
         :rtype: str
         """
         n = cls.code2number(code) if number is None else number
         c = cls.number2code(number) if code is None else code
 
         if verbose:
@@ -69,15 +75,14 @@
             elif number is None:
                 return str(n)
             else:
                 return "{n:3d} - {c}".format(n=n, c=c)
 
     @classmethod
     def parse(cls):
-
         if len(sys.argv) < 2:
             cls.print_help()
             exit()
 
         invalids = dict()
         verbose_option = sys.argv[1]
         if verbose_option == "-v":
@@ -92,41 +97,63 @@
         else:
             verbose_option = ""
             code_or_number = sys.argv[1]
 
         if code_or_number.lower() == "list":
             for n in cls.NUMBER_RANGE:
                 try:
-                    print(cls.convert(number=n, code=cls.number2code(n), verbose=bool(verbose_option)))
+                    print(
+                        cls.convert(
+                            number=n,
+                            code=cls.number2code(n),
+                            verbose=bool(verbose_option),
+                        )
+                    )
                 except Exception as e:
                     invalids[n] = e
 
         elif code_or_number.isdigit():
             try:
-                print(cls.convert(number=int(code_or_number), verbose=bool(verbose_option)))
+                print(
+                    cls.convert(
+                        number=int(code_or_number), verbose=bool(verbose_option)
+                    )
+                )
             except Exception as e:
                 invalids[code_or_number] = e
 
         else:
             try:
                 print(cls.convert(code=code_or_number, verbose=bool(verbose_option)))
             except Exception as e:
                 if verbose_option:
                     print(
                         "No {name} matched the input {i!r} ({e}). Try to match as re:".format(
-                             name=cls.NAME,          i=code_or_number, e=e),
+                            name=cls.NAME, i=code_or_number, e=e
+                        ),
                         file=sys.stderr,
                     )
                 search = re.compile(code_or_number, flags=re.IGNORECASE)
                 for att in cls.get_candidates():
                     try:
                         number = cls.code2number(att)
                         desc = cls.number2description(number)
-                        if search.search(att) or search.search(str(number)) or search.search(desc) and bool(verbose_option):
-                            print(cls.convert(number=number, code=att, verbose=bool(verbose_option)))
+                        if (
+                            search.search(att)
+                            or search.search(str(number))
+                            or search.search(desc)
+                            and bool(verbose_option)
+                        ):
+                            print(
+                                cls.convert(
+                                    number=number,
+                                    code=att,
+                                    verbose=bool(verbose_option),
+                                )
+                            )
                     except:
                         pass
 
         if invalids and verbose_option:
             if all(isinstance(e, (ValueError, KeyError)) for e in invalids.values()):
                 print("invalids: {}".format(set(invalids.keys())), file=sys.stderr)
             else:
```

### Comparing `errno_converter-0.1.2/src/errno_converter.egg-info/PKG-INFO` & `errno_converter-0.1.4/src/errno_converter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: errno-converter
-Version: 0.1.2
+Version: 0.1.4
 Summary: As simple command line tool to convert error numbers (of C errno.h), http status codes and signal numbers to human readable strings or back zu numbers.
 Author-email: Heinrich Kießling <heinrich@kiess.link>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
```

### Comparing `errno_converter-0.1.2/src/errno_converter.py` & `errno_converter-0.1.4/src/errno_converter.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,9 +21,10 @@
     def get_candidates():
         return dir(errno)
 
     @staticmethod
     def number2description(number):
         return os.strerror(number)
 
+
 def main():
     return ErrnoConverter.parse()
```

### Comparing `errno_converter-0.1.2/src/http_converter.py` & `errno_converter-0.1.4/src/http_converter.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -21,10 +21,10 @@
     def get_candidates():
         return dir(http.HTTPStatus)
 
     @staticmethod
     def number2description(number):
         return http.HTTPStatus(int(number)).description
 
+
 def main():
     return HttpConverter.parse()
-
```

### Comparing `errno_converter-0.1.2/src/signal_converter.py` & `errno_converter-0.1.4/src/signal_converter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     def get_candidates():
         return dir(signal)
 
     @staticmethod
     def number2description(number):
         return signal.strsignal(signal.Signals(int(number)))  # Python3.8
 
+
 def main():
     return SignalConverter.parse()
-
```

