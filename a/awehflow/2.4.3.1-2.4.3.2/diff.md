# Comparing `tmp/awehflow-2.4.3.1.tar.gz` & `tmp/awehflow-2.4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awehflow-2.4.3.1.tar", last modified: Wed Jun 28 16:20:36 2023, max compression
+gzip compressed data, was "dist/awehflow-2.4.3.2.tar", last modified: Tue Jul  4 13:51:26 2023, max compression
```

## Comparing `awehflow-2.4.3.1.tar` & `awehflow-2.4.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10513 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10068 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow/alerts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/alerts/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3727 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/alerts/googlechat.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/alerts/slack.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/config.py
--rw-rw-rw-   0 root         (0) root         (0)    13108 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/events/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/events/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/events/gcp.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/events/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow/operators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/operators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5996 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/operators/etl.py
--rw-rw-rw-   0 root         (0) root         (0)     3307 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/operators/flow.py
--rw-rw-rw-   0 root         (0) root         (0)    10418 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/operators/gcp.py
--rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/operators/gcs.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/operators/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     7215 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/operators/taxonomy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow/sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/sensors/http.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/sensors/sql_sensor.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/awehflow/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10513 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      778 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/awehflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 16:20:36.000000 awehflow-2.4.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-28 16:20:19.000000 awehflow-2.4.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8472 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8027 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/alerts/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3727 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/alerts/googlechat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4551 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/alerts/slack.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    12283 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/events/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/events/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/events/gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/events/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow/operators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5996 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/operators/etl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/operators/flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     8828 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/operators/gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10526 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/operators/gcs.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/operators/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     7053 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/operators/taxonomy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/sensors/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/sensors/sql_sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/awehflow/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8472 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      778 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/awehflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 13:51:26.000000 awehflow-2.4.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-04 13:51:09.000000 awehflow-2.4.3.2/setup.py
```

### Comparing `awehflow-2.4.3.1/LICENSE` & `awehflow-2.4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/PKG-INFO` & `awehflow-2.4.3.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awehflow
-Version: 2.4.3.1
+Version: 2.4.3.2
 Summary: Configuration based Apache Airflow
 Home-page: UNKNOWN
 Author: Philip Perold
 Author-email: philip@spatialedge.co.za
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -20,73 +20,14 @@
 ![coverage report](https://gitlab.com/spatialedge/awehflow/badges/master/coverage.svg)
 ![pipeline status](https://gitlab.com/spatialedge/awehflow/badges/master/pipeline.svg)
 
 Configuration based Airflow pipelines with metric logging and alerting out the box.
 
 ## Prerequisites
 
-### Development environment
-In order to develop awehflow for a given version of Airflow follow these steps
-1. Install and configure miniconda
-  1. On Mac, if running ARM create an x86 version of conda using the snippet below
-    ```bash
-    ### add this to ~/.zshrc (or ~/.bashrc if you're using Bash)
-    create_x86_conda_environment () {
-      # create a conda environment using x86 architecture
-      # first argument is environment name, all subsequent arguments will be passed to `conda create`
-      # example usage: create_x86_conda_environment myenv_x86 python=3.9
-      
-      CONDA_SUBDIR=osx-64 conda create $@
-      conda activate $2
-      conda config --env --set subdir osx-64
-    }
-  ```
-1. Define the version that you'd like to install
-  ```bash
-  export AIRFLOW_VERSION="2.1.4"
-  ```
-1. Create a conda environment for your version of Airflow, the bash below
-  ```bash
-  create_x86_conda_environment -n "airflow_$AIRFLOW_VERSION" "python=3.8.12"
-  ```
-1. Configure the AIRFLOW_HOME directory
-  ```bash
-  conda deactivate
-  conda activate "airflow_$AIRFLOW_VERSION"
-  conda env config vars set AIRFLOW_HOME="$HOME/airflow/airflow_$AIRFLOW_VERSION"
-  conda deactivate
-  conda activate airflow_"$AIRFLOW_VERSION"
-  echo "$AIRFLOW_HOME"
-  ```
-1. Install airflow using `pip`
-  ```bash
-  conda activate airflow_$AIRFLOW_VERSION
-  pip install --no-cache-dir "apache-airflow==$AIRFLOW_VERSION"
-  ```
-1. Install required providers
-  ```bash
-  conda activate airflow_$AIRFLOW_VERSION
-  pip install --no-cache-dir "apache-airflow[google]==$AIRFLOW_VERSION"
-  pip install --no-cache-dir "apache-airflow[postgres]==$AIRFLOW_VERSION"
-  ```
-  1. On MacOS ARM install the psycop binary
-    ```bash
-    pip install --no-cache-dir "psycopg2-binary==`pip list | grep -i 'psycopg2 ' | tr -s ' ' | cut -d' ' -f 2`"
-    ```
-1. Customisation per version
-  1. For `2.2.3`
-    1. force the MarkupSafe package version
-      ```bash
-      pip install --no-cache-dir markupsafe==2.0.1
-      ```
-1. Init the airflow db
-  ```bash
-  airflow db init
-  ```
-
 You will need the following to run this code:
   * Python 3
 
 ## Installation
 
 ```
 pip install awehflow[default]
```

### Comparing `awehflow-2.4.3.1/README.md` & `awehflow-2.4.3.2/awehflow.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,33 @@
+Metadata-Version: 2.1
+Name: awehflow
+Version: 2.4.3.2
+Summary: Configuration based Apache Airflow
+Home-page: UNKNOWN
+Author: Philip Perold
+Author-email: philip@spatialedge.co.za
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: default
+Provides-Extra: composer
+License-File: LICENSE
+
 # Awehflow
 
 ![coverage report](https://gitlab.com/spatialedge/awehflow/badges/master/coverage.svg)
 ![pipeline status](https://gitlab.com/spatialedge/awehflow/badges/master/pipeline.svg)
 
 Configuration based Airflow pipelines with metric logging and alerting out the box.
 
 ## Prerequisites
 
-### Development environment
-In order to develop awehflow for a given version of Airflow follow these steps
-1. Install and configure miniconda
-  1. On Mac, if running ARM create an x86 version of conda using the snippet below
-    ```bash
-    ### add this to ~/.zshrc (or ~/.bashrc if you're using Bash)
-    create_x86_conda_environment () {
-      # create a conda environment using x86 architecture
-      # first argument is environment name, all subsequent arguments will be passed to `conda create`
-      # example usage: create_x86_conda_environment myenv_x86 python=3.9
-      
-      CONDA_SUBDIR=osx-64 conda create $@
-      conda activate $2
-      conda config --env --set subdir osx-64
-    }
-  ```
-1. Define the version that you'd like to install
-  ```bash
-  export AIRFLOW_VERSION="2.1.4"
-  ```
-1. Create a conda environment for your version of Airflow, the bash below
-  ```bash
-  create_x86_conda_environment -n "airflow_$AIRFLOW_VERSION" "python=3.8.12"
-  ```
-1. Configure the AIRFLOW_HOME directory
-  ```bash
-  conda deactivate
-  conda activate "airflow_$AIRFLOW_VERSION"
-  conda env config vars set AIRFLOW_HOME="$HOME/airflow/airflow_$AIRFLOW_VERSION"
-  conda deactivate
-  conda activate airflow_"$AIRFLOW_VERSION"
-  echo "$AIRFLOW_HOME"
-  ```
-1. Install airflow using `pip`
-  ```bash
-  conda activate airflow_$AIRFLOW_VERSION
-  pip install --no-cache-dir "apache-airflow==$AIRFLOW_VERSION"
-  ```
-1. Install required providers
-  ```bash
-  conda activate airflow_$AIRFLOW_VERSION
-  pip install --no-cache-dir "apache-airflow[google]==$AIRFLOW_VERSION"
-  pip install --no-cache-dir "apache-airflow[postgres]==$AIRFLOW_VERSION"
-  ```
-  1. On MacOS ARM install the psycop binary
-    ```bash
-    pip install --no-cache-dir "psycopg2-binary==`pip list | grep -i 'psycopg2 ' | tr -s ' ' | cut -d' ' -f 2`"
-    ```
-1. Customisation per version
-  1. For `2.2.3`
-    1. force the MarkupSafe package version
-      ```bash
-      pip install --no-cache-dir markupsafe==2.0.1
-      ```
-1. Init the airflow db
-  ```bash
-  airflow db init
-  ```
-
 You will need the following to run this code:
   * Python 3
 
 ## Installation
 
 ```
 pip install awehflow[default]
@@ -297,7 +255,9 @@
 
 or to run code coverage too:
 
 ```bash
 coverage run -m unittest discover tests && coverage html
 ```
 
+
+
```

### Comparing `awehflow-2.4.3.1/awehflow/alerts/googlechat.py` & `awehflow-2.4.3.2/awehflow/alerts/googlechat.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/awehflow/alerts/slack.py` & `awehflow-2.4.3.2/awehflow/alerts/slack.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/awehflow/config.py` & `awehflow-2.4.3.2/awehflow/config.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/awehflow/core.py` & `awehflow-2.4.3.2/awehflow/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import os
 from pyhocon import ConfigFactory
 
 import pendulum
 from pendulum.tz import timezone as pd_tz
 
 import yaml
-import re
-from airflow.version import version as airflow_version
-from airflow.models.dag import DAG
+from airflow import DAG
 from airflow.configuration import conf as airflow_config
 from airflow.utils.trigger_rule import TriggerRule
 from jinja2.utils import import_string
 
 from awehflow.config import Config
 from awehflow.events.alerts import AlertsEventHandler
 from awehflow.operators.flow import StartOperator
@@ -133,43 +131,28 @@
             'end_date': config.get('end_date'),
             'email_on_failure': False,
             'email_on_retry': False,
             'retries': 0,
             'on_failure_callback': self.generate_on_failure_callback(config, event_handlers)
         }, config.get('default_dag_args'))
 
-        local_airflow_version = int(re.sub('[^0-9]', '', airflow_version))
-
-        concurrency_default = None
-        if local_airflow_version < 220:
-            concurrency_default = airflow_config.getint('core', 'dag_concurrency')
-        else:
-            concurrency_default = airflow_config.getint('core', 'max_active_tasks_per_dag')
-
-        dag_kwargs = dict()
-        dag_kwargs['dag_id'] = config.get('dag_id') # type: ignore
-        dag_kwargs['description'] = config.get('description')
-        dag_kwargs['schedule_interval'] = config.get('schedule')
-        dag_kwargs['catchup'] = config.get('catchup', False)
-        dag_kwargs['template_searchpath'] = self.configs_path
-        dag_kwargs['user_defined_macros'] = self.generate_user_defined_macros(config)
-        dag_kwargs['default_args'] = default_dag_args
-        dag_kwargs['concurrency'] = config.get('concurrency', config.get('dag_concurrency', concurrency_default)) # type: ignore
-        
-        if local_airflow_version >= 220:
-            dag_kwargs['max_active_tasks'] = config.get('max_active_tasks', airflow_config.getint('core', 'max_active_tasks_per_dag'))
-        
-        dag_kwargs['max_active_runs'] = config.get('max_active_runs', airflow_config.getint('core', 'max_active_runs_per_dag'))
-        dag_kwargs['dagrun_timeout'] = config.get('dagrun_timeout', None)
-        dag_kwargs['doc_md'] = config.get('doc_md', None)
-        dag_kwargs['access_control'] = config.get('access_control', None)
-        dag_kwargs['is_paused_upon_creation'] = config.get('is_paused_upon_creation', None)
-        dag_kwargs['tags'] = config.get('tags', None)
-
-        dag = DAG(**dag_kwargs)
+        dag = DAG(dag_id=config.get('dag_id'), # type: ignore
+            description=config.get('description'),
+            schedule_interval=config.get('schedule'),
+            catchup=config.get('catchup', False),
+            template_searchpath=self.configs_path,
+            user_defined_macros=self.generate_user_defined_macros(config),
+            default_args=default_dag_args,
+            concurrency=config.get('dag_concurrency', airflow_config.getint('core', 'dag_concurrency')),
+            max_active_runs=config.get('max_active_runs_per_dag', airflow_config.getint('core', 'max_active_runs_per_dag')),
+            dagrun_timeout=config.get('dagrun_timeout', None),
+            doc_md=config.get('doc_md', None),
+            access_control=config.get('access_control', None),
+            is_paused_upon_creation=config.get('is_paused_upon_creation', None),
+            tags=config.get('tags', None))
 
         start = StartOperator(
             task_id='start',
             dag=dag,
             project=self.project,
             job_name=config.get('name'),
             engineers=config.get('engineers'),
```

### Comparing `awehflow-2.4.3.1/awehflow/events/base.py` & `awehflow-2.4.3.2/awehflow/events/base.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/awehflow/events/gcp.py` & `awehflow-2.4.3.2/awehflow/events/gcp.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/awehflow/events/postgres.py` & `awehflow-2.4.3.2/awehflow/events/postgres.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/awehflow/operators/etl.py` & `awehflow-2.4.3.2/awehflow/operators/etl.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/awehflow/operators/flow.py` & `awehflow-2.4.3.2/awehflow/operators/flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import logging
-import re
 
 from airflow.models.baseoperator import BaseOperator
 from airflow.utils.decorators import apply_defaults
-from airflow.version import version as airflow_version
 
 from awehflow.utils import utc_now, JobStatus
 
 
 class EventEmittingOperator(BaseOperator):
     @apply_defaults
     def __init__(
@@ -53,28 +51,23 @@
         self.project = project
         self.job_name = job_name
         self.engineers = engineers
 
 
 class StartOperator(FlowOperator):
     def execute(self, context):
-        if int(re.sub('[^0-9]', '', airflow_version)) < 220:
-            next_execution_date = context['next_execution_date']
-        else:
-            next_execution_date = context['data_interval_end']
-
         self.emit_event('start', {
             'run_id': context['dag_run'].run_id,
             'dag_id': self.dag.dag_id,
             'name': self.job_name,
             'project': self.project,
             'engineers': self.engineers,
             'status': JobStatus.RUNNING,
             'start_time': utc_now(),
-            'reference_time': next_execution_date
+            'reference_time': context['next_execution_date']
         })
 
 
 class SuccessOperator(FlowOperator):
     def execute(self, context):
         self.emit_event('success', {
             'run_id': context['dag_run'].run_id,
```

### Comparing `awehflow-2.4.3.1/awehflow/operators/gcp.py` & `awehflow-2.4.3.2/awehflow/operators/gcp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from typing import Optional
-import re
-
-from airflow.version import version as airflow_version
 from airflow.providers.google.cloud.hooks.bigquery import BigQueryHook
 from airflow.providers.google.cloud.operators.bigquery import BigQueryExecuteQueryOperator
 from airflow.exceptions import AirflowException
 from airflow.models.baseoperator import BaseOperator
 from airflow.models.skipmixin import SkipMixin
 from airflow.utils.decorators import apply_defaults
 
@@ -24,26 +20,20 @@
                  **kwargs):
         super(BigQueryJobOperator, self).__init__(*args, **kwargs)
         self.cleanup_query = cleanup_query 
                 
 
     def execute(self, context):
         if self.hook is None:
-            hook_kwargs=dict()
-            hook_kwargs['gcp_conn_id'] = self.gcp_conn_id
-            hook_kwargs['use_legacy_sql'] = self.use_legacy_sql
-            hook_kwargs['location'] = self.location
-
-            if int(re.sub('[^0-9]', '', airflow_version)) < 240:
-                hook_kwargs['delegate_to'] = self.delegate_to
-            else:
-                hook_kwargs['impersonation_chain'] = self.impersonation_chain
-
             self.hook = BigQueryHook(
-                **hook_kwargs
+                gcp_conn_id=self.gcp_conn_id,
+                use_legacy_sql=self.use_legacy_sql,
+                delegate_to=self.delegate_to,
+                location=self.location,
+                impersonation_chain=self.impersonation_chain,
             )
             credential_email = self.hook._get_credentials_email()
             self.log.info(f"Created BigQueryHook with account: {credential_email}")
 
         if self.cleanup_query:
             if self.destination_dataset_table == None:
                 raise ValueError('No destination_dataset_table was given, set a destination_dataset_table in the following format: project_id.dataset_id.table_id')
@@ -119,36 +109,31 @@
     """
 
     @apply_defaults
     def __init__(
             self,
             task_ids: list=[],
             xcom_key: str='return_value',
-            bigquery_conn_id: str=None, # type: ignore
-            gcp_conn_id: str='google_cloud_default',
+            bigquery_conn_id: str='bigquery_default',
+            gcp_conn_id: str=None, # type: ignore
             *args, **kwargs):
         """
         :param task_ids: List of task_ids saying which tasks to sink their job_metrics for
         :param xcom_key: XCOM key used to pull the bigquery job id from the specified tasks
         """
         self.task_ids = task_ids
         self.xcom_key = xcom_key
-        self.gcp_conn_id = gcp_conn_id
-        if bigquery_conn_id:
-            self.gcp_conn_id = bigquery_conn_id
+        self.gcp_conn_id = bigquery_conn_id
+        if gcp_conn_id:
+            self.gcp_conn_id = gcp_conn_id
 
         super(BigQueryJobTaskMetricOperator, self).__init__(*args, **kwargs)
-
+        
 
     def execute(self, context):
-        if int(re.sub('[^0-9]', '', airflow_version)) < 220:
-            next_execution_date = context['next_execution_date']
-        else:
-            next_execution_date = context['data_interval_end']
-    
         hook = BigQueryHook(
             gcp_conn_id=self.gcp_conn_id
         )
         credential_email = hook._get_credentials_email()
         self.log.info(f"Created BigQueryHook with account: {credential_email}")
 
         jobs = hook.get_service().jobs()
@@ -168,15 +153,15 @@
                     self.emit_event('task_metric', {
                         'run_id': context['dag_run'].run_id,
                         'dag_id': self.dag.dag_id,
                         'job_name': context['task'].params.get('job_name', ''),
                         'task_id': task_id,
                         'value': job,
                         'created_time': utc_now(),
-                        'reference_time': next_execution_date
+                        'reference_time': context['next_execution_date']
                     })
 
 
 class BigQueryShortCircuitOperator(BaseOperator, SkipMixin):
     """
     A "short circuit" operator that can be used a a "pre check" system.  The supplied sql statement should turn a single BOOL column.
 
@@ -188,25 +173,25 @@
     template_fields = ('sql',)
     template_ext = ('.sql',)
 
     @apply_defaults
     def __init__(
             self,
             sql: str,
-            gcp_conn_id: str='google_cloud_default',
-            bigquery_conn_id: str=None, # type: ignore
+            bigquery_conn_id: str='bigquery_default',
+            gcp_conn_id: str=None, # type: ignore
             use_legacy_sql: bool=True,
             *args, **kwargs):
         
         self.sql = sql
-        self.gcp_conn_id = gcp_conn_id
-        if bigquery_conn_id:
-            self.gcp_conn_id = bigquery_conn_id
-        self.use_legacy_sql = use_legacy_sql
+        self.gcp_conn_id = bigquery_conn_id
+        if gcp_conn_id:
+            self.gcp_conn_id = gcp_conn_id
 
+        self.use_legacy_sql = use_legacy_sql
         super(BigQueryShortCircuitOperator, self).__init__(*args, **kwargs)
 
 
     def execute(self, context):
         records = self.db_hook.get_first(self.sql)
         success = records and all([bool(r) for r in records])
 
@@ -225,38 +210,7 @@
 
     @property
     def db_hook(self):
         hook = BigQueryHook(gcp_conn_id=self.gcp_conn_id, use_legacy_sql=self.use_legacy_sql)
         credential_email = hook._get_credentials_email()
         self.log.info(f"Created BigQueryHook with account: {credential_email}")
         return hook
-
-
-class BigQueryPushFirstResultToXComOperator(BaseOperator):
-    template_fields = ('sql',)
-
-    @apply_defaults
-    def __init__(
-            self,
-            sql,
-            gcp_conn_id: str='gcp_default',
-            bigquery_conn_id: Optional[str] = None,
-            use_legacy_sql=True,
-            *args, **kwargs):
-        """
-        :param sql: Source table name that has been materialized (:project_id.:dataset_id.:table_name)
-        :param use_legacy_sql: Whether to execute the query in legacy SQL mode or not
-        """
-        if bigquery_conn_id:
-            gcp_conn_id = bigquery_conn_id
-
-        super(BigQueryPushFirstResultToXComOperator, self).__init__(*args, **kwargs)
-        self.sql = sql
-        self.use_legacy_sql = use_legacy_sql
-        self.gcp_conn_id = gcp_conn_id
-
-    def execute(self, context):
-        hook = BigQueryHook(gcp_conn_id=self.gcp_conn_id, use_legacy_sql=self.use_legacy_sql)
-        result = hook.get_first(self.sql)
-        if not result:
-            raise Exception("No materialized date found")
-        return result
```

### Comparing `awehflow-2.4.3.1/awehflow/operators/gcs.py` & `awehflow-2.4.3.2/awehflow/operators/gcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
                  temp_dataset_name: str,
                  print_header: bool = True,
                  field_delimiter: str = ',',
                  bigquery_conn_id: str = 'bigquery_default',
                  gcp_conn_id: str = 'gcp_conn_id',
                  location=None,
                  *args, **kwargs) -> None:
-
         """
         Create an instance of the BigQueryCSVExtractAndComposeOperator
         :param source_dataset_table: The source BigQuery table to extract, including the data set and table name ie. dev_temp.some_table_to_extract
         :param destination_object_name: The destination filename as a bucket URI ie gs://dev_extract_data/some_sub_folder/my_extract.csv
         :param temp_bucket_name: The temporary bucket area where files can be extracted and composed
         :param temp_dataset_name: A temp dataset where temporary tables can be created and saved, while processing
         :param print_header: Whether or not the extracted data should contain a header or not
```

### Comparing `awehflow-2.4.3.1/awehflow/operators/metrics.py` & `awehflow-2.4.3.2/awehflow/operators/metrics.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/awehflow/operators/taxonomy.py` & `awehflow-2.4.3.2/awehflow/operators/taxonomy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Optional
 from airflow.utils.decorators import apply_defaults
 from airflow.operators.python import PythonVirtualenvOperator
 
-def set_policy_tag(project_id, dataset_id, table_names, policy_tags, gcp_conn_id, testing=False):
+def set_policy_tag(project_id, dataset_id, table_names, policy_tags, bigquery_conn_id, testing=False):
     from airflow.providers.google.cloud.hooks.bigquery import BigQueryHook
 
     from google.api_core.exceptions import NotFound
     from google.cloud import bigquery
     from google.cloud.bigquery import schema
 
     import logging
@@ -80,23 +79,23 @@
                                                     policy_tags=schema.PolicyTagList((get_pii_tag(column, policy_tags),))))
             else:
                 logging.debug(f'Not modifying column: {column.name}')
                 new_schema.append(column)
 
         return new_schema
 
-    def update_policy_tag(project_id: str, dataset_id: str, table_names: list, policy_tags: dict, gcp_conn_id: str): #pragma: no cover
+    def update_policy_tag(project_id: str, dataset_id: str, table_names: list, policy_tags: dict, bigquery_conn_id: str): #pragma: no cover
         hook = BigQueryHook(
-            gcp_conn_id=gcp_conn_id,
+            gcp_conn_id=bigquery_conn_id,
             use_legacy_sql=False
         )
         credential_email = hook._get_credentials_email()
         logging.info(f"Created BigQueryHook with account: {credential_email}")
 
-        client = hook.get_client()
+        client = bigquery.Client(project=project_id, credentials=hook._get_credentials())
 
         if isinstance(table_names, str):
             table_names = [table_names]
 
         if not isinstance(table_names, list):
             raise ValueError(f'table_names should be of type str or list, not of type {type(table_names)}')
 
@@ -120,15 +119,15 @@
             'get_pii_tag': get_pii_tag,
             'get_pii_description': get_pii_description,
             '_schema_builder': _schema_builder,
             'update_policy_tag': update_policy_tag
             
         }
 
-    update_policy_tag(project_id, dataset_id, table_names, policy_tags, gcp_conn_id) #pragma: no cover
+    update_policy_tag(project_id, dataset_id, table_names, policy_tags, bigquery_conn_id) #pragma: no cover
     
 class ApplyTaxonomyOperator(PythonVirtualenvOperator): #pragma: no cover
     # """
     # Adds policy tags to columns in a BigQuery Table.
 
     # param project_id: The name of the project that the BigQuery table is in.
     # type project_id: str
@@ -137,38 +136,28 @@
     # param table_name: The table name that the policy tags should be applied to.
     # type table_name: str
     # param policy_tags: The policy tags that needs to be applied to the table.
     # type policy_tags: dict
     
     # """
     @apply_defaults
-    def __init__(
-            self, 
-            task_id: str, 
-            project_id: str, 
-            dataset_id: str, 
-            table_names: list, 
+    def __init__(self, task_id: str, project_id: str, dataset_id: str, table_names: list, 
             policy_tags: dict,
-            gcp_conn_id: str='gcp_default',
-            bigquery_conn_id: Optional[str] = None,
-            *args, **kwargs):
-        
-        if bigquery_conn_id:
-            gcp_conn_id = bigquery_conn_id
+            bigquery_conn_id: str, *args, **kwargs):
 
         super(ApplyTaxonomyOperator, self).__init__(
             task_id=task_id,
             python_callable=set_policy_tag,
             requirements=["google-cloud-bigquery==2.13.1"],
             system_site_packages=True,
             op_kwargs={
                 'project_id': project_id,
                 'dataset_id': dataset_id,
                 'table_names': table_names,
                 'policy_tags': policy_tags,
-                'gcp_conn_id': gcp_conn_id,
+                'bigquery_conn_id': bigquery_conn_id,
             },
             *args, **kwargs
         )
 
 class TaxonomyException(Exception):
     pass
```

### Comparing `awehflow-2.4.3.1/awehflow/sensors/http.py` & `awehflow-2.4.3.2/awehflow/sensors/http.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/awehflow/sensors/sql_sensor.py` & `awehflow-2.4.3.2/awehflow/sensors/sql_sensor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 from time import sleep
 from datetime import timedelta
-import re
-
-from airflow.version import version as airflow_version
 from airflow.utils import timezone
+
 from airflow.models.taskreschedule import TaskReschedule
 from airflow.exceptions import AirflowSensorTimeout, AirflowSkipException, AirflowRescheduleException
-
-if int(re.sub('[^0-9]', '', airflow_version)) < 240:
-    from airflow.sensors.sql import SqlSensor
-else:
-    from airflow.providers.common.sql.sensors.sql import SqlSensor
+from airflow.sensors.sql import SqlSensor
 
 class SqlSensor(SqlSensor):
     """
     Override of the default SqlSensor with modified 'execute' logic.  Sensor now fails quitely in soft_fail mode
     """
     def execute(self, context):
         started_at = timezone.utcnow()
```

### Comparing `awehflow-2.4.3.1/awehflow/utils.py` & `awehflow-2.4.3.2/awehflow/utils.py`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/awehflow.egg-info/SOURCES.txt` & `awehflow-2.4.3.2/awehflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awehflow-2.4.3.1/setup.py` & `awehflow-2.4.3.2/setup.py`

 * *Files identical despite different names*

