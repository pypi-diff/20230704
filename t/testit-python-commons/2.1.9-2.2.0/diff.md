# Comparing `tmp/testit-python-commons-2.1.9.tar.gz` & `tmp/testit-python-commons-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-python-commons-2.1.9.tar", last modified: Fri May 26 08:37:04 2023, max compression
+gzip compressed data, was "testit-python-commons-2.2.0.tar", last modified: Tue Jul  4 08:50:10 2023, max compression
```

## Comparing `testit-python-commons-2.1.9.tar` & `testit-python-commons-2.2.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/testit_python_commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/app_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/testit_python_commons/client/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/client/client_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/client/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/dynamic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/testit_python_commons/models/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/adapter_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/link.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/link_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/outcome_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/step_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/test_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/testit_python_commons/services/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/adapter_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/adapter_manager_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-26 08:37:04.000000 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-26 08:37:04.000000 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:04.000000 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 08:37:04.000000 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 08:37:04.000000 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.559405 testit-python-commons-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 08:50:10.559405 testit-python-commons-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:50:10.559405 testit-python-commons-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.555405 testit-python-commons-2.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.555405 testit-python-commons-2.2.0/src/testit_python_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/app_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.559405 testit-python-commons-2.2.0/src/testit_python_commons/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/client/client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/client/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/dynamic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.559405 testit-python-commons-2.2.0/src/testit_python_commons/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/models/adapter_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/models/link_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/models/outcome_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/models/step_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/models/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.559405 testit-python-commons-2.2.0/src/testit_python_commons/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/services/adapter_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/services/adapter_manager_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/services/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/services/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/services/step_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/services/step_result_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-04 08:49:58.000000 testit-python-commons-2.2.0/src/testit_python_commons/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.555405 testit-python-commons-2.2.0/src/testit_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 08:50:10.000000 testit-python-commons-2.2.0/src/testit_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-04 08:50:10.000000 testit-python-commons-2.2.0/src/testit_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:50:10.000000 testit-python-commons-2.2.0/src/testit_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-04 08:50:10.000000 testit-python-commons-2.2.0/src/testit_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-04 08:50:10.000000 testit-python-commons-2.2.0/src/testit_python_commons.egg-info/top_level.txt
```

### Comparing `testit-python-commons-2.1.9/PKG-INFO` & `testit-python-commons-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 2.1.9
+Version: 2.2.0
 Summary: Python commons for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-python-commons-2.1.9/setup.py` & `testit-python-commons-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-python-commons',
-    version='2.1.9',
+    version='2.2.0',
     description='Python commons for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
```

### Comparing `testit-python-commons-2.1.9/src/testit.py` & `testit-python-commons-2.2.0/src/testit.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     addLink,
     addLinks,
     addMessage,
     attachments,
     message
 )
 from testit_python_commons.models import LinkType
-from testit_python_commons.step import Step as step  # noqa: N813
+from testit_python_commons.step import step
 
 __all__ = [
     'externalID',
     'externalId',
     'displayName',
     'nameSpace',
     'className',
```

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/app_properties.py` & `testit-python-commons-2.2.0/src/testit_python_commons/app_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,14 +173,17 @@
             logging.error('Private token was not found!')
             raise SystemExit
 
         if properties.get('configurationid') is None:
             logging.error('Configuration ID was not found!')
             raise SystemExit
 
+        if properties.get('testrunname'):
+            properties['testrunname'] = properties['testrunname'].encode('cp1251').decode('utf8')
+
         if properties.get('certvalidation'):
             properties['certvalidation'] = properties['certvalidation'].lower()
 
         if properties.get('automaticcreationtestcases'):
             properties['automaticcreationtestcases'] = properties['automaticcreationtestcases'].lower()
 
     @staticmethod
```

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/client/api_client.py` & `testit-python-commons-2.2.0/src/testit_python_commons/client/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 class ApiClientWorker:
     def __init__(self, config: ClientConfiguration):
         client_config = Configuration(host=config.get_url())
 
         if config.get_cert_validation() == 'false':
             client_config.verify_ssl = False
 
+        client_config.proxy = config.get_proxy()
+
         self.__api_client = ApiClient(
             configuration=client_config,
             header_name='Authorization',
             header_value='PrivateToken ' + config.get_private_token()
         )
         self.__config = config
 
@@ -60,15 +62,16 @@
 
     @adapter_logger
     def write_test(self, test_result: TestResult):
         test_run_api = TestRunsApi(api_client=self.__api_client)
         autotest_api = AutoTestsApi(api_client=self.__api_client)
 
         autotest = autotest_api.get_all_auto_tests(project_id=self.__config.get_project_id(),
-                                                   external_id=test_result.get_external_id())
+                                                   external_id=test_result.get_external_id(),
+                                                  deleted=False)
 
         if autotest:
             logging.debug(f'Autotest "{test_result.get_autotest_name()}" was found')
 
             model = Converter.test_result_to_autotest_put_model(
                 test_result,
                 self.__config.get_project_id())
