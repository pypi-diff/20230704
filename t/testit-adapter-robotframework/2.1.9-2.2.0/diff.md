# Comparing `tmp/testit-adapter-robotframework-2.1.9.tar.gz` & `tmp/testit-adapter-robotframework-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-robotframework-2.1.9.tar", last modified: Fri May 26 08:37:07 2023, max compression
+gzip compressed data, was "testit-adapter-robotframework-2.2.0.tar", last modified: Tue Jul  4 08:50:16 2023, max compression
```

## Comparing `testit-adapter-robotframework-2.1.9.tar` & `testit-adapter-robotframework-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:07.845603 testit-adapter-robotframework-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-26 08:37:07.845603 testit-adapter-robotframework-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:07.845603 testit-adapter-robotframework-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:07.841603 testit-adapter-robotframework-2.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:07.845603 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/TMSLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:07.845603 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-26 08:37:07.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 08:37:07.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:07.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 08:37:07.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 08:37:07.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:16.678968 testit-adapter-robotframework-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-07-04 08:50:16.678968 testit-adapter-robotframework-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-07-04 08:50:03.000000 testit-adapter-robotframework-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:50:16.678968 testit-adapter-robotframework-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-04 08:50:03.000000 testit-adapter-robotframework-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:16.678968 testit-adapter-robotframework-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:16.678968 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework/
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-04 08:50:03.000000 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework/TMSLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:03.000000 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-04 08:50:03.000000 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-07-04 08:50:03.000000 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-04 08:50:03.000000 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:16.678968 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-07-04 08:50:16.000000 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 08:50:16.000000 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:50:16.000000 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 08:50:16.000000 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-04 08:50:16.000000 testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework.egg-info/top_level.txt
```

### Comparing `testit-adapter-robotframework-2.1.9/PKG-INFO` & `testit-adapter-robotframework-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.1.9
+Version: 2.2.0
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -34,15 +34,15 @@
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
@@ -54,15 +54,15 @@
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

### Comparing `testit-adapter-robotframework-2.1.9/README.md` & `testit-adapter-robotframework-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
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
@@ -39,15 +39,15 @@
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

### Comparing `testit-adapter-robotframework-2.1.9/setup.py` & `testit-adapter-robotframework-2.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-robotframework',
-    version='2.1.9',
+    version='2.2.0',
     description='Robot Framework adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,9 +16,9 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_robotframework'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.1.9']
+    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.2.0']
 )
```

### Comparing `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/TMSLibrary.py` & `testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework/TMSLibrary.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/listeners.py` & `testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework/listeners.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/models.py` & `testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework/models.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/utils.py` & `testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework/utils.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/PKG-INFO` & `testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.1.9
+Version: 2.2.0
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -34,15 +34,15 @@
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
@@ -54,15 +54,15 @@
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

### Comparing `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/SOURCES.txt` & `testit-adapter-robotframework-2.2.0/src/testit_adapter_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

