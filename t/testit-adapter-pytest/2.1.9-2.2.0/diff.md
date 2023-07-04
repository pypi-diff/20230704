# Comparing `tmp/testit-adapter-pytest-2.1.9.tar.gz` & `tmp/testit-adapter-pytest-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-pytest-2.1.9.tar", last modified: Fri May 26 08:37:14 2023, max compression
+gzip compressed data, was "testit-adapter-pytest-2.2.0.tar", last modified: Tue Jul  4 08:50:12 2023, max compression
```

## Comparing `testit-adapter-pytest-2.1.9.tar` & `testit-adapter-pytest-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:14.716844 testit-adapter-pytest-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-05-26 08:37:14.716844 testit-adapter-pytest-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:14.716844 testit-adapter-pytest-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:14.708845 testit-adapter-pytest-2.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:14.712844 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:14.712844 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:12.162275 testit-adapter-pytest-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-07-04 08:50:12.162275 testit-adapter-pytest-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:50:12.162275 testit-adapter-pytest-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:12.158275 testit-adapter-pytest-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:12.162275 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-07-04 08:50:00.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:12.162275 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 08:50:12.000000 testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/top_level.txt
```

### Comparing `testit-adapter-pytest-2.1.9/PKG-INFO` & `testit-adapter-pytest-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 2.1.9
+Version: 2.2.0
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -36,15 +36,15 @@
 | ID of project in TMS instance [How to getting project ID?](https://github.com/testit-tms/.github/tree/main/configuration#projectid)                                                                                                                                                                                                                                                    | projectId                  | TMS_PROJECT_ID                    | tmsProjectId                  |
 | ID of configuration in TMS instance [How to getting configuration ID?](https://github.com/testit-tms/.github/tree/main/configuration#configurationid)                                                                                                                                                                                                                                  | configurationId            | TMS_CONFIGURATION_ID              | tmsConfigurationId            |
 | ID of the created test run in TMS instance.<br/>It's necessary for **adapterMode** 0 or 1                                                                                                                                                                                                                                                                                              | testRunId                  | TMS_TEST_RUN_ID                   | tmsTestRunId                  |
 | Parameter for specifying the name of test run in TMS instance (**It's optional**). If it is not provided, it is created automatically                                                                                                                                                                                                                                                  | testRunName                | TMS_TEST_RUN_NAME                 | tmsTestRunName                |
 | Adapter mode. Default value - 0. The adapter supports following modes:<br/>0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run<br/>1 - in this mode, the adapter sends all results to the test run without filtering<br/>2 - in this mode, the adapter creates a new test run and sends results to the new test run | adapterMode                | TMS_ADAPTER_MODE                  | tmsAdapterMode                |
 | It enables/disables certificate validation (**It's optional**). Default value - true                                                                                                                                                                                                                                                                                                   | certValidation             | TMS_CERT_VALIDATION               | tmsCertValidation             |
 | Mode of automatic creation test cases (**It's optional**). Default value - false. The adapter supports following modes:<br/>true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest)<br/>false - in this mode, the adapter will not create a test case                                                                    | automaticCreationTestCases | TMS_AUTOMATIC_CREATION_TEST_CASES | tmsAutomaticCreationTestCases |
-| It enables debug mode (**It's optional**)                                                                                                                                                                                                                                                                                                                                              | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
+| Url of proxy server (**It's optional**)                                                                                                                                                                                                                                                                                                                                                | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
 | Name of the configuration file If it is not provided, it is used default file name (**It's optional**)                                                                                                                                                                                                                                                                                 | -                          | TMS_CONFIG_FILE                   | tmsConfigFile                 |
 
 #### File
 
 Create **connection_config.ini** file in the root directory of the project:
 ```
 [testit]
@@ -56,15 +56,15 @@
 testRunName = TEST_RUN_NAME
 adapterMode = ADAPTER_MODE
 certValidation = CERT_VALIDATION
 automaticCreationTestCases = AUTOMATIC_CREATION_TEST_CASES
 
 # This section are optional. It enables debug mode.
 [debug]
-tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
+tmsProxy = TMS_PROXY
 ```
 
 #### Examples
 
 Launch with a connection_config.ini file in the root directory of the project:
 
 ```
```

### Comparing `testit-adapter-pytest-2.1.9/README.md` & `testit-adapter-pytest-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 | ID of project in TMS instance [How to getting project ID?](https://github.com/testit-tms/.github/tree/main/configuration#projectid)                                                                                                                                                                                                                                                    | projectId                  | TMS_PROJECT_ID                    | tmsProjectId                  |
 | ID of configuration in TMS instance [How to getting configuration ID?](https://github.com/testit-tms/.github/tree/main/configuration#configurationid)                                                                                                                                                                                                                                  | configurationId            | TMS_CONFIGURATION_ID              | tmsConfigurationId            |
 | ID of the created test run in TMS instance.<br/>It's necessary for **adapterMode** 0 or 1                                                                                                                                                                                                                                                                                              | testRunId                  | TMS_TEST_RUN_ID                   | tmsTestRunId                  |
 | Parameter for specifying the name of test run in TMS instance (**It's optional**). If it is not provided, it is created automatically                                                                                                                                                                                                                                                  | testRunName                | TMS_TEST_RUN_NAME                 | tmsTestRunName                |
 | Adapter mode. Default value - 0. The adapter supports following modes:<br/>0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run<br/>1 - in this mode, the adapter sends all results to the test run without filtering<br/>2 - in this mode, the adapter creates a new test run and sends results to the new test run | adapterMode                | TMS_ADAPTER_MODE                  | tmsAdapterMode                |
 | It enables/disables certificate validation (**It's optional**). Default value - true                                                                                                                                                                                                                                                                                                   | certValidation             | TMS_CERT_VALIDATION               | tmsCertValidation             |
 | Mode of automatic creation test cases (**It's optional**). Default value - false. The adapter supports following modes:<br/>true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest)<br/>false - in this mode, the adapter will not create a test case                                                                    | automaticCreationTestCases | TMS_AUTOMATIC_CREATION_TEST_CASES | tmsAutomaticCreationTestCases |
-| It enables debug mode (**It's optional**)                                                                                                                                                                                                                                                                                                                                              | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
+| Url of proxy server (**It's optional**)                                                                                                                                                                                                                                                                                                                                                | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
 | Name of the configuration file If it is not provided, it is used default file name (**It's optional**)                                                                                                                                                                                                                                                                                 | -                          | TMS_CONFIG_FILE                   | tmsConfigFile                 |
 
 #### File
 
 Create **connection_config.ini** file in the root directory of the project:
 ```
 [testit]
@@ -41,15 +41,15 @@
 testRunName = TEST_RUN_NAME
 adapterMode = ADAPTER_MODE
 certValidation = CERT_VALIDATION
 automaticCreationTestCases = AUTOMATIC_CREATION_TEST_CASES
 
 # This section are optional. It enables debug mode.
 [debug]
-tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
+tmsProxy = TMS_PROXY
 ```
 
 #### Examples
 
 Launch with a connection_config.ini file in the root directory of the project:
 
 ```
```

### Comparing `testit-adapter-pytest-2.1.9/setup.py` & `testit-adapter-pytest-2.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-pytest',
-    version='2.1.9',
+    version='2.2.0',
     description='Pytest adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,10 +16,10 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_pytest'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['pytest', 'pytest-xdist', 'testit-python-commons==2.1.9'],
+    install_requires=['pytest', 'pytest-xdist', 'testit-python-commons==2.2.0'],
     entry_points={'pytest11': ['testit_adapter_pytest = testit_adapter_pytest.plugin']}
 )
```

### Comparing `testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/listener.py` & `testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/listener.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from packaging import version
 
 import pytest
 
 import testit_python_commons.services as adapter
 from testit_python_commons.models.outcome_type import OutcomeType
 from testit_python_commons.services import AdapterManager
-from testit_python_commons.step import Step
+from testit_python_commons.services import StepManager
 
 import testit_adapter_pytest.utils as utils
 
 STATUS = {
     'passed': OutcomeType.PASSED,
     'failed': OutcomeType.FAILED,
     'skipped': OutcomeType.SKIPPED
@@ -19,16 +19,17 @@
 
 
 class TmsListener(object):
     __executable_test = None
     __pytest_check_info = None
     __failures = None
 
-    def __init__(self, adapter_manager: AdapterManager):
+    def __init__(self, adapter_manager: AdapterManager, step_manager: StepManager):
         self.__adapter_manager = adapter_manager
+        self.__step_manager = step_manager
 
     @pytest.hookimpl
     def pytest_configure(self, config):
         if not hasattr(config, "workerinput") and not hasattr(self, "test_run_id"):
             config.test_run_id = self.__adapter_manager.get_test_run_id()
         else:
             config.test_run_id = pickle.loads(config.workerinput["test_run_id"])
@@ -121,40 +122,37 @@
 
         self.__executable_test = utils.form_test(item)
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_fixture_setup(self, fixturedef):
         yield
         if self.__executable_test:
-            steps_data, results_steps_data = Step.get_steps_data()
+            results_steps_data = self.__step_manager.get_steps_tree()
 
             if fixturedef.scope == 'function':
-                self.__executable_test['setUp'] += steps_data
                 self.__executable_test['setUpResults'] += results_steps_data
 
     @pytest.hookimpl(hookwrapper=True, trylast=True)
     def pytest_runtest_call(self):
         yield
 
         if not self.__executable_test:
             return
 
-        test_steps, test_results_steps = Step.get_steps_data()
-        self.__executable_test['steps'] = test_steps
+        test_results_steps = self.__step_manager.get_steps_tree()
         self.__executable_test['stepResults'] = test_results_steps
 
     @pytest.hookimpl
     def pytest_fixture_post_finalizer(self, fixturedef):
         if not self.__executable_test:
             return
 
-        teardown_steps, teardown_results_steps = Step.get_steps_data()
+        teardown_results_steps = self.__step_manager.get_steps_tree()
 
         if fixturedef.scope == 'function':
-            self.__executable_test['tearDown'] += teardown_steps
             self.__executable_test['tearDownResults'] += teardown_results_steps
 
     @pytest.hookimpl
     def pytest_runtest_logreport(self, report):
         if self.__executable_test:
             if report.when == 'setup':
                 self.__executable_test['outcome'] = STATUS.get(report.outcome, None)
```

### Comparing `testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/plugin.py` & `testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,11 +100,12 @@
     )
 
 
 @pytest.mark.tryfirst
 def pytest_cmdline_main(config):
     if config.option.tms_report:
         listener = TmsListener(
-            TmsPluginManager.get_adapter_manager(config.option))
+            TmsPluginManager.get_adapter_manager(config.option),
+            TmsPluginManager.get_step_manager())
 
         config.pluginmanager.register(listener)
         TmsPluginManager.get_plugin_manager().register(listener)
```

### Comparing `testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/utils.py` & `testit-adapter-pytest-2.2.0/src/testit_adapter_pytest/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,22 +239,21 @@
     if not test_workitems_id:
         return []
 
     if hasattr(item, 'array_parametrize_mark_id'):
         result, param_id = mass_param_attribute_collector(
             test_workitems_id[0], item.own_markers,
             item.array_parametrize_mark_id, item.index)
+
         if param_id is not None and test_workitems_id[0][1:-1] in \
                 item.name[(item.name.find('[') + 1):(item.name.rfind(']'))].split(
                     '-')[param_id]:
             return result
-        else:
-            return [result]
-    else:
-        return test_workitems_id
+
+    return test_workitems_id
 
 
 def param_attribute_collector(attribute, run_param):
     result = attribute
     param_keys = re.findall(r"\{(.*?)\}", attribute)
     if len(param_keys) > 0:
         for param_key in param_keys:
@@ -320,20 +319,17 @@
     md = hashlib.sha256(bytes(value, encoding='utf-8'))
     return md.hexdigest()
 
 def convert_executable_test_to_test_result_model(executable_test: dict) -> TestResult:
     return TestResult()\
         .set_external_id(executable_test['externalID'])\
         .set_autotest_name(executable_test['autoTestName'])\
-        .set_step_results(
-            step_results_to_autotest_steps_model(executable_test['stepResults']))\
-        .set_setup_results(
-            step_results_to_autotest_steps_model(executable_test['setUpResults']))\
-        .set_teardown_results(
-            step_results_to_autotest_steps_model(executable_test['tearDownResults']))\
+        .set_step_results(executable_test['stepResults'])\
+        .set_setup_results(executable_test['setUpResults'])\
+        .set_teardown_results(executable_test['tearDownResults'])\
         .set_duration(executable_test['duration'])\
         .set_outcome(executable_test['outcome'])\
         .set_traces(executable_test['traces'])\
         .set_attachments(executable_test['attachments'])\
         .set_parameters(executable_test['parameters'])\
         .set_properties(executable_test['properties'])\
         .set_namespace(executable_test['namespace'])\
```

### Comparing `testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/PKG-INFO` & `testit-adapter-pytest-2.2.0/src/testit_adapter_pytest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 2.1.9
+Version: 2.2.0
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -36,15 +36,15 @@
 | ID of project in TMS instance [How to getting project ID?](https://github.com/testit-tms/.github/tree/main/configuration#projectid)                                                                                                                                                                                                                                                    | projectId                  | TMS_PROJECT_ID                    | tmsProjectId                  |
 | ID of configuration in TMS instance [How to getting configuration ID?](https://github.com/testit-tms/.github/tree/main/configuration#configurationid)                                                                                                                                                                                                                                  | configurationId            | TMS_CONFIGURATION_ID              | tmsConfigurationId            |
 | ID of the created test run in TMS instance.<br/>It's necessary for **adapterMode** 0 or 1                                                                                                                                                                                                                                                                                              | testRunId                  | TMS_TEST_RUN_ID                   | tmsTestRunId                  |
 | Parameter for specifying the name of test run in TMS instance (**It's optional**). If it is not provided, it is created automatically                                                                                                                                                                                                                                                  | testRunName                | TMS_TEST_RUN_NAME                 | tmsTestRunName                |
 | Adapter mode. Default value - 0. The adapter supports following modes:<br/>0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run<br/>1 - in this mode, the adapter sends all results to the test run without filtering<br/>2 - in this mode, the adapter creates a new test run and sends results to the new test run | adapterMode                | TMS_ADAPTER_MODE                  | tmsAdapterMode                |
 | It enables/disables certificate validation (**It's optional**). Default value - true                                                                                                                                                                                                                                                                                                   | certValidation             | TMS_CERT_VALIDATION               | tmsCertValidation             |
 | Mode of automatic creation test cases (**It's optional**). Default value - false. The adapter supports following modes:<br/>true - in this mode, the adapter will create a test case linked to the created autotest (not to the updated autotest)<br/>false - in this mode, the adapter will not create a test case                                                                    | automaticCreationTestCases | TMS_AUTOMATIC_CREATION_TEST_CASES | tmsAutomaticCreationTestCases |
-| It enables debug mode (**It's optional**)                                                                                                                                                                                                                                                                                                                                              | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
+| Url of proxy server (**It's optional**)                                                                                                                                                                                                                                                                                                                                                | tmsProxy                   | TMS_PROXY                         | tmsProxy                      |
 | Name of the configuration file If it is not provided, it is used default file name (**It's optional**)                                                                                                                                                                                                                                                                                 | -                          | TMS_CONFIG_FILE                   | tmsConfigFile                 |
 
 #### File
 
 Create **connection_config.ini** file in the root directory of the project:
 ```
 [testit]
@@ -56,15 +56,15 @@
 testRunName = TEST_RUN_NAME
 adapterMode = ADAPTER_MODE
 certValidation = CERT_VALIDATION
 automaticCreationTestCases = AUTOMATIC_CREATION_TEST_CASES
 
 # This section are optional. It enables debug mode.
 [debug]
-tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
+tmsProxy = TMS_PROXY
 ```
 
 #### Examples
 
 Launch with a connection_config.ini file in the root directory of the project:
 
 ```
```