@@ -93,15 +96,15 @@
         if autotest_global_id:
             for work_item_id in test_result.get_work_item_ids():
                 try:
                     autotest_api.link_auto_test_to_work_item(
                         autotest_global_id,
                         work_item_id_model=WorkItemIdModel(id=work_item_id))
 
-                    logging.debug(f'Autotest "{test_result["autoTestName"]}" was linked with workItem "{work_item_id}"')
+                    logging.debug(f'Autotest "{test_result.get_autotest_name()}" was linked with workItem "{work_item_id}"')
                 except Exception as exc:
                     logging.error(f'Link with workItem "{work_item_id}" status: {exc.status}\n{exc.body}')
 
         model = Converter.test_result_to_testrun_result_post_model(
             test_result,
             self.__config.get_configuration_id())
```

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/client/client_configuration.py` & `testit-python-commons-2.2.0/src/testit_python_commons/client/client_configuration.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/client/converter.py` & `testit-python-commons-2.2.0/src/testit_python_commons/client/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
             put_model_links.append(
                 cls.link_to_link_put_model(link)
             )
 
         return put_model_links
 
     @classmethod
-    @adapter_logger
+    # @adapter_logger
     def step_results_to_autotest_steps_model(cls, step_results: typing.List[StepResult]):
         autotest_model_steps = []
 
         for step_result in step_results:
             autotest_model_steps.append(
                 AutoTestStepModel(
                     title=step_result.get_title(),
```

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/decorators.py` & `testit-python-commons-2.2.0/src/testit_python_commons/decorators.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/dynamic_methods.py` & `testit-python-commons-2.2.0/src/testit_python_commons/dynamic_methods.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
 from testit_python_commons.models.link import Link
 from testit_python_commons.services import TmsPluginManager
 from testit_python_commons.services.logger import adapter_logger
 from testit_python_commons.services.utils import Utils
-from testit_python_commons.step import Step
 
 
 @Utils.deprecated('Use "addLinks" instead.')
 @adapter_logger
 def addLink(url: str, title: str = None, type: str = None, description: str = None):  # noqa: A002,VNE003,N802
     if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_link'):
         TmsPluginManager.get_plugin_manager().hook \
@@ -57,44 +56,61 @@
         TmsPluginManager.get_plugin_manager().hook \
             .add_message(test_message=test_message)
 
 
 @Utils.deprecated('Use "addAttachments" instead.')
 @adapter_logger
 def attachments(*attachments_paths):
-    if Step.step_is_active():
-        Step.add_attachments(attachments_paths)
+    active_step = TmsPluginManager.get_step_manager().get_active_step()
+
+    if active_step:
+        attachment_ids = TmsPluginManager.get_adapter_manager().load_attachments(attachments_paths)
+
+        active_step.set_attachments(active_step.get_attachments() + attachment_ids)
     else:
         if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_attachments'):
             TmsPluginManager.get_plugin_manager().hook \
                 .add_attachments(attach_paths=attachments_paths)
 
 
 @adapter_logger
 def addAttachments(data, is_text: bool = False, name: str = None):   # noqa: N802
-    if Step.step_is_active():
-        if is_text:
-            Step.create_attachment(
-                str(data),
-                name)
-        else:
-            if isinstance(data, str):
-                Step.add_attachments([data])
-            elif isinstance(data, tuple) or isinstance(data, list):
-                Step.add_attachments(data)
-            else:
-                logging.warning(f'File ({data}) not found!')
+    active_step = TmsPluginManager.get_step_manager().get_active_step()
+
+    if active_step:
+        add_attachments_to_step(active_step, data, is_text, name)
+    else:
+        add_attachments_to_test(data, is_text, name)
+
+
+@adapter_logger
+def add_attachments_to_step(step, data, is_text: bool = False, name: str = None):
+    if is_text:
+        attachment_ids = TmsPluginManager.get_adapter_manager().create_attachment(str(data), name)
     else:
