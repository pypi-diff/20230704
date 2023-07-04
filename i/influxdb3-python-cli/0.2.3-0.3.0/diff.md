# Comparing `tmp/influxdb3-python-cli-0.2.3.tar.gz` & `tmp/influxdb3-python-cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-cli-0.2.3.tar", last modified: Fri Jun 30 17:12:16 2023, max compression
+gzip compressed data, was "influxdb3-python-cli-0.3.0.tar", last modified: Tue Jul  4 15:23:42 2023, max compression
```

## Comparing `influxdb3-python-cli-0.2.3.tar` & `influxdb3-python-cli-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:12:16.831888 influxdb3-python-cli-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 17:12:06.000000 influxdb3-python-cli-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-30 17:12:16.831888 influxdb3-python-cli-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-30 17:12:06.000000 influxdb3-python-cli-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:12:16.831888 influxdb3-python-cli-0.2.3/influxdb3_python_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-30 17:12:16.000000 influxdb3-python-cli-0.2.3/influxdb3_python_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-30 17:12:16.000000 influxdb3-python-cli-0.2.3/influxdb3_python_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:12:16.000000 influxdb3-python-cli-0.2.3/influxdb3_python_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 17:12:16.000000 influxdb3-python-cli-0.2.3/influxdb3_python_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 17:12:16.000000 influxdb3-python-cli-0.2.3/influxdb3_python_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 17:12:16.000000 influxdb3-python-cli-0.2.3/influxdb3_python_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:12:16.831888 influxdb3-python-cli-0.2.3/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:12:06.000000 influxdb3-python-cli-0.2.3/influxdb_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-30 17:12:06.000000 influxdb3-python-cli-0.2.3/influxdb_cli/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9531 2023-06-30 17:12:06.000000 influxdb3-python-cli-0.2.3/influxdb_cli/influx3.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:12:16.831888 influxdb3-python-cli-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-30 17:12:06.000000 influxdb3-python-cli-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:23:42.668692 influxdb3-python-cli-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-04 15:23:42.668692 influxdb3-python-cli-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:23:42.668692 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 15:23:42.000000 influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:23:42.668692 influxdb3-python-cli-0.3.0/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/influxdb_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/influxdb_cli/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11720 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/influxdb_cli/influx3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/influxdb_cli/openai_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:23:42.672693 influxdb3-python-cli-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-04 15:23:31.000000 influxdb3-python-cli-0.3.0/setup.py
```

### Comparing `influxdb3-python-cli-0.2.3/LICENSE` & `influxdb3-python-cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.2.3/PKG-INFO` & `influxdb3-python-cli-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.2.3
+Version: 0.3.0
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -70,15 +70,15 @@
     --name="my-config" \
     --database="<database or bucket name>" \
     --host="us-east-1-1.aws.cloud2.influxdata.com" \
     --token="<your token>" \
     --org="<your org ID>"
     ```
     
-  The output is the configuration in a `config.json` file. This is saved within a directory called `config` located with the influx3 application.
+  The output is the configuration in a `config.json` file. This is saved within a directory called `config` located within your `Documents` folder.
 
 
 If you're running the CLI against InfluxDB Cloud Serverless, replace `your-database` in the examples with your Cloud Serverless _bucket name_.
 
 ## Run as a command
 
 ```
@@ -214,15 +214,31 @@
 
 ```bash
 influx3.py config list
 ```
 
 Please replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `"<your token>"`, `"<database or bucket name>"`, and `"<your org ID>"` with your actual values.
 
+## (Beta) OpenAI (ChatGPT) Support
+The CLI also contians a beta feature that allows you to query your data using OpenAI's ChatGPT. To use this feature, you must have an OpenAI API key. You can get one by signing up for the [OpenAI waitlist](https://share.hsforms.com/1Lfc7WtPLRk2ppXhPjcYY-A4sk30). Once you have an API key, you can set it as an environment variable called `OPENAI_API_KEY`.
 
