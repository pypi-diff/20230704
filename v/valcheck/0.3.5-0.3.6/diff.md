# Comparing `tmp/valcheck-0.3.5.tar.gz` & `tmp/valcheck-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valcheck-0.3.5.tar", last modified: Mon Feb 20 08:47:35 2023, max compression
+gzip compressed data, was "valcheck-0.3.6.tar", last modified: Tue Jul  4 15:47:11 2023, max compression
```

## Comparing `valcheck-0.3.5.tar` & `valcheck-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 nishant   (1000) nishant   (1000)        0 2023-02-20 08:47:35.665888 valcheck-0.3.5/
--rw-rw-r--   0 nishant   (1000) nishant   (1000)     1067 2022-08-31 05:58:34.000000 valcheck-0.3.5/LICENSE
--rw-rw-r--   0 nishant   (1000) nishant   (1000)      751 2023-02-20 08:47:35.665888 valcheck-0.3.5/PKG-INFO
--rw-rw-r--   0 nishant   (1000) nishant   (1000)      231 2023-02-19 10:00:55.000000 valcheck-0.3.5/README.md
--rw-rw-r--   0 nishant   (1000) nishant   (1000)       38 2023-02-20 08:47:35.665888 valcheck-0.3.5/setup.cfg
--rw-rw-r--   0 nishant   (1000) nishant   (1000)     1515 2023-02-20 08:43:00.000000 valcheck-0.3.5/setup.py
-drwxrwxr-x   0 nishant   (1000) nishant   (1000)        0 2023-02-20 08:47:35.665888 valcheck-0.3.5/valcheck/
--rw-rw-r--   0 nishant   (1000) nishant   (1000)        0 2022-08-11 04:27:42.000000 valcheck-0.3.5/valcheck/__init__.py
--rw-rw-r--   0 nishant   (1000) nishant   (1000)    11895 2023-02-20 08:45:15.000000 valcheck-0.3.5/valcheck/base_validator.py
--rw-rw-r--   0 nishant   (1000) nishant   (1000)     1229 2023-02-19 07:11:39.000000 valcheck-0.3.5/valcheck/exceptions.py
--rw-rw-r--   0 nishant   (1000) nishant   (1000)    11410 2023-02-20 08:38:59.000000 valcheck-0.3.5/valcheck/fields.py
--rw-rw-r--   0 nishant   (1000) nishant   (1000)     1601 2023-02-11 07:15:53.000000 valcheck-0.3.5/valcheck/models.py
--rw-rw-r--   0 nishant   (1000) nishant   (1000)     2397 2023-02-20 08:35:31.000000 valcheck-0.3.5/valcheck/utils.py
-drwxrwxr-x   0 nishant   (1000) nishant   (1000)        0 2023-02-20 08:47:35.665888 valcheck-0.3.5/valcheck.egg-info/
--rw-rw-r--   0 nishant   (1000) nishant   (1000)      751 2023-02-20 08:47:35.000000 valcheck-0.3.5/valcheck.egg-info/PKG-INFO
--rw-rw-r--   0 nishant   (1000) nishant   (1000)      281 2023-02-20 08:47:35.000000 valcheck-0.3.5/valcheck.egg-info/SOURCES.txt
--rw-rw-r--   0 nishant   (1000) nishant   (1000)        1 2023-02-20 08:47:35.000000 valcheck-0.3.5/valcheck.egg-info/dependency_links.txt
--rw-rw-r--   0 nishant   (1000) nishant   (1000)        9 2023-02-20 08:47:35.000000 valcheck-0.3.5/valcheck.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 15:47:11.107472 valcheck-0.3.6/
+-rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      751 2023-07-04 15:47:11.105483 valcheck-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-02 09:39:38.000000 valcheck-0.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 15:47:11.107472 valcheck-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1559 2023-07-02 14:40:18.000000 valcheck-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 15:47:11.074530 valcheck-0.3.6/valcheck/
+-rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-0.3.6/valcheck/__init__.py
+-rw-rw-rw-   0        0        0     1270 2023-07-02 09:39:38.000000 valcheck-0.3.6/valcheck/exceptions.py
+-rw-rw-rw-   0        0        0    17995 2023-07-04 15:25:07.000000 valcheck-0.3.6/valcheck/fields.py
+-rw-rw-rw-   0        0        0     2202 2023-07-04 15:28:12.000000 valcheck-0.3.6/valcheck/models.py
+-rw-rw-rw-   0        0        0     2490 2023-07-03 16:41:25.000000 valcheck-0.3.6/valcheck/utils.py
+-rw-rw-rw-   0        0        0     6365 2023-07-04 15:41:10.000000 valcheck-0.3.6/valcheck/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-04 15:47:11.101527 valcheck-0.3.6/valcheck.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-07-04 15:47:11.000000 valcheck-0.3.6/valcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-04 15:47:11.000000 valcheck-0.3.6/valcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 15:47:11.000000 valcheck-0.3.6/valcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 15:47:11.000000 valcheck-0.3.6/valcheck.egg-info/top_level.txt
```

### Comparing `valcheck-0.3.5/LICENSE` & `valcheck-0.3.6/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Nishant Rao
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 Nishant Rao
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `valcheck-0.3.5/PKG-INFO` & `valcheck-0.3.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1
-Name: valcheck
-Version: 0.3.5
-Summary: Package for quick data validation (in Python)
-Home-page: https://github.com/Nishant173/valcheck
-Author: Nishant Rao
-Author-email: nishant.rao173@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-License-File: LICENSE
-
-Package for quick data validation (in Python). Our repository: https://github.com/Nishant173/valcheck
-
+Metadata-Version: 2.1
+Name: valcheck
+Version: 0.3.6
+Summary: Package for quick data validation (in Python)
+Home-page: https://github.com/Nishant173/valcheck
+Author: Nishant Rao
+Author-email: nishant.rao173@gmail.com
+License: MIT
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+License-File: LICENSE
+
+Package for quick data validation (in Python). Our repository: https://github.com/Nishant173/valcheck
```

