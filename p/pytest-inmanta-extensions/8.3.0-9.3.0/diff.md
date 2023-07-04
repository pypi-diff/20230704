# Comparing `tmp/pytest-inmanta-extensions-8.3.0.tar.gz` & `tmp/pytest-inmanta-extensions-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-inmanta-extensions-8.3.0.tar", last modified: Wed Apr 12 07:26:49 2023, max compression
+gzip compressed data, was "pytest-inmanta-extensions-9.3.0.tar", last modified: Tue Jul  4 11:30:21 2023, max compression
```

## Comparing `pytest-inmanta-extensions-8.3.0.tar` & `pytest-inmanta-extensions-9.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.465607 pytest-inmanta-extensions-8.3.0/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      199 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/MANIFEST.in
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-04-12 07:26:49.465607 pytest-inmanta-extensions-8.3.0/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      467 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/README.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       59 2023-04-12 07:26:49.466607 pytest-inmanta-extensions-8.3.0/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2481 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.463606 pytest-inmanta-extensions-8.3.0/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.464607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    68790 2023-04-12 07:26:26.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/conftest.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.464607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.462607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.464607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6223 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.chain
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2069 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.crt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1237 2023-04-12 07:26:26.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/server.crt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1679 2023-04-12 07:26:26.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/server.open.key
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.464607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      980 2023-04-12 07:26:26.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/common.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.465607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/simple_project/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      212 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/simple_project/main.cf
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      185 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/simple_project/project.yml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      685 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/plugin.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    25441 2023-04-12 07:26:26.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/utils.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.465607 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      882 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       55 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      122 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       14 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      199 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      467 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/README.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       59 2023-07-04 11:30:21.852827 pytest-inmanta-extensions-9.3.0/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2481 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.848827 pytest-inmanta-extensions-9.3.0/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.849827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    70339 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/conftest.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.850827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.848827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.850827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6223 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.chain
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2069 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.crt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1237 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.crt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1679 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.open.key
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.850827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      980 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/common.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/simple_project/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      212 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/simple_project/main.cf
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      185 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/simple_project/project.yml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      685 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/plugin.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    25613 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/utils.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      882 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       55 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      122 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       14 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/top_level.txt
```

### Comparing `pytest-inmanta-extensions-8.3.0/PKG-INFO` & `pytest-inmanta-extensions-9.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-extensions
-Version: 8.3.0
+Version: 9.3.0
 Summary: Inmanta tests package
 Home-page: https://github.com/inmanta/inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Keywords: pytest inmanta tests
```

### Comparing `pytest-inmanta-extensions-8.3.0/setup.py` & `pytest-inmanta-extensions-9.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     Contact: code@inmanta.com
 """
 from os import path
 
 from setuptools import find_namespace_packages, setup
 
-version = "8.3.0"
+version = "9.3.0"
 
 requires = [
     "asyncpg",
     "click",
     f"inmanta-core~={version}.dev",
     "pip2pi",
     "pyformance",
```

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/__init__.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/conftest.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     Contact: code@inmanta.com
 """
 import warnings
 
 import toml
 from inmanta.config import AuthJWTConfig
