# Comparing `tmp/spai-2023.5.30.post3.tar.gz` & `tmp/spai-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2023.5.30.post3.tar", max compression
+gzip compressed data, was "spai-2023.7.4.tar", max compression
```

## Comparing `spai-2023.5.30.post3.tar` & `spai-2023.7.4.tar`

### file list

```diff
@@ -1,45 +1,64 @@
--rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.30.post3/README.md
--rw-r--r--   0        0        0      380 2023-05-30 17:28:06.654999 spai-2023.5.30.post3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.30.post3/spai/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:47:16.135084 spai-2023.5.30.post3/spai/cli/__init__.py
--rw-r--r--   0        0        0     3997 2023-05-30 17:07:38.527006 spai-2023.5.30.post3/spai/cli/cloud.py
--rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.30.post3/spai/cli/commands/__init__.py
--rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.30.post3/spai/cli/commands/hello.py
--rw-r--r--   0        0        0     3192 2023-05-30 14:36:50.431336 spai-2023.5.30.post3/spai/cli/local.py
--rw-r--r--   0        0        0     5617 2023-05-26 12:00:02.150333 spai-2023.5.30.post3/spai/cli/project-template/README.md
--rw-r--r--   0        0        0      648 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0     1570 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0   780104 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0   783403 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/notebooks/analytics/output.ipynb
--rw-r--r--   0        0        0       54 2023-05-26 11:59:24.882199 spai-2023.5.30.post3/spai/cli/project-template/scripts/downloader/.env.example
--rw-r--r--   0        0        0     1198 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0      524 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/scripts/ndvi/main.py
--rw-r--r--   0        0        0      529 2023-05-26 12:01:08.490568 spai-2023.5.30.post3/spai/cli/project-template/spai.config.yml
--rw-r--r--   0        0        0     1421 2023-05-26 11:56:34.225566 spai-2023.5.30.post3/spai/cli/project-template/uis/map/main.py
--rw-r--r--   0        0        0     3692 2023-05-30 17:01:01.845727 spai-2023.5.30.post3/spai/cli/validate.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.30.post3/spai/data/__init__.py
--rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.30.post3/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.30.post3/spai/data/satellite/download.py
--rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.30.post3/spai/data/satellite/explore.py
--rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.5.30.post3/spai/image/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.30.post3/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.5.30.post3/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.5.30.post3/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.5.30.post3/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.5.30.post3/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.5.30.post3/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0     3065 2023-05-30 16:44:50.254663 spai-2023.5.30.post3/spai/main.py
--rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.5.30.post3/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.5.30.post3/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     2537 2023-05-30 10:26:02.759827 spai-2023.5.30.post3/spai/storage/Storage.py
--rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.30.post3/spai/storage/__init__.py
--rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.30.post3/spai/storage/minio.py
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 spai-2023.5.30.post3/setup.py
--rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 spai-2023.5.30.post3/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2023.7.4/README.md
+-rw-r--r--   0        0        0      378 2023-07-04 15:45:54.547735 spai-2023.7.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.7.4/spai/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:26:06.805927 spai-2023.7.4/spai/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.7.4/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      950 2023-06-09 08:58:19.195513 spai-2023.7.4/spai/cli/commands/auth.py
+-rw-r--r--   0        0        0        0 2023-06-09 08:55:40.482622 spai-2023.7.4/spai/cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-09 08:55:40.490621 spai-2023.7.4/spai/cli/src/errors/auth.py
+-rw-r--r--   0        0        0     2479 2023-06-12 10:28:14.981273 spai-2023.7.4/spai/cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      985 2023-06-09 08:57:32.155257 spai-2023.7.4/spai/cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       60 2023-06-09 08:57:23.015206 spai-2023.7.4/spai/cli/src/repos/__init__.py
+-rw-r--r--   0        0        0     1587 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-09 08:57:34.415269 spai-2023.7.4/spai/cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      466 2023-06-09 11:53:22.345855 spai-2023.7.4/spai/cli/src/usecases/project/GetLogs.py
+-rw-r--r--   0        0        0      669 2023-07-04 12:57:35.512652 spai-2023.7.4/spai/cli/src/usecases/project/GetServices.py
+-rw-r--r--   0        0        0      482 2023-06-09 11:33:56.178515 spai-2023.7.4/spai/cli/src/usecases/project/RunService.py
+-rw-r--r--   0        0        0      492 2023-06-09 11:53:19.529847 spai-2023.7.4/spai/cli/src/usecases/project/ScheduleService.py
+-rw-r--r--   0        0        0      510 2023-06-09 11:19:01.311705 spai-2023.7.4/spai/cli/src/usecases/project/StopService.py
+-rw-r--r--   0        0        0      125 2023-06-09 11:48:45.469043 spai-2023.7.4/spai/cli/src/usecases/project/__init__.py
+-rw-r--r--   0        0        0      391 2023-06-09 11:06:06.948997 spai-2023.7.4/spai/cli/src/usecases/project/init_project.py
+-rw-r--r--   0        0        0     1350 2023-06-09 11:53:23.257858 spai-2023.7.4/spai/cli/src/usecases/project/main.py
+-rw-r--r--   0        0        0     5617 2023-05-26 12:00:02.150333 spai-2023.7.4/spai/cli/src/usecases/project/project-template/README.md
+-rw-r--r--   0        0        0      648 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0     1570 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0   780104 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0   783403 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb
+-rw-r--r--   0        0        0       54 2023-05-26 11:59:24.882199 spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/downloader/.env.example
+-rw-r--r--   0        0        0     1198 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0      524 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py
+-rw-r--r--   0        0        0      529 2023-05-26 12:01:08.490568 spai-2023.7.4/spai/cli/src/usecases/project/project-template/spai.config.yml
+-rw-r--r--   0        0        0     1421 2023-05-26 11:56:34.225566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/uis/map/main.py
+-rw-r--r--   0        0        0      108 2023-06-09 10:28:57.166050 spai-2023.7.4/spai/cli/src/usecases/run/__init__.py
+-rw-r--r--   0        0        0     3591 2023-06-09 12:16:07.390164 spai-2023.7.4/spai/cli/src/usecases/run/cloud.py
+-rw-r--r--   0        0        0     3143 2023-06-09 10:29:07.730004 spai-2023.7.4/spai/cli/src/usecases/run/local.py
+-rw-r--r--   0        0        0     3698 2023-07-04 10:07:01.300284 spai-2023.7.4/spai/cli/src/usecases/run/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.7.4/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.7.4/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.7.4/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.7.4/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.7.4/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.7.4/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.7.4/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.7.4/spai/image/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.7.4/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.7.4/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.7.4/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.7.4/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.7.4/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.7.4/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0     2298 2023-07-04 14:28:43.830331 spai-2023.7.4/spai/main.py
+-rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.7.4/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.7.4/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     2537 2023-05-30 10:26:02.759827 spai-2023.7.4/spai/storage/Storage.py
+-rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.7.4/spai/storage/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.7.4/spai/storage/minio.py
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 spai-2023.7.4/setup.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 spai-2023.7.4/PKG-INFO
```

### Comparing `spai-2023.5.30.post3/spai/cli/local.py` & `spai-2023.7.4/spai/cli/src/usecases/run/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import os
-from dotenv import load_dotenv
-import subprocess
 import schedule
 import time
 from multiprocessing import Process
 
 
 def run_item(item, command):
     if item.command:
