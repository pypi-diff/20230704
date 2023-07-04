# Comparing `tmp/testit-adapter-behave-2.1.9.tar.gz` & `tmp/testit-adapter-behave-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-behave-2.1.9.tar", last modified: Fri May 26 08:37:09 2023, max compression
+gzip compressed data, was "testit-adapter-behave-2.2.0.tar", last modified: Tue Jul  4 08:50:10 2023, max compression
```

## Comparing `testit-adapter-behave-2.1.9.tar` & `testit-adapter-behave-2.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:09.894211 testit-adapter-behave-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-26 08:37:09.894211 testit-adapter-behave-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:09.894211 testit-adapter-behave-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:09.886211 testit-adapter-behave-2.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:09.890211 testit-adapter-behave-2.1.9/src/testit_adapter_behave/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:09.894211 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/label.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/option.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/test_result_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/url_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/scenario_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/tags_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:09.894211 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-26 08:37:09.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 08:37:09.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:09.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 08:37:09.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 08:37:09.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.591503 testit-adapter-behave-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-07-04 08:50:10.591503 testit-adapter-behave-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:50:10.591503 testit-adapter-behave-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.587503 testit-adapter-behave-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.591503 testit-adapter-behave-2.2.0/src/testit_adapter_behave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.591503 testit-adapter-behave-2.2.0/src/testit_adapter_behave/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/models/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/models/test_result_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/models/url_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/scenario_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/tags_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-04 08:49:57.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:10.591503 testit-adapter-behave-2.2.0/src/testit_adapter_behave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-07-04 08:50:10.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-04 08:50:10.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:50:10.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-04 08:50:10.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 08:50:10.000000 testit-adapter-behave-2.2.0/src/testit_adapter_behave.egg-info/top_level.txt
```

### Comparing `testit-adapter-behave-2.1.9/PKG-INFO` & `testit-adapter-behave-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-behave
-Version: 2.1.9
+Version: 2.2.0
 Summary: Behave adapter for Test IT
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

### Comparing `testit-adapter-behave-2.1.9/README.md` & `testit-adapter-behave-2.2.0/README.md`

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

### Comparing `testit-adapter-behave-2.1.9/setup.py` & `testit-adapter-behave-2.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-behave',
-    version='2.1.9',
+    version='2.2.0',
     description='Behave adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -18,10 +18,10 @@
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_behave'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'behave',
-        'testit-python-commons==2.1.9',
+        'testit-python-commons==2.2.0',
         'attrs'],
 )
```

### Comparing `testit-adapter-behave-2.1.9/src/testit_adapter_behave/formatter.py` & `testit-adapter-behave-2.2.0/src/testit_adapter_behave/formatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
     def __init__(self, stream_opener, config):
         super(AdapterFormatter, self).__init__(stream_opener, config)
 
         option = parse_userdata(config.userdata)
 
         self.__listener = AdapterListener(
-            TmsPluginManager.get_adapter_manager(option))
+            TmsPluginManager.get_adapter_manager(option),
+            TmsPluginManager.get_step_manager())
 
         TmsPluginManager.get_plugin_manager().register(self.__listener)
 
     def start_adapter_launch(self):
         self.__listener.start_launch()
 
         self.__tests_for_launch = self.__listener.get_tests_for_launch()
```

### Comparing `testit-adapter-behave-2.1.9/src/testit_adapter_behave/listener.py` & `testit-adapter-behave-2.2.0/src/testit_adapter_behave/listener.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import testit_python_commons.services as adapter
 from testit_python_commons.models.outcome_type import OutcomeType
-from testit_python_commons.services import AdapterManager
-from testit_python_commons.step import Step
+from testit_python_commons.services import (
+    AdapterManager,
+    StepManager)
 
 from .models.test_result_step import get_test_result_step_model
 from .scenario_parser import (
     parse_scenario,
     parse_status)
 from .utils import (
-    convert_step_to_step,
-    convert_step_to_step_result,
+    convert_step_to_step_result_model,
     convert_executable_test_to_test_result_model)
 
 
 class AdapterListener(object):
     __executable_test = None
     __background_steps_count = 0
     __steps_count = 0
 
-    def __init__(self, adapter_manager: AdapterManager):
+    def __init__(self, adapter_manager: AdapterManager, step_manager: StepManager):
         self.__adapter_manager = adapter_manager
+        self.__step_manager = step_manager
 
     def start_launch(self):
         test_run_id = self.__adapter_manager.get_test_run_id()
 
         self.__adapter_manager.set_test_run_id(test_run_id)
 
     def get_tests_for_launch(self):