-        if is_text and hasattr(TmsPluginManager.get_plugin_manager().hook, 'create_attachment'):
+        if isinstance(data, str):
+            attachment_ids = TmsPluginManager.get_adapter_manager().load_attachments([data])
+        elif isinstance(data, tuple) or isinstance(data, list):
+            attachment_ids = TmsPluginManager.get_adapter_manager().load_attachments(data)
+        else:
+            logging.warning(f'File ({data}) not found!')
+            return
+
+    step.set_attachments(step.get_attachments() + attachment_ids)
+
+
+@adapter_logger
+def add_attachments_to_test(data, is_text: bool = False, name: str = None):
+    if is_text and hasattr(TmsPluginManager.get_plugin_manager().hook, 'create_attachment'):
+        TmsPluginManager.get_plugin_manager().hook \
+            .create_attachment(
+            body=str(data),
+            name=name)
+    elif hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_attachments'):
+        if isinstance(data, str):
             TmsPluginManager.get_plugin_manager().hook \
-                .create_attachment(
-                body=str(data),
-                name=name)
-        elif hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_attachments'):
-            if isinstance(data, str):
-                TmsPluginManager.get_plugin_manager().hook \
-                    .add_attachments(attach_paths=[data])
-            elif isinstance(data, tuple) or isinstance(data, list):
-                TmsPluginManager.get_plugin_manager().hook \
-                    .add_attachments(attach_paths=data)
-            else:
-                logging.warning(f'({data}) is not path!')
+                .add_attachments(attach_paths=[data])
+        elif isinstance(data, tuple) or isinstance(data, list):
+            TmsPluginManager.get_plugin_manager().hook \
+                .add_attachments(attach_paths=data)
+        else:
+            logging.warning(f'({data}) is not path!')
```

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/models/link.py` & `testit-python-commons-2.2.0/src/testit_python_commons/models/link.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/models/test_result.py` & `testit-python-commons-2.2.0/src/testit_python_commons/models/test_result.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/services/adapter_manager.py` & `testit-python-commons-2.2.0/src/testit_python_commons/services/adapter_manager.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/services/adapter_manager_configuration.py` & `testit-python-commons-2.2.0/src/testit_python_commons/services/adapter_manager_configuration.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/services/logger.py` & `testit-python-commons-2.2.0/src/testit_python_commons/services/logger.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/services/plugin_manager.py` & `testit-python-commons-2.2.0/src/testit_python_commons/services/plugin_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 
 from pluggy import PluginManager
 
+from testit_python_commons.services.step_manager import StepManager
 from testit_python_commons.app_properties import AppProperties
 
 
 class TmsPluginManager:
     __plugin_manager = None
     __adapter_manager = None
+    __step_manager = None
     __logger = None
 
     @classmethod
     def get_plugin_manager(cls):
         if cls.__plugin_manager is None:
             cls.__plugin_manager = PluginManager('testit')
 
@@ -32,14 +34,21 @@
             adapter_configuration = AdapterManagerConfiguration(app_properties)
 
             cls.__adapter_manager = AdapterManager(adapter_configuration, client_configuration)
 
         return cls.__adapter_manager
 
     @classmethod
+    def get_step_manager(cls) -> StepManager:
+        if cls.__step_manager is None:
+            cls.__step_manager = StepManager()
+
+        return cls.__step_manager
+
+    @classmethod
     def get_logger(cls, debug: bool = False):
         if cls.__logger is None:
             if debug:
                 logging.basicConfig(format='\n%(levelname)s (%(asctime)s): %(message)s', level=logging.DEBUG)
 
             cls.__logger = logging.getLogger('TmsLogger')
```

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons/services/utils.py` & `testit-python-commons-2.2.0/src/testit_python_commons/services/utils.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons.egg-info/PKG-INFO` & `testit-python-commons-2.2.0/src/testit_python_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 2.1.9
+Version: 2.2.0
 Summary: Python commons for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-python-commons-2.1.9/src/testit_python_commons.egg-info/SOURCES.txt` & `testit-python-commons-2.2.0/src/testit_python_commons.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,8 +23,10 @@
 src/testit_python_commons/models/step_result.py
 src/testit_python_commons/models/test_result.py
 src/testit_python_commons/services/__init__.py
 src/testit_python_commons/services/adapter_manager.py
 src/testit_python_commons/services/adapter_manager_configuration.py
 src/testit_python_commons/services/logger.py
 src/testit_python_commons/services/plugin_manager.py
+src/testit_python_commons/services/step_manager.py
+src/testit_python_commons/services/step_result_storage.py
 src/testit_python_commons/services/utils.py
```

