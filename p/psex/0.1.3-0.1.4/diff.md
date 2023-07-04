# Comparing `tmp/psex-0.1.3.tar.gz` & `tmp/psex-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psex-0.1.3.tar", max compression
+gzip compressed data, was "psex-0.1.4.tar", max compression
```

## Comparing `psex-0.1.3.tar` & `psex-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1061 2022-08-11 05:37:04.272502 psex-0.1.3/LICENSE
--rw-r--r--   0        0        0     2096 2022-08-11 05:37:04.272502 psex-0.1.3/README.md
--rw-r--r--   0        0        0       54 2022-08-16 02:34:24.368643 psex-0.1.3/psex/__init__.py
--rw-r--r--   0        0        0       29 2022-08-11 05:37:04.275835 psex-0.1.3/psex/funcs/__init__.py
--rw-r--r--   0        0        0     2050 2022-08-11 06:09:31.369567 psex-0.1.3/psex/funcs/assetio.py
--rw-r--r--   0        0        0     1255 2022-08-16 02:34:24.521977 psex-0.1.3/psex/pse.py
--rw-r--r--   0        0        0       42 2022-08-11 05:37:04.275835 psex-0.1.3/psex/weaks/__init__.py
--rw-r--r--   0        0        0      181 2022-08-11 05:37:04.275835 psex-0.1.3/psex/weaks/clickhouse.yaml
--rw-r--r--   0        0        0      238 2022-08-11 05:37:04.275835 psex-0.1.3/psex/weaks/elasticsearch.yaml
--rw-r--r--   0        0        0      154 2022-08-11 05:37:04.275835 psex-0.1.3/psex/weaks/mongodb.yaml
--rw-r--r--   0        0        0      275 2022-08-11 05:37:04.275835 psex-0.1.3/psex/weaks/mssql.yaml
--rw-r--r--   0        0        0      132 2022-08-11 05:37:04.275835 psex-0.1.3/psex/weaks/mysql.yaml
--rw-r--r--   0        0        0      135 2022-08-11 05:37:04.275835 psex-0.1.3/psex/weaks/postgresql.yaml
--rw-r--r--   0        0        0      236 2022-08-11 05:37:04.275835 psex-0.1.3/psex/weaks/redis.yaml
--rw-r--r--   0        0        0      342 2022-08-11 06:09:31.289567 psex-0.1.3/psex/weaks/weak_user_pwd.py
--rw-r--r--   0        0        0      686 2022-08-16 02:34:24.478643 psex-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2923 2022-08-16 02:35:03.785175 psex-0.1.3/setup.py
--rw-r--r--   0        0        0     2840 2022-08-16 02:35:03.785438 psex-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-04 01:06:15.837545 psex-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2430 2023-07-04 03:00:37.551682 psex-0.1.4/README.md
+-rw-r--r--   0        0        0       54 2023-07-04 03:13:11.889027 psex-0.1.4/psex/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-04 01:06:15.837545 psex-0.1.4/psex/funcs/__init__.py
+-rw-r--r--   0        0        0     2310 2023-07-04 03:00:37.558349 psex-0.1.4/psex/funcs/assetio.py
+-rw-r--r--   0        0        0     1255 2023-07-04 01:06:15.837545 psex-0.1.4/psex/pse.py
+-rw-r--r--   0        0        0       42 2023-07-04 01:06:15.837545 psex-0.1.4/psex/weaks/__init__.py
+-rw-r--r--   0        0        0     1394 2023-07-04 03:05:54.576687 psex-0.1.4/psex/weaks/clickhouse.yaml
+-rw-r--r--   0        0        0      745 2023-07-04 03:05:54.610020 psex-0.1.4/psex/weaks/elasticsearch.yaml
+-rw-r--r--   0        0        0     1208 2023-07-04 03:13:11.949027 psex-0.1.4/psex/weaks/mongodb.yaml
+-rw-r--r--   0        0        0      664 2023-07-04 03:13:11.965694 psex-0.1.4/psex/weaks/mssql.yaml
+-rw-r--r--   0        0        0      558 2023-07-04 03:00:37.611682 psex-0.1.4/psex/weaks/mysql.yaml
+-rw-r--r--   0        0        0      692 2023-07-04 03:13:11.989028 psex-0.1.4/psex/weaks/postgresql.yaml
+-rw-r--r--   0        0        0      455 2023-07-04 03:13:12.005694 psex-0.1.4/psex/weaks/redis.yaml
+-rw-r--r--   0        0        0      342 2023-07-04 01:06:15.837545 psex-0.1.4/psex/weaks/weak_user_pwd.py
+-rw-r--r--   0        0        0      692 2023-07-04 03:13:42.525857 psex-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 psex-0.1.4/PKG-INFO
```

### Comparing `psex-0.1.3/LICENSE` & `psex-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psex-0.1.3/README.md` & `psex-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 ## Usage
 
 ### PSE Sample:
 
 ```python
 # Title: xxxxxxx
-# Author: antx
-# Email: wkaifeng2007@163.com
+# Author: antx-code
+# Email: 7877940+antx-code@users.noreply.github.com
 
 from loguru import logger
 from redis import Redis
 from psex import ScannerEngine
 from psex.funcs.assetio import AssetIO
 from psex.weaks import weak_passwords
 
@@ -52,15 +52,26 @@
         connection = Redis(host=args[0], port=args[1], password=args[3], db=0, socket_connect_timeout=self.timeout,
                            socket_timeout=self.timeout)
         return connection
 
     @logger.catch(level='ERROR')
     def dia(self):
         asset_io = AssetIO()
-        ips = asset_io.get_file_assets('source_redis.csv')
+        ips = asset_io.get_file_assets('input/source_redis.csv')
+        """
+        
+        or use fofa search and parse assets to verify.
+        
+        grammar = 'xxx'
+        api_key='xxxxxxxxxxxxxxxxxxxxxx'
+        api_email='xxxx@email.com'
+        ips = asset_io.get_fofa_assets(grammar, api_key, api_email, 'fofa_redis.csv')
+        
+        """
+        
         passwords = weak_passwords('redis')
         for password in passwords:
             for ip_port in ips:
                 ip_port = ip_port.strip()
                 ip = ip_port.split(':')[0]
                 port = int(ip_port.split(':')[1])
                 logger.debug(f'Connecting to {ip} ......')
```