+from inmanta.logging import InmantaLoggerConfig
 
 """
 About the use of @parametrize_any and @slowtest:
 
 For parametrized tests:
 - if the test is fast and tests different things for each parameter, use @parametrize
 - if the parameters only slightly increase the coverage of the test (some different exception path,...), use @parametrize_any.
@@ -91,25 +92,25 @@
 import pyformance
 import pytest
 from asyncpg.exceptions import DuplicateDatabaseError
 from click import testing
 from pkg_resources import Requirement
 from pyformance.registry import MetricsRegistry
 from tornado import netutil
-from tornado.platform.asyncio import AnyThreadEventLoopPolicy
 
 import build.env
 import inmanta
 import inmanta.agent
 import inmanta.app
 import inmanta.compiler as compiler
 import inmanta.compiler.config
 import inmanta.main
 import inmanta.user_setup
 from inmanta import config, const, data, env, loader, protocol, resources
+from inmanta.agent import config as agent_cfg
 from inmanta.agent import handler
 from inmanta.agent.agent import Agent
 from inmanta.ast import CompilerException
 from inmanta.data.schema import SCHEMA_VERSION_TABLE
 from inmanta.db import util as db_util
 from inmanta.env import LocalPackagePath, VirtualEnv, mock_process_env
 from inmanta.export import ResourceDict, cfg_env, unknown_parameters
@@ -122,14 +123,15 @@
 from inmanta.server.protocol import Server, SliceStartupException
 from inmanta.server.services import orchestrationservice
 from inmanta.server.services.compilerservice import CompilerService, CompileRun
 from inmanta.types import JsonType
 from inmanta.warnings import WarningsManager
 from libpip2pi.commands import dir2pi
 from packaging.version import Version
+from pytest_postgresql import factories
 
 # Import test modules differently when conftest is put into the inmanta_tests packages
 PYTEST_PLUGIN_MODE: bool = __file__ and os.path.dirname(__file__).split("/")[-1] == "inmanta_tests"
 if PYTEST_PLUGIN_MODE:
     from inmanta_tests import utils  # noqa: F401
 else:
     import utils
@@ -144,14 +146,16 @@
 
 TABLES_TO_KEEP = [x.table_name() for x in data._classes] + ["resourceaction_resource"]  # Join table
 
 # Save the cwd as early as possible to prevent that it gets overridden by another fixture
 # before it's saved.
 initial_cwd = os.getcwd()
 
+pg_logfile = os.path.join(initial_cwd, "pg.log")
+
 
 def _pytest_configure_plugin_mode(config: "pytest.Config") -> None:
     # register custom markers
     config.addinivalue_line(
         "markers",
         "slowtest",
     )
@@ -220,28 +224,61 @@
         timestamp: str = match.group(1)
         test_creation_date: datetime.datetime = datetime.datetime(int(timestamp[0:4]), int(timestamp[4:6]), int(timestamp[6:8]))
         elapsed_days: int = (datetime.datetime.today() - test_creation_date).days
         if elapsed_days > 30:
             pytest.skip("Skipping old migration test")
 
 
+# adds a custom log location for postgres
+postgresql_proc_with_log = factories.postgresql_proc(startparams=f"--log='{pg_logfile}'")
+
+
 @pytest.fixture(scope="session")
 def postgres_db(request: pytest.FixtureRequest):
     """This fixture loads the pytest-postgresql fixture. When --postgresql-host is set, it will use the noproc
     fixture to use an external database. Without this option, an "embedded" postgres is started.
     """
+
     option_name = "postgresql_host"
     conf = request.config.getoption(option_name)
     if conf:
         fixture = "postgresql_noproc"
     else:
-        fixture = "postgresql_proc"
+        fixture = "postgresql_proc_with_log"
 
     logger.info("Using database fixture %s", fixture)
-    yield request.getfixturevalue(fixture)
+    pg = request.getfixturevalue(fixture)
+    yield pg
+
+    if os.path.exists(pg_logfile):
+        has_deadlock = False
+        with open(pg_logfile, "r") as fh:
+            for line in fh:
+                if "deadlock" in line:
+                    has_deadlock = True
+                    break
+            sublogger = logging.getLogger("pytest.postgresql.deadlock")
+            for line in fh:
+                sublogger.warning("%s", line)
+        os.remove(pg_logfile)
+        assert not has_deadlock
+
+
+@pytest.fixture
+async def run_without_keeping_psql_logs(postgres_db):
+    if os.path.exists(pg_logfile):
+        # Store the original content of the logfile
+        with open(pg_logfile, "r") as file:
+            original_content = file.read()
+    yield
+
+    if os.path.exists(pg_logfile):
+        # Restore the original content of the logfile
+        with open(pg_logfile, "w") as file:
+            file.write(original_content)
 
 
 @pytest.fixture
 async def postgres_db_debug(postgres_db, database_name) -> abc.AsyncIterator[None]:
     """
     Fixture meant for debugging through manual interaction with the database. Run pytest with `-s/--capture=no`.
     """
@@ -511,14 +548,15 @@
     handler.Commander.reset()
     Project._project = None
     unknown_parameters.clear()
     InmantaBootloader.AVAILABLE_EXTENSIONS = None
     V2ModuleBuilder.DISABLE_ISOLATED_ENV_BUILDER_CACHE = False
     compiler.Finalizers.reset_finalizers()
     AuthJWTConfig.reset()
+    InmantaLoggerConfig.clean_instance()
 
 
 @pytest.fixture()
 def disable_isolated_env_builder_cache() -> None:
     V2ModuleBuilder.DISABLE_ISOLATED_ENV_BUILDER_CACHE = True
 
 
@@ -528,19 +566,19 @@
     Restore the current working directory after search test.
     """
     yield
     os.chdir(initial_cwd)
 
 
 @pytest.fixture(scope="function")
