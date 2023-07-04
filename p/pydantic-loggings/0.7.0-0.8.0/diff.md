# Comparing `tmp/pydantic-loggings-0.7.0.tar.gz` & `tmp/pydantic-loggings-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-0.7.0.tar", last modified: Mon Jul  3 12:52:26 2023, max compression
+gzip compressed data, was "pydantic-loggings-0.8.0.tar", last modified: Mon Jul  3 16:26:50 2023, max compression
```

## Comparing `pydantic-loggings-0.7.0.tar` & `pydantic-loggings-0.8.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:52:26.193944 pydantic-loggings-0.7.0/
--rw-r--r--   0 root         (0) root         (0)     1516 2023-07-03 12:52:26.193944 pydantic-loggings-0.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1195 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1765 2023-07-03 12:52:13.000000 pydantic-loggings-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 12:52:26.193944 pydantic-loggings-0.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:52:26.189944 pydantic-loggings-0.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:52:26.189944 pydantic-loggings-0.7.0/src/pydantic_loggings/
--rw-r--r--   0 root         (0) root         (0)      616 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:52:26.193944 pydantic-loggings-0.7.0/src/pydantic_loggings/base/
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      300 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/base/logs.py
--rw-r--r--   0 root         (0) root         (0)     3724 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:52:26.193944 pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/logs.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/types_.py
--rw-r--r--   0 root         (0) root         (0)      145 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/src/pydantic_loggings/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:52:26.193944 pydantic-loggings-0.7.0/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1516 2023-07-03 12:52:26.000000 pydantic-loggings-0.7.0/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      874 2023-07-03 12:52:26.000000 pydantic-loggings-0.7.0/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:52:26.000000 pydantic-loggings-0.7.0/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-03 12:52:26.000000 pydantic-loggings-0.7.0/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 12:52:26.000000 pydantic-loggings-0.7.0/src/pydantic_loggings.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:52:26.193944 pydantic-loggings-0.7.0/tests/
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-03 12:52:12.000000 pydantic-loggings-0.7.0/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-07-03 16:26:39.000000 pydantic-loggings-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.935611 pydantic-loggings-0.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.935611 pydantic-loggings-0.8.0/src/pydantic_loggings/
+-rw-r--r--   0 root         (0) root         (0)      616 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/src/pydantic_loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      300 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/base/loggings.py
+-rw-r--r--   0 root         (0) root         (0)     3724 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      656 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/loggings.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/types_.py
+-rw-r--r--   0 root         (0) root         (0)      145 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/src/pydantic_loggings/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.935611 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-03 16:26:50.000000 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      882 2023-07-03 16:26:50.000000 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 16:26:50.000000 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-03 16:26:50.000000 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 16:26:50.000000 pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:26:50.939611 pydantic-loggings-0.8.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-03 16:26:38.000000 pydantic-loggings-0.8.0/tests/test_main.py
```

### Comparing `pydantic-loggings-0.7.0/PKG-INFO` & `pydantic-loggings-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,84 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.7.0
+Version: 0.8.0
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Configure Python logging from environment variables with pydantic (settings) Model
 
 [![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
 
-## Installation
+## [Installation](https://img.shields.io/pypi/v/pydantic-loggings)
 
 ```shell
 pip install pydantic-loggings
 ```
 
+## [Usage](./examples)
+
 ### out of the box
 
 ```py
-from pydantic_loggings import BaseLog
+from pydantic_loggings.base import Logging # base Logging
+
 
-logger = BaseLog().configure_and_get_logger()
+logger = Logging().configure_and_get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
 # 01-01 00:00:00 WARNING root warning
 ```
 
+### default logging
+
+```py
+from pydantic_loggings.not_set import Logging
+
+
+logger = Logging().configure_and_get_logger()
+logger.debug('debug')
+logger.info('info')
+logger.warning('warning')
+
+# warning
+```
+
 ### from env file
 
 ```shell
-# ./log.conf.env
-log__formatters__base__datefmt='%m-%dT%X'
+# .env
+log__formatters__base__datefmt='%m-%d %H:%M:%S'
 log__formatters__base__format='{asctime} {levelname:5} {name} {message}'
 log__formatters__base__style='{'
 
 log__handlers__base__class_='logging.StreamHandler'
 log__handlers__base__formatter='base'
 
 log__loggers__root__level='DEBUG'
 log__loggers__root__handlers='["base"]'
 ```
 
 ```py
-from pydantic_loggings import Log
+from pathlib import Path
+
+from pydantic_loggings.not_set import Logging
+
 
-logger = Log(_env_file='./log.conf.env').configure_and_get_logger()
+env_file = Path(__file__).parent / '.env'
+logger = Logging(
+    _env_file=env_file  # pyright: ignore [reportGeneralTypeIssues]
+).configure_and_get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
```

### Comparing `pydantic-loggings-0.7.0/README.md` & `pydantic-loggings-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,75 @@
 # Configure Python logging from environment variables with pydantic (settings) Model
 
 [![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
 
-## Installation
+## [Installation](https://img.shields.io/pypi/v/pydantic-loggings)
 
 ```shell
 pip install pydantic-loggings
 ```
 
+## [Usage](./examples)
+
 ### out of the box
 
 ```py
-from pydantic_loggings import BaseLog
+from pydantic_loggings.base import Logging # base Logging
+
 
-logger = BaseLog().configure_and_get_logger()
+logger = Logging().configure_and_get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
 # 01-01 00:00:00 WARNING root warning
 ```
 
+### default logging
+
+```py
+from pydantic_loggings.not_set import Logging
+
+
+logger = Logging().configure_and_get_logger()
+logger.debug('debug')
+logger.info('info')
+logger.warning('warning')
+
+# warning
+```
+
 ### from env file
 
 ```shell
-# ./log.conf.env
-log__formatters__base__datefmt='%m-%dT%X'
+# .env
+log__formatters__base__datefmt='%m-%d %H:%M:%S'
 log__formatters__base__format='{asctime} {levelname:5} {name} {message}'
 log__formatters__base__style='{'
 
 log__handlers__base__class_='logging.StreamHandler'
 log__handlers__base__formatter='base'
 
 log__loggers__root__level='DEBUG'
 log__loggers__root__handlers='["base"]'
 ```
 
 ```py
-from pydantic_loggings import Log
+from pathlib import Path
+
+from pydantic_loggings.not_set import Logging
+
 
-logger = Log(_env_file='./log.conf.env').configure_and_get_logger()
+env_file = Path(__file__).parent / '.env'
+logger = Logging(
+    _env_file=env_file  # pyright: ignore [reportGeneralTypeIssues]
+).configure_and_get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
```

### Comparing `pydantic-loggings-0.7.0/pyproject.toml` & `pydantic-loggings-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 authors = [
   {name = "m9810223", email = "m9810223@gmail.com"},
 ]
 name = "pydantic-loggings"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "0.7.0"
+version = "0.8.0"
 
 dependencies = [
   "pydantic>=2.0",
   "pydantic-settings>=2.0",
 ]
 
 [project.urls]
```

### Comparing `pydantic-loggings-0.7.0/src/pydantic_loggings/__init__.py` & `pydantic-loggings-0.8.0/src/pydantic_loggings/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.7.0/src/pydantic_loggings/base/logs.py` & `pydantic-loggings-0.8.0/src/pydantic_loggings/base/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.7.0/src/pydantic_loggings/mixins.py` & `pydantic-loggings-0.8.0/src/pydantic_loggings/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/formatters.py` & `pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/handlers.py` & `pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,8 +28,9 @@
         mode='before',
     )
     def _list_validator(  # ? TODO
         cls,  # noqa: N805
         json_dict_str: str,
         info: FieldValidationInfo,
     ):
-        return StrList.model_validate_json(json_dict_str)
+        obj = StrList.model_validate_json(json_dict_str)
+        return obj
```

### Comparing `pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/loggers.py` & `pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/loggers.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,8 +19,9 @@
         mode='before',
     )
     def _list_validator(  # ? TODO
         cls,  # noqa: N805
         json_dict_str: str,
         info: FieldValidationInfo,
     ):
-        return StrList.model_validate_json(json_dict_str)
+        obj = StrList.model_validate_json(json_dict_str)
+        return obj
```

### Comparing `pydantic-loggings-0.7.0/src/pydantic_loggings/not_set/logs.py` & `pydantic-loggings-0.8.0/src/pydantic_loggings/not_set/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.7.0/src/pydantic_loggings.egg-info/PKG-INFO` & `pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,84 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.7.0
+Version: 0.8.0
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Configure Python logging from environment variables with pydantic (settings) Model
 
 [![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
 
-## Installation
+## [Installation](https://img.shields.io/pypi/v/pydantic-loggings)
 
 ```shell
 pip install pydantic-loggings
 ```
 
+## [Usage](./examples)
+
 ### out of the box
 
 ```py
-from pydantic_loggings import BaseLog
+from pydantic_loggings.base import Logging # base Logging
+
 
-logger = BaseLog().configure_and_get_logger()
+logger = Logging().configure_and_get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
 # 01-01 00:00:00 WARNING root warning
 ```
 
+### default logging
+
+```py
+from pydantic_loggings.not_set import Logging
+
+
+logger = Logging().configure_and_get_logger()
+logger.debug('debug')
+logger.info('info')
+logger.warning('warning')
+
+# warning
+```
+
 ### from env file
 
 ```shell
-# ./log.conf.env
-log__formatters__base__datefmt='%m-%dT%X'
+# .env
+log__formatters__base__datefmt='%m-%d %H:%M:%S'
 log__formatters__base__format='{asctime} {levelname:5} {name} {message}'
 log__formatters__base__style='{'
 
 log__handlers__base__class_='logging.StreamHandler'
 log__handlers__base__formatter='base'
 
 log__loggers__root__level='DEBUG'
 log__loggers__root__handlers='["base"]'
 ```
 
 ```py
-from pydantic_loggings import Log
+from pathlib import Path
+
+from pydantic_loggings.not_set import Logging
+
 
-logger = Log(_env_file='./log.conf.env').configure_and_get_logger()
+env_file = Path(__file__).parent / '.env'
+logger = Logging(
+    _env_file=env_file  # pyright: ignore [reportGeneralTypeIssues]
+).configure_and_get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
```

### Comparing `pydantic-loggings-0.7.0/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-0.8.0/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 src/pydantic_loggings.egg-info/requires.txt
 src/pydantic_loggings.egg-info/top_level.txt
 src/pydantic_loggings/base/__init__.py
 src/pydantic_loggings/base/filters.py
 src/pydantic_loggings/base/formatters.py
 src/pydantic_loggings/base/handlers.py
 src/pydantic_loggings/base/loggers.py
-src/pydantic_loggings/base/logs.py
+src/pydantic_loggings/base/loggings.py
 src/pydantic_loggings/not_set/__init__.py
 src/pydantic_loggings/not_set/filters.py
 src/pydantic_loggings/not_set/formatters.py
 src/pydantic_loggings/not_set/handlers.py
 src/pydantic_loggings/not_set/loggers.py
-src/pydantic_loggings/not_set/logs.py
+src/pydantic_loggings/not_set/loggings.py
 tests/test_main.py
```