### Comparing `psex-0.1.3/psex/funcs/assetio.py` & `psex-0.1.4/psex/funcs/assetio.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,46 +5,51 @@
 
 
 class AssetIO():
     def __init__(self):
         pass
 
     @logger.catch(level='ERROR')
-    def get_fofa_assets(self, grammar: str, fofa_key: str, fofa_email: str, filename: str = None):
+    def get_fofa_assets(self, grammar: str, fofa_key: str, fofa_email: str, to_file: str = None):
         assets = []
         fofa = Fofa()
         fofa.set_config(api_key=fofa_key, api_email=fofa_email)
         logger.warning(f'[+] the asset account of grammar: {grammar} are: {fofa.asset_counts(grammar)}')
         pages = fofa.asset_pages(grammar)
         for page in range(1, pages + 1):
             logger.info(f'[*] page {page}')
             urls = fofa.assets(grammar, page)
             for url in urls:
                 asset = url.strip().split('//')[1]
                 assets.append(asset)
-                if filename:
-                    with open(f'input/{filename}', 'a+') as f:
+                if to_file:
+                    base_path = os.getcwd()
+                    if not os.path.exists(f'{base_path}/input'):
+                        os.mkdir(f'{base_path}/input')
+                    with open(f'{base_path}/input/{to_file}', 'a+') as f:
                         f.write(asset + '\n')
         return assets
 
     @logger.catch(level='ERROR')
     def get_file_assets(self, filename: str):
         assets = []
-        with open(f'input/{filename}', 'r+') as f:
+        with open(filename, 'r+') as f:
             ips = f.readlines()
         for asset in ips:
             assets.append(asset.strip())
         assets = list(set(assets))
         return assets
 
     @logger.catch(level='ERROR')
     def save2file(self, filename: str, ip: str, port: int, username: str, password: str):
         username = '空' if username == '' else username
         password = '空' if password == '' else password
         base_path = os.getcwd()