### Comparing `valcheck-0.3.5/setup.py` & `valcheck-0.3.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import os
-from setuptools import find_packages, setup
-
-# Constants
-PACKAGE_NAME = "valcheck"
-PACKAGE_VERSION = "0.3.5"
-AUTHOR_NAME = "Nishant Rao"
-AUTHOR_EMAIL_ID = "nishant.rao173@gmail.com"
-FILEPATH_TO_README = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
-FILEPATH_TO_REQUIREMENTS = os.path.join(os.path.abspath(os.path.dirname(__file__)), "requirements.txt")
-REPOSITORY_URL = "https://github.com/Nishant173/valcheck"
-
-# Requirements
-install_requires = []
-with open(file=FILEPATH_TO_REQUIREMENTS, mode="r") as fp:
-    install_requires.extend(
-        [s for s in [line.strip(" \n") for line in fp] if not s.startswith("#") and s != ""]
-    )
-
-# Setup
-setup(
-    name=PACKAGE_NAME,
-    version=PACKAGE_VERSION,
-    description="Package for quick data validation (in Python)",
-    long_description=f"Package for quick data validation (in Python). Our repository: {REPOSITORY_URL}",
-    author=AUTHOR_NAME,
-    author_email=AUTHOR_EMAIL_ID,
-    url=REPOSITORY_URL,
-    packages=find_packages(where="."),
-    include_package_data=True,
-    install_requires=install_requires,
-    license="MIT",
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: ISC License (ISCL)",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3.6",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ],
-)
-
+import os
+from setuptools import find_packages, setup
+
+# Constants
+PACKAGE_NAME = "valcheck"
+PACKAGE_VERSION = "0.3.6"
+AUTHOR_NAME = "Nishant Rao"
+AUTHOR_EMAIL_ID = "nishant.rao173@gmail.com"
+FILEPATH_TO_README = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
+FILEPATH_TO_REQUIREMENTS = os.path.join(os.path.abspath(os.path.dirname(__file__)), "requirements.txt")
+REPOSITORY_URL = "https://github.com/Nishant173/valcheck"
+
+# Requirements
+install_requires = []
+with open(file=FILEPATH_TO_REQUIREMENTS, mode="r") as fp:
+    install_requires.extend(
+        [s for s in [line.strip(" \n") for line in fp] if not s.startswith("#") and s != ""]
+    )
+
+# Setup
+setup(
+    name=PACKAGE_NAME,
+    version=PACKAGE_VERSION,
+    description="Package for quick data validation (in Python)",
+    long_description=f"Package for quick data validation (in Python). Our repository: {REPOSITORY_URL}",
+    author=AUTHOR_NAME,
+    author_email=AUTHOR_EMAIL_ID,
+    url=REPOSITORY_URL,
+    packages=find_packages(where="."),
+    include_package_data=True,
+    install_requires=install_requires,
+    license="MIT",
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: ISC License (ISCL)",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3.6",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ],
+)
+
```

### Comparing `valcheck-0.3.5/valcheck.egg-info/PKG-INFO` & `valcheck-0.3.6/valcheck.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1
-Name: valcheck
-Version: 0.3.5
-Summary: Package for quick data validation (in Python)
-Home-page: https://github.com/Nishant173/valcheck
-Author: Nishant Rao
-Author-email: nishant.rao173@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-License-File: LICENSE
-
-Package for quick data validation (in Python). Our repository: https://github.com/Nishant173/valcheck
-
+Metadata-Version: 2.1
+Name: valcheck
+Version: 0.3.6
+Summary: Package for quick data validation (in Python)
+Home-page: https://github.com/Nishant173/valcheck
+Author: Nishant Rao
+Author-email: nishant.rao173@gmail.com
+License: MIT
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+License-File: LICENSE
+
+Package for quick data validation (in Python). Our repository: https://github.com/Nishant173/valcheck
```