-def no_agent_backoff():
-    backoff = inmanta.agent.agent.GET_RESOURCE_BACKOFF
-    inmanta.agent.agent.GET_RESOURCE_BACKOFF = 0
+def no_agent_backoff(inmanta_config: ConfigParser) -> None:
+    old_backoff = agent_cfg.agent_get_resource_backoff.get()
+    inmanta_config.set(section="config", option="agent-get-resource-backoff", value="0")
     yield
-    inmanta.agent.agent.GET_RESOURCE_BACKOFF = backoff
+    inmanta_config.set(section="config", option="agent-get-resource-backoff", value=str(old_backoff))
 
 
 @pytest.fixture()
 def free_socket():
     bound_sockets = []
 
     def _free_socket():
@@ -629,24 +667,29 @@
         return a
 
     yield create_agent
     await asyncio.gather(*[agent.stop() for agent in started_agents])
 
 
 @pytest.fixture(scope="function")
-async def autostarted_agent(server, environment):
+async def autostarted_agent(server, client, environment):
     """Configure agent1 as an autostarted agent."""
-    env = await data.Environment.get_by_id(uuid.UUID(environment))
-    await env.set(data.AUTOSTART_AGENT_MAP, {"internal": "", "agent1": ""})
-    await env.set(data.AUTO_DEPLOY, True)
-    await env.set(data.PUSH_ON_AUTO_DEPLOY, True)
+    result = await client.set_setting(environment, data.AUTOSTART_AGENT_MAP, {"internal": "", "agent1": ""})
+    assert result.code == 200
+    result = await client.set_setting(environment, data.AUTO_DEPLOY, True)
+    assert result.code == 200
+    result = await client.set_setting(environment, data.PUSH_ON_AUTO_DEPLOY, True)
+    assert result.code == 200
     # disable deploy and repair intervals
-    await env.set(data.AUTOSTART_AGENT_DEPLOY_INTERVAL, 0)
-    await env.set(data.AUTOSTART_AGENT_REPAIR_INTERVAL, 0)
-    await env.set(data.AUTOSTART_ON_START, True)
+    result = await client.set_setting(environment, data.AUTOSTART_AGENT_DEPLOY_INTERVAL, 0)
+    assert result.code == 200
+    result = await client.set_setting(environment, data.AUTOSTART_AGENT_REPAIR_INTERVAL, 0)
+    assert result.code == 200
+    result = await client.set_setting(environment, data.AUTOSTART_ON_START, True)
+    assert result.code == 200
 
 
 @pytest.fixture(scope="function")
 def client_v2(server):
     client = protocol.Client("client", version_match=VersionMatch.exact, exact_version=2)
     yield client
 
@@ -986,20 +1029,14 @@
         if resources:
             # we are behind report formatting, so write to report, not item
             rep.sections.append(
                 ("Resources Kept", "\n".join(["%s %s" % (label, resource) for label, resource in resources.items()]))
             )
 
 
