# Comparing `tmp/uasset_dump-0.0.6.tar.gz` & `tmp/uasset_dump-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uasset_dump-0.0.6.tar", max compression
+gzip compressed data, was "uasset_dump-0.0.7.tar", max compression
```

## Comparing `uasset_dump-0.0.6.tar` & `uasset_dump-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      306 2023-07-03 10:31:07.319944 uasset_dump-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 uasset_dump-0.0.6/LICENSE.md
--rw-r--r--   0        0        0     3959 2023-07-03 08:35:15.010465 uasset_dump-0.0.6/README.md
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.6/bootloader/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.6/bootloader/ue/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.6/bootloader/ue/cli/__init__.py
--rwxr-xr-x   0        0        0     2612 2023-07-03 10:30:58.186203 uasset_dump-0.0.6/bootloader/ue/cli/uassetdump.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.6/bootloader/ue/constant/__init__.py
--rw-r--r--   0        0        0     4797 2023-04-05 15:31:25.693554 uasset_dump-0.0.6/bootloader/ue/constant/uasset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.6/bootloader/ue/model/__init__.py
--rw-r--r--   0        0        0     2914 2023-06-14 02:27:45.682247 uasset_dump-0.0.6/bootloader/ue/model/uasset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.6/bootloader/ue/utils/__init__.py
--rw-r--r--   0        0        0     5492 2023-07-03 10:30:58.180530 uasset_dump-0.0.6/bootloader/ue/utils/uasset_dump.py
--rw-r--r--   0        0        0     1024 2023-07-03 10:31:07.323386 uasset_dump-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 uasset_dump-0.0.6/setup.py
--rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 uasset_dump-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      393 2023-07-04 08:39:55.405156 uasset_dump-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 uasset_dump-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0     4093 2023-07-04 01:21:15.627422 uasset_dump-0.0.7/README.md
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.7/bootloader/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.7/bootloader/ue/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.7/bootloader/ue/cli/__init__.py
+-rwxr-xr-x   0        0        0     2975 2023-07-04 08:38:03.671218 uasset_dump-0.0.7/bootloader/ue/cli/uassetdump.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.7/bootloader/ue/constant/__init__.py
+-rw-r--r--   0        0        0     4797 2023-04-05 15:31:25.693554 uasset_dump-0.0.7/bootloader/ue/constant/uasset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.7/bootloader/ue/model/__init__.py
+-rw-r--r--   0        0        0     2914 2023-06-14 02:27:45.682247 uasset_dump-0.0.7/bootloader/ue/model/uasset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.7/bootloader/ue/utils/__init__.py
+-rw-r--r--   0        0        0     5492 2023-07-03 10:30:58.180530 uasset_dump-0.0.7/bootloader/ue/utils/uasset_dump.py
+-rw-r--r--   0        0        0     1024 2023-07-04 08:40:04.636745 uasset_dump-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 uasset_dump-0.0.7/setup.py
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 uasset_dump-0.0.7/PKG-INFO
```

### Comparing `uasset_dump-0.0.6/LICENSE.md` & `uasset_dump-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.6/README.md` & `uasset_dump-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ### Poetry
 
 _Unreal Engine Assets Dump_ project used Poetry to declare all its dependencies.  [Poetry](https://python-poetry.org/) is a python dependency management tool to manage dependencies, packages, and libraries in your python project.
 
 We need to create the Python virtual environment using Poetry:
 
 ```shell
-poetry env use /Users/Shared/Epic\ Games/UE_5.1/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3
+poetry env use /Users/Shared/Epic\ Games/UE_5.2/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3
 ```
 
 We can enter this virtual environment and install all the required dependencies:
 
 ```shell
 poetry shell
 poetry update
@@ -103,16 +103,25 @@
   (...)
 ]
 ```
 
 ```shell
 export UNREAL_ENGINE_PROJECT_PATH=/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Scooby.uproject
 
+export UNREAL_ENGINE_ASSET_DUMP_FILE_PATH=/Users/admin/bootloader-scooby-uassets.dump.json
+
 "`find "/Users/Shared/Epic Games/UE_5.2" -name UnrealEditor-Cmd`" \
     "$UNREAL_ENGINE_PROJECT_PATH" \
     -run=pythonscript \
     -stdout \
     -Unattended \
     -script="/Users/admin/Downloads/run.py"
 
 echo $?;
+```
+
+# Command Line Execution
+
+```shell
+
+
 ```
```

### Comparing `uasset_dump-0.0.6/bootloader/__init__.py` & `uasset_dump-0.0.7/bootloader/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.6/bootloader/ue/__init__.py` & `uasset_dump-0.0.7/bootloader/ue/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.6/bootloader/ue/cli/__init__.py` & `uasset_dump-0.0.7/bootloader/ue/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.6/bootloader/ue/cli/uassetdump.py` & `uasset_dump-0.0.7/bootloader/ue/cli/uassetdump.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # SUITABILITY OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT
 # NOT LIMITED TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR
 # A PARTICULAR PURPOSE, OR NON-INFRINGEMENT.  BOOTLOADER SHALL NOT BE
 # LIABLE FOR ANY LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF
 # USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
 
 import argparse
+import logging
 import sys
 from pathlib import Path
 
 from majormode.perseus.constant.logging import LOGGING_LEVEL_LITERAL_STRINGS
 from majormode.perseus.constant.logging import LoggingLevelLiteral
 from majormode.perseus.utils.logging import DEFAULT_LOGGING_FORMATTER
 from majormode.perseus.utils.logging import cast_string_to_logging_level
@@ -59,20 +60,32 @@
         dest='path',
         metavar='PATH',
         required=True,
         type=cast_string_to_path,
         help="specify the path to root folder of the Unreal Engine project' assets"
     )
 
