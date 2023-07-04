# Comparing `tmp/testit-adapter-nose-2.1.9.tar.gz` & `tmp/testit-adapter-nose-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-nose-2.1.9.tar", last modified: Fri May 26 08:37:02 2023, max compression
+gzip compressed data, was "testit-adapter-nose-2.2.0.tar", last modified: Tue Jul  4 08:50:14 2023, max compression
```

## Comparing `testit-adapter-nose-2.1.9.tar` & `testit-adapter-nose-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/src/testit_adapter_nose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:14.124272 testit-adapter-nose-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-04 08:50:14.124272 testit-adapter-nose-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:50:14.124272 testit-adapter-nose-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:14.120272 testit-adapter-nose-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:14.120272 testit-adapter-nose-2.2.0/src/testit_adapter_nose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-07-04 08:50:02.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:14.124272 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 08:50:14.000000 testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/top_level.txt
```

### Comparing `testit-adapter-nose-2.1.9/PKG-INFO` & `testit-adapter-nose-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-nose
-Version: 2.1.9
+Version: 2.2.0
 Summary: Nose adapter for Test IT
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

### Comparing `testit-adapter-nose-2.1.9/README.md` & `testit-adapter-nose-2.2.0/README.md`

 * *Files 3% similar despite different names*

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

### Comparing `testit-adapter-nose-2.1.9/setup.py` & `testit-adapter-nose-2.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testit-adapter-nose',
-    version='2.1.9',
+    version='2.2.0',
     description='Nose adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,14 +16,14 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_nose'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'nose2', 'testit-python-commons==2.1.9'],
+    install_requires=['attrs', 'nose2', 'testit-python-commons==2.2.0'],
     entry_points={
             'nose.plugins.0.10': [
                 'testit_adapter_nose = testit_adapter_nose.plugin:TmsPlugin',
             ]
     }
 )
```

### Comparing `testit-adapter-nose-2.1.9/src/testit_adapter_nose/listener.py` & `testit-adapter-nose-2.2.0/src/testit_adapter_nose/listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import testit_python_commons.services as adapter
-from testit_python_commons.services import AdapterManager
-from testit_python_commons.step import Step
+from testit_python_commons.services import (
+    AdapterManager,
+    StepManager)
 from .utils import (
     form_test,
     get_outcome,
     convert_executable_test_to_test_result_model
 )
 
 
 class AdapterListener(object):
     __executable_test = None
 
-    def __init__(self, adapter_manager: AdapterManager):
+    def __init__(self, adapter_manager: AdapterManager, step_manager: StepManager):
         self.__adapter_manager = adapter_manager
+        self.__step_manager = step_manager
 
     def start_launch(self):
         test_run_id = self.__adapter_manager.get_test_run_id()
 
         self.__adapter_manager.set_test_run_id(test_run_id)
 
     def get_tests_for_launch(self):
@@ -29,17 +31,15 @@
         outcome, message, trace = get_outcome(event)
 
         self.__executable_test['outcome'] = outcome
         self.__executable_test['message'] = message
         self.__executable_test['traces'] = trace
 
     def stop_test(self):
-        test_steps, test_results_steps = Step.get_steps_data()
-
-        self.__executable_test['steps'] = test_steps
+        test_results_steps = self.__step_manager.get_steps_tree()
         self.__executable_test['stepResults'] = test_results_steps
 
         self.__adapter_manager.write_test(
             convert_executable_test_to_test_result_model(self.__executable_test))
         self.__executable_test = None
 
     @adapter.hookimpl
```

### Comparing `testit-adapter-nose-2.1.9/src/testit_adapter_nose/plugin.py` & `testit-adapter-nose-2.2.0/src/testit_adapter_nose/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     __tests_for_launch = None
 
     def __init__(self, *args, **kwargs):
         super(TmsPlugin, self).__init__(*args, **kwargs)
 
     def startTestRun(self, event):
         self.__listener = AdapterListener(
-            TmsPluginManager.get_adapter_manager())
+            TmsPluginManager.get_adapter_manager(),
+            TmsPluginManager.get_step_manager())
 
         TmsPluginManager.get_plugin_manager().register(self.__listener)
 
         self.__listener.start_launch()
         self.__tests_for_launch = self.__listener.get_tests_for_launch()
 
     def startTest(self, event):
```

### Comparing `testit-adapter-nose-2.1.9/src/testit_adapter_nose/utils.py` & `testit-adapter-nose-2.2.0/src/testit_adapter_nose/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -312,20 +312,17 @@
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
@@ -333,30 +330,7 @@
         .set_title(executable_test['title'])\
         .set_description(executable_test['description'])\
         .set_links(executable_test['links'])\
         .set_result_links(executable_test['resultLinks'])\
         .set_labels(executable_test['labels'])\
         .set_work_item_ids(executable_test['workItemsID'])\
         .set_message(executable_test['message'])
-
-
-def step_results_to_autotest_steps_model(step_results: dict) -> typing.List[StepResult]:
-    autotest_model_steps = []
-
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
-
-        autotest_model_steps.append(step_result_model)
-
-    return autotest_model_steps
```

### Comparing `testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/PKG-INFO` & `testit-adapter-nose-2.2.0/src/testit_adapter_nose.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-nose
-Version: 2.1.9
+Version: 2.2.0
 Summary: Nose adapter for Test IT
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

