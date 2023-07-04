# Comparing `tmp/inmanta-ui-4.0.2.tar.gz` & `tmp/inmanta-ui-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmanta-ui-4.0.2.tar", last modified: Wed Apr 12 07:26:08 2023, max compression
+gzip compressed data, was "inmanta-ui-4.0.3.tar", last modified: Tue Jul  4 11:29:35 2023, max compression
```

## Comparing `inmanta-ui-4.0.2.tar` & `inmanta-ui-4.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.197758 inmanta-ui-4.0.2/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10173 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/LICENSE
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      264 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/MANIFEST.in
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      321 2023-04-12 07:26:08.197758 inmanta-ui-4.0.2/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       58 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/README.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      384 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/pyproject.toml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      558 2023-04-12 07:26:08.198758 inmanta-ui-4.0.2/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      789 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.195758 inmanta-ui-4.0.2/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.195758 inmanta-ui-4.0.2/src/inmanta_ext/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.196758 inmanta-ui-4.0.2/src/inmanta_ext/ui/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ext/ui/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      815 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ext/ui/extension.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.196758 inmanta-ui-4.0.2/src/inmanta_ui/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ui/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1765 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ui/config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      646 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ui/const.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4114 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ui/ui.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.197758 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      321 2023-04-12 07:26:08.000000 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      472 2023-04-12 07:26:08.000000 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-04-12 07:26:08.000000 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       37 2023-04-12 07:26:08.000000 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       23 2023-04-12 07:26:08.000000 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.197758 inmanta-ui-4.0.2/tests/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1962 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/tests/conftest.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2392 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/tests/web_console_handler_test.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1174 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/tox.ini
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:29:35.793805 inmanta-ui-4.0.3/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10173 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/LICENSE
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      264 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      321 2023-07-04 11:29:35.793805 inmanta-ui-4.0.3/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       58 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/README.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      384 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/pyproject.toml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      558 2023-07-04 11:29:35.794805 inmanta-ui-4.0.3/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      789 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:29:35.790804 inmanta-ui-4.0.3/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:29:35.790804 inmanta-ui-4.0.3/src/inmanta_ext/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:29:35.791805 inmanta-ui-4.0.3/src/inmanta_ext/ui/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/src/inmanta_ext/ui/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      815 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/src/inmanta_ext/ui/extension.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:29:35.792805 inmanta-ui-4.0.3/src/inmanta_ui/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/src/inmanta_ui/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1928 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/src/inmanta_ui/config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      646 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/src/inmanta_ui/const.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4567 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/src/inmanta_ui/ui.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:29:35.793805 inmanta-ui-4.0.3/src/inmanta_ui.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      321 2023-07-04 11:29:35.000000 inmanta-ui-4.0.3/src/inmanta_ui.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      472 2023-07-04 11:29:35.000000 inmanta-ui-4.0.3/src/inmanta_ui.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-07-04 11:29:35.000000 inmanta-ui-4.0.3/src/inmanta_ui.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       37 2023-07-04 11:29:35.000000 inmanta-ui-4.0.3/src/inmanta_ui.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       23 2023-07-04 11:29:35.000000 inmanta-ui-4.0.3/src/inmanta_ui.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:29:35.793805 inmanta-ui-4.0.3/tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2017 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/tests/conftest.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3057 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/tests/web_console_handler_test.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1174 2023-07-04 11:27:32.000000 inmanta-ui-4.0.3/tox.ini
```

### Comparing `inmanta-ui-4.0.2/LICENSE` & `inmanta-ui-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.2/setup.cfg` & `inmanta-ui-4.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.2/setup.py` & `inmanta-ui-4.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "inmanta-core>=6.0.0.dev",
     "tornado~=6.0",
 ]
 
 namespace_packages = ["inmanta_ext.ui"]
 
 setup(
-    version="4.0.2",
+    version="4.0.3",
     python_requires=">=3.9",  # also update classifiers
     # Meta data
     name="inmanta-ui",
     description="Slice serving the inmanta UI",
     author="Inmanta",
     author_email="code@inmanta.com",
     url="https://github.com/inmanta/inmanta-ui",
```

### Comparing `inmanta-ui-4.0.2/src/inmanta_ext/ui/__init__.py` & `inmanta-ui-4.0.3/src/inmanta_ext/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.2/src/inmanta_ext/ui/extension.py` & `inmanta-ui-4.0.3/src/inmanta_ext/ui/extension.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.2/src/inmanta_ui/__init__.py` & `inmanta-ui-4.0.3/src/inmanta_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.2/src/inmanta_ui/config.py` & `inmanta-ui-4.0.3/src/inmanta_ui/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
-from inmanta.config import Option, is_bool, is_str
+from inmanta.config import Option, is_bool, is_list, is_str
 
 web_console_enabled = Option(
     "web-ui", "console_enabled", True, "Whether the server should host the web-console or not", is_bool
 )
 web_console_path = Option(
     "web-ui",
     "console_path",
@@ -31,14 +31,22 @@
     "web-ui",
     "console_json_parser",
     "Native",
     "Whether the web-console should use the 'Native' or the 'BigInt' JSON Parser. "
     "'BigInt' is useful when the web-console has to show very large integers (larger than 2^53 - 1).",
     is_str,
 )
+web_console_features = Option(
+    "web-ui",
+    "features",
+    "",
+    "A list of features that should be enabled in the web console.",
+    is_list,
+)
+
 ################################
 # OpenID Connect authentication
 ################################
 
 oidc_realm = Option("web-ui", "oidc_realm", "inmanta", "The realm to use for OpenID Connect authentication.", is_str)
 oidc_auth_url = Option("web-ui", "oidc_auth_url", None, "The auth url of the OpenID Connect server to use.", is_str)
 oidc_client_id = Option(
```

### Comparing `inmanta-ui-4.0.2/src/inmanta_ui/const.py` & `inmanta-ui-4.0.3/src/inmanta_ui/const.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.2/src/inmanta_ui/ui.py` & `inmanta-ui-4.0.3/src/inmanta_ui/ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,39 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
+import json
+import logging
 import os
 from typing import List, cast
 
 from tornado import routing, web
 
 from inmanta.server import SLICE_SERVER, SLICE_TRANSPORT
 from inmanta.server import config as opt
 from inmanta.server import protocol
 from inmanta.server.protocol import ServerSlice
 from inmanta.server.server import Server
 from inmanta_ui.const import SLICE_UI
 
-from .config import oidc_auth_url, oidc_client_id, oidc_realm, web_console_enabled, web_console_json_parser, web_console_path
+from .config import (
+    oidc_auth_url,
+    oidc_client_id,
+    oidc_realm,
+    web_console_enabled,
+    web_console_features,
+    web_console_json_parser,
+    web_console_path,
+)
+
+LOGGER = logging.getLogger(__name__)
 
 
 class UISlice(ServerSlice):
     def __init__(self) -> None:
         super().__init__(SLICE_UI)
 
     async def prestart(self, server: protocol.Server) -> None:
@@ -53,33 +65,37 @@
 
     def get_depended_by(self) -> List[str]:
         # Ensure we are started before the HTTP endpoint becomes available
         return [SLICE_TRANSPORT]
 
     def add_web_console_handler(self, server: Server) -> None:
         if not web_console_enabled.get():
+            LOGGER.info("The web-console is disabled.")
             return
 
         path = web_console_path.get()
-        if path is None:
-            return
+        if not os.path.isdir(path):
+            raise Exception(f"The web-ui.console_path config option references the non-existing directory {path}.")
+        LOGGER.info("Serving the web-console from %s", path)
 
         config_js_content = ""
         if opt.server_enable_auth.get():
             config_js_content = f"""
         window.auth = {{
             'realm': '{oidc_realm.get()}',
             'url': '{oidc_auth_url.get()}',
             'clientId': '{oidc_client_id.get()}'
         }};\n"""  # Use the same client-id as the dashboard
         json_parser_option = web_console_json_parser.get()
         if json_parser_option == "BigInt":
             config_js_content += f"window.jsonParserId = '{json_parser_option}';\n"
 
-        server.add_static_content("/console/config.js", content=config_js_content)
+        config_js_content += f"\nexport const features = {json.dumps(web_console_features.get())};\n"
+
+        server.add_static_content(r"/console/(.*)config.js", content=config_js_content)
         location = "/console/"
         options = {"path": path, "default_filename": "index.html"}
         server._handlers.append(
             routing.Rule(
                 routing.PathMatches(r"%s(.*\.\w{2,5}$)" % location),
                 FlatFileHandler,
                 options,
```

### Comparing `inmanta-ui-4.0.2/tests/conftest.py` & `inmanta-ui-4.0.3/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 logger = logging.getLogger(__name__)
 
 
 @pytest.fixture
 def inmanta_ui_config(server_config, postgres_db, database_name, web_console_path):
     config.Config.set("server", "enabled_extensions", "ui")
     config.Config.set("web-ui", "console_path", str(web_console_path))
+    config.Config.set("web-ui", "features", "A, B, C")
 
 
 @pytest.fixture
 async def server(inmanta_ui_config, server_config):
     """
     Override standard inmanta server to allow more config to be injected
     """
```

### Comparing `inmanta-ui-4.0.2/tests/web_console_handler_test.py` & `inmanta-ui-4.0.3/tests/web_console_handler_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,7 +59,25 @@
     response_url = "http://localhost:%s/console/" % (port,)
     http_client = AsyncHTTPClient()
     request = HTTPRequest(
         url="http://localhost:%s/" % (port),
     )
     response = await http_client.fetch(request, raise_error=False)
     assert response.effective_url == response_url
+
+
+@pytest.mark.asyncio
+async def test_web_console_config(server, inmanta_ui_config):
+    base_url = f"http://127.0.0.1:{config.get_bind_port()}/console/config.js"
+    client = AsyncHTTPClient()
+    response = await client.fetch(base_url)
+    assert response.code == 200
+
+    assert '\nexport const features = ["A", "B", "C"];' in response.body.decode()
+
+    # test fetching from a deeper path
+    base_url = f"http://127.0.0.1:{config.get_bind_port()}/console/lsm/config.js"
+    client = AsyncHTTPClient()
+    response = await client.fetch(base_url)
+    assert response.code == 200
+
+    assert '\nexport const features = ["A", "B", "C"];' in response.body.decode()
```

### Comparing `inmanta-ui-4.0.2/tox.ini` & `inmanta-ui-4.0.3/tox.ini`

 * *Files identical despite different names*