```

### Comparing `spai-2023.5.30.post3/spai/cli/project-template/README.md` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/cli/project-template/apis/analytics/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/cli/project-template/apis/xyz/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/xyz/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/cli/project-template/notebooks/analytics/main.ipynb` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/cli/project-template/notebooks/analytics/output.ipynb` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/cli/project-template/scripts/downloader/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/cli/project-template/scripts/ndvi/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/cli/project-template/spai.config.yml` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/spai.config.yml`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/cli/project-template/uis/map/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/uis/map/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/cli/validate.py` & `spai-2023.7.4/spai/cli/src/usecases/run/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         )
     # check folder has file
     if not file in os.listdir(dir / folder / item.name):
         raise typer.BadParameter(f"{name} '{item.name}' is missing file 'main.py'.")
     # TODO: check optionals: reqs, env...
 
 
-def load_and_validate_config(dir, typer, cloud):
+def load_and_validate_config(dir, typer, cloud=False):
     # check dir exists
     if not dir.exists():
         raise typer.BadParameter(f"Directory '{dir}' does not exist.")
     # check dir is a spai project
     if not "spai.config.yml" in os.listdir(dir):
         raise typer.BadParameter(
             f"Directory '{dir}' is not a spai project. No spai.config.yml file found."
```

### Comparing `spai-2023.5.30.post3/spai/data/satellite/download.py` & `spai-2023.7.4/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/data/satellite/explore.py` & `spai-2023.7.4/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/image/utils.py` & `spai-2023.7.4/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/image/xyz/cache.py` & `spai-2023.7.4/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/image/xyz/errors.py` & `spai-2023.7.4/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/image/xyz/get_image_tile.py` & `spai-2023.7.4/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/image/xyz/image_utils.py` & `spai-2023.7.4/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/storage/BaseStorage.py` & `spai-2023.7.4/spai/storage/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/storage/CloudStorage.py` & `spai-2023.7.4/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/storage/Storage.py` & `spai-2023.7.4/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/spai/storage/minio.py` & `spai-2023.7.4/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post3/setup.py` & `spai-2023.7.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['spai',
  'spai.cli',
  'spai.cli.commands',
- 'spai.cli.project-template.apis.analytics',
- 'spai.cli.project-template.apis.xyz',
- 'spai.cli.project-template.scripts.downloader',
- 'spai.cli.project-template.scripts.ndvi',
- 'spai.cli.project-template.uis.map',
+ 'spai.cli.src.errors',
+ 'spai.cli.src.repos',
+ 'spai.cli.src.usecases.auth',
+ 'spai.cli.src.usecases.project',
+ 'spai.cli.src.usecases.project.project-template.apis.analytics',
+ 'spai.cli.src.usecases.project.project-template.apis.xyz',
+ 'spai.cli.src.usecases.project.project-template.scripts.downloader',
+ 'spai.cli.src.usecases.project.project-template.scripts.ndvi',
+ 'spai.cli.src.usecases.project.project-template.uis.map',
+ 'spai.cli.src.usecases.run',
  'spai.data',
  'spai.data.satellite',
  'spai.data.satellite.sentinelhub',
  'spai.image',
  'spai.image.xyz',
  'spai.storage']
 
 package_data = \
 {'': ['*'],
- 'spai.cli': ['project-template/*', 'project-template/notebooks/analytics/*']}
+ 'spai.cli.src.usecases.project': ['project-template/*',
+                                   'project-template/notebooks/analytics/*']}
 
 install_requires = \
 ['minio>=7.1.15,<8.0.0', 'pandas>=2.0.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['spai = spai.main:app']}
 
 setup_kwargs = {
     'name': 'spai',
-    'version': '2023.5.30.post3',
+    'version': '2023.7.4',
     'description': '',
-    'long_description': '',
+    'long_description': '# SPAI CLI\n\n## Create new project\n\n```bash\nspai init\n```\n',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