+        if not os.path.exists(f'{base_path}/output'):
+            os.mkdir(f'{base_path}/output')
         target_file_path = f'{base_path}/output/{filename}.csv'
         fieldnames = ['IP', 'Port', 'Username', 'Password']
         content = {
             'IP': ip,
             'Port': port,
             'Username': username,
             'Password': password
```

### Comparing `psex-0.1.3/psex/pse.py` & `psex-0.1.4/psex/pse.py`

 * *Files identical despite different names*

### Comparing `psex-0.1.3/pyproject.toml` & `psex-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "psex"
-version = "0.1.3"
+version = "0.1.4"
 description = "A simple, fast and powerful password scanner engine tool was built by antx."
 authors = ["antx-code <wkaifeng2007@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/antx-code/psex"
 repository = "https://github.com/antx-code/psex"
 keywords = ["poc", "engine", "psex", "database", "weak password"]
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple"
-default = true
+priority = "primary"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pocx = "^0.2.2"
+pocx = "^0.2.3"
 pyyaml = "^6.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `psex-0.1.3/setup.py` & `psex-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,109 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: psex
+Version: 0.1.4
+Summary: A simple, fast and powerful password scanner engine tool was built by antx.
+Home-page: https://github.com/antx-code/psex
+License: MIT
+Keywords: poc,engine,psex,database,weak password
+Author: antx-code
+Author-email: wkaifeng2007@163.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pocx (>=0.2.3,<0.3.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Repository, https://github.com/antx-code/psex
+Description-Content-Type: text/markdown
+
+# psex
+A simple, fast and powerful password scanner engine tool was built by antx.
+
+## Description
+psex is a simple, fast and powerful password scanner engine tool was built by antx. psex also 
+support some useful features, which like fofa search and parse assets to verify. psex has been built in some weak username and password. 
+
+## Install
+
+```bash
+pip3 install psex
+```
+
+## Usage
+
+### PSE Sample:
+
+```python
+# Title: xxxxxxx
+# Author: antx-code
+# Email: 7877940+antx-code@users.noreply.github.com
+
+from loguru import logger
+from redis import Redis
+from psex import ScannerEngine
+from psex.funcs.assetio import AssetIO
+from psex.weaks import weak_passwords
+
+
+class Scanner(ScannerEngine):
+    def __init__(self):
+        super(Scanner, self).__init__()
+
+    @logger.catch(level='ERROR')
+    def is_connected(self, connection):
+        """
+        check if the connection is connected.
+        """
+        try:
+            connection.ping()
+            return True
+        except Exception as e:
+            return False
+
+    @logger.catch(level='ERROR')
+    def create_connect(self, *args):
+        """
+        
+        create a connection.
+        
+        """
+        connection = Redis(host=args[0], port=args[1], password=args[3], db=0, socket_connect_timeout=self.timeout,
+                           socket_timeout=self.timeout)
+        return connection
+
+    @logger.catch(level='ERROR')
+    def dia(self):
+        asset_io = AssetIO()
+        ips = asset_io.get_file_assets('input/source_redis.csv')
+        """
+        
+        or use fofa search and parse assets to verify.
+        
+        grammar = 'xxx'
+        api_key='xxxxxxxxxxxxxxxxxxxxxx'
+        api_email='xxxx@email.com'
+        ips = asset_io.get_fofa_assets(grammar, api_key, api_email, 'fofa_redis.csv')
+        
+        """
+        
+        passwords = weak_passwords('redis')
+        for password in passwords:
+            for ip_port in ips:
+                ip_port = ip_port.strip()
+                ip = ip_port.split(':')[0]
+                port = int(ip_port.split(':')[1])
+                logger.debug(f'Connecting to {ip} ......')
+                logger.warning(f'Testing {ip_port} with password: "{password}" !')
+                result = self.poc(ip, port, '', password)
+                if result:
+                    asset_io.save2file('redis_success', ip, port, '', password)
+
+
+if __name__ == '__main__':
+    ds = Scanner()
+    ds.dia()
+```
 
-packages = \
-['psex', 'psex.funcs', 'psex.weaks']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pocx>=0.2.2,<0.3.0', 'pyyaml>=6.0,<7.0']
-
-setup_kwargs = {
-    'name': 'psex',
-    'version': '0.1.3',
-    'description': 'A simple, fast and powerful password scanner engine tool was built by antx.',
-    'long_description': '# psex\nA simple, fast and powerful password scanner engine tool was built by antx.\n\n## Description\npsex is a simple, fast and powerful password scanner engine tool was built by antx. psex also \nsupport some useful features, which like fofa search and parse assets to verify. psex has been built in some weak username and password. \n\n## Install\n\n```bash\npip3 install psex\n```\n\n## Usage\n\n### PSE Sample:\n\n```python\n# Title: xxxxxxx\n# Author: antx\n# Email: wkaifeng2007@163.com\n\nfrom loguru import logger\nfrom redis import Redis\nfrom psex import ScannerEngine\nfrom psex.funcs.assetio import AssetIO\nfrom psex.weaks import weak_passwords\n\n\nclass Scanner(ScannerEngine):\n    def __init__(self):\n        super(Scanner, self).__init__()\n\n    @logger.catch(level=\'ERROR\')\n    def is_connected(self, connection):\n        """\n        check if the connection is connected.\n        """\n        try:\n            connection.ping()\n            return True\n        except Exception as e:\n            return False\n\n    @logger.catch(level=\'ERROR\')\n    def create_connect(self, *args):\n        """\n        \n        create a connection.\n        \n        """\n        connection = Redis(host=args[0], port=args[1], password=args[3], db=0, socket_connect_timeout=self.timeout,\n                           socket_timeout=self.timeout)\n        return connection\n\n    @logger.catch(level=\'ERROR\')\n    def dia(self):\n        asset_io = AssetIO()\n        ips = asset_io.get_file_assets(\'source_redis.csv\')\n        passwords = weak_passwords(\'redis\')\n        for password in passwords:\n            for ip_port in ips:\n                ip_port = ip_port.strip()\n                ip = ip_port.split(\':\')[0]\n                port = int(ip_port.split(\':\')[1])\n                logger.debug(f\'Connecting to {ip} ......\')\n                logger.warning(f\'Testing {ip_port} with password: "{password}" !\')\n                result = self.poc(ip, port, \'\', password)\n                if result:\n                    asset_io.save2file(\'redis_success\', ip, port, \'\', password)\n\n\nif __name__ == \'__main__\':\n    ds = Scanner()\n    ds.dia()\n```\n',
-    'author': 'antx-code',
-    'author_email': 'wkaifeng2007@163.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/antx-code/psex',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