-async def off_main_thread(func):
-    # work around for https://github.com/pytest-dev/pytest-asyncio/issues/168
-    asyncio.set_event_loop_policy(AnyThreadEventLoopPolicy())
-    return await asyncio.get_event_loop().run_in_executor(None, func)
-
-
 class ReentrantVirtualEnv(VirtualEnv):
     """
     A virtual env that can be de-activated and re-activated
 
     This allows faster reloading due to improved caching of the working set
 
     This is intended for use in testcases to require a lot of venv switching
@@ -1032,15 +1069,15 @@
             pkg_resources.working_set = self.working_set
             self._using_venv = True
 
 
 class SnippetCompilationTest(KeepOnFail):
     def setUpClass(self):
         self.libs = tempfile.mkdtemp()
-        self.repo = "https://github.com/inmanta/"
+        self.repo: str = "https://github.com/inmanta/"
         self.env = tempfile.mkdtemp()
         self.venv = ReentrantVirtualEnv(env_path=self.env)
         config.Config.load_config()
         self.keep_shared = False
         self.project = None
 
     def tearDownClass(self):
@@ -1076,14 +1113,15 @@
         add_to_module_path: Optional[List[str]] = None,
         python_package_sources: Optional[List[str]] = None,
         project_requires: Optional[List[InmantaModuleRequirement]] = None,
         python_requires: Optional[List[Requirement]] = None,
         install_mode: Optional[InstallMode] = None,
         relation_precedence_rules: Optional[List[RelationPrecedenceRule]] = None,
         strict_deps_check: Optional[bool] = None,
+        use_pip_config_file: Optional[bool] = False,
     ) -> Project:
         """
         Sets up the project to compile a snippet of inmanta DSL. Activates the compiler environment (and patches
         env.process_env).
 
         :param install_project: Install the project and all its modules. This is required to be able to compile the model.
         :param install_v2_modules: Indicates which V2 modules should be installed in the compiler venv
@@ -1094,23 +1132,26 @@
                                  file
         :param python_requires: The dependencies on Python packages providing v2 modules.
         :param install_mode: The install mode to configure in the project.yml file of the inmanta project. If None,
                              no install mode is set explicitly in the project.yml file.
         :param relation_precedence_policy: The relation precedence policy that should be stored in the project.yml file of the
                                            Inmanta project.
         :param strict_deps_check: True iff the returned project should have strict dependency checking enabled.
+        :param use_pip_config_file: True iff the pip config file should be used and no source is required for v2 to work
+                                    False if a package source is needed for v2 modules to work
         """
         self.setup_for_snippet_external(
             snippet,
             add_to_module_path,
             python_package_sources,
             project_requires,
             python_requires,
             install_mode,
             relation_precedence_rules,
+            use_pip_config_file,
         )
         return self._load_project(autostd, install_project, install_v2_modules, strict_deps_check=strict_deps_check)
 
     def _load_project(
         self,
         autostd: bool,
         install_project: bool,
@@ -1158,14 +1199,15 @@
         snippet: str,
         add_to_module_path: Optional[List[str]] = None,
         python_package_sources: Optional[List[str]] = None,
         project_requires: Optional[List[InmantaModuleRequirement]] = None,
         python_requires: Optional[List[Requirement]] = None,
         install_mode: Optional[InstallMode] = None,
         relation_precedence_rules: Optional[List[RelationPrecedenceRule]] = None,
+        use_pip_config_file: bool = False,
     ) -> None:
         add_to_module_path = add_to_module_path if add_to_module_path is not None else []
         python_package_sources = python_package_sources if python_package_sources is not None else []
         project_requires = project_requires if project_requires is not None else []
         python_requires = python_requires if python_requires is not None else []
         relation_precedence_rules = relation_precedence_rules if relation_precedence_rules else []
         with open(os.path.join(self.project_dir, "project.yml"), "w", encoding="utf-8") as cfg:
@@ -1175,31 +1217,30 @@
             modulepath: {self._get_modulepath_for_project_yml_file(add_to_module_path)}
             downloadpath: {self.libs}
             version: 1.0
             repo:
                 - {{type: git, url: {self.repo} }}
             """.rstrip()
             )
