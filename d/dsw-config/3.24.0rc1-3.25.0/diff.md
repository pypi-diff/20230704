# Comparing `tmp/dsw-config-3.24.0rc1.tar.gz` & `tmp/dsw-config-3.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-config-3.24.0rc1.tar", last modified: Tue May 30 11:45:41 2023, max compression
+gzip compressed data, was "dsw-config-3.25.0.tar", last modified: Tue Jul  4 07:29:28 2023, max compression
```

## Comparing `dsw-config-3.24.0rc1.tar` & `dsw-config-3.25.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/dsw/config/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-30 11:45:40.000000 dsw-config-3.24.0rc1/dsw/config/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/dsw_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:28.387395 dsw-config-3.25.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-04 07:29:18.000000 dsw-config-3.25.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-04 07:29:28.387395 dsw-config-3.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-04 07:29:18.000000 dsw-config-3.25.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:28.383395 dsw-config-3.25.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:28.387395 dsw-config-3.25.0/dsw/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-04 07:29:18.000000 dsw-config-3.25.0/dsw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 07:29:27.000000 dsw-config-3.25.0/dsw/config/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-04 07:29:18.000000 dsw-config-3.25.0/dsw/config/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-04 07:29:18.000000 dsw-config-3.25.0/dsw/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-07-04 07:29:18.000000 dsw-config-3.25.0/dsw/config/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-04 07:29:18.000000 dsw-config-3.25.0/dsw/config/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-04 07:29:18.000000 dsw-config-3.25.0/dsw/config/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:28.387395 dsw-config-3.25.0/dsw_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-04 07:29:28.000000 dsw-config-3.25.0/dsw_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 07:29:28.000000 dsw-config-3.25.0/dsw_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:28.000000 dsw-config-3.25.0/dsw_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:28.000000 dsw-config-3.25.0/dsw_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 07:29:28.000000 dsw-config-3.25.0/dsw_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-04 07:29:28.000000 dsw-config-3.25.0/dsw_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-04 07:29:18.000000 dsw-config-3.25.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:28.387395 dsw-config-3.25.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:18.000000 dsw-config-3.25.0/setup.py
```

### Comparing `dsw-config-3.24.0rc1/LICENSE` & `dsw-config-3.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0rc1/PKG-INFO` & `dsw-config-3.25.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-config
-Version: 3.24.0rc1
+Version: 3.25.0
 Summary: Library for DSW config manipulation
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-config-3.24.0rc1/README.md` & `dsw-config-3.25.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0rc1/dsw/config/keys.py` & `dsw-config-3.25.0/dsw/config/keys.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 T = TypeVar('T')
 
 
 def cast_bool(value: Any) -> bool:
     return bool(value)
 
 
+def cast_optional_bool(value: Any) -> Optional[bool]:
+    if value is None:
+        return None
+    return bool(value)
+
+
 def cast_int(value: Any) -> int:
     return int(value)
 
 
 def cast_optional_int(value: Any) -> Optional[int]:
     if value is None:
         return None
@@ -265,26 +271,25 @@
         yaml_path=['mail', 'security'],
         var_names=['MAIL_SECURITY'],
         cast=cast_optional_str,
     )
     auth_enabled = ConfigKey(
         yaml_path=['mail', 'authEnabled'],
         var_names=[],
-        default=False,
-        cast=cast_bool,
+        cast=cast_optional_bool,
     )
     username = ConfigKey(
         yaml_path=['mail', 'username'],
         var_names=['MAIL_USERNAME'],
-        cast=cast_str,
+        cast=cast_optional_str,
     )
     password = ConfigKey(
         yaml_path=['mail', 'password'],
         var_names=['MAIL_PASSWORD'],
-        cast=cast_str,
+        cast=cast_optional_str,
     )
     rate_limit_window = ConfigKey(
         yaml_path=['mail', 'rateLimit', 'window'],
         var_names=['MAIL_RATE_LIMIT_WINDOW'],
         default=0,
         cast=cast_int,
     )
```

### Comparing `dsw-config-3.24.0rc1/dsw/config/logging.py` & `dsw-config-3.25.0/dsw/config/logging.py`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0rc1/dsw/config/model.py` & `dsw-config-3.25.0/dsw/config/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,32 +80,34 @@
         self.multi_tenant = multi_tenant
 
 
 class MailConfig(ConfigModel):
 
     def __init__(self, enabled: bool, ssl: Optional[bool], name: str, email: str,
                  host: str, port: Optional[int], security: Optional[str],
-                 auth: Optional[bool], username: Optional[str],
+                 auth_enabled: Optional[bool], username: Optional[str],
                  password: Optional[str], rate_limit_window: int,
                  rate_limit_count: int, timeout: int,
                  dkim_selector: Optional[str] = None,
                  dkim_privkey_file: Optional[str] = None):
         self.enabled = enabled
         self.name = name
         self.email = email
         self.host = host
         self.security = 'plain'
         if security is not None:
             self.security = security.lower()
         elif ssl is not None:
             self.security = 'ssl' if ssl else 'plain'
         self.port = port or self._default_port()
-        self.auth = auth or (username is not None and password is not None)
-        self.username = username if self.auth is not None else None
-        self.password = password if self.auth is not None else None
+        self.auth = auth_enabled
+        if self.auth is None:
+            self.auth = username is not None and password is not None
+        self.username = username
+        self.password = password
         self.rate_limit_window = rate_limit_window
         self.rate_limit_count = rate_limit_count
         self.timeout = timeout
         self.dkim_selector = dkim_selector
         self.dkim_privkey_file = dkim_privkey_file
         self.dkim_privkey = b''
```

### Comparing `dsw-config-3.24.0rc1/dsw/config/parser.py` & `dsw-config-3.25.0/dsw/config/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             enabled=self.get(self.keys.mail.enabled),
             name=self.get(self.keys.mail.name),
             email=self.get(self.keys.mail.email),
             host=self.get(self.keys.mail.host),
             ssl=self.get(self.keys.mail.ssl),
             port=self.get(self.keys.mail.port),
             security=self.get(self.keys.mail.security),
-            auth=self.get(self.keys.mail.auth_enabled),
+            auth_enabled=self.get(self.keys.mail.auth_enabled),
             username=self.get(self.keys.mail.username),
             password=self.get(self.keys.mail.password),
             rate_limit_window=int(self.get(self.keys.mail.rate_limit_window)),
             rate_limit_count=int(self.get(self.keys.mail.rate_limit_count)),
             timeout=int(self.get(self.keys.mail.timeout)),
             dkim_selector=self.get(self.keys.mail.dkim_selector),
             dkim_privkey_file=self.get(self.keys.mail.dkim_privkey_file),
```

### Comparing `dsw-config-3.24.0rc1/dsw/config/sentry.py` & `dsw-config-3.25.0/dsw/config/sentry.py`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0rc1/dsw_config.egg-info/PKG-INFO` & `dsw-config-3.25.0/dsw_config.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-config
-Version: 3.24.0rc1
+Version: 3.25.0
 Summary: Library for DSW config manipulation
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-config-3.24.0rc1/pyproject.toml` & `dsw-config-3.25.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-config'
-version = "3.24.0rc.1"
+version = "3.25.0"
 description = 'Library for DSW config manipulation'
 readme = 'README.md'
 keywords = ['dsw', 'config', 'yaml', 'parser']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
```