+To use this feature, you can use the `chatgpt` command:
+```
+export OPENAI_API_KEY=sk-o2Sbq3aVBp
+
+influx3 chatgpt get average vibration grouped by machineID from machine_data
+Run InfluxQL query: SELECT MEAN(vibration) AS avg_vibration FROM machine_data GROUP BY machineID
+|    | iox::measurement   | time                | machineID   |   avg_vibration |
+|---:|:-------------------|:--------------------|:------------|----------------:|
+|  0 | machine_data       | 1970-01-01 00:00:00 | machine1    |         85.2356 |
+|  1 | machine_data       | 1970-01-01 00:00:00 | machine2    |        190.273  |
+|  2 | machine_data       | 1970-01-01 00:00:00 | machine3    |         85.4789 |
+Press TAB to fetch next chunk of data
+
+```
 
 
 ## Client library
 
 The underlying client library is also available for use in your own code: https://github.com/InfluxCommunity/influxdb3-python
 
 ## Contribution
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.3 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.3.0 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -26,15 +26,15 @@
 (without administrative rights), pass the `--user` flag in the `pip` command. -
 To install the client in your system-wide path, use `sudo` with admin
 privileges. ## Add a config To configure the CLI, do _one_ of the following: -
 Use the `influx3 create config` command to create or modify config--for
 example: ```bash influx3 create config \ --name="my-config" \ --database="" \ -
 -host="us-east-1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The
 output is the configuration in a `config.json` file. This is saved within a
-directory called `config` located with the influx3 application. If you're
+directory called `config` located within your `Documents` folder. If you're
 running the CLI against InfluxDB Cloud Serverless, replace `your-database` in
 the examples with your Cloud Serverless _bucket name_. ## Run as a command ```
 influx3 sql "select * from anomalies" ``` ``` influx3 write testmes f=7 ``` ##
 Query and write interactively In your terminal, enter the following command:
 ``` influx3 ``` `influx3` displays the `(>)` interactive prompt and waits for
 input. ``` Welcome to my IOx CLI. (>) ``` To query, type `sql` at the prompt.
 ``` (>) sql ``` At the `(sql >)` prompt, enter your query statement: ``` (sql
@@ -74,12 +74,25 @@
 parameter is required to specify which configuration to use. Example usage:
 ```bash influx3.py config use --name="my-config" ``` ### Delete The `delete`
 subcommand deletes a configuration. The `--name` parameter is required to
 specify which configuration to delete. Example usage: ```bash influx3.py config
 delete --name="my-config" ``` ### List The `list` subcommand lists all the
 configurations. Example usage: ```bash influx3.py config list ``` Please
 replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`, `""`,
-and `""` with your actual values. ## Client library The underlying client
-library is also available for use in your own code: https://github.com/
-InfluxCommunity/influxdb3-python ## Contribution When developing a new feature
-for the CLI or the client library, make sure to test your feature in both for
-breaking changes. #
+and `""` with your actual values. ## (Beta) OpenAI (ChatGPT) Support The CLI
+also contians a beta feature that allows you to query your data using OpenAI's
+ChatGPT. To use this feature, you must have an OpenAI API key. You can get one
+by signing up for the [OpenAI waitlist](https://share.hsforms.com/
+1Lfc7WtPLRk2ppXhPjcYY-A4sk30). Once you have an API key, you can set it as an
+environment variable called `OPENAI_API_KEY`. To use this feature, you can use
+the `chatgpt` command: ``` export OPENAI_API_KEY=sk-o2Sbq3aVBp influx3 chatgpt
+get average vibration grouped by machineID from machine_data Run InfluxQL
+query: SELECT MEAN(vibration) AS avg_vibration FROM machine_data GROUP BY
+machineID | | iox::measurement | time | machineID | avg_vibration | |---:|:----
+---------------|:--------------------|:------------|----------------:| | 0 |
+machine_data | 1970-01-01 00:00:00 | machine1 | 85.2356 | | 1 | machine_data |
+1970-01-01 00:00:00 | machine2 | 190.273 | | 2 | machine_data | 1970-01-01 00:
+00:00 | machine3 | 85.4789 | Press TAB to fetch next chunk of data ``` ##
+Client library The underlying client library is also available for use in your
+own code: https://github.com/InfluxCommunity/influxdb3-python ## Contribution
+When developing a new feature for the CLI or the client library, make sure to
+test your feature in both for breaking changes. #
```

### Comparing `influxdb3-python-cli-0.2.3/README.md` & `influxdb3-python-cli-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     --name="my-config" \
     --database="<database or bucket name>" \
     --host="us-east-1-1.aws.cloud2.influxdata.com" \
     --token="<your token>" \
     --org="<your org ID>"
     ```
     
-  The output is the configuration in a `config.json` file. This is saved within a directory called `config` located with the influx3 application.
+  The output is the configuration in a `config.json` file. This is saved within a directory called `config` located within your `Documents` folder.
 
 
 If you're running the CLI against InfluxDB Cloud Serverless, replace `your-database` in the examples with your Cloud Serverless _bucket name_.
 
 ## Run as a command
 
 ```
@@ -195,15 +195,31 @@
 
 ```bash
 influx3.py config list
 ```
 
 Please replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `"<your token>"`, `"<database or bucket name>"`, and `"<your org ID>"` with your actual values.
 
+## (Beta) OpenAI (ChatGPT) Support
+The CLI also contians a beta feature that allows you to query your data using OpenAI's ChatGPT. To use this feature, you must have an OpenAI API key. You can get one by signing up for the [OpenAI waitlist](https://share.hsforms.com/1Lfc7WtPLRk2ppXhPjcYY-A4sk30). Once you have an API key, you can set it as an environment variable called `OPENAI_API_KEY`.
 
+To use this feature, you can use the `chatgpt` command:
+```
+export OPENAI_API_KEY=sk-o2Sbq3aVBp
+
+influx3 chatgpt get average vibration grouped by machineID from machine_data
+Run InfluxQL query: SELECT MEAN(vibration) AS avg_vibration FROM machine_data GROUP BY machineID
+|    | iox::measurement   | time                | machineID   |   avg_vibration |
+|---:|:-------------------|:--------------------|:------------|----------------:|
+|  0 | machine_data       | 1970-01-01 00:00:00 | machine1    |         85.2356 |
+|  1 | machine_data       | 1970-01-01 00:00:00 | machine2    |        190.273  |
+|  2 | machine_data       | 1970-01-01 00:00:00 | machine3    |         85.4789 |
+Press TAB to fetch next chunk of data
+
+```
 
 
 ## Client library
 
 The underlying client library is also available for use in your own code: https://github.com/InfluxCommunity/influxdb3-python
 
 ## Contribution
```

#### html2text {}

```diff
@@ -16,15 +16,15 @@
 (without administrative rights), pass the `--user` flag in the `pip` command. -
 To install the client in your system-wide path, use `sudo` with admin
 privileges. ## Add a config To configure the CLI, do _one_ of the following: -
 Use the `influx3 create config` command to create or modify config--for
 example: ```bash influx3 create config \ --name="my-config" \ --database="" \ -
 -host="us-east-1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The
 output is the configuration in a `config.json` file. This is saved within a
-directory called `config` located with the influx3 application. If you're
+directory called `config` located within your `Documents` folder. If you're
 running the CLI against InfluxDB Cloud Serverless, replace `your-database` in
 the examples with your Cloud Serverless _bucket name_. ## Run as a command ```
 influx3 sql "select * from anomalies" ``` ``` influx3 write testmes f=7 ``` ##
 Query and write interactively In your terminal, enter the following command:
 ``` influx3 ``` `influx3` displays the `(>)` interactive prompt and waits for
 input. ``` Welcome to my IOx CLI. (>) ``` To query, type `sql` at the prompt.
 ``` (>) sql ``` At the `(sql >)` prompt, enter your query statement: ``` (sql
@@ -64,12 +64,25 @@
 parameter is required to specify which configuration to use. Example usage:
 ```bash influx3.py config use --name="my-config" ``` ### Delete The `delete`
 subcommand deletes a configuration. The `--name` parameter is required to
 specify which configuration to delete. Example usage: ```bash influx3.py config
 delete --name="my-config" ``` ### List The `list` subcommand lists all the
 configurations. Example usage: ```bash influx3.py config list ``` Please
 replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`, `""`,
-and `""` with your actual values. ## Client library The underlying client
-library is also available for use in your own code: https://github.com/
-InfluxCommunity/influxdb3-python ## Contribution When developing a new feature
-for the CLI or the client library, make sure to test your feature in both for
-breaking changes. #
+and `""` with your actual values. ## (Beta) OpenAI (ChatGPT) Support The CLI
+also contians a beta feature that allows you to query your data using OpenAI's
+ChatGPT. To use this feature, you must have an OpenAI API key. You can get one
+by signing up for the [OpenAI waitlist](https://share.hsforms.com/
+1Lfc7WtPLRk2ppXhPjcYY-A4sk30). Once you have an API key, you can set it as an
+environment variable called `OPENAI_API_KEY`. To use this feature, you can use
+the `chatgpt` command: ``` export OPENAI_API_KEY=sk-o2Sbq3aVBp influx3 chatgpt
+get average vibration grouped by machineID from machine_data Run InfluxQL
+query: SELECT MEAN(vibration) AS avg_vibration FROM machine_data GROUP BY
+machineID | | iox::measurement | time | machineID | avg_vibration | |---:|:----
+---------------|:--------------------|:------------|----------------:| | 0 |
+machine_data | 1970-01-01 00:00:00 | machine1 | 85.2356 | | 1 | machine_data |
+1970-01-01 00:00:00 | machine2 | 190.273 | | 2 | machine_data | 1970-01-01 00:
+00:00 | machine3 | 85.4789 | Press TAB to fetch next chunk of data ``` ##
+Client library The underlying client library is also available for use in your
+own code: https://github.com/InfluxCommunity/influxdb3-python ## Contribution
+When developing a new feature for the CLI or the client library, make sure to
+test your feature in both for breaking changes. #
```

### Comparing `influxdb3-python-cli-0.2.3/influxdb3_python_cli.egg-info/PKG-INFO` & `influxdb3-python-cli-0.3.0/influxdb3_python_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.2.3
+Version: 0.3.0
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -70,15 +70,15 @@
     --name="my-config" \
     --database="<database or bucket name>" \
     --host="us-east-1-1.aws.cloud2.influxdata.com" \
     --token="<your token>" \
     --org="<your org ID>"
     ```
     
-  The output is the configuration in a `config.json` file. This is saved within a directory called `config` located with the influx3 application.
+  The output is the configuration in a `config.json` file. This is saved within a directory called `config` located within your `Documents` folder.
 
 
 If you're running the CLI against InfluxDB Cloud Serverless, replace `your-database` in the examples with your Cloud Serverless _bucket name_.
 
 ## Run as a command
 
 ```
@@ -214,15 +214,31 @@
 
 ```bash
 influx3.py config list
 ```
 
 Please replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `"<your token>"`, `"<database or bucket name>"`, and `"<your org ID>"` with your actual values.
 
+## (Beta) OpenAI (ChatGPT) Support
+The CLI also contians a beta feature that allows you to query your data using OpenAI's ChatGPT. To use this feature, you must have an OpenAI API key. You can get one by signing up for the [OpenAI waitlist](https://share.hsforms.com/1Lfc7WtPLRk2ppXhPjcYY-A4sk30). Once you have an API key, you can set it as an environment variable called `OPENAI_API_KEY`.
 
+To use this feature, you can use the `chatgpt` command:
+```
+export OPENAI_API_KEY=sk-o2Sbq3aVBp
+
+influx3 chatgpt get average vibration grouped by machineID from machine_data
+Run InfluxQL query: SELECT MEAN(vibration) AS avg_vibration FROM machine_data GROUP BY machineID
+|    | iox::measurement   | time                | machineID   |   avg_vibration |
+|---:|:-------------------|:--------------------|:------------|----------------:|
+|  0 | machine_data       | 1970-01-01 00:00:00 | machine1    |         85.2356 |
+|  1 | machine_data       | 1970-01-01 00:00:00 | machine2    |        190.273  |
+|  2 | machine_data       | 1970-01-01 00:00:00 | machine3    |         85.4789 |
+Press TAB to fetch next chunk of data
+
+```
 
 
 ## Client library
 
 The underlying client library is also available for use in your own code: https://github.com/InfluxCommunity/influxdb3-python
 
 ## Contribution
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.3 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.3.0 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -26,15 +26,15 @@
 (without administrative rights), pass the `--user` flag in the `pip` command. -
 To install the client in your system-wide path, use `sudo` with admin
 privileges. ## Add a config To configure the CLI, do _one_ of the following: -
 Use the `influx3 create config` command to create or modify config--for
 example: ```bash influx3 create config \ --name="my-config" \ --database="" \ -
 -host="us-east-1-1.aws.cloud2.influxdata.com" \ --token="" \ --org="" ``` The
 output is the configuration in a `config.json` file. This is saved within a
-directory called `config` located with the influx3 application. If you're
+directory called `config` located within your `Documents` folder. If you're
 running the CLI against InfluxDB Cloud Serverless, replace `your-database` in
 the examples with your Cloud Serverless _bucket name_. ## Run as a command ```
 influx3 sql "select * from anomalies" ``` ``` influx3 write testmes f=7 ``` ##
 Query and write interactively In your terminal, enter the following command:
 ``` influx3 ``` `influx3` displays the `(>)` interactive prompt and waits for
 input. ``` Welcome to my IOx CLI. (>) ``` To query, type `sql` at the prompt.
 ``` (>) sql ``` At the `(sql >)` prompt, enter your query statement: ``` (sql
@@ -74,12 +74,25 @@
 parameter is required to specify which configuration to use. Example usage:
 ```bash influx3.py config use --name="my-config" ``` ### Delete The `delete`
 subcommand deletes a configuration. The `--name` parameter is required to
 specify which configuration to delete. Example usage: ```bash influx3.py config
 delete --name="my-config" ``` ### List The `list` subcommand lists all the
 configurations. Example usage: ```bash influx3.py config list ``` Please
 replace `"my-config"`, `"us-east-1-1.aws.cloud2.influxdata.com"`, `""`, `""`,
-and `""` with your actual values. ## Client library The underlying client
-library is also available for use in your own code: https://github.com/
-InfluxCommunity/influxdb3-python ## Contribution When developing a new feature
-for the CLI or the client library, make sure to test your feature in both for
-breaking changes. #
+and `""` with your actual values. ## (Beta) OpenAI (ChatGPT) Support The CLI
+also contians a beta feature that allows you to query your data using OpenAI's
+ChatGPT. To use this feature, you must have an OpenAI API key. You can get one
+by signing up for the [OpenAI waitlist](https://share.hsforms.com/
+1Lfc7WtPLRk2ppXhPjcYY-A4sk30). Once you have an API key, you can set it as an
+environment variable called `OPENAI_API_KEY`. To use this feature, you can use
+the `chatgpt` command: ``` export OPENAI_API_KEY=sk-o2Sbq3aVBp influx3 chatgpt
+get average vibration grouped by machineID from machine_data Run InfluxQL
+query: SELECT MEAN(vibration) AS avg_vibration FROM machine_data GROUP BY
+machineID | | iox::measurement | time | machineID | avg_vibration | |---:|:----
+---------------|:--------------------|:------------|----------------:| | 0 |
+machine_data | 1970-01-01 00:00:00 | machine1 | 85.2356 | | 1 | machine_data |
+1970-01-01 00:00:00 | machine2 | 190.273 | | 2 | machine_data | 1970-01-01 00:
+00:00 | machine3 | 85.4789 | Press TAB to fetch next chunk of data ``` ##
+Client library The underlying client library is also available for use in your
+own code: https://github.com/InfluxCommunity/influxdb3-python ## Contribution
+When developing a new feature for the CLI or the client library, make sure to
+test your feature in both for breaking changes. #
```

### Comparing `influxdb3-python-cli-0.2.3/influxdb_cli/helper.py` & `influxdb3-python-cli-0.3.0/influxdb_cli/helper.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.2.3/influxdb_cli/influx3.py` & `influxdb3-python-cli-0.3.0/influxdb_cli/influx3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python3
 
 import cmd
 import argparse
 from prompt_toolkit import PromptSession
+from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.lexers import PygmentsLexer
 from pygments.lexers import SqlLexer
 from influxdb_client_3 import InfluxDBClient3
 from .helper import config_helper
+from .openai_helper import OpenAIHelper
 
 _usage_string = """
 to write data use influxdb line protocol:
 > influx3 write testmes,tag1=tagvalue field1=0.0 <optional timestamp>
 
 to read data with sql:
 > influx3 sql select * from testmes where time > now() - interval'1 minute'
@@ -18,45 +20,86 @@
 to enter interactive mode:
 > influx3
 """
 
 _description_string = 'CLI application for Querying IOx with arguments and interactive mode.'
 
 class IOXCLI(cmd.Cmd):
-    intro = 'Welcome to my IOx CLI.\n'
+    intro = 'InfluxDB 3.0 CLI.\n'
     prompt = '(>) '
 
     def __init__(self):
-        super().__init__()
+        super(IOXCLI, self).__init__()
         self.config_helper = config_helper()
         self.active_config = self.config_helper._get_active()
         self._setup_client()
         self._sql_prompt_session = PromptSession(lexer=PygmentsLexer(SqlLexer))
         self._write_prompt_session = PromptSession(lexer=None)
        
 
-    def do_sql(self, arg):
+    
+
+    def do_query(self, arg, language):
         if self.active_config == {}:
             print("can't query, no active configs")
             return
-        try: 
-            table = self.influxdb_client.query(query=arg, language="sql")
-            print(table.to_pandas().to_markdown())
-        except Exception as e:
-            print(e)
+        
+        # Retrieve the iterator
+        reader = self._query_chunks(arg, language)
 
-    def do_influxql(self, arg):
-        if self.active_config == {}:
-            print("can't query, no active configs")
+        if reader is None:
             return
-        try: 
-            table = self.influxdb_client.query(query=arg, language="influxql")
-            print(table.to_pandas().to_markdown())
+
+        # Create custom key bindings
+        bindings = KeyBindings()
+
+        # Flag to determine if there is more data
+        has_more_data = True
+
+        # Bind the 'tab' key
+        @bindings.add('tab')
+        def _(event):
+            nonlocal has_more_data
+            if has_more_data:
+                try:
+                    batch, buff = reader.read_chunk()
+                    print(batch.to_pandas().to_markdown())
+                except StopIteration:
+                    print("End of data. Press Enter to continue.")
+                    has_more_data = False
+                except Exception as e:
+                    print(e)
+                    has_more_data = False
+
+        # Create a session with the bindings
+        session = PromptSession(key_bindings=bindings)
+        try:
+            batch, buff = reader.read_chunk()
+            print(batch.to_pandas().to_markdown())
+        except StopIteration:
+            print("End of data. Press Enter to continue.")
+            has_more_data = False
+  
+        while True:
+            try:
+                if not has_more_data:
+                    break
+                # Prompt loop to capture key presses
+                print("Press TAB to fetch next chunk of data")
+                session.prompt()
+            except KeyboardInterrupt:
+                break
+    
+    def _query_chunks(self, arg, language):
+        try:
+            table = self.influxdb_client.query(query=arg, language=language, mode="chunk")
+            return table
         except Exception as e:
             print(e)
+            return None
 
     def do_write(self, arg):
         if self.active_config == {}:
             print("can't write, no active configs")
             return
         if arg == "":
             print("can't write, no line protocol supplied")
@@ -91,25 +134,38 @@
         print('\nExiting ...')
         return True
 
     def do_EOF(self, arg):
         'Exit the shell with Ctrl-D'
         return self.do_exit(arg)
 
+    def do_chatgpt(self, arg):
+        if arg == "":
+            print("can't write, no line protocol supplied")
+            return
+        openai_helper = OpenAIHelper()
+        query = openai_helper.nl_to_sql(arg)
+        print(f"Run InfluxQL query: {query}")
+        self.do_query(query, language='influxql')
+        
+
  
     def precmd(self, line):
         if line.strip() == 'sql':
-            self._run_prompt_loop('(sql >) ', self.do_sql, 'SQL mode')
+            self._run_prompt_loop('(sql >) ', lambda arg: self.do_query(arg, language='sql'), 'SQL mode')
             return ''
         if line.strip() == 'influxql':
-            self._run_prompt_loop('(influxql >) ', self.do_influxql, 'INFLUXQL mode')
+            self._run_prompt_loop('(influxql >) ', lambda arg: self.do_query(arg, language='influxql'), 'INFLUXQL mode')
             return ''
         if line.strip() == 'write':
             self._run_prompt_loop('(write >) ', self.do_write, 'write mode')
             return ''
+        if line.strip() == 'chatgpt':
+            self._run_prompt_loop('(chatgpt >) ', self.do_chatgpt, 'chatgpt mode')
+            return ''
         return line
 
     def _run_prompt_loop(self, prompt, action, mode_name):
         prompt_session = self._sql_prompt_session if mode_name == 'SQL mode' else self._write_prompt_session
         while True:
             try:
                 statement = prompt_session.prompt(prompt)
@@ -167,14 +223,17 @@
     subparsers = parser.add_subparsers(dest='command')
 
     sql_parser = subparsers.add_parser('sql', help='execute the given SQL query')
     sql_parser.add_argument('query', metavar='QUERY', nargs='*', action=StoreRemainingInput, help='the SQL query to execute')
     influxql_parser = subparsers.add_parser('influxql', help='execute the given InfluxQL query')
     influxql_parser.add_argument('query', metavar='QUERY', nargs='*', action=StoreRemainingInput, help='the INFLUXQL query to execute')
 
+    chatgpt_parser = subparsers.add_parser('chatgpt', help='execute the given chatgpt statement')
+    chatgpt_parser.add_argument('query', metavar='QUERY', nargs='*', action=StoreRemainingInput, help='the chatgpt query to execute')
+
     write_parser = subparsers.add_parser('write', help='write line protocol to InfluxDB')
     write_parser.add_argument('line_protocol', metavar='LINE PROTOCOL',  nargs='*', action=StoreRemainingInput, help='the data to write')
 
     write_csv_parser = subparsers.add_parser('write_csv', help='write CSV data to InfluxDB')
     write_csv_parser.add_argument('--file', help='the CSV file to import', required=True)
     write_csv_parser.add_argument('--measurement', help='Define the name of the measurement', required=True)
     write_csv_parser.add_argument('--time', help='Define the name of the time column with the csv file', required=True)
@@ -215,17 +274,19 @@
 
 def main():
     args = parse_args()
     app = IOXCLI()
 
 
     if args.command == 'sql':
-        app.do_sql(args.query)
+        app.do_query(args.query, language='sql')
     if args.command == 'influxql':
-        app.do_influxql(args.query)
+        app.do_query(args.query, language='influxql')
+    if args.command == 'chatgpt':
+        app.do_chatgpt(args.query)
     if args.command == 'write':
         app.do_write(args.line_protocol)
     if args.command == 'write_csv':
         app.do_write_csv(args)
     if args.command == 'config':
         if args.config_command == 'create':
             app.create_config(args)
```

### Comparing `influxdb3-python-cli-0.2.3/setup.py` & `influxdb3-python-cli-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     description='Community Python client for InfluxDB 3.0 (CLI)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='InfluxData',
     author_email='contact@influxdata.com',
     url='https://github.com/InfluxCommunity/influxdb-python-cli',
     packages=find_packages(),  # Automatically find packages in the current directory
-    install_requires=['influxdb3-python', 'pygments', 'prompt_toolkit', 'pandas', 'tabulate'],
+    install_requires=['influxdb3-python', 'pygments', 'prompt_toolkit', 'pandas', 'tabulate', 'openai'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