+    parser.add_argument(
+        '--output',
+        dest='output_file',
+        metavar='FILE',
+        required=True,
+        type=cast_string_to_path,
+        help="specify the path and the name of the file in which the JSON dump needs to be written in"
+    )
+
     return parser.parse_args()
 
 
 def run():
     arguments = parse_arguments()
 
     set_up_logger(logging_formatter=DEFAULT_LOGGING_FORMATTER, logging_level=arguments.logging_level)
 
     from timeit import default_timer as timer
     start = timer()
-    print(uasset_dump.dump_assets(arguments.path))
+    json_string = uasset_dump.dump_assets(arguments.path)
     end = timer()
-    sys.stderr.write(f"Asset dump completed in {end - start}s")
+    logging.debug(f"Asset dump completed in {end - start}s")
+
+    with open(arguments.output_file, 'w') as fd:
+        fd.write(json_string)
```

### Comparing `uasset_dump-0.0.6/bootloader/ue/constant/__init__.py` & `uasset_dump-0.0.7/bootloader/ue/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.6/bootloader/ue/constant/uasset.py` & `uasset_dump-0.0.7/bootloader/ue/constant/uasset.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.6/bootloader/ue/model/__init__.py` & `uasset_dump-0.0.7/bootloader/ue/model/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.6/bootloader/ue/model/uasset.py` & `uasset_dump-0.0.7/bootloader/ue/model/uasset.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.6/bootloader/ue/utils/__init__.py` & `uasset_dump-0.0.7/bootloader/ue/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.6/bootloader/ue/utils/uasset_dump.py` & `uasset_dump-0.0.7/bootloader/ue/utils/uasset_dump.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.6/pyproject.toml` & `uasset_dump-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 keywords = ["cli", "tool", "utility", "unreal", "engine", "asset", "inventory", "dump", "json"]
 license = "SEE LICENSE IN <LICENSE.md>"
 name = "uasset-dump"
 packages = [{ include = "bootloader" }]
 readme = "README.md"
 repository = "https://github.com/bootloader-studio/cli-uasset-dump"
