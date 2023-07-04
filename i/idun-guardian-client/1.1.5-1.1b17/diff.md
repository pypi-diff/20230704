# Comparing `tmp/idun_guardian_client-1.1.5.tar.gz` & `tmp/idun_guardian_client-1.1b17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_guardian_client-1.1.5.tar", max compression
+gzip compressed data, was "idun_guardian_client-1.1b17.tar", last modified: Fri May 26 09:10:06 2023, max compression
```

## Comparing `idun_guardian_client-1.1.5.tar` & `idun_guardian_client-1.1b17.tar`

### file list

```diff
@@ -1,14 +1,28 @@
--rw-r--r--   0        0        0      857 2023-07-04 10:20:09.985747 idun_guardian_client-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     8680 2023-06-02 08:49:58.338164 idun_guardian_client-1.1.5/README.md
--rw-r--r--   0        0        0     3381 2023-06-02 08:49:58.369414 idun_guardian_client-1.1.5/src/idun_guardian_client/.gitignore
--rw-r--r--   0        0        0      351 2023-06-02 08:49:58.369414 idun_guardian_client-1.1.5/src/idun_guardian_client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 08:49:58.369414 idun_guardian_client-1.1.5/src/idun_guardian_client/__main__.py
--rw-r--r--   0        0        0    10327 2023-07-04 10:20:09.986751 idun_guardian_client-1.1.5/src/idun_guardian_client/client.py
--rw-r--r--   0        0        0     1631 2023-07-04 08:32:44.211268 idun_guardian_client-1.1.5/src/idun_guardian_client/config.py
--rw-r--r--   0        0        0    15292 2023-07-04 10:20:09.987746 idun_guardian_client-1.1.5/src/idun_guardian_client/debug_logs.py
--rw-r--r--   0        0        0    25872 2023-07-04 10:20:09.988747 idun_guardian_client-1.1.5/src/idun_guardian_client/igeb_api.py
--rw-r--r--   0        0        0    34960 2023-07-04 10:20:09.988747 idun_guardian_client-1.1.5/src/idun_guardian_client/igeb_bluetooth.py
--rw-r--r--   0        0        0     7605 2023-07-04 10:20:09.989746 idun_guardian_client-1.1.5/src/idun_guardian_client/igeb_utils.py
--rw-r--r--   0        0        0      200 2023-06-02 08:49:58.369414 idun_guardian_client-1.1.5/src/idun_guardian_client/mock_utils.py
--rw-r--r--   0        0        0     1263 2023-06-02 08:49:58.369414 idun_guardian_client-1.1.5/src/idun_guardian_client/test_producer_consumer.py
--rw-r--r--   0        0        0     9175 1970-01-01 00:00:00.000000 idun_guardian_client-1.1.5/PKG-INFO
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 09:10:06.585058 idun_guardian_client-1.1b17/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8992 2023-05-26 09:10:06.584856 idun_guardian_client-1.1b17/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)     8426 2023-04-11 13:19:07.000000 idun_guardian_client-1.1b17/README.md
+-rw-r--r--   0 waddaben   (501) staff       (20)      870 2023-05-26 09:09:21.000000 idun_guardian_client-1.1b17/pyproject.toml
+-rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-05-26 09:10:06.585110 idun_guardian_client-1.1b17/setup.cfg
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 09:10:06.578138 idun_guardian_client-1.1b17/src/
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 09:10:06.582225 idun_guardian_client-1.1b17/src/idun_guardian_client/
+-rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/__init__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/__main__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     9408 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/client.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1591 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/config.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    12613 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/debug_logs.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    20719 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/igeb_api.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    34157 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/igeb_bluetooth.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-14 11:38:29.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/igeb_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/mock_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/setup.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/test_producer_consumer.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 09:10:06.583798 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8992 2023-05-26 09:10:06.000000 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-05-26 09:10:06.000000 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/SOURCES.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-05-26 09:10:06.000000 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/dependency_links.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-05-26 09:10:06.000000 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/requires.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-05-26 09:10:06.000000 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/top_level.txt
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 09:10:06.584559 idun_guardian_client-1.1b17/tests/
+-rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/tests/test_ble.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1677 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/tests/test_ble_record.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/tests/test_utils.py
```

### Comparing `idun_guardian_client-1.1.5/README.md` & `idun_guardian_client-1.1b17/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,254 +1,254 @@
-# User guide and documentation
-
-## What can you do with the Python SDK?
-
-1. You can use the Python SDK to search for the device.
-2. You can use the Python SDK to connect and record data from the earbud.
-3. You can download the data to your local machine.
-
----
-
-## Prerequisites
-
-- [Python 3.10](https://www.python.org/downloads/release/python-3100), if you already have another python version installed and you do not want to create a virtual environment to run the SDK, then you have to install Python 3.10 and [set it as your default Python](https://www.youtube.com/watch?v=zriWqGNJg4k).
-    - If you have conflicts with other packages when installing the Python SDK:
-        -  Use [Conda](https://www.anaconda.com/products/distribution) which will create an environment and configure your python version to the correct one with the following command: 
-        
-        ```bash
-        conda create -n idun_env python=3.10
-        ```
-        or
-        - Use [Pipenv](https://pypi.org/project/pipenv/) which will create your virtual environment manually using the following command.
-        ```bash
-        pipenv install --python 3.10
-        ```
----
-
-## Quick installation guide
-
-1. Create a new repository or folder
-2. Open the terminal in the same folder location or direct to that location within an already open terminal. For Windows you can use command prompt or Anaconda prompt, and Mac OS you can use the terminal or Anaconda prompt.
-
-3. First activate the virtual environment if you have created one by using the following command, this command must always be run before using the python SDK:
-    ```bash
-    conda activate idun_env
-    ```
-    or
-    ```bash
-    pipenv shell
-    ```
-
-4. After the environment is activated, install the Python SDK using the following command:
-    - With a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) use the following command:
-    ```bash
-    pip install idun-guardian-client
-    ```
-    or
-    - With a [pipenv environment](https://pypi.org/project/pipenv/) use the following command:
-    ```bash
-    pipenv install idun-guardian-client
-    ```
-
-5. After installing the package, make sure that the dependencies are correctly installed by running the following command and inspecting the packages installed in the terminal output:
-
-    ```bash
-    pip list
-    ```
-
----
-
-## How to use the Python SDK
-
-You can also download all the SDK example files from our [GitHub repository](https://github.com/iduntech/idun-guardian-client-examples.git), or copy and paste it from the examples below.
-
-### Example 1: Search for the device
-
-1. Create a new file inside the folder where you created your environment and name it `search.py`
-2. Open the terminal in the folder and activate your virtual environment using the steps from the [Quick installation guide](#quick-installation-guide).
-3. Open the `search.py` file and copy the code from step 1 below.
-4. Activate the virtual environment **only** if you have not already done so by using:
-
-    ```bash
-    conda activate idun_env
-    ```
-    or
-    ```bash
-    pipenv shell
-    ```
-4. Run the following command in the terminal to run the code after you have activate the enviroment:
-    ```bash
-    python search.py
-    ```
-
-#### Recommendation of steps to follow which is elaborated further below
-
-1. Search for the device
-2. Check the battery level
-3. Check the impedance
-4. Record data from the earbud
-5. Download the data from the cloud using the recording ID
-
-### **1. Search the earbud manually**
-
-- To search for the earbud, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-bci = GuardianClient()
-
-device_address = asyncio.run(bci.search_device())
-```
-
-- Follow the steps in the terminal to search for the earbud with the name `IGEB`
-- If there are more than one IGEB device in the area, you will be asked to select the device you want to connect to connect to, a list such as below will pop up in the terminal:
-
-    - For Windows:
-    ```bash
-    ----- Available devices -----
-
-    Index | Name | Address
-    ----------------------------
-    0     | IGEB | XX:XX:XX:XX:XX:XX
-    1     | IGEB | XX:XX:XX:XX:XX:XX
-    2     | IGEB | XX:XX:XX:XX:XX:XX
-    ----------------------------
-    ```
-    - For Mac OS:
-    ```bash
-    ----- Available devices -----
-    Index | Name | UUID
-    ----------------------------
-    0    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    1    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    2    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    ----------------------------
-    ```
-
-- Enter the index number of the device you want to connect to.
-
-
-### **2. Check battery level**
-
-- To read out the battery level, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-asyncio.run(bci.start_battery())
-```
-
-### **3. Check impedance values**
-
-- To read out the impedance values, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-IMPEDANCE_DURATION = 5  # duration of impedance measurement in seconds
-MAINS_FREQUENCY_60Hz = False
-# mains frequency in Hz (50 or 60), for Europe 50Hz, for US 60Hz
-
-
-# Get device address
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-# start a recording session
-asyncio.run(
-    bci.start_recording(
-        recording_timer=IMPEDANCE_DURATION,
-        mains_freq_60hz=MAINS_FREQUENCY_60Hz,
-        impedance_measurement=True)
-)
-```
-
-### **4. Start a recording**
-
-- To start a recording with a pre-defined timer (e.g. `100` in seconds), you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-EXPERIMENT: str = "Sleeping"
-RECORDING_TIMER: int = 36000 # 10 hours in seconds
-LED_SLEEP: bool = False
-SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
-BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
-
-# start a recording session
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-# start a recording session
-asyncio.run(
-    bci.start_recording(
-        recording_timer=RECORDING_TIMER,
-        led_sleep=LED_SLEEP,
-        experiment=EXPERIMENT,
-        sending_timout=SENDING_TIMEOUT,
-        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
-    )
-)
-
-```
-
-- To stop the recording, either wait for the timer to run out or interrupt the recording
-    - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
-    - with Windows enter the cancellation command in the terminal running the script, this would be `Ctrl+C` or `Ctrl+Shift+C`
-
-### **4. Get all recorded info**
-
-- To download the data, you need to first get the list of all your recordings and choose the one you would like to download
-- Run the following command in your python shell or in your python script:
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# get a list of all recordings
-recording_list = api.get_recordings_info_all(device_id = "XX-XX-XX-XX-XX-XX") # Device ID is derived from the MAC address of the earbud and in the log file
-
-```
-
-### **5. Get recording info**
-
-- To list the information on a specific recording, you need to run the following command in your python shell or in your python script:
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# get single recording
-api.get_recording_info_by_id(
-    device_id = "XX-XX-XX-XX-XX-XX",
-    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
-)
-
-```
-
-### **5. Download recording**
-
-- To download the data insert the `device_id` along with the `recording_id` and run the following command in your python shell or in your python script
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# download recording
-api.download_recording_by_id(
-    device_id = "XX-XX-XX-XX-XX-XX",
-    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx"
-)
-# The info about th recording can be found in the log file
-```
+# User guide and documentation
+
+## What can you do with the Python SDK?
+
+1. You can use the Python SDK to search for the device.
+2. You can use the Python SDK to connect and record data from the earbud.
+3. You can download the data to your local machine.
+
+---
+
+## Prerequisites
+
+- [Python 3.10](https://www.python.org/downloads/release/python-3100), if you already have another python version installed and you do not want to create a virtual environment to run the SDK, then you have to install Python 3.10 and [set it as your default Python](https://www.youtube.com/watch?v=zriWqGNJg4k).
+    - If you have conflicts with other packages when installing the Python SDK:
+        -  Use [Conda](https://www.anaconda.com/products/distribution) which will create an environment and configure your python version to the correct one with the following command: 
+        
+        ```bash
+        conda create -n idun_env python=3.10
+        ```
+        or
+        - Use [Pipenv](https://pypi.org/project/pipenv/) which will create your virtual environment manually using the following command.
+        ```bash
+        pipenv install --python 3.10
+        ```
+---
+
+## Quick installation guide
+
+1. Create a new repository or folder
+2. Open the terminal in the same folder location or direct to that location within an already open terminal. For Windows you can use command prompt or Anaconda prompt, and Mac OS you can use the terminal or Anaconda prompt.
+
+3. First activate the virtual environment if you have created one by using the following command, this command must always be run before using the python SDK:
+    ```bash
+    conda activate idun_env
+    ```
+    or
+    ```bash
+    pipenv shell
+    ```
+
+4. After the environment is activated, install the Python SDK using the following command:
+    - With a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) use the following command:
+    ```bash
+    pip install idun-guardian-client
+    ```
+    or
+    - With a [pipenv environment](https://pypi.org/project/pipenv/) use the following command:
+    ```bash
+    pipenv install idun-guardian-client
+    ```
+
+5. After installing the package, make sure that the dependencies are correctly installed by running the following command and inspecting the packages installed in the terminal output:
+
+    ```bash
+    pip list
+    ```
+
+---
+
+## How to use the Python SDK
+
+You can also download all the SDK example files from our [GitHub repository](https://github.com/iduntech/idun-guardian-client-examples.git), or copy and paste it from the examples below.
+
+### Example 1: Search for the device
+
+1. Create a new file inside the folder where you created your environment and name it `search.py`
+2. Open the terminal in the folder and activate your virtual environment using the steps from the [Quick installation guide](#quick-installation-guide).
+3. Open the `search.py` file and copy the code from step 1 below.
+4. Activate the virtual environment **only** if you have not already done so by using:
+
+    ```bash
+    conda activate idun_env
+    ```
+    or
+    ```bash
+    pipenv shell
+    ```
+4. Run the following command in the terminal to run the code after you have activate the enviroment:
+    ```bash
+    python search.py
+    ```
+
+#### Recommendation of steps to follow which is elaborated further below
+
+1. Search for the device
+2. Check the battery level
+3. Check the impedance
+4. Record data from the earbud
+5. Download the data from the cloud using the recording ID
+
+### **1. Search the earbud manually**
+
+- To search for the earbud, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+bci = GuardianClient()
+
+device_address = asyncio.run(bci.search_device())
+```
+
+- Follow the steps in the terminal to search for the earbud with the name `IGEB`
+- If there are more than one IGEB device in the area, you will be asked to select the device you want to connect to connect to, a list such as below will pop up in the terminal:
+
+    - For Windows:
+    ```bash
+    ----- Available devices -----
+
+    Index | Name | Address
+    ----------------------------
+    0     | IGEB | XX:XX:XX:XX:XX:XX
+    1     | IGEB | XX:XX:XX:XX:XX:XX
+    2     | IGEB | XX:XX:XX:XX:XX:XX
+    ----------------------------
+    ```
+    - For Mac OS:
+    ```bash
+    ----- Available devices -----
+    Index | Name | UUID
+    ----------------------------
+    0    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    1    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    2    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    ----------------------------
+    ```
+
+- Enter the index number of the device you want to connect to.
+
+
+### **2. Check battery level**
+
+- To read out the battery level, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+asyncio.run(bci.start_battery())
+```
+
+### **3. Check impedance values**
+
+- To read out the impedance values, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+IMPEDANCE_DURATION = 5  # duration of impedance measurement in seconds
+MAINS_FREQUENCY_60Hz = False
+# mains frequency in Hz (50 or 60), for Europe 50Hz, for US 60Hz
+
+
+# Get device address
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+# start a recording session
+asyncio.run(
+    bci.start_recording(
+        recording_timer=IMPEDANCE_DURATION,
+        mains_freq_60hz=MAINS_FREQUENCY_60Hz,
+        impedance_measurement=True)
+)
+```
+
+### **4. Start a recording**
+
+- To start a recording with a pre-defined timer (e.g. `100` in seconds), you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+EXPERIMENT: str = "Sleeping"
+RECORDING_TIMER: int = 36000 # 10 hours in seconds
+LED_SLEEP: bool = False
+SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
+BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
+
+# start a recording session
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+# start a recording session
+asyncio.run(
+    bci.start_recording(
+        recording_timer=RECORDING_TIMER,
+        led_sleep=LED_SLEEP,
+        experiment=EXPERIMENT,
+        sending_timout=SENDING_TIMEOUT,
+        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
+    )
+)
+
+```
+
+- To stop the recording, either wait for the timer to run out or interrupt the recording
+    - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
+    - with Windows enter the cancellation command in the terminal running the script, this would be `Ctrl+C` or `Ctrl+Shift+C`
+
+### **4. Get all recorded info**
+
+- To download the data, you need to first get the list of all your recordings and choose the one you would like to download
+- Run the following command in your python shell or in your python script:
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# get a list of all recordings
+recording_list = api.get_recordings_info_all(device_id = "XX-XX-XX-XX-XX-XX") # Device ID is derived from the MAC address of the earbud and in the log file
+
+```
+
+### **5. Get recording info**
+
+- To list the information on a specific recording, you need to run the following command in your python shell or in your python script:
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# get single recording
+api.get_recording_info_by_id(
+    device_id = "XX-XX-XX-XX-XX-XX",
+    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
+)
+
+```
+
+### **5. Download recording**
+
+- To download the data insert the `device_id` along with the `recording_id` and run the following command in your python shell or in your python script
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# download recording
+api.download_recording_by_id(
+    device_id = "XX-XX-XX-XX-XX-XX",
+    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx"
+)
+# The info about th recording can be found in the log file
+```
```

### Comparing `idun_guardian_client-1.1.5/src/idun_guardian_client/client.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,253 +1,239 @@
-"""
-Initialization of the IDUN Guardian Client
-"""
-import os
-import asyncio
-from typing import Union
-import logging
-from datetime import datetime
-from .igeb_bluetooth import GuardianBLE
-from .igeb_api import GuardianAPI
-from .igeb_utils import check_platform, check_valid_mac, check_valid_uuid
-import uuid
-import gc
-from typing import Union
-from bleak import exc
-from idun_data_models.rest_data_model import RecordingIn, DataStreams, RecordingConfig
-
-
-class GuardianClient:
-    """
-    Class object for the communication between Guardian Earbuds and Cloud API
-    """
-
-    def __init__(
-        self,
-        address: Union[str, None] = None,
-        debug=True,
-        debug_console=True,
-    ) -> None:
-        """Initialize the Guardian Client
-
-        Args:
-            address (str, optional): The MAC address of the Guardian Earbuds. Defaults to "00000000-0000-0000-0000-000000000000".
-            debug (bool, optional): Enable debug logging. Defaults to True.
-            debug_console (bool, optional): Enable debug logging to console. Defaults to True.
-
-        Raises:
-            ValueError: If the MAC address is not valid
-        """
-        self.is_connected = False
-        self.debug = debug
-        self.debug_to_console = debug_console
-        self.connection_status = 0
-        if self.debug:
-            self.configure_logger()
-
-        if address is not None:
-            if self.check_ble_address(address):
-                self.guardian_ble = GuardianBLE(address, debug=self.debug)
-                self.address = address
-        else:
-            logging.info("No BLE address provided, will search for device...")
-            print("No BLE address provided, will search for device..")
-            self.guardian_ble = GuardianBLE(debug=self.debug)
-
-        self.guardian_api = GuardianAPI(debug=self.debug)
-
-    def configure_logger(self):
-        """Configure the logger for the Guardian Client"""
-        if not os.path.exists("./logs"):
-            os.makedirs("logs")
-
-        datestr = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
-        log_filename = f"./logs/ble_info-{datestr}.log"
-
-        if not os.path.exists(os.path.dirname(log_filename)):
-            os.makedirs(os.path.dirname(log_filename))
-        log_handlers = [logging.FileHandler(log_filename)]
-
-        if self.debug_to_console:
-            log_handlers.append(logging.StreamHandler())
-
-        logging.basicConfig(
-            level=logging.INFO,
-            datefmt="%d-%b-%y %H:%M:%S",
-            format="%(asctime)s: %(name)s - %(levelname)s - %(message)s",
-            handlers=log_handlers,
-        )
-
-    def check_ble_address(self, address: str) -> bool:
-        """Check if the BLE address is valid
-
-        Args:
-            address (str): The MAC address of the Guardian Earbuds
-
-        Returns:
-            bool: True if the address is valid, False otherwise
-        """
-        if (
-            check_platform() == "Windows"
-            or check_platform() == "Linux"
-            and check_valid_mac(address)
-        ):
-            return True
-        elif check_platform() == "Darwin" and check_valid_uuid(address):
-            logging.info("Platform detected: Darwin")
-            # print(f"UUID is valid for system Darwin: {address}")
-            return True
-        else:
-            logging.error("Invalid BLE address")
-            raise ValueError("Invalid BLE address")
-
-    async def search_device(self):
-        """Connect to the Guardian Earbuds
-
-        Returns:
-            is_connected: bool
-        """
-
-        self.address = await self.guardian_ble.search_device()
-
-        return self.address
-
-    async def get_device_address(self) -> str:
-        """Get the MAC address of the Guardian Earbuds.
-        It searches the MAC address of the device automatically. This
-        address is used as the deviceID for cloud communication
-        """
-        device_address = await self.guardian_ble.get_device_mac(
-            self.guardian_ble.client
-        )
-        return device_address
-
-    async def start_recording(
-        self,
-        recording_timer: int = 36000,
-        led_sleep: bool = False,
-        experiment: str = "None provided",
-        impedance_measurement: bool = False,
-        mains_freq_60hz: bool = False,
-        sending_timout: float = 2,
-        bi_directional_receiving_timeout: float = 5,
-    ):
-        """
-        Start recording data from the Guardian Earbuds.
-        Unidirectional websocket connection to the Guardian Cloud API.
-
-        Args:
-            recording_timer (int, optional): The duration of the recording in seconds. Defaults to 36000.
-            led_sleep (bool, optional): Enable LED sleep mode. Defaults to False.
-            experiment (str, optional): The name of the experiment. Defaults to "None provided". This will
-                                        go to the log file.
-            impedance_measurement (bool, optional): Enable impedance measurement. Defaults to False.
-            mains_freq_60hz (bool, optional): Set to True if the mains frequency is 60Hz. Defaults to False.
-            sending_timout (float): The timeout in seconds for sending data to the cloud. Defaults to 1.
-                                    If no data is sent for a second the sending is interupted and the data
-                                    is buffered. If you have a fast internet and you do not want to lose any data,
-                                    then make 0.5 seconds. If you have slow internet and are fine with losing some data,
-                                    then make 5 seconds. The seconds will be the amount lost before noticing internet loss.
-            bi_directional_receiving_timeout (float): The timeout in seconds for receiving data from the cloud. Defaults to 4.
-                                                      If no data is received for 5 seconds the receiving is interupted and the data
-                                                      the connection will be re-established. If you have a fast internet and you do not want to lose
-                                                      bi-directional data, then make 5 seconds. If you have slow internet and are fine with losing some data,
-                                                      then make 10 seconds. The seconds will be the amount lost before noticing internet loss.
-
-
-        Raises:
-            ValueError: If the recording timer is not valid
-        """
-        # set the timers
-        self.guardian_api.runtime_receipt_timeout = sending_timout
-        self.guardian_api.runtime_bi_directional_timeout = (
-            bi_directional_receiving_timeout
-        )
-        try:
-            if self.debug:
-                logging.info(
-                    "[CLIENT]: Recording timer set to: %s seconds", recording_timer
-                )
-                logging.info("[CLIENT]: Start recording")
-
-            print(f"[CLIENT]: Recording timer set to: {recording_timer} seconds")
-            print("-----Recording starting------")
-
-            data_queue: asyncio.Queue = asyncio.Queue(maxsize=86400)
-
-            recording_id = "py-" + str(
-                uuid.uuid4()
-            )  # the recordingID is a unique ID for each recording
-            logging.info("[CLIENT] Recording ID: %s", recording_id)
-            # log the experiment name in bold using the logging module
-            logging.info("[CLIENT] Experiment description: %s", experiment)
-
-            while self.connection_status == 0:  # TRUE FALSE
-                self.connection_status = await self.guardian_ble.connect_to_device()
-                print("Current Device Status=", self.connection_status)
-            data_stream = RecordingConfig(
-                data_stream_subscription=DataStreams(bandpass_eeg=True)
-            )
-
-            self.guardian_api.guardian_rec = RecordingIn(
-                recordingID=recording_id,
-                deviceID=self.guardian_ble.mac_id,
-                displayName="Your Recording",
-                config=data_stream,
-            )
-            task_list = []
-            task_list.append(
-                asyncio.create_task(
-                    self.guardian_ble.run_ble_record(
-                        data_queue,
-                        recording_timer,
-                        self.guardian_ble.mac_id,
-                        led_sleep,
-                        impedance_measurement,
-                        mains_freq_60hz,
-                    )
-                )
-            )
-            task_list.append(
-                asyncio.create_task(
-                    self.guardian_api.connect_ws_api(
-                        data_queue,
-                        self.guardian_ble.mac_id,
-                        recording_id,
-                        impedance_measurement,
-                    )
-                )
-            )
-
-            await asyncio.wait(task_list)
-
-        except exc.BleakError as err:
-            logging.error("[CLIENT]: BLE error: %s", err)
-
-        if self.debug:
-            logging.info("[CLIENT]: -----------  All tasks are COMPLETED -----------")
-        print(f"-----Recording ID {recording_id}------")
-        try:
-            print(f"-----Device ID {self.guardian_ble.mac_id}------")
-        except Exception:
-            print("An exception occurred, check if your device is switched on")
-
-        print("-----Recording stopped------")
-
-    def stop_recording(self):
-        """Stop recording data from the Guardian Earbuds"""
-
-    async def start_battery(self):
-        """
-        Start recording data from the Guardian Earbuds.
-        Unidirectional websocket connection to the Guardian Cloud API.
-        """
-        print("-----Battery readout started------")
-        if self.debug:
-            logging.info("[CLIENT]: Start recording")
-
-        ble_client_task = asyncio.create_task(self.guardian_ble.read_battery_level())
-        await asyncio.wait([ble_client_task])
-
-        if self.debug:
-            logging.info("[CLIENT]: Disconnect BLE and close websocket connection")
-        print("-----Battery check stopped------")
+"""
+Initialization of the IDUN Guardian Client
+"""
+import os
+import asyncio
+from typing import Union
+import logging
+from datetime import datetime
+from .igeb_bluetooth import GuardianBLE
+from .igeb_api import GuardianAPI
+from .igeb_utils import check_platform, check_valid_mac, check_valid_uuid
+import uuid
+import gc
+from typing import Union
+from bleak import exc
+
+
+class GuardianClient:
+    """
+    Class object for the communication between Guardian Earbuds and Cloud API
+    """
+
+    def __init__(
+        self,
+        address: Union[str, None] = None,
+        debug=True,
+        debug_console=True,
+    ) -> None:
+        """Initialize the Guardian Client
+
+        Args:
+            address (str, optional): The MAC address of the Guardian Earbuds. Defaults to "00000000-0000-0000-0000-000000000000".
+            debug (bool, optional): Enable debug logging. Defaults to True.
+            debug_console (bool, optional): Enable debug logging to console. Defaults to True.
+
+        Raises:
+            ValueError: If the MAC address is not valid
+        """
+        self.is_connected = False
+        self.debug = debug
+        self.debug_to_console = debug_console
+        self.connection_status = 0
+        if self.debug:
+            self.configure_logger()
+
+        if address is not None:
+            if self.check_ble_address(address):
+                self.guardian_ble = GuardianBLE(address, debug=self.debug)
+                self.address = address
+        else:
+            logging.info("No BLE address provided, will search for device...")
+            print("No BLE address provided, will search for device..")
+            self.guardian_ble = GuardianBLE(debug=self.debug)
+
+        self.guardian_api = GuardianAPI(debug=self.debug)
+
+    def configure_logger(self):
+        """Configure the logger for the Guardian Client"""
+        if not os.path.exists("./logs"):
+            os.makedirs("logs")
+
+        datestr = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
+        log_filename = f"./logs/ble_info-{datestr}.log"
+
+        if not os.path.exists(os.path.dirname(log_filename)):
+            os.makedirs(os.path.dirname(log_filename))
+        log_handlers = [logging.FileHandler(log_filename)]
+
+        if self.debug_to_console:
+            log_handlers.append(logging.StreamHandler())
+
+        logging.basicConfig(
+            level=logging.INFO,
+            datefmt="%d-%b-%y %H:%M:%S",
+            format="%(asctime)s: %(name)s - %(levelname)s - %(message)s",
+            handlers=log_handlers,
+        )
+
+    def check_ble_address(self, address: str) -> bool:
+        """Check if the BLE address is valid
+
+        Args:
+            address (str): The MAC address of the Guardian Earbuds
+
+        Returns:
+            bool: True if the address is valid, False otherwise
+        """
+        if (
+            check_platform() == "Windows"
+            or check_platform() == "Linux"
+            and check_valid_mac(address)
+        ):
+            return True
+        elif check_platform() == "Darwin" and check_valid_uuid(address):
+            logging.info("Platform detected: Darwin")
+            # print(f"UUID is valid for system Darwin: {address}")
+            return True
+        else:
+            logging.error("Invalid BLE address")
+            raise ValueError("Invalid BLE address")
+
+    async def search_device(self):
+        """Connect to the Guardian Earbuds
+
+        Returns:
+            is_connected: bool
+        """
+
+        self.address = await self.guardian_ble.search_device()
+
+        return self.address
+
+    async def get_device_address(self) -> str:
+        """Get the MAC address of the Guardian Earbuds.
+        It searches the MAC address of the device automatically. This
+        address is used as the deviceID for cloud communication
+        """
+        device_address = await self.guardian_ble.get_device_mac(
+            self.guardian_ble.client
+        )
+        return device_address
+
+    async def start_recording(
+        self,
+        recording_timer: int = 36000,
+        led_sleep: bool = False,
+        experiment: str = "None provided",
+        impedance_measurement: bool = False,
+        mains_freq_60hz: bool = False,
+        sending_timout: float = 2,
+        bi_directional_receiving_timeout: float = 5,
+    ):
+        """
+        Start recording data from the Guardian Earbuds.
+        Unidirectional websocket connection to the Guardian Cloud API.
+
+        Args:
+            recording_timer (int, optional): The duration of the recording in seconds. Defaults to 36000.
+            led_sleep (bool, optional): Enable LED sleep mode. Defaults to False.
+            experiment (str, optional): The name of the experiment. Defaults to "None provided". This will
+                                        go to the log file.
+            impedance_measurement (bool, optional): Enable impedance measurement. Defaults to False.
+            mains_freq_60hz (bool, optional): Set to True if the mains frequency is 60Hz. Defaults to False.
+            sending_timout (float): The timeout in seconds for sending data to the cloud. Defaults to 1.
+                                    If no data is sent for a second the sending is interupted and the data
+                                    is buffered. If you have a fast internet and you do not want to lose any data,
+                                    then make 0.5 seconds. If you have slow internet and are fine with losing some data,
+                                    then make 5 seconds. The seconds will be the amount lost before noticing internet loss.
+            bi_directional_receiving_timeout (float): The timeout in seconds for receiving data from the cloud. Defaults to 4.
+                                                      If no data is received for 5 seconds the receiving is interupted and the data
+                                                      the connection will be re-established. If you have a fast internet and you do not want to lose
+                                                      bi-directional data, then make 5 seconds. If you have slow internet and are fine with losing some data,
+                                                      then make 10 seconds. The seconds will be the amount lost before noticing internet loss.
+
+
+        Raises:
+            ValueError: If the recording timer is not valid
+        """
+        # set the timers
+        self.guardian_api.runtime_receipt_timeout = sending_timout
+        self.guardian_api.runtime_bi_directional_timeout = (
+            bi_directional_receiving_timeout
+        )
+        try:
+            if self.debug:
+                logging.info(
+                    "[CLIENT]: Recording timer set to: %s seconds", recording_timer
+                )
+                logging.info("[CLIENT]: Start recording")
+
+            print(f"[CLIENT]: Recording timer set to: {recording_timer} seconds")
+            print("-----Recording starting------")
+
+            data_queue: asyncio.Queue = asyncio.Queue(maxsize=86400)
+
+            recording_id = "py-" + str(
+                uuid.uuid4()
+            )  # the recordingID is a unique ID for each recording
+            logging.info("[CLIENT] Recording ID: %s", recording_id)
+            # log the experiment name in bold using the logging module
+            logging.info("[CLIENT] Experiment description: %s", experiment)
+
+            while self.connection_status == 0:  # TRUE FALSE
+                self.connection_status = await self.guardian_ble.connect_to_device()
+                print("Current Device Status=", self.connection_status)
+
+            tasks = []
+            tasks.append(
+                self.guardian_ble.run_ble_record(
+                    data_queue,
+                    recording_timer,
+                    self.guardian_ble.mac_id,
+                    led_sleep,
+                    impedance_measurement,
+                    mains_freq_60hz,
+                )
+            )
+            tasks.append(
+                self.guardian_api.connect_ws_api(
+                    data_queue,
+                    self.guardian_ble.mac_id,
+                    recording_id,
+                    impedance_measurement,
+                )
+            )
+
+            await asyncio.wait(tasks)
+
+        except exc.BleakError as err:
+            logging.error("[CLIENT]: BLE error: %s", err)
+
+        if self.debug:
+            logging.info("[CLIENT]: -----------  All tasks are COMPLETED -----------")
+        print(f"-----Recording ID {recording_id}------")
+        try:
+            print(f"-----Device ID {self.guardian_ble.mac_id}------")
+        except Exception:
+            print("An exception occurred, check if your device is switched on")
+
+        print("-----Recording stopped------")
+
+    def stop_recording(self):
+        """Stop recording data from the Guardian Earbuds"""
+
+    async def start_battery(self):
+        """
+        Start recording data from the Guardian Earbuds.
+        Unidirectional websocket connection to the Guardian Cloud API.
+        """
+        print("-----Battery readout started------")
+        if self.debug:
+            logging.info("[CLIENT]: Start recording")
+
+        ble_client_task = self.guardian_ble.read_battery_level()
+        await asyncio.wait([ble_client_task])
+
+        if self.debug:
+            logging.info("[CLIENT]: Disconnect BLE and close websocket connection")
+        print("-----Battery check stopped------")
```

### Comparing `idun_guardian_client-1.1.5/src/idun_guardian_client/config.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/config.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from pydantic import BaseSettings
-
-
-class Settings(BaseSettings):
-    """
-    Microservice settings. They can be set as environment variables.
-    """
-
-    # GDK 2.0 BLE characteristic
-    STARTBYTE: str = "0xF0"
-    ENDBYTE: str = "0x0F"
-    DEVICE_ID: str = "703DF80E-F543-1947-C0AD-2178ACACAFC7"
-    UUID_MEAS_EEGIMU: str = "beffd56c-c915-48f5-930d-4c1feee0fcc4"
-    UUID_MEAS_EEG: str = "beffd56c-c915-48f5-930d-4c1feee0fcc5"
-    UUID_MEAS_IMP: str = "beffd56c-c915-48f5-930d-4c1feee0fcc8"
-    UUID_DEVICE_SERVICE: str = "0000180a-0000-1000-8000-00805f9b34fb"
-    UUID_MAC_ID: str = "00002a25-0000-1000-8000-00805f9b34fb"
-    UUID_FIRMWARE_VERSION: str = "00002a26-0000-1000-8000-00805f9b34fb"
-    UUID_BATTERY_ID: str = "00002a19-0000-1000-8000-00805f9b34fb"
-    UUID_CFG: str = "beffd56c-c915-48f5-930d-4c1feee0fcc9"
-    UUID_CMD: str = "beffd56c-c915-48f5-930d-4c1feee0fcca"
-    LED_ON_CFG: str = "d1"
-    LED_OFF_CFG: str = "d0"
-    NOTCH_FREQ_50_CFG: str = "n0"
-    NOTCH_FREQ_60_CFG: str = "n1"
-    START_CMD: str = "M"  #'\x62' #b -> start measurement
-    STOP_CMD: str = "S"  # '\x73' #s -> stop measurement
-    START_IMP_CMD: str = "Z"  # '\x7a' #z -> start impedance
-    STOP_IMP_CMD: str = "X"  # '\x78' #x -> stop impedance
-    UUID_BATT_GDK: str = "00002a19-0000-1000-8000-00805f9b34fb"
-    CONNECTION_TIME = 60
-
-    # Websocket Connection API Gateway
-    WS_IDENTIFIER: str = "wss://wpcg36nil5.execute-api.eu-central-1.amazonaws.com/v1/"
-
-    # REST API Gateway
-    REST_API_LOGIN: str = "https://d3pq71txhb.execute-api.eu-central-1.amazonaws.com/"
-
-
-settings = Settings()
+from pydantic import BaseSettings
+
+
+class Settings(BaseSettings):
+    """
+    Microservice settings. They can be set as environment variables.
+    """
+
+    # GDK 2.0 BLE characteristic
+    STARTBYTE: str = "0xF0"
+    ENDBYTE: str = "0x0F"
+    DEVICE_ID: str = "703DF80E-F543-1947-C0AD-2178ACACAFC7"
+    UUID_MEAS_EEGIMU: str = "beffd56c-c915-48f5-930d-4c1feee0fcc4"
+    UUID_MEAS_EEG: str = "beffd56c-c915-48f5-930d-4c1feee0fcc5"
+    UUID_MEAS_IMP: str = "beffd56c-c915-48f5-930d-4c1feee0fcc8"
+    UUID_DEVICE_SERVICE: str = "0000180a-0000-1000-8000-00805f9b34fb"
+    UUID_MAC_ID: str = "00002a25-0000-1000-8000-00805f9b34fb"
+    UUID_FIRMWARE_VERSION: str = "00002a26-0000-1000-8000-00805f9b34fb"
+    UUID_BATTERY_ID: str = "00002a19-0000-1000-8000-00805f9b34fb"
+    UUID_CFG: str = "beffd56c-c915-48f5-930d-4c1feee0fcc9"
+    UUID_CMD: str = "beffd56c-c915-48f5-930d-4c1feee0fcca"
+    LED_ON_CFG: str = "d1"
+    LED_OFF_CFG: str = "d0"
+    NOTCH_FREQ_50_CFG: str = "n0"
+    NOTCH_FREQ_60_CFG: str = "n1"
+    START_CMD: str = "M"  #'\x62' #b -> start measurement
+    STOP_CMD: str = "S"  # '\x73' #s -> stop measurement
+    START_IMP_CMD: str = "Z"  # '\x7a' #z -> start impedance
+    STOP_IMP_CMD: str = "X"  # '\x78' #x -> stop impedance
+    UUID_BATT_GDK: str = "00002a19-0000-1000-8000-00805f9b34fb"
+    CONNECTION_TIME = 60
+
+    # Websocket Connection API Gateway
+    WS_IDENTIFIER: str = "wss://wpcg36nil5.execute-api.eu-central-1.amazonaws.com/v1/"
+
+    # REST API Gateway
+    REST_API_LOGIN: str = "https://d3pq71txhb.execute-api.eu-central-1.amazonaws.com/"
+
+
+settings = Settings()
```

### Comparing `idun_guardian_client-1.1.5/src/idun_guardian_client/igeb_bluetooth.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/igeb_bluetooth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,849 +1,854 @@
-"""
-Guardian Bluetooth utils.
-"""
-import sys
-import asyncio
-import os
-from codecs import utf_8_encode
-import logging
-import time
-import base64
-import datetime
-import gc
-from bleak import BleakClient, BleakScanner, exc
-import typing
-import platform
-from .config import settings
-from .debug_logs import *
-
-SEARCH_BREAK = 3
-
-
-class GuardianBLE:
-    """Main Guardian BLE client."""
-
-    def __init__(self, address: str = "", debug: bool = True) -> None:
-        """Initialize the Guardian BLE client.
-
-        Args:
-            address (str, optional): BLE device address. Defaults to "".
-            debug (bool, optional): Debug mode. Defaults to True.
-        """
-        self.client: typing.Optional[BleakClient] = None
-
-        # Debugging mode
-        self.address = address
-        self.debug = debug
-        self.write_to_file: bool = debug
-
-        # Initial connection flags
-        self.initialise_connection: bool = True
-        self.connection_established = False
-        self.time_left = True
-        self.initial_time = True
-
-        # Bluetooth reconnect delay
-        self.original_time = time.time()
-        self.reconnect_try_amount = 50
-        self.try_to_connect_timeout = self.reconnect_try_amount
-
-        # Bluetooth timings
-        self.ble_delay = 1
-        self.ble_stop_delay = 1
-        self.device_lost = False
-
-        # API timeings
-        self.sent_final_package_time = 1
-
-        # The timing constants
-        self.sample_rate = 250
-        self.amount_samples_packet = 20
-        self.max_index = 256
-        self.prev_index = 0
-        self.prev_timestamp = 0
-
-        self.remaining_time = 1
-
-        self.get_ble_characteristic()
-        self.device = None
-        self.mac_id = ""
-        self.platform = platform.system()
-        self.teminating_ble_process = False
-        loggig_ble_init(self.debug)
-
-    def get_ble_characteristic(self) -> None:
-        """Get the environment variables."""
-        # General information
-        self.battery_id = settings.UUID_BATT_GDK
-        self.device_service = settings.UUID_DEVICE_SERVICE
-        self.mac_uuid = settings.UUID_MAC_ID
-        self.firmware_uuid = settings.UUID_FIRMWARE_VERSION
-
-        # EEG/IMU measurement
-        self.meas_eeg_id = settings.UUID_MEAS_EEGIMU
-        self.command_id = settings.UUID_CMD
-        self.start_cmd = settings.START_CMD
-        self.stop_cmd = settings.STOP_CMD
-
-        # Impedance measurement
-        self.meas_imp_id = settings.UUID_MEAS_IMP
-        self.start_imp_cmd = settings.START_IMP_CMD
-        self.stop_imp_cmd = settings.STOP_IMP_CMD
-        self.notch_freq_50_cfg = settings.NOTCH_FREQ_50_CFG
-        self.notch_freq_60_cfg = settings.NOTCH_FREQ_60_CFG
-
-        # LED control
-        self.cfg_id = settings.UUID_CFG
-        self.led_on_cfg = settings.LED_ON_CFG
-        self.led_off_cfg = settings.LED_OFF_CFG
-
-    async def get_ble_devices(self) -> list:
-        """
-        Scan for devices and return a list of devices.
-        """
-        devices_dict: dict = {}
-        ble_device_list: list = []
-        devices = await BleakScanner.discover()
-        igeb_name = "IGEB"
-        device_id = 0
-        print("\n----- Available devices -----\n")
-        print("Index | Name | Address")
-        print("----------------------------")
-        for _, device in enumerate(devices):
-            # print device discovered
-            if device.name == igeb_name:
-                print(f"{device_id}     | {device.name} | {device.address}")
-                devices_dict[device.address] = []
-                devices_dict[device.address].append(device.name)
-                ble_device_list.append(device.address)
-                device_id += 1
-        print("----------------------------\n")
-        return ble_device_list
-
-    async def get_device_mac(self, client) -> str:
-        """Get the device MAC address.
-        This is different from BLE device address
-        (UUID on Mac or MAC address on Windows)
-
-        Args:
-            device_name (str): Device name
-
-        Returns:
-            str: MAC address
-        """
-        # async with BleakClient(self.address) as client:
-        logging_searching(self.debug)
-        value = bytes(await client.read_gatt_char(self.mac_uuid))
-        await asyncio.sleep(self.ble_delay)
-        firmware_version = bytes(await client.read_gatt_char(self.firmware_uuid))
-        mac_address = value.decode("utf-8")
-        firmware_decoded = firmware_version.decode("utf-8")
-        mac_address = mac_address.replace(":", "-")
-
-        logging_device_info(self.debug, mac_address, firmware_decoded)
-        return mac_address
-
-    async def search_device(self) -> str:
-        """This function searches for the device and returns the address of the device.
-        If the device is not found, it exits the program. If multiple devices are found,
-        it asks the user to select the device. If one device is found, it returns the
-        address of the device.
-
-        Returns:
-            _type_: _description_
-        """
-
-        while True:
-            ble_device_list = await self.get_ble_devices()
-            if len(ble_device_list) == 0:
-                logging_device_not_found(self.debug, SEARCH_BREAK)
-                await asyncio.sleep(SEARCH_BREAK)
-
-            elif len(ble_device_list) == 1:
-                logging_device_found(self.debug, ble_device_list)
-                self.address = ble_device_list[0]
-                break
-            else:
-                index_str = input(
-                    "Enter the index of the GDK device you want to connect to \
-                    \nIf cannot find the device, please restart the program and try again: "
-                )
-                index = int(index_str)
-                self.address = ble_device_list[index]
-                break
-
-        logging_device_address(self.debug, self.address)
-
-        return self.address
-
-    async def connect_to_device(self):
-        """
-        This function initialises the connection to the device.
-        It finds the device using the address, sets up callback,
-        and connects to the device.
-        """
-        logging_trying_to_connect(self.debug, self.address)
-
-        if not self.device:
-            self.device = await BleakScanner.find_device_by_address(
-                self.address, timeout=20.0
-            )
-        if not self.device:
-            raise exc.BleakError(
-                f"A device with address {self.address} could not be found."
-            )
-
-        if self.platform == "Windows":
-            if not self.client:
-                self.client = BleakClient(
-                    self.device, disconnected_callback=self.disconnected_callback
-                )
-        else:
-            self.client = None
-            self.client = BleakClient(
-                self.device, disconnected_callback=self.disconnected_callback
-            )
-        if self.client is not None:
-            try:
-                await asyncio.wait_for(self.client.connect(), timeout=4)
-            except asyncio.TimeoutError:
-                log_timeout_while_trying_connection(self.debug)
-                pass
-            except Exception as err:
-                log_exception_while_trying_connection(self.debug, err)
-                pass
-            if self.client.is_connected:
-                if self.mac_id == "":
-                    try:
-                        self.mac_id = await self.get_device_mac(self.client)
-
-                    except Exception as err:
-                        log_exception_unable_to_find_MACaddress(self.debug)
-                        self.initialise_connection = True
-                        self.connection_established = False
-                        return 0
-                if self.mac_id:
-                    self.connection_established = True
-                    self.initialise_connection = False
-                    logging_connected(self.debug, self.address)
-                    return 1
-
-            else:
-                log_no_connection_established(self.debug)
-                try:
-                    await self.client.disconnect()
-                    await asyncio.sleep(4)
-                except Exception:
-                    log_exception_in_disconnecting(self.debug)
-                gc.collect()
-                self.initialise_connection = True
-                self.connection_established = False
-                return 0
-        else:
-            log_not_client_found(self.debug)
-
-    def disconnected_callback(self, client):  # pylint: disable=unused-argument
-        """
-        Callback function when device is disconnected.
-
-        Args:
-            client (BleakClient): BleakClient object
-        """
-        logging_disconnected_recognised(self.debug)
-        self.connection_established = False
-        self.initialise_connection = True
-
-    async def run_ble_record(
-        self,
-        data_queue: asyncio.Queue,
-        record_time=60,
-        mac_id="MAC_ID",
-        led_sleep: bool = False,
-        impedance_measurement: bool = False,
-        mains_freq_60hz: bool = False,
-    ) -> None:
-        """
-        This function runs the recording of the data. It sets up the bluetooth
-        connection, starts the recording, and then reads the data and adds it to
-        the queue. The API class then reads the data from the queue and sends it
-        to the cloud.
-
-        Args:
-            data_queue (asyncio.Queue): Queue to store the data
-            record_time (_type_): The time to record for
-            mac_id (_type_): The MAC address of the device
-            led_sleep (_type_): Whether to turn off the LED
-
-        Raises:
-            BleakError: _description_
-        """
-
-        def time_stamp_creator(new_index):
-            """
-            This function creates a timestamp for the cloud based on the
-            time the recording started. Each time stamp is based on the index
-            of that is sent from the device. The index is the number of iterates
-            between 0 and 256. The time stamp is the 1/250s multiplied by the
-            index.
-
-            Args:
-                new_index (int): Index of the data point from the ble packet
-
-            Returns:
-                str: Timestamp in the format of YYYY-MM-DDTHH:MM:SS
-            """
-            index_diff = new_index - self.prev_index
-
-            if self.prev_timestamp == 0:
-                time_data = datetime.datetime.now().astimezone().isoformat()
-                # convert time_data to a float in seconds
-                time_data = time.mktime(
-                    datetime.datetime.strptime(
-                        time_data, "%Y-%m-%dT%H:%M:%S.%f%z"
-                    ).timetuple()
-                )
-                new_time_stamp = time_data
-            else:
-                multiplier = (index_diff + self.max_index) % self.max_index
-                new_time_stamp = (
-                    self.amount_samples_packet * (1 / self.sample_rate) * multiplier
-                ) + self.prev_timestamp
-
-            self.prev_index = new_index
-            self.prev_timestamp = new_time_stamp
-
-            time_stamp_isoformat = (
-                datetime.datetime.fromtimestamp(new_time_stamp).astimezone().isoformat()
-            )
-
-            return time_stamp_isoformat
-
-        async def data_handler(_, data):
-            """Data handler for the BLE client.
-                Data is put in a queue and forwarded to the API.
-
-            Args:
-                callback (handler Object): Handler object
-                data (bytes): Binary data package
-            """
-            data_base_64 = base64.b64encode(data).decode("ascii")
-            new_time_stamp = time_stamp_creator(data[1])
-
-            if self.write_to_file:
-                self.data_recording_logfile.write(f"{data_base_64},\n")
-
-            package = {
-                "timestamp": new_time_stamp,
-                "deviceID": mac_id,
-                "data": data_base_64,
-                "stop": False,
-            }
-            if not data_queue.full():
-                await asyncio.shield(data_queue.put(package))
-            else:
-                await asyncio.shield(data_queue.get())
-
-        async def battery_handler(_, data):
-            """Battery handler for the BLE client.
-            Args:
-                callback (handler Object): Handler object
-                data (bytes): Battery Level as uint8_t
-            """
-            logging_batterylevel(self.debug, data)
-
-        async def impedance_handler(_, data):
-            """Impedance handler for the BLE client.
-                Data is put in a queue and forwarded to the API.
-
-            Args:
-                callback (handler Object): Handler object
-                data (bytes): Binary data package with impedance values
-            """
-            data_int = int.from_bytes(data, byteorder="little")
-            print(f"[BLE]: Impedance value : {round(data_int/1000,2)} kOhms")
-            if self.write_to_file:
-                self.data_recording_logfile.write(f"{data_int}\n")
-
-            package = {
-                "timestamp": datetime.datetime.now().astimezone().isoformat(),
-                "deviceID": mac_id,
-                "stop": False,
-                "impedance": data_int,
-            }
-            # add the received impedance data to the queue
-            if not data_queue.full():
-                await data_queue.put(package)
-            else:
-                await data_queue.get()
-
-        async def send_start_commands_recording():
-            """Send start commands to the device."""
-            logging_sending_start(self.debug)
-
-            # ------------------ Configuration ------------------
-            if led_sleep:
-                await asyncio.sleep(self.ble_delay)
-                await self.client.write_gatt_char(
-                    self.cfg_id, utf_8_encode(self.led_off_cfg)[0]
-                )
-            # ------------------ Subscribe to notifications ------------------
-            # Notify the client that these two services are required
-            logging_subscribing_eeg_notification(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            await self.client.start_notify(self.meas_eeg_id, data_handler)
-
-            logging_subscribing_battery_notification(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            await self.client.start_notify(self.battery_id, battery_handler)
-
-            # ------------------ Start commands ------------------
-            # sleep so that cleint can respond
-            await asyncio.sleep(self.ble_delay)
-            # send start command for recording data
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.start_cmd)[0]
-            )
-
-        async def send_start_commands_impedance():
-            # ----------------- Configuration -----------------
-            if mains_freq_60hz:
-                await asyncio.sleep(self.ble_delay)
-                await self.client.write_gatt_char(
-                    self.cfg_id, utf_8_encode(self.notch_freq_60_cfg)[0]
-                )
-            else:
-                await asyncio.sleep(self.ble_delay)
-                await self.client.write_gatt_char(
-                    self.cfg_id, utf_8_encode(self.notch_freq_50_cfg)[0]
-                )
-
-            # ----------------- Subscribe -----------------
-            logging_subscribing_impedance_notification(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            await self.client.start_notify(self.meas_imp_id, impedance_handler)
-
-            # ----------------- Send start command -----------------
-            logging_starting_impedance_measurement_commands(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.start_imp_cmd)[0]
-            )
-
-        async def stop_impedance_timeout():
-            """Stop recording gracefully."""
-            # make sure the last data is now a stop command
-            package = {
-                "timestamp": datetime.datetime.now().astimezone().isoformat(),
-                "deviceID": mac_id,
-                "stop": True,
-            }
-            # ------------------ Load final stop package ------------------
-            if not data_queue.full():
-                await data_queue.put(package)
-            else:
-                await data_queue.get()
-                await data_queue.put(package)
-            logging_sending_stop(self.debug)
-            # ------------------ API should send already loaded package  ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # This gives time for the api to send already loaded data
-            logging_sending_stop_device(self.debug)
-            await asyncio.sleep(self.ble_delay)
-
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.stop_imp_cmd)[0]
-            )
-
-            # ------------------ Disconnect command to device ------------------
-            logging_sending_disconnect(self.debug)
-            await asyncio.sleep(self.ble_stop_delay)
-            await self.client.disconnect()
-            await asyncio.sleep(self.ble_stop_delay)
-
-            if self.write_to_file:
-                self.data_recording_logfile.close()
-            logging_recording_successfully_stopped(self.debug)
-
-        async def stop_recording_timeout():
-            """Stop recording gracefully."""
-
-            # make sure the last data is now a stop command
-            package = {
-                "timestamp": datetime.datetime.now().astimezone().isoformat(),
-                "deviceID": mac_id,
-                "data": "STOP_TIMEOUT",
-                "stop": True,
-            }
-            # ------------------ Load final stop package ------------------
-            if not data_queue.full():
-                await data_queue.put(package)
-            else:
-                await data_queue.get()
-                await data_queue.put(package)
-            logging_sending_stop(self.debug)
-            # ------------------ API should send already loaded package  ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # This gives time for the api to send already loaded data
-            logging_sending_stop_device(self.debug)
-            await asyncio.sleep(self.ble_delay)
-
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.stop_cmd)[0]
-            )
-
-            if led_sleep:
-                logging_turn_ble_on(self.debug)
-                await asyncio.sleep(self.ble_delay)
-                await self.client.write_gatt_char(
-                    self.cfg_id, utf_8_encode(self.led_on_cfg)[0]
-                )
-            # ------------------ Disconnect command to device ------------------
-            logging_sending_disconnect(self.debug)
-            await asyncio.sleep(self.ble_stop_delay)
-            await self.client.disconnect()
-            await asyncio.sleep(self.ble_stop_delay)
-
-            if self.write_to_file:
-                self.data_recording_logfile.close()
-            logging_recording_successfully_stopped(self.debug)
-
-        async def stop_impedance_cancelled_script():
-            """Stop recording abruptly."""
-            logging_keyboard_interrupt(self.debug)
-
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # Give API time to send last package
-            # With its own interupt handling
-            # ------------------ Send stop EEG recording command ------------------
-            logging_sending_stop_device(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            try:
-                await self.client.write_gatt_char(
-                    self.command_id, utf_8_encode(self.stop_imp_cmd)[0]
-                )
-            except Exception:
-                log_device_not_connected_cannot_stop(self.debug)
-
-            # ------------------ Disconnecting commands ------------------
-            logging_sending_disconnect(self.debug)
-            await asyncio.sleep(self.ble_stop_delay)
-
-            await self.client.disconnect()
-
-            log_exception_in_disconnecting(self.debug)
-            await asyncio.sleep(self.ble_stop_delay)
-            # ------------------ Closing file  ------------------
-            if self.write_to_file:
-                self.data_recording_logfile.close()
-            logging_recording_successfully_stopped(self.debug)
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # Give API time to send last package
-            # With its own interupt handling
-
-        async def stop_recording_cancelled_script():
-            """Stop recording abruptly."""
-            logging_keyboard_interrupt(self.debug)
-
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # Give API time to send last package
-            # With its own interupt handling
-            # ------------------ Send stop EEG recording command ------------------
-            logging_sending_stop_device(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            try:
-                await self.client.write_gatt_char(
-                    self.command_id, utf_8_encode(self.stop_cmd)[0]
-                )
-            except Exception:
-                log_device_not_connected_cannot_stop(self.debug)
-
-            # ------------------ Configuring LED back on ------------------
-            if led_sleep:
-                logging_turn_led_on(self.debug)
-                await asyncio.sleep(self.ble_delay)
-                await self.client.write_gatt_char(
-                    self.cfg_id, utf_8_encode(self.led_on_cfg)[0]
-                )
-            # ------------------ Disconnecting commands ------------------
-            logging_sending_disconnect(self.debug)
-            await asyncio.sleep(self.ble_stop_delay)
-
-            await self.client.disconnect()
-
-            await asyncio.sleep(self.ble_stop_delay)
-            # ------------------ Closing file  ------------------
-            if self.write_to_file:
-                self.data_recording_logfile.close()
-            logging_recording_successfully_stopped(self.debug)
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # Give API time to send last package
-            # With its own interupt handling
-
-        async def stop_recording_device_lost():
-            """Stop recording device lost."""
-            logging_device_lost_give_up(self.debug)
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(self.ble_delay)  # Give API time to send last package
-            # ------------------ Loading last package ------------------
-            logging_sending_stop(self.debug)
-            package = {
-                "timestamp": datetime.datetime.now().astimezone().isoformat(),
-                "deviceID": mac_id,
-                "data": "STOP_DEVICE_LOST",
-                "stop": True,
-            }
-            # pack the stop command
-            if not data_queue.full():
-                await data_queue.put(package)
-            else:
-                await data_queue.get()
-                await data_queue.put(package)
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # Give API time to send last package
-            # ------------------ Closing file ------------------
-            if self.write_to_file:
-                self.data_recording_logfile.close()
-
-            return True
-
-        async def bluetooth_reconnect():
-            """Set flags to reconnect to bluetooth device."""
-            self.try_to_connect_timeout = self.try_to_connect_timeout - 1
-            if self.try_to_connect_timeout <= 0:
-                self.device_lost = await stop_recording_device_lost()
-            logging_trying_to_connect_again(self.debug, self.try_to_connect_timeout)
-            self.connection_established = False
-            self.initialise_connection = True
-
-        def initialise_file():
-            """Initialise file for recording."""
-            if self.write_to_file:
-                if not os.path.exists("./logs"):
-                    os.makedirs("logs")
-
-                if not impedance_measurement:
-                    measurement_type = "rec"
-                else:
-                    measurement_type = "imp"
-
-                datestr = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
-                recording_filename = f"./logs/IGEB-{measurement_type}-{datestr}.txt"
-                self.data_recording_logfile = open(
-                    recording_filename, "w", encoding="utf-8"
-                )
-
-        def initialise_timestamps():
-            if self.initial_time:
-                self.initial_time = False  # record that this is the initial time
-                self.original_time = time.time()
-
-        async def main_loop():
-            while True:
-                if self.connection_established:
-                    await asyncio.shield(
-                        asyncio.sleep(self.ble_delay)
-                    )  # sleep so that everything can happen
-                    self.remaining_time = record_time - (
-                        time.time() - self.original_time
-                    )
-                    print(f"Time left: {round(self.remaining_time)}s")
-
-                    if self.remaining_time <= 0:
-                        logging_time_reached(self.debug, self.original_time)
-                        if not impedance_measurement:
-                            await stop_recording_timeout()
-                        else:
-                            await stop_impedance_timeout()
-                        break
-
-                else:
-                    break
-
-        # >>>>>>>>>>>>>>>>>>>>> Start of recording process <<<<<<<<<<<<<<<<<<<<<<<<
-        # ------------------ Initialise values for timestamps ------------------
-        self.prev_timestamp = 0
-        self.prev_index = -1
-        # ------------------ Initialise time values for recording timeout ------------------
-        # This has been decoupled from the device timing for robustness
-        self.original_time = time.time()
-        self.initial_time = True
-        self.time_left = True
-        self.initial_time = True
-        # ------------------ Initialise connection values for trying to connect again ------------------
-        # self.connection_established = False
-        self.try_to_connect_timeout = self.reconnect_try_amount
-        # ------------------ Initialise log file ------------------
-        initialise_file()
-
-        while not self.teminating_ble_process:
-            print("connection:", self.connection_established)
-            print("initialize:", self.initialise_connection)
-            try:
-                if self.initialise_connection:
-                    while self.initialise_connection == True:
-                        await self.connect_to_device()
-                if self.client is not None:
-                    if self.client.is_connected:
-                        logging_device_connected_general(self.debug)
-                        # for windows reconnection
-                        self.initialise_connection = True
-
-                    if not impedance_measurement:
-                        await send_start_commands_recording()
-                    else:
-                        await send_start_commands_impedance()
-
-                    logging_recording_started(self.debug)
-                    self.try_to_connect_timeout = (
-                        self.reconnect_try_amount
-                    )  # reset counter
-                    # >>>>>>>>>>>>>>>>>>>>> Main loop <<<<<<<<<<<<<<<<<<<<<<<<
-                    initialise_timestamps()
-                    await asyncio.shield(main_loop())
-                    # >>>>>>>>>>>>>>>>>>>>> Main loop <<<<<<<<<<<<<<<<<<<<<<<<
-
-                if self.remaining_time <= 0:
-                    self.teminating_ble_process = True
-                    break
-
-                if not self.connection_established:
-                    logging_disconnected_recognised(self.debug)
-                    await bluetooth_reconnect()
-                    if self.device_lost:
-                        break
-
-            except asyncio.CancelledError:
-                if not impedance_measurement:
-                    await stop_recording_cancelled_script()
-                else:
-                    await stop_impedance_cancelled_script()
-                self.teminating_ble_process = True
-                self.connection_established = False
-                self.initialise_connection = False
-                break
-
-            except Exception as error:
-                logging_ble_client_lost(self.debug, error)
-
-            finally:
-                logging_ensuring_ble_disconnected(self.debug)
-                await asyncio.sleep(self.ble_stop_delay)
-                if self.client is not None:
-                    if self.client.is_connected:
-                        try:
-                            print("Stop notification")
-                            await self.client.stop_notify(self.meas_eeg_id)
-                            await asyncio.sleep(self.ble_delay)
-                            await self.client.stop_notify(self.battery_id)
-                            await asyncio.sleep(self.ble_delay)
-                            await self.client.disconnect()
-                            gc.collect()
-                        except Exception:
-                            log_exception_in_disconnecting(self.debug)
-
-                await asyncio.sleep(self.ble_stop_delay)
-                self.connection_established = False
-
-        logging_ble_complete(self.debug)
-
-    async def get_service_and_char(self) -> None:
-        """Get the services and characteristics of the device."""
-        try:
-            async with BleakClient(self.address) as client:
-                logging_device_connected_general(self.debug)
-
-                for service in client.services:
-                    logging_device_info_uuid(self.debug, service)
-
-                    for char in service.characteristics:
-                        if "read" in char.properties:
-                            try:
-                                value = bytes(await client.read_gatt_char(char.uuid))
-                            except exc.BleakError as err:
-                                value = str(err).encode()
-                        else:
-                            value = None
-                        logging_device_info_characteristic(self.debug, char, value)
-
-                await asyncio.sleep(self.ble_stop_delay)
-                await client.disconnect()
-                await asyncio.sleep(self.ble_stop_delay)
-                logging_sending_disconnect(self.debug)
-
-        except exc.BleakError as err:
-            logging_device_connection_failed(self.debug, err)
-
-    async def read_battery_level(self) -> None:
-        """Read the battery level of the device given pre-defined interval."""
-        logging_reading_battery_level(self.debug)
-        while True:
-            try:
-                async with BleakClient(self.address) as client:
-                    logging_device_connected_general(self.debug)
-
-                    await asyncio.sleep(self.ble_delay)
-                    value = int.from_bytes(
-                        (await client.read_gatt_char(self.battery_id)),
-                        byteorder="little",
-                    )
-                    print("-----------------------------")
-                    print(f"\nBattery level: {value}%\n")
-                    print("-----------------------------")
-                    logging_batterylevel_int(self.debug, value)
-
-                    await asyncio.sleep(self.ble_stop_delay)
-                    await client.disconnect()
-                    await asyncio.sleep(self.ble_stop_delay)
-                    logging_sending_disconnect(self.debug)
-                    break
-
-            except exc.BleakError as err:
-                # log the error
-                logging_device_connection_failed(self.debug, err)
-                await asyncio.sleep(3)
-                continue
-
-    async def get_device_information(self) -> dict:
-        """Read the device information of the device."""
-
-        device_info = {}
-
-        async with BleakClient(self.address) as client:
-            logging_device_connected_general(self.debug)
-
-            for service in client.services:
-                if service.uuid == self.device_service:
-                    for char in service.characteristics:
-                        if "read" in char.properties:
-                            try:
-                                value = bytes(await client.read_gatt_char(char.uuid))
-                            except exc.BleakError as err:
-                                value = str(err).encode()
-                        else:
-                            value = None
-
-                        print(f"{ char.description}:{str(value)}")
-                        device_info[char.description] = str(value)
-                        logging_device_description_list(self.debug, char, value)
-
-        return device_info
+"""
+Guardian Bluetooth utils.
+"""
+import sys
+import asyncio
+import os
+from codecs import utf_8_encode
+import logging
+import time
+import base64
+import datetime
+import gc
+from bleak import BleakClient, BleakScanner, exc
+import typing
+import platform
+from .config import settings
+from .debug_logs import *
+
+SEARCH_BREAK = 3
+
+
+class GuardianBLE:
+    """Main Guardian BLE client."""
+
+    def __init__(self, address: str = "", debug: bool = True) -> None:
+        """Initialize the Guardian BLE client.
+
+        Args:
+            address (str, optional): BLE device address. Defaults to "".
+            debug (bool, optional): Debug mode. Defaults to True.
+        """
+        self.client: typing.Optional[BleakClient] = None
+
+        # Debugging mode
+        self.address = address
+        self.debug = debug
+        self.write_to_file: bool = debug
+
+        # Initial connection flags
+        self.initialise_connection: bool = True
+        self.connection_established = False
+        self.time_left = True
+        self.initial_time = True
+
+        # Bluetooth reconnect delay
+        self.original_time = time.time()
+        self.reconnect_try_amount = 50
+        self.try_to_connect_timeout = self.reconnect_try_amount
+
+        # Bluetooth timings
+        self.ble_delay = 1
+        self.ble_stop_delay = 1
+        self.device_lost = False
+
+        # API timeings
+        self.sent_final_package_time = 1
+
+        # The timing constants
+        self.sample_rate = 250
+        self.amount_samples_packet = 20
+        self.max_index = 256
+        self.prev_index = 0
+        self.prev_timestamp = 0
+
+        self.remaining_time = 1
+
+        self.get_ble_characteristic()
+        self.device = None
+        self.mac_id = ""
+        self.platform = platform.system()
+        self.teminating_ble_process = False
+        loggig_ble_init(self.debug)
+
+    def get_ble_characteristic(self) -> None:
+        """Get the environment variables."""
+        # General information
+        self.battery_id = settings.UUID_BATT_GDK
+        self.device_service = settings.UUID_DEVICE_SERVICE
+        self.mac_uuid = settings.UUID_MAC_ID
+        self.firmware_uuid = settings.UUID_FIRMWARE_VERSION
+
+        # EEG/IMU measurement
+        self.meas_eeg_id = settings.UUID_MEAS_EEGIMU
+        self.command_id = settings.UUID_CMD
+        self.start_cmd = settings.START_CMD
+        self.stop_cmd = settings.STOP_CMD
+
+        # Impedance measurement
+        self.meas_imp_id = settings.UUID_MEAS_IMP
+        self.start_imp_cmd = settings.START_IMP_CMD
+        self.stop_imp_cmd = settings.STOP_IMP_CMD
+        self.notch_freq_50_cfg = settings.NOTCH_FREQ_50_CFG
+        self.notch_freq_60_cfg = settings.NOTCH_FREQ_60_CFG
+
+        # LED control
+        self.cfg_id = settings.UUID_CFG
+        self.led_on_cfg = settings.LED_ON_CFG
+        self.led_off_cfg = settings.LED_OFF_CFG
+
+    async def get_ble_devices(self) -> list:
+        """
+        Scan for devices and return a list of devices.
+        """
+        devices_dict: dict = {}
+        ble_device_list: list = []
+        devices = await BleakScanner.discover()
+        igeb_name = "IGEB"
+        device_id = 0
+        print("\n----- Available devices -----\n")
+        print("Index | Name | Address")
+        print("----------------------------")
+        for _, device in enumerate(devices):
+            # print device discovered
+            if device.name == igeb_name:
+                print(f"{device_id}     | {device.name} | {device.address}")
+                devices_dict[device.address] = []
+                devices_dict[device.address].append(device.name)
+                ble_device_list.append(device.address)
+                device_id += 1
+        print("----------------------------\n")
+        return ble_device_list
+
+    async def get_device_mac(self, client) -> str:
+        """Get the device MAC address.
+        This is different from BLE device address
+        (UUID on Mac or MAC address on Windows)
+
+        Args:
+            device_name (str): Device name
+
+        Returns:
+            str: MAC address
+        """
+        # async with BleakClient(self.address) as client:
+        logging_searching(self.debug)
+        value = bytes(await client.read_gatt_char(self.mac_uuid))
+        await asyncio.sleep(self.ble_delay)
+        firmware_version = bytes(await client.read_gatt_char(self.firmware_uuid))
+        mac_address = value.decode("utf-8")
+        firmware_decoded = firmware_version.decode("utf-8")
+        mac_address = mac_address.replace(":", "-")
+
+        logging_device_info(self.debug, mac_address, firmware_decoded)
+        return mac_address
+
+    async def search_device(self) -> str:
+        """This function searches for the device and returns the address of the device.
+        If the device is not found, it exits the program. If multiple devices are found,
+        it asks the user to select the device. If one device is found, it returns the
+        address of the device.
+
+        Returns:
+            _type_: _description_
+        """
+
+        while True:
+            ble_device_list = await self.get_ble_devices()
+            if len(ble_device_list) == 0:
+                logging_device_not_found(self.debug, SEARCH_BREAK)
+                await asyncio.sleep(SEARCH_BREAK)
+
+            elif len(ble_device_list) == 1:
+                logging_device_found(self.debug, ble_device_list)
+                self.address = ble_device_list[0]
+                break
+            else:
+                index_str = input(
+                    "Enter the index of the GDK device you want to connect to \
+                    \nIf cannot find the device, please restart the program and try again: "
+                )
+                index = int(index_str)
+                self.address = ble_device_list[index]
+                break
+
+        logging_device_address(self.debug, self.address)
+
+        return self.address
+
+    def exit_system(self) -> None:
+        """Exit the system."""
+        try:
+            sys.exit(0)
+        except SystemExit:
+            os._exit(0)
+
+    async def connect_to_device(self):
+        """
+        This function initialises the connection to the device.
+        It finds the device using the address, sets up callback,
+        and connects to the device.
+        """
+        logging_trying_to_connect(self.debug, self.address)
+
+        if not self.device:
+            self.device = await BleakScanner.find_device_by_address(
+                self.address, timeout=20.0
+            )
+        if not self.device:
+            raise exc.BleakError(
+                f"A device with address {self.address} could not be found."
+            )
+
+        if self.platform == "Windows":
+            if not self.client:
+                self.client = BleakClient(
+                    self.device, disconnected_callback=self.disconnected_callback
+                )
+        else:
+            self.client = None
+            self.client = BleakClient(
+                self.device, disconnected_callback=self.disconnected_callback
+            )
+        if self.client is not None:
+            try:
+                await asyncio.wait_for(self.client.connect(), timeout=4)
+            except asyncio.TimeoutError:
+                log_timeout_while_trying_connection(self.debug)
+                pass
+            except Exception as err:
+                log_exception_while_trying_connection(self.debug, err)
+                pass
+            if self.client.is_connected:
+                if self.mac_id == "":
+                    try:
+                        self.mac_id = await self.get_device_mac(self.client)
+
+                    except Exception as err:
+                        log_exception_unable_to_find_MACaddress(self.debug)
+                        self.initialise_connection = True
+                        self.connection_established = False
+                        return 0
+                if self.mac_id:
+                    self.connection_established = True
+                    self.initialise_connection = False
+                    logging_connected(self.debug, self.address)
+                    return 1
+
+            else:
+                log_no_connection_established(self.debug)
+                try:
+                    await self.client.disconnect()
+                    await asyncio.sleep(4)
+                except Exception:
+                    log_exception_in_disconnecting(self.debug)
+                gc.collect()
+                self.initialise_connection = True
+                self.connection_established = False
+                return 0
+        else:
+            log_not_client_found(self.debug)
+
+    def disconnected_callback(self, client):  # pylint: disable=unused-argument
+        """
+        Callback function when device is disconnected.
+
+        Args:
+            client (BleakClient): BleakClient object
+        """
+        logging_disconnected_recognised(self.debug)
+        self.connection_established = False
+        self.initialise_connection = True
+
+    async def run_ble_record(
+        self,
+        data_queue: asyncio.Queue,
+        record_time=60,
+        mac_id="MAC_ID",
+        led_sleep: bool = False,
+        impedance_measurement: bool = False,
+        mains_freq_60hz: bool = False,
+    ) -> None:
+        """
+        This function runs the recording of the data. It sets up the bluetooth
+        connection, starts the recording, and then reads the data and adds it to
+        the queue. The API class then reads the data from the queue and sends it
+        to the cloud.
+
+        Args:
+            data_queue (asyncio.Queue): Queue to store the data
+            record_time (_type_): The time to record for
+            mac_id (_type_): The MAC address of the device
+            led_sleep (_type_): Whether to turn off the LED
+
+        Raises:
+            BleakError: _description_
+        """
+
+        def time_stamp_creator(new_index):
+            """
+            This function creates a timestamp for the cloud based on the
+            time the recording started. Each time stamp is based on the index
+            of that is sent from the device. The index is the number of iterates
+            between 0 and 256. The time stamp is the 1/250s multiplied by the
+            index.
+
+            Args:
+                new_index (int): Index of the data point from the ble packet
+
+            Returns:
+                str: Timestamp in the format of YYYY-MM-DDTHH:MM:SS
+            """
+            index_diff = new_index - self.prev_index
+
+            if self.prev_timestamp == 0:
+                time_data = datetime.datetime.now().astimezone().isoformat()
+                # convert time_data to a float in seconds
+                time_data = time.mktime(
+                    datetime.datetime.strptime(
+                        time_data, "%Y-%m-%dT%H:%M:%S.%f%z"
+                    ).timetuple()
+                )
+                new_time_stamp = time_data
+            else:
+                multiplier = (index_diff + self.max_index) % self.max_index
+                new_time_stamp = (
+                    self.amount_samples_packet * (1 / self.sample_rate) * multiplier
+                ) + self.prev_timestamp
+
+            self.prev_index = new_index
+            self.prev_timestamp = new_time_stamp
+
+            time_stamp_isoformat = (
+                datetime.datetime.fromtimestamp(new_time_stamp).astimezone().isoformat()
+            )
+
+            return time_stamp_isoformat
+
+        async def data_handler(_, data):
+            """Data handler for the BLE client.
+                Data is put in a queue and forwarded to the API.
+
+            Args:
+                callback (handler Object): Handler object
+                data (bytes): Binary data package
+            """
+            data_base_64 = base64.b64encode(data).decode("ascii")
+            new_time_stamp = time_stamp_creator(data[1])
+
+            if self.write_to_file:
+                self.data_recording_logfile.write(f"{data_base_64},\n")
+
+            package = {
+                "timestamp": new_time_stamp,
+                "deviceID": mac_id,
+                "data": data_base_64,
+                "stop": False,
+            }
+            if not data_queue.full():
+                await asyncio.shield(data_queue.put(package))
+            else:
+                await asyncio.shield(data_queue.get())
+
+        async def battery_handler(_, data):
+            """Battery handler for the BLE client.
+            Args:
+                callback (handler Object): Handler object
+                data (bytes): Battery Level as uint8_t
+            """
+            logging_batterylevel(self.debug, data)
+
+        async def impedance_handler(_, data):
+            """Impedance handler for the BLE client.
+                Data is put in a queue and forwarded to the API.
+
+            Args:
+                callback (handler Object): Handler object
+                data (bytes): Binary data package with impedance values
+            """
+            data_int = int.from_bytes(data, byteorder="little")
+            print(f"[BLE]: Impedance value : {round(data_int/1000,2)} kOhms")
+            if self.write_to_file:
+                self.data_recording_logfile.write(f"{data_int}\n")
+
+            package = {
+                "timestamp": datetime.datetime.now().astimezone().isoformat(),
+                "deviceID": mac_id,
+                "stop": False,
+                "impedance": data_int,
+            }
+            # add the received impedance data to the queue
+            if not data_queue.full():
+                await data_queue.put(package)
+            else:
+                await data_queue.get()
+
+        async def send_start_commands_recording():
+            """Send start commands to the device."""
+            logging_sending_start(self.debug)
+
+            # ------------------ Configuration ------------------
+            if led_sleep:
+                await asyncio.sleep(self.ble_delay)
+                await self.client.write_gatt_char(
+                    self.cfg_id, utf_8_encode(self.led_off_cfg)[0]
+                )
+            # ------------------ Subscribe to notifications ------------------
+            # Notify the client that these two services are required
+            logging_subscribing_eeg_notification(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            await self.client.start_notify(self.meas_eeg_id, data_handler)
+
+            logging_subscribing_battery_notification(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            await self.client.start_notify(self.battery_id, battery_handler)
+
+            # ------------------ Start commands ------------------
+            # sleep so that cleint can respond
+            await asyncio.sleep(self.ble_delay)
+            # send start command for recording data
+            await self.client.write_gatt_char(
+                self.command_id, utf_8_encode(self.start_cmd)[0]
+            )
+
+        async def send_start_commands_impedance():
+            # ----------------- Configuration -----------------
+            if mains_freq_60hz:
+                await asyncio.sleep(self.ble_delay)
+                await self.client.write_gatt_char(
+                    self.cfg_id, utf_8_encode(self.notch_freq_60_cfg)[0]
+                )
+            else:
+                await asyncio.sleep(self.ble_delay)
+                await self.client.write_gatt_char(
+                    self.cfg_id, utf_8_encode(self.notch_freq_50_cfg)[0]
+                )
+
+            # ----------------- Subscribe -----------------
+            logging_subscribing_impedance_notification(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            await self.client.start_notify(self.meas_imp_id, impedance_handler)
+
+            # ----------------- Send start command -----------------
+            logging_starting_impedance_measurement_commands(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            await self.client.write_gatt_char(
+                self.command_id, utf_8_encode(self.start_imp_cmd)[0]
+            )
+
+        async def stop_impedance_timeout():
+            """Stop recording gracefully."""
+            # make sure the last data is now a stop command
+            package = {
+                "timestamp": datetime.datetime.now().astimezone().isoformat(),
+                "deviceID": mac_id,
+                "stop": True,
+            }
+            # ------------------ Load final stop package ------------------
+            if not data_queue.full():
+                await data_queue.put(package)
+            else:
+                await data_queue.get()
+                await data_queue.put(package)
+            logging_sending_stop(self.debug)
+            # ------------------ API should send already loaded package  ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # This gives time for the api to send already loaded data
+            logging_sending_stop_device(self.debug)
+            await asyncio.sleep(self.ble_delay)
+
+            await self.client.write_gatt_char(
+                self.command_id, utf_8_encode(self.stop_imp_cmd)[0]
+            )
+
+            # ------------------ Disconnect command to device ------------------
+            logging_sending_disconnect(self.debug)
+            await asyncio.sleep(self.ble_stop_delay)
+            await self.client.disconnect()
+            await asyncio.sleep(self.ble_stop_delay)
+
+            if self.write_to_file:
+                self.data_recording_logfile.close()
+            logging_recording_successfully_stopped(self.debug)
+
+        async def stop_recording_timeout():
+            """Stop recording gracefully."""
+
+            # make sure the last data is now a stop command
+            package = {
+                "timestamp": datetime.datetime.now().astimezone().isoformat(),
+                "deviceID": mac_id,
+                "data": "STOP_TIMEOUT",
+                "stop": True,
+            }
+            # ------------------ Load final stop package ------------------
+            if not data_queue.full():
+                await data_queue.put(package)
+            else:
+                await data_queue.get()
+                await data_queue.put(package)
+            logging_sending_stop(self.debug)
+            # ------------------ API should send already loaded package  ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # This gives time for the api to send already loaded data
+            logging_sending_stop_device(self.debug)
+            await asyncio.sleep(self.ble_delay)
+
+            await self.client.write_gatt_char(
+                self.command_id, utf_8_encode(self.stop_cmd)[0]
+            )
+
+            if led_sleep:
+                logging_turn_ble_on(self.debug)
+                await asyncio.sleep(self.ble_delay)
+                await self.client.write_gatt_char(
+                    self.cfg_id, utf_8_encode(self.led_on_cfg)[0]
+                )
+            # ------------------ Disconnect command to device ------------------
+            logging_sending_disconnect(self.debug)
+            await asyncio.sleep(self.ble_stop_delay)
+            await self.client.disconnect()
+            await asyncio.sleep(self.ble_stop_delay)
+
+            if self.write_to_file:
+                self.data_recording_logfile.close()
+            logging_recording_successfully_stopped(self.debug)
+
+        async def stop_impedance_cancelled_script():
+            """Stop recording abruptly."""
+            logging_keyboard_interrupt(self.debug)
+
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # Give API time to send last package
+            # With its own interupt handling
+            # ------------------ Send stop EEG recording command ------------------
+            logging_sending_stop_device(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            try:
+                await self.client.write_gatt_char(
+                    self.command_id, utf_8_encode(self.stop_imp_cmd)[0]
+                )
+            except Exception:
+                log_device_not_connected_cannot_stop(self.debug)
+
+            # ------------------ Disconnecting commands ------------------
+            logging_sending_disconnect(self.debug)
+            await asyncio.sleep(self.ble_stop_delay)
+
+            await self.client.disconnect()
+
+            log_exception_in_disconnecting(self.debug)
+            await asyncio.sleep(self.ble_stop_delay)
+            # ------------------ Closing file  ------------------
+            if self.write_to_file:
+                self.data_recording_logfile.close()
+            logging_recording_successfully_stopped(self.debug)
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # Give API time to send last package
+            # With its own interupt handling
+
+        async def stop_recording_cancelled_script():
+            """Stop recording abruptly."""
+            logging_keyboard_interrupt(self.debug)
+
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # Give API time to send last package
+            # With its own interupt handling
+            # ------------------ Send stop EEG recording command ------------------
+            logging_sending_stop_device(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            try:
+                await self.client.write_gatt_char(
+                    self.command_id, utf_8_encode(self.stop_cmd)[0]
+                )
+            except Exception:
+                log_device_not_connected_cannot_stop(self.debug)
+
+            # ------------------ Configuring LED back on ------------------
+            if led_sleep:
+                logging_turn_led_on(self.debug)
+                await asyncio.sleep(self.ble_delay)
+                await self.client.write_gatt_char(
+                    self.cfg_id, utf_8_encode(self.led_on_cfg)[0]
+                )
+            # ------------------ Disconnecting commands ------------------
+            logging_sending_disconnect(self.debug)
+            await asyncio.sleep(self.ble_stop_delay)
+
+            await self.client.disconnect()
+
+            await asyncio.sleep(self.ble_stop_delay)
+            # ------------------ Closing file  ------------------
+            if self.write_to_file:
+                self.data_recording_logfile.close()
+            logging_recording_successfully_stopped(self.debug)
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # Give API time to send last package
+            # With its own interupt handling
+
+        async def stop_recording_device_lost():
+            """Stop recording device lost."""
+            logging_device_lost_give_up(self.debug)
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(self.ble_delay)  # Give API time to send last package
+            # ------------------ Loading last package ------------------
+            logging_sending_stop(self.debug)
+            package = {
+                "timestamp": datetime.datetime.now().astimezone().isoformat(),
+                "deviceID": mac_id,
+                "data": "STOP_DEVICE_LOST",
+                "stop": True,
+            }
+            # pack the stop command
+            if not data_queue.full():
+                await data_queue.put(package)
+            else:
+                await data_queue.get()
+                await data_queue.put(package)
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # Give API time to send last package
+            # ------------------ Closing file ------------------
+            if self.write_to_file:
+                self.data_recording_logfile.close()
+
+            return True
+
+        async def bluetooth_reconnect():
+            """Set flags to reconnect to bluetooth device."""
+            self.try_to_connect_timeout = self.try_to_connect_timeout - 1
+            if self.try_to_connect_timeout <= 0:
+                self.device_lost = await stop_recording_device_lost()
+            logging_trying_to_connect_again(self.debug, self.try_to_connect_timeout)
+            self.connection_established = False
+            self.initialise_connection = True
+
+        def initialise_file():
+            """Initialise file for recording."""
+            if self.write_to_file:
+                if not os.path.exists("./logs"):
+                    os.makedirs("logs")
+
+                if not impedance_measurement:
+                    measurement_type = "rec"
+                else:
+                    measurement_type = "imp"
+
+                datestr = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
+                recording_filename = f"./logs/IGEB-{measurement_type}-{datestr}.txt"
+                self.data_recording_logfile = open(
+                    recording_filename, "w", encoding="utf-8"
+                )
+
+        def initialise_timestamps():
+            if self.initial_time:
+                self.initial_time = False  # record that this is the initial time
+                self.original_time = time.time()
+
+        async def main_loop():
+            while True:
+                if self.connection_established:
+                    await asyncio.shield(
+                        asyncio.sleep(self.ble_delay)
+                    )  # sleep so that everything can happen
+                    self.remaining_time = record_time - (
+                        time.time() - self.original_time
+                    )
+                    print(f"Time left: {round(self.remaining_time)}s")
+
+                    if self.remaining_time <= 0:
+                        logging_time_reached(self.debug, self.original_time)
+                        if not impedance_measurement:
+                            await stop_recording_timeout()
+                        else:
+                            await stop_impedance_timeout()
+                        break
+
+                else:
+                    break
+
+        # >>>>>>>>>>>>>>>>>>>>> Start of recording process <<<<<<<<<<<<<<<<<<<<<<<<
+        # ------------------ Initialise values for timestamps ------------------
+        self.prev_timestamp = 0
+        self.prev_index = -1
+        # ------------------ Initialise time values for recording timeout ------------------
+        # This has been decoupled from the device timing for robustness
+        self.original_time = time.time()
+        self.initial_time = True
+        self.time_left = True
+        self.initial_time = True
+        # ------------------ Initialise connection values for trying to connect again ------------------
+        # self.connection_established = False
+        self.try_to_connect_timeout = self.reconnect_try_amount
+        # ------------------ Initialise log file ------------------
+        initialise_file()
+
+        while not self.teminating_ble_process:
+            print("connection:", self.connection_established)
+            print("initialize:", self.initialise_connection)
+            try:
+                if self.initialise_connection:
+                    while self.initialise_connection == True:
+                        await self.connect_to_device()
+                if self.client is not None:
+                    if self.client.is_connected:
+                        logging_device_connected_general(self.debug)
+
+                    if not impedance_measurement:
+                        await send_start_commands_recording()
+                    else:
+                        await send_start_commands_impedance()
+
+                    logging_recording_started(self.debug)
+                    self.try_to_connect_timeout = (
+                        self.reconnect_try_amount
+                    )  # reset counter
+                    # >>>>>>>>>>>>>>>>>>>>> Main loop <<<<<<<<<<<<<<<<<<<<<<<<
+                    initialise_timestamps()
+                    await asyncio.shield(main_loop())
+                    # >>>>>>>>>>>>>>>>>>>>> Main loop <<<<<<<<<<<<<<<<<<<<<<<<
+
+                if self.remaining_time <= 0:
+                    self.teminating_ble_process = True
+                    break
+
+                if not self.connection_established:
+                    logging_disconnected_recognised(self.debug)
+                    await bluetooth_reconnect()
+                    if self.device_lost:
+                        break
+
+            except asyncio.CancelledError:
+                if not impedance_measurement:
+                    await stop_recording_cancelled_script()
+                else:
+                    await stop_impedance_cancelled_script()
+                self.teminating_ble_process = True
+                self.connection_established = False
+                self.initialise_connection = False
+                break
+
+            except Exception as error:
+                logging_ble_client_lost(self.debug, error)
+
+            finally:
+                logging_ensuring_ble_disconnected(self.debug)
+                await asyncio.sleep(self.ble_stop_delay)
+                if self.client is not None:
+                    if self.client.is_connected:
+                        try:
+                            print("Stop notification")
+                            await self.client.stop_notify(self.meas_eeg_id)
+                            await asyncio.sleep(self.ble_delay)
+                            await self.client.stop_notify(self.battery_id)
+                            await asyncio.sleep(self.ble_delay)
+                            await self.client.disconnect()
+                            gc.collect()
+                        except Exception:
+                            log_exception_in_disconnecting(self.debug)
+
+                await asyncio.sleep(self.ble_stop_delay)
+                self.connection_established = False
+
+        logging_ble_complete(self.debug)
+
+    async def get_service_and_char(self) -> None:
+        """Get the services and characteristics of the device."""
+        try:
+            async with BleakClient(self.address) as client:
+                logging_device_connected_general(self.debug)
+
+                for service in client.services:
+                    logging_device_info_uuid(self.debug, service)
+
+                    for char in service.characteristics:
+                        if "read" in char.properties:
+                            try:
+                                value = bytes(await client.read_gatt_char(char.uuid))
+                            except exc.BleakError as err:
+                                value = str(err).encode()
+                        else:
+                            value = None
+                        logging_device_info_characteristic(self.debug, char, value)
+
+                await asyncio.sleep(self.ble_stop_delay)
+                await client.disconnect()
+                await asyncio.sleep(self.ble_stop_delay)
+                logging_sending_disconnect(self.debug)
+
+        except exc.BleakError as err:
+            logging_device_connection_failed(self.debug, err)
+
+    async def read_battery_level(self) -> None:
+        """Read the battery level of the device given pre-defined interval."""
+        logging_reading_battery_level(self.debug)
+        while True:
+            try:
+                async with BleakClient(self.address) as client:
+                    logging_device_connected_general(self.debug)
+
+                    await asyncio.sleep(self.ble_delay)
+                    value = int.from_bytes(
+                        (await client.read_gatt_char(self.battery_id)),
+                        byteorder="little",
+                    )
+                    print("-----------------------------")
+                    print(f"\nBattery level: {value}%\n")
+                    print("-----------------------------")
+                    logging_batterylevel_int(self.debug, value)
+
+                    await asyncio.sleep(self.ble_stop_delay)
+                    await client.disconnect()
+                    await asyncio.sleep(self.ble_stop_delay)
+                    logging_sending_disconnect(self.debug)
+                    break
+
+            except exc.BleakError as err:
+                # log the error
+                logging_device_connection_failed(self.debug, err)
+                await asyncio.sleep(3)
+                continue
+
+    async def get_device_information(self) -> dict:
+        """Read the device information of the device."""
+
+        device_info = {}
+
+        async with BleakClient(self.address) as client:
+            logging_device_connected_general(self.debug)
+
+            for service in client.services:
+                if service.uuid == self.device_service:
+                    for char in service.characteristics:
+                        if "read" in char.properties:
+                            try:
+                                value = bytes(await client.read_gatt_char(char.uuid))
+                            except exc.BleakError as err:
+                                value = str(err).encode()
+                        else:
+                            value = None
+
+                        print(f"{ char.description}:{str(value)}")
+                        device_info[char.description] = str(value)
+                        logging_device_description_list(self.debug, char, value)
+
+        return device_info
```

### Comparing `idun_guardian_client-1.1.5/src/idun_guardian_client/test_producer_consumer.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/test_producer_consumer.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import asyncio, random
-
-
-async def rnd_sleep(t):
-    # sleep for T seconds on average
-    await asyncio.sleep(t * random.random() * 2)
-
-
-async def producer(queue):
-    while True:
-        # produce a token and send it to a consumer
-        token = random.random()
-        print(f"produced {token}")
-        if token < 0.05:
-            break
-        await queue.put(token)
-        await rnd_sleep(0.1)
-
-
-async def consumer(queue):
-    while True:
-        token = await queue.get()
-        # process the token received from a producer
-        await rnd_sleep(0.3)
-        queue.task_done()
-        print(f"consumed {token}")
-
-
-async def main():
-    queue = asyncio.Queue()
-
-    # fire up the both producers and consumers
-    producers = [asyncio.create_task(producer(queue)) for _ in range(3)]
-    consumers = [asyncio.create_task(consumer(queue)) for _ in range(10)]
-
-    # with both producers and consumers running, wait for
-    # the producers to finish
-    await asyncio.gather(*producers)
-    print("---- done producing")
-
-    # wait for the remaining tasks to be processed
-    await queue.join()
-
-    # cancel the consumers, which are now idle
-    for c in consumers:
-        c.cancel()
-
-
-asyncio.run(main())
+import asyncio, random
+
+
+async def rnd_sleep(t):
+    # sleep for T seconds on average
+    await asyncio.sleep(t * random.random() * 2)
+
+
+async def producer(queue):
+    while True:
+        # produce a token and send it to a consumer
+        token = random.random()
+        print(f"produced {token}")
+        if token < 0.05:
+            break
+        await queue.put(token)
+        await rnd_sleep(0.1)
+
+
+async def consumer(queue):
+    while True:
+        token = await queue.get()
+        # process the token received from a producer
+        await rnd_sleep(0.3)
+        queue.task_done()
+        print(f"consumed {token}")
+
+
+async def main():
+    queue = asyncio.Queue()
+
+    # fire up the both producers and consumers
+    producers = [asyncio.create_task(producer(queue)) for _ in range(3)]
+    consumers = [asyncio.create_task(consumer(queue)) for _ in range(10)]
+
+    # with both producers and consumers running, wait for
+    # the producers to finish
+    await asyncio.gather(*producers)
+    print("---- done producing")
+
+    # wait for the remaining tasks to be processed
+    await queue.join()
+
+    # cancel the consumers, which are now idle
+    for c in consumers:
+        c.cancel()
+
+
+asyncio.run(main())
```

### Comparing `idun_guardian_client-1.1.5/PKG-INFO` & `idun_guardian_client-1.1b17/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 Metadata-Version: 2.1
-Name: idun-guardian-client
-Version: 1.1.5
+Name: idun_guardian_client
+Version: 1.1b17
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
-Author: IDUN Technologies
-Author-email: contact@iduntechnologies.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
+Author-email: IDUN Technologies <contact@iduntechnologies.com>
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: Other/Proprietary License
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asyncio (>=3.4)
-Requires-Dist: bleak (==0.20.1)
-Requires-Dist: idun-data-models (==0.2)
-Requires-Dist: numpy (>=1.23)
-Requires-Dist: pycryptodome (>=3.15)
-Requires-Dist: pydantic (>=1.10)
-Requires-Dist: python-dotenv (==0.21.*)
-Requires-Dist: requests (>=2.28)
-Requires-Dist: websockets (>=10.3)
+Classifier: Natural Language :: English
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # User guide and documentation
 
 ## What can you do with the Python SDK?
 
 1. You can use the Python SDK to search for the device.
@@ -269,8 +262,7 @@
 # download recording
 api.download_recording_by_id(
     device_id = "XX-XX-XX-XX-XX-XX",
     recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx"
 )
 # The info about th recording can be found in the log file
 ```
-
```