@@ -56,23 +57,20 @@
 
         self.__executable_test[scope][-1]['title'] = result.name
         self.__executable_test[scope][-1]['outcome'] = outcome
         self.__executable_test[scope][-1]['duration'] = round(result.duration * 1000)
         self.__executable_test['duration'] += result.duration * 1000
 
         # TODO: Add to python-commons
-        nested_steps, nested_step_results = Step.get_steps_data()
+        nested_step_results = self.__step_manager.get_steps_tree()
         executable_step = self.__executable_test[scope][-1]
         # TODO: Fix in python-commons
         result_scope = f'{scope}Results' if scope == 'setUp' else 'stepResults'
-        self.__executable_test[scope][-1] = convert_step_to_step(
-            executable_step,
-            nested_steps)
         self.__executable_test[result_scope].append(
-            convert_step_to_step_result(
+            convert_step_to_step_result_model(
                 executable_step,
                 nested_step_results))
 
         if outcome != OutcomeType.PASSED:
             self.__executable_test['traces'] = result.error_message
             self.__executable_test['outcome'] = outcome
             self.set_scenario()
```

### Comparing `testit-adapter-behave-2.1.9/src/testit_adapter_behave/scenario_parser.py` & `testit-adapter-behave-2.2.0/src/testit_adapter_behave/scenario_parser.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.9/src/testit_adapter_behave/tags_parser.py` & `testit-adapter-behave-2.2.0/src/testit_adapter_behave/tags_parser.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.9/src/testit_adapter_behave/utils.py` & `testit-adapter-behave-2.2.0/src/testit_adapter_behave/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -65,53 +65,21 @@
                 included_scenarios.append(scenarios[i])
 
         scenarios = included_scenarios
 
     return scenarios
 
 
-# TODO: Add to python-commons
-def convert_step_to_step(step, nested_steps):
-    return {
-        'title': step['title'],
-        'description': step['description'],
-        'steps': nested_steps,
-    }
-
-
-# TODO: Add to python-commons
-def convert_step_to_step_result(step, nested_step_results):
-    model = {
-        'title': step['title'],
-        'description': step['description'],
-        'duration': step['duration'],
-        'outcome': step['outcome'],
-        'parameters': step['parameters'],
-        'attachments': step['attachments'],
-        # TODO: Add to model
-        # started_on: started_on,
-        # completed_on: completed_on
-    }
-
-    if nested_step_results:
-        model['step_results'] = nested_step_results
-
-    return model
-
-
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
@@ -121,33 +89,27 @@
         .set_links(executable_test['links'])\
         .set_result_links(executable_test['resultLinks'])\
         .set_labels(executable_test['labels'])\
         .set_work_item_ids(executable_test['workItemsID'])\
         .set_message(executable_test['message'])
 
 
-def step_results_to_autotest_steps_model(step_results: dict) -> typing.List[StepResult]:
-    autotest_model_steps = []
+def convert_step_to_step_result_model(step: dict, nested_step_results: typing.List[StepResult]) -> StepResult:
+    step_result_model = StepResult()\
+        .set_title(step['title'])\
+        .set_description(step['description'])\
+        .set_outcome(step['outcome'])\
+        .set_duration(step['duration'])\
+        .set_attachments(step['attachments'])
 
-    for step_result in step_results:
-        step_result_model = StepResult()\
-            .set_title(step_result['title'])\
-            .set_description(step_result['description'])\
-            .set_outcome(step_result['outcome'])\
-            .set_duration(step_result['duration'])\
-            .set_attachments(step_result['attachments'])
-
-        if 'parameters' in step_result:
-            step_result_model.set_parameters(step_result['parameters'])
-
-        if 'step_results' in step_result:
-            step_result_model.set_step_results(
-                step_results_to_autotest_steps_model(step_result['step_results']))
+    if 'parameters' in step:
+        step_result_model.set_parameters(step['parameters'])
 
-        autotest_model_steps.append(step_result_model)
+    if nested_step_results:
+        step_result_model.set_step_results(nested_step_results)
 
-    return autotest_model_steps
+    return step_result_model
 
 
 def get_hash(value: str):
     md = hashlib.sha256(bytes(value, encoding='utf-8'))
     return md.hexdigest()
```

### Comparing `testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/PKG-INFO` & `testit-adapter-behave-2.2.0/src/testit_adapter_behave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-behave
-Version: 2.1.9
+Version: 2.2.0
 Summary: Behave adapter for Test IT
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

### Comparing `testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/SOURCES.txt` & `testit-adapter-behave-2.2.0/src/testit_adapter_behave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