-version = "0.0.6"
+version = "0.0.7"
 
 [tool.poetry.dependencies]
 perseus-core-library = "^1.19.3"
 python = "^3.9"
 
 [tool.poetry.scripts]
 ueprjver = 'bootloader.ue.cli.uassetdump:run'
```

### Comparing `uasset_dump-0.0.6/setup.py` & `uasset_dump-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 ['perseus-core-library>=1.19.3,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ueprjver = bootloader.ue.cli.uassetdump:run']}
 
 setup_kwargs = {
     'name': 'uasset-dump',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Command-line Interface (CLI) responsible for returning the list of the assets of an Unreal Engine project into a JSON structure',
-    'long_description': '# Unreal Engine Assets Dump\n\nCommand-line Interface (CLI) responsible for returning the list of the assets of an Unreal Engine project into a JSON structure.\n\n## Development\n\n### Poetry\n\n_Unreal Engine Assets Dump_ project used Poetry to declare all its dependencies.  [Poetry](https://python-poetry.org/) is a python dependency management tool to manage dependencies, packages, and libraries in your python project.\n\nWe need to create the Python virtual environment using Poetry:\n\n```shell\npoetry env use /Users/Shared/Epic\\ Games/UE_5.1/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3\n```\n\nWe can enter this virtual environment and install all the required dependencies:\n\n```shell\npoetry shell\npoetry update\n```\n\n\n## Publication\n\nTo publish a new version of the _Unreal Engine Assets Dump_ library to [Pypi](https://pypi.org/), we need to execute the following command:\n\n```shell\npoetry publish --build --username $PYPI_USERNAME --password $PYPI_PASSWORD\n```\n\nWhere the environment variables:\n\n- `$PYPI_USERNAME`: The value `__token__`\n- `$PYPI_PASSWORD`: The [API token](https://pypi.org/manage/account/token/) used to authenticate when uploading packages to PyPI (e.g., `pypi-...`)\n\nWe generally defined a `.env` file and add these environment variables:\n\n```text\n# Copyright (C) 2023 Bootloader.  All rights reserved.\n#\n# This software is the confidential and proprietary information of\n# Bootloader or one of its subsidiaries.  You shall not disclose this\n# confidential information and shall use it only in accordance with the\n# terms of the license agreement or other applicable agreement you\n# entered into with Bootloader.\n#\n# BOOTLOADER MAKES NO REPRESENTATIONS OR WARRANTIES ABOUT THE\n# SUITABILITY OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT\n# NOT LIMITED TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR\n# A PARTICULAR PURPOSE, OR NON-INFRINGEMENT.  BOOTLOADER SHALL NOT BE\n# LIABLE FOR ANY LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF\n# USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.\n\n# The Python Package Index (PyPI) API token to authenticate when\n# uploading this package to PyPI.\nPYPI_USERNAME=__token__\nPYPI_PASSWORD=pypi-(...)\n```\n\n\n## Installation\n\nTo install _Unreal Engine Assets Dump_ library to Unreal Engine, execute the following command.\n\n```shell\n/Users/Shared/Epic\\ Games/UE_5.1/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3 -m pip install --upgrade uasset-dump\n/Users/Shared/Epic\\ Games/UE_5.2/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3 -m pip install --upgrade uasset-dump\n```\n\n/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Content\n\n## Execution\n\nThen we can load our Unreal Engine project in Unreal Engine Editor and execute the following Python instructions in the Output Log drawer:\n\n```shell\nfrom bootloader.ue.utils import uasset_dump\nuasset_dump.dump_assets(\'/Users/dcaune/Devel/Bootloader/bootloader-human-trainer-ar5/Content\')\n```\n\nThis prints long JSON data.  For instance:\n\n```json\n[\n  {\n    "asset_name": "A_d2_ChangeOutfit_01",\n    "asset_class_path": "/Script/Engine/AnimSequence",\n    "package_name": "/Game/ArtAssets/Pets/QuadrupedDog/Animations/A_d2_ChangeOutfit_01",\n    "dependencies": [\n      "/Game/ArtAssets/Pets/QuadrupedDog/Mesh/S_d2"\n    ]\n  },\n  {\n    "asset_name": "A_d2_ChangeOutfit_02",\n    "asset_class_path": "/Script/Engine/AnimSequence",\n    "package_name": "/Game/ArtAssets/Pets/QuadrupedDog/Animations/A_d2_ChangeOutfit_02",\n    "dependencies": [\n      "/Game/ArtAssets/Pets/QuadrupedDog/Mesh/S_d2"\n    ]\n  },\n  (...)\n]\n```\n\n```shell\nexport UNREAL_ENGINE_PROJECT_PATH=/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Scooby.uproject\n\n"`find "/Users/Shared/Epic Games/UE_5.2" -name UnrealEditor-Cmd`" \\\n    "$UNREAL_ENGINE_PROJECT_PATH" \\\n    -run=pythonscript \\\n    -stdout \\\n    -Unattended \\\n    -script="/Users/admin/Downloads/run.py"\n\necho $?;\n```',
+    'long_description': '# Unreal Engine Assets Dump\n\nCommand-line Interface (CLI) responsible for returning the list of the assets of an Unreal Engine project into a JSON structure.\n\n## Development\n\n### Poetry\n\n_Unreal Engine Assets Dump_ project used Poetry to declare all its dependencies.  [Poetry](https://python-poetry.org/) is a python dependency management tool to manage dependencies, packages, and libraries in your python project.\n\nWe need to create the Python virtual environment using Poetry:\n\n```shell\npoetry env use /Users/Shared/Epic\\ Games/UE_5.2/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3\n```\n\nWe can enter this virtual environment and install all the required dependencies:\n\n```shell\npoetry shell\npoetry update\n```\n\n\n## Publication\n\nTo publish a new version of the _Unreal Engine Assets Dump_ library to [Pypi](https://pypi.org/), we need to execute the following command:\n\n```shell\npoetry publish --build --username $PYPI_USERNAME --password $PYPI_PASSWORD\n```\n\nWhere the environment variables:\n\n- `$PYPI_USERNAME`: The value `__token__`\n- `$PYPI_PASSWORD`: The [API token](https://pypi.org/manage/account/token/) used to authenticate when uploading packages to PyPI (e.g., `pypi-...`)\n\nWe generally defined a `.env` file and add these environment variables:\n\n```text\n# Copyright (C) 2023 Bootloader.  All rights reserved.\n#\n# This software is the confidential and proprietary information of\n# Bootloader or one of its subsidiaries.  You shall not disclose this\n# confidential information and shall use it only in accordance with the\n# terms of the license agreement or other applicable agreement you\n# entered into with Bootloader.\n#\n# BOOTLOADER MAKES NO REPRESENTATIONS OR WARRANTIES ABOUT THE\n# SUITABILITY OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT\n# NOT LIMITED TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR\n# A PARTICULAR PURPOSE, OR NON-INFRINGEMENT.  BOOTLOADER SHALL NOT BE\n# LIABLE FOR ANY LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF\n# USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.\n\n# The Python Package Index (PyPI) API token to authenticate when\n# uploading this package to PyPI.\nPYPI_USERNAME=__token__\nPYPI_PASSWORD=pypi-(...)\n```\n\n\n## Installation\n\nTo install _Unreal Engine Assets Dump_ library to Unreal Engine, execute the following command.\n\n```shell\n/Users/Shared/Epic\\ Games/UE_5.1/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3 -m pip install --upgrade uasset-dump\n/Users/Shared/Epic\\ Games/UE_5.2/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3 -m pip install --upgrade uasset-dump\n```\n\n/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Content\n\n## Execution\n\nThen we can load our Unreal Engine project in Unreal Engine Editor and execute the following Python instructions in the Output Log drawer:\n\n```shell\nfrom bootloader.ue.utils import uasset_dump\nuasset_dump.dump_assets(\'/Users/dcaune/Devel/Bootloader/bootloader-human-trainer-ar5/Content\')\n```\n\nThis prints long JSON data.  For instance:\n\n```json\n[\n  {\n    "asset_name": "A_d2_ChangeOutfit_01",\n    "asset_class_path": "/Script/Engine/AnimSequence",\n    "package_name": "/Game/ArtAssets/Pets/QuadrupedDog/Animations/A_d2_ChangeOutfit_01",\n    "dependencies": [\n      "/Game/ArtAssets/Pets/QuadrupedDog/Mesh/S_d2"\n    ]\n  },\n  {\n    "asset_name": "A_d2_ChangeOutfit_02",\n    "asset_class_path": "/Script/Engine/AnimSequence",\n    "package_name": "/Game/ArtAssets/Pets/QuadrupedDog/Animations/A_d2_ChangeOutfit_02",\n    "dependencies": [\n      "/Game/ArtAssets/Pets/QuadrupedDog/Mesh/S_d2"\n    ]\n  },\n  (...)\n]\n```\n\n```shell\nexport UNREAL_ENGINE_PROJECT_PATH=/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Scooby.uproject\n\nexport UNREAL_ENGINE_ASSET_DUMP_FILE_PATH=/Users/admin/bootloader-scooby-uassets.dump.json\n\n"`find "/Users/Shared/Epic Games/UE_5.2" -name UnrealEditor-Cmd`" \\\n    "$UNREAL_ENGINE_PROJECT_PATH" \\\n    -run=pythonscript \\\n    -stdout \\\n    -Unattended \\\n    -script="/Users/admin/Downloads/run.py"\n\necho $?;\n```\n\n# Command Line Execution\n\n```shell\n\n\n```',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel@bootloader.studio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bootloader-studio/cli-uasset-dump',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `uasset_dump-0.0.6/PKG-INFO` & `uasset_dump-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uasset-dump
-Version: 0.0.6
+Version: 0.0.7
 Summary: Command-line Interface (CLI) responsible for returning the list of the assets of an Unreal Engine project into a JSON structure
 Home-page: https://github.com/bootloader-studio/cli-uasset-dump
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: cli,tool,utility,unreal,engine,asset,inventory,dump,json
 Author: Daniel CAUNE
 Author-email: daniel@bootloader.studio
 Requires-Python: >=3.9,<4.0
@@ -30,15 +30,15 @@
 ### Poetry
 
 _Unreal Engine Assets Dump_ project used Poetry to declare all its dependencies.  [Poetry](https://python-poetry.org/) is a python dependency management tool to manage dependencies, packages, and libraries in your python project.
 
 We need to create the Python virtual environment using Poetry:
 
 ```shell
-poetry env use /Users/Shared/Epic\ Games/UE_5.1/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3
+poetry env use /Users/Shared/Epic\ Games/UE_5.2/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3
 ```
 
 We can enter this virtual environment and install all the required dependencies:
 
 ```shell
 poetry shell
 poetry update
@@ -126,16 +126,25 @@
   (...)
 ]
 ```
 
 ```shell
 export UNREAL_ENGINE_PROJECT_PATH=/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Scooby.uproject
 
+export UNREAL_ENGINE_ASSET_DUMP_FILE_PATH=/Users/admin/bootloader-scooby-uassets.dump.json
+
 "`find "/Users/Shared/Epic Games/UE_5.2" -name UnrealEditor-Cmd`" \
     "$UNREAL_ENGINE_PROJECT_PATH" \
     -run=pythonscript \
     -stdout \
     -Unattended \
     -script="/Users/admin/Downloads/run.py"
 
 echo $?;
 ```
+
+# Command Line Execution
+
+```shell
+
+
+```
```