-            if python_package_sources:
-                cfg.write(
-                    "".join(
-                        f"""
-                - {{type: package, url: {source} }}
-                        """.rstrip()
-                        for source in python_package_sources
-                    )
-                )
+
             if relation_precedence_rules:
                 cfg.write("\n            relation_precedence_policy:\n")
                 cfg.write("\n".join(f"                - {rule}" for rule in relation_precedence_rules))
             if project_requires:
                 cfg.write("\n            requires:\n")
                 cfg.write("\n".join(f"                - {req}" for req in project_requires))
             if install_mode:
                 cfg.write(f"\n            install_mode: {install_mode.value}")
+            cfg.write(
+                f"""
+            pip:
+                use_config_file: {use_pip_config_file}
+                index_urls: [{", ".join(url for url in python_package_sources)}]
+            """
+            )
         with open(os.path.join(self.project_dir, "requirements.txt"), "w", encoding="utf-8") as fd:
             fd.write("\n".join(str(req) for req in python_requires))
         self.main = os.path.join(self.project_dir, "main.cf")
         with open(self.main, "w", encoding="utf-8") as x:
             x.write(snippet)
 
     def _get_modulepath_for_project_yml_file(self, add_to_module_path: List[str] = []) -> str:
@@ -1278,22 +1319,23 @@
     async def do_export_and_deploy(
         self,
         include_status=False,
         do_raise=True,
         partial_compile: bool = False,
         resource_sets_to_remove: Optional[List[str]] = None,
     ) -> Union[tuple[int, ResourceDict], tuple[int, ResourceDict, dict[str, const.ResourceState], Optional[dict[str, object]]]]:
-        return await off_main_thread(
+        return await asyncio.get_running_loop().run_in_executor(
+            None,
             lambda: self._do_export(
                 deploy=True,
                 include_status=include_status,
                 do_raise=do_raise,
                 partial_compile=partial_compile,
                 resource_sets_to_remove=resource_sets_to_remove,
-            )
+            ),
         )
 
     def setup_for_error(self, snippet, shouldbe, indent_offset=0):
         """
         Set up project to expect an error during compilation or project install.
         """
         try:
@@ -1394,18 +1436,15 @@
 
 @pytest.fixture
 def cli(caplog):
     # caplog will break this code when emitting any log line to cli
     # due to mysterious interference when juggling with sys.stdout
     # https://github.com/pytest-dev/pytest/issues/10553
     with caplog.at_level(logging.FATAL):
-        # work around for https://github.com/pytest-dev/pytest-asyncio/issues/168
-        asyncio.set_event_loop_policy(AnyThreadEventLoopPolicy())
-        o = CLI()
-        yield o
+        yield CLI()
 
 
 class AsyncCleaner(object):
     def __init__(self):
         self.register = []
 
     def add(self, method):
```

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.chain` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.chain`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.crt` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.crt`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/server.crt` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.crt`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/server.open.key` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.open.key`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/common.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/common.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/plugin.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/utils.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,23 +266,27 @@
     async with data.Compile._connection_pool.acquire() as con:
         result = await con.fetch(q)
 
     for row in result:
         print(row)
 
 
-async def wait_for_version(client, environment, cnt):
+async def wait_for_version(client, environment, cnt, compile_timeout: int = 30):
+    """
+    :param compile_timeout: Raise an AssertionError if the compilation didn't finish after this amount of seconds.
+    """
+
     # Wait until the server is no longer compiling
     # wait for it to finish
     async def compile_done():
         compiling = await client.is_compiling(environment)
         code = compiling.code
         return code == 204
 
-    await retry_limited(compile_done, 30)
+    await retry_limited(compile_done, compile_timeout)
 
     reports = await client.get_reports(environment)
     for report in reports.result["reports"]:
         data = await client.get_report(report["id"])
         print(json.dumps(data.result, indent=4))
         assert report["success"]
```

### Comparing `pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO` & `pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-extensions
-Version: 8.3.0
+Version: 9.3.0
 Summary: Inmanta tests package
 Home-page: https://github.com/inmanta/inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Keywords: pytest inmanta tests
```

### Comparing `pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt` & `pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

