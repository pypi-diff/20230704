# Comparing `tmp/bitbucket_pipeline_runner-0.3.7.tar.gz` & `tmp/bitbucket_pipeline_runner-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbucket_pipeline_runner-0.3.7.tar", max compression
+gzip compressed data, was "bitbucket_pipeline_runner-0.3.8.tar", max compression
```

## Comparing `bitbucket_pipeline_runner-0.3.7.tar` & `bitbucket_pipeline_runner-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1070 2023-05-17 21:36:28.964914 bitbucket_pipeline_runner-0.3.7/LICENSE
--rw-r--r--   0        0        0     1046 2023-05-17 21:36:28.964914 bitbucket_pipeline_runner-0.3.7/README.md
--rw-r--r--   0        0        0       29 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/__init__.py
--rw-r--r--   0        0        0       61 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/__main__.py
--rw-r--r--   0        0        0     2943 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/artifacts.py
--rw-r--r--   0        0        0     7691 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/cache.py
--rw-r--r--   0        0        0     4725 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/cli.py
--rw-r--r--   0        0        0     3190 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/config.py
--rw-r--r--   0        0        0    14535 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/container.py
--rw-r--r--   0        0        0     5501 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/context.py
--rw-r--r--   0        0        0    12858 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/models.py
--rw-r--r--   0        0        0      352 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/parse.py
--rw-r--r--   0        0        0     4144 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/repository.py
--rw-r--r--   0        0        0    14318 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/runner.py
--rw-r--r--   0        0        0     8847 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/service.py
--rw-r--r--   0        0        0        0 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/static/__init__.py
--rwxr-xr-x   0        0        0     1521 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/static/dind
--rwxr-xr-x   0        0        0      304 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/static/runit.sh
--rw-r--r--   0        0        0     3388 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/utils.py
--rw-r--r--   0        0        0     2233 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 bitbucket_pipeline_runner-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1046 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/README.md
+-rw-r--r--   0        0        0       29 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/__main__.py
+-rw-r--r--   0        0        0     3049 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/artifacts.py
+-rw-r--r--   0        0        0     7900 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/cache.py
+-rw-r--r--   0        0        0     4929 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/cli.py
+-rw-r--r--   0        0        0     3342 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/config.py
+-rw-r--r--   0        0        0    16688 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/container.py
+-rw-r--r--   0        0        0     5721 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/context.py
+-rw-r--r--   0        0        0    13114 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/models.py
+-rw-r--r--   0        0        0      352 2023-07-04 14:16:54.108568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/parse.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:16:54.112568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/py.typed
+-rw-r--r--   0        0        0     4265 2023-07-04 14:16:54.112568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/repository.py
+-rw-r--r--   0        0        0    15515 2023-07-04 14:16:54.112568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/runner.py
+-rw-r--r--   0        0        0     9198 2023-07-04 14:16:54.112568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/service.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:16:54.112568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/static/__init__.py
+-rw-r--r--   0        0        0     1665 2023-07-04 14:16:54.112568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/static/known_hosts
+-rwxr-xr-x   0        0        0      451 2023-07-04 14:16:54.112568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/static/runit.sh
+-rw-r--r--   0        0        0     4300 2023-07-04 14:16:54.112568 bitbucket_pipeline_runner-0.3.8/pipeline_runner/utils.py
+-rw-r--r--   0        0        0     2653 2023-07-04 14:16:54.112568 bitbucket_pipeline_runner-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 bitbucket_pipeline_runner-0.3.8/PKG-INFO
```

### Comparing `bitbucket_pipeline_runner-0.3.7/LICENSE` & `bitbucket_pipeline_runner-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.3.7/README.md` & `bitbucket_pipeline_runner-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/artifacts.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/artifacts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import io
 import logging
 import os.path
 import tarfile
 from tarfile import TarInfo
 from time import time as ts
-from typing import List
 from uuid import UUID
 
-from . import utils
 from .config import config
 from .container import ContainerRunner
+from .utils import FileStreamer, get_human_readable_size, safe_extract_tar
 
 logger = logging.getLogger(__name__)
 
 
 class ArtifactManager:
     def __init__(self, container: ContainerRunner, artifact_directory: str, step_uuid: UUID):
         self._container = container
         self._artifact_directory = artifact_directory
         self._step_uuid = step_uuid
 
-    def upload(self):
+    def upload(self) -> None:
         logger.info("Loading artifacts")
 
         t = ts()
 
         tar_data = io.BytesIO()
 
         with tarfile.open(fileobj=tar_data, mode="w|") as tar:
@@ -46,15 +45,15 @@
         if not res:
             raise Exception(f"Error loading artifact: {af}")
 
         t = ts() - t
 
         logger.info("Artifacts loaded in %.3fs", t)
 
-    def download(self, artifacts: List[str]):
+    def download(self, artifacts: list[str]) -> None:
         if not artifacts:
             return
 
         artifact_file = f"artifacts-{self._step_uuid}.tar"
         artifact_remote_path = os.path.join(config.build_dir, artifact_file)
         artifact_local_directory = self._artifact_directory
 
@@ -70,21 +69,21 @@
         if not self._container.path_exists(artifact_remote_path):
             logger.info("No artifacts found. Skipping")
             return
 
         data, stats = self._container.get_archive(artifact_remote_path, encode_stream=True)
         logger.debug("artifacts stats: %s", stats)
 
-        # noinspection PyTypeChecker
-        with tarfile.open(fileobj=utils.FileStreamer(data), mode="r|") as wrapper_tar:
+        # FileStreamer only implements `read` which is all that is needed.
+        with tarfile.open(fileobj=FileStreamer(data), mode="r|") as wrapper_tar:  # type: ignore[abstract]
             for entry in wrapper_tar:
                 with tarfile.open(fileobj=wrapper_tar.extractfile(entry), mode="r|") as tar:
-                    tar.extractall(artifact_local_directory)
+                    safe_extract_tar(tar, artifact_local_directory)
 
         t = ts() - t
 
         logger.info(
             "Artifacts saved %s to %s in %.3fs",
-            utils.get_human_readable_size(stats["size"]),
+            get_human_readable_size(stats["size"]),
             artifact_local_directory,
             t,
         )
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/cache.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 import logging
 import os.path
 from tempfile import NamedTemporaryFile
 from time import time as ts
-from typing import Dict, List
+from typing import Optional, Union
 
 from . import utils
 from .config import config
 from .container import ContainerRunner
 
 logger = logging.getLogger(__name__)
 
 DOCKER_IMAGES_ARCHIVE_FILE_NAME = "images.tar"
 
 
 class CacheManager:
-    def __init__(self, container: ContainerRunner, cache_directory: str, cache_definitions: Dict[str, str]):
+    def __init__(self, container: ContainerRunner, cache_directory: str, cache_definitions: dict[str, str]):
         self._container = container
         self._cache_directory = cache_directory
         self._cache_definitions = cache_definitions
 
         self._ignored_caches = {"docker"}
 
-    def upload(self, cache_names: List[str]):
+    def upload(self, cache_names: list[str]) -> None:
         for name in cache_names:
             cu = CacheRestoreFactory.get(self._container, self._cache_directory, self._cache_definitions, name)
             cu.restore()
 
-    def download(self, cache_names: List[str]):
+    def download(self, cache_names: list[str]) -> None:
         for name in cache_names:
             cd = CacheSaveFactory.get(self._container, self._cache_directory, self._cache_definitions, name)
             cd.save()
 
 
 class CacheRestore:
     def __init__(
-        self, container: ContainerRunner, cache_directory: str, cache_definitions: Dict[str, str], cache_name: str
+        self, container: ContainerRunner, cache_directory: str, cache_definitions: dict[str, str], cache_name: str
     ):
         self._container = container
         self._cache_directory = cache_directory
         self._cache_definitions = cache_definitions
         self._cache_name = cache_name
 
-    def restore(self):
+    def restore(self) -> None:
         cache_file = self._get_local_cache_file()
 
         if not cache_file:
             logger.info("Cache '%s': Not found: Skipping", self._cache_name)
             return
 
         self._upload_cache(cache_file)
         self._restore_cache()
 
-    def _get_local_cache_file(self):
+    def _get_local_cache_file(self) -> Optional[str]:
         local_cache_archive_path = get_local_cache_archive_path(self._cache_directory, self._cache_name)
         if not os.path.exists(local_cache_archive_path):
             return None
 
         return local_cache_archive_path
 
-    def _upload_cache(self, cache_file):
+    def _upload_cache(self, cache_file: str) -> None:
         remote_cache_directory = get_remote_temp_directory(self._cache_name)
         remote_cache_parent_directory = os.path.dirname(remote_cache_directory)
 
         cache_archive_size = os.path.getsize(cache_file)
 
         logger.info("Cache '%s': Uploading", self._cache_name)
 
@@ -84,15 +84,15 @@
 
         t = ts() - t
 
         logger.info(
             "Cache '%s': Uploaded %s in %.3fs", self._cache_name, utils.get_human_readable_size(cache_archive_size), t
         )
 
-    def _restore_cache(self):
+    def _restore_cache(self) -> None:
         temp_dir = get_remote_temp_directory(self._cache_name)
         target_dir = sanitize_remote_path(self._cache_definitions[self._cache_name])
 
         logger.info("Cache '%s': Restoring", self._cache_name)
 
         t = ts()
 
@@ -108,41 +108,43 @@
 
         t = ts() - t
 
         logger.info("Cache '%s': Restored in %.3fs", self._cache_name, t)
 
 
 class NullCacheRestore(CacheRestore):
-    def restore(self):
+    def restore(self) -> None:
         logger.info("Cache '%s': Ignoring", self._cache_name)
 
 
 class CacheRestoreFactory:
     @staticmethod
     def get(
-        container: ContainerRunner, cache_directory: str, cache_definitions: Dict[str, str], cache_name: str
+        container: ContainerRunner, cache_directory: str, cache_definitions: dict[str, str], cache_name: str
     ) -> CacheRestore:
+        cls: type[Union[CacheRestore, NullCacheRestore]]
+
         if cache_name == "docker":
             cls = NullCacheRestore
         else:
             cls = CacheRestore
 
         return cls(container, cache_directory, cache_definitions, cache_name)
 
 
 class CacheSave:
     def __init__(
-        self, container: ContainerRunner, cache_directory: str, cache_definitions: Dict[str, str], cache_name: str
+        self, container: ContainerRunner, cache_directory: str, cache_definitions: dict[str, str], cache_name: str
     ):
         self._container = container
         self._cache_directory = cache_directory
         self._cache_definitions = cache_definitions
         self._cache_name = cache_name
 
-    def save(self):
+    def save(self) -> None:
         remote_cache_directory = self._prepare()
 
         local_cache_archive_path = get_local_cache_archive_path(self._cache_directory, self._cache_name)
         self._download(remote_cache_directory, local_cache_archive_path)
 
     def _prepare(self) -> str:
         remote_dir = sanitize_remote_path(self._cache_definitions[self._cache_name])
@@ -160,15 +162,15 @@
 
         t = ts() - t
 
         logger.info("Cache '%s': Prepared in %.3fs", self._cache_name, t)
 
         return target_dir
 
-    def _download(self, src: str, dst: str):
+    def _download(self, src: str, dst: str) -> None:
         if not self._container.path_exists(src):
             logger.info("Cache '%s': Not found", self._cache_name)
             return
 
         logger.info("Cache '%s': Downloading", self._cache_name)
 
         t = ts()
@@ -191,23 +193,25 @@
 
         t = ts() - t
 
         logger.info("Cache '%s': Downloaded %s in %.3fs", self._cache_name, utils.get_human_readable_size(size), t)
 
 
 class NullCacheSave(CacheSave):
-    def save(self):
+    def save(self) -> None:
         logger.info("Cache '%s': Ignoring", self._cache_name)
 
 
 class CacheSaveFactory:
     @staticmethod
     def get(
-        container: ContainerRunner, cache_directory: str, cache_definitions: Dict[str, str], cache_name: str
+        container: ContainerRunner, cache_directory: str, cache_definitions: dict[str, str], cache_name: str
     ) -> CacheSave:
+        cls: type[Union[CacheSave, NullCacheSave]]
+
         if cache_name == "docker":
             cls = NullCacheSave
         else:
             cls = CacheSave
 
         return cls(container, cache_directory, cache_definitions, cache_name)
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/cli.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import logging
 import logging.config
 import os
 import shutil
 import sys
-from typing import List, Optional
+from typing import Optional
 
 import click
 import pkg_resources
-from pyfzf import FzfPrompt
+from pyfzf import FzfPrompt  # type: ignore
 
 from . import utils
 from .config import config
 from .parse import parse_pipeline_file
 from .runner import PipelineRunner, PipelineRunRequest
 
 logger = logging.getLogger(__name__)
 
 
-def _init_logger():
+def _init_logger() -> None:
     logging.config.dictConfig(config.log_config)
 
 
-def _get_pipelines_list(pipeline_file: str) -> List[str]:
+def _get_pipelines_list(pipeline_file: str) -> list[str]:
     pipelines_definition = parse_pipeline_file(pipeline_file)
 
     return pipelines_definition.get_available_pipelines()
 
 
-def _prompt_for_pipeline(pipeline_file) -> Optional[str]:
+def _prompt_for_pipeline(pipeline_file: str) -> Optional[str]:
     pipeline = None
     pipelines = _get_pipelines_list(pipeline_file)
 
     try:
         fzf = FzfPrompt()
         pipeline = next(iter(fzf.prompt(pipelines)), None)
         if not pipeline:
@@ -47,26 +47,26 @@
     "-V",
     "--version",
     "show_version",
     is_flag=True,
     help="Print project version and exit.",
 )
 @click.pass_context
-def main(ctx, show_version):
+def main(ctx: click.Context, show_version: bool) -> None:
     if show_version:
         print(f"Pipeline Runner {pkg_resources.get_distribution('bitbucket_pipeline_runner').version}")
         ctx.exit()
 
     if not ctx.invoked_subcommand:
         print(ctx.get_help())
         ctx.exit(1)
 
 
 @main.command()
-@click.argument("pipeline", default="")
+@click.argument("pipeline", required=False)
 @click.option(
     "-r",
     "--repository-path",
     help="Path to the git repository. Defaults to current directory.",
 )
 @click.option(
     "-s",
@@ -89,15 +89,17 @@
     help="Enable colored output. Default: True",
 )
 @click.option(
     "--cpu-limits/--no-cpu-limits",
     default=False,
     help="Enable to enforce cpu limits for the runner. Default: False",
 )
-def run(pipeline, repository_path, steps, env_files, color, cpu_limits):
+def run(
+    pipeline: Optional[str], repository_path: str, steps: list[str], env_files: list[str], color: bool, cpu_limits: bool
+) -> None:
     """
     Runs the pipeline PIPELINE.
 
     PIPELINE is the full path to the pipeline to run. Ex: branches.master
     """
     config.color = color
     config.cpu_limits = cpu_limits
@@ -129,55 +131,54 @@
 )
 @click.option(
     "-c",
     "--color/--no-color",
     default=True,
     help="Enable colored output",
 )
-def list_(repository_path, color):
+def list_(repository_path: str, color: bool) -> None:
     """
     List the available pipelines.
     """
     config.color = color
 
     _init_logger()
 
     pipelines = _get_pipelines_list(os.path.join(repository_path or ".", "bitbucket-pipelines.yml"))
 
     logger.info("Available pipelines:\n\t%s", "\n\t".join(sorted(pipelines)))
 
 
 @main.command()
-@click.argument("pipeline", default="")
+@click.argument("pipeline", required=False)
 @click.option(
     "-r",
     "--repository-path",
     help="Path to the git repository. Defaults to current directory.",
 )
-def parse(pipeline, repository_path):
+def parse(pipeline: Optional[str], repository_path: str) -> None:
     """
     Parse the pipeline file.
     """
     pipeline_file = os.path.join(repository_path or ".", "bitbucket-pipelines.yml")
 
     pipelines_definition = parse_pipeline_file(pipeline_file)
 
     if pipeline:
         parsed = pipelines_definition.get_pipeline(pipeline)
         if not parsed:
             raise ValueError(f"Invalid pipeline: {pipeline}")
+        print(parsed.json(indent=2))
     else:
-        parsed = pipelines_definition
-
-    print(parsed.json(indent=2))
+        print(pipelines_definition.json(indent=2))
 
 
 @main.command()
 @click.argument("action", type=click.Choice(["clear", "list"]))
-def cache(action):
+def cache(action: str) -> None:
     cache_dir = utils.get_cache_directory()
     if not os.path.isdir(cache_dir):
         return
 
     projects = sorted(os.listdir(cache_dir))
     if action == "list":
         print("Caches:")
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/config.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import getpass
 import logging
 import os
 import posixpath
-from typing import Dict
+from typing import Any
 
 from . import __name__ as __project_name__
 
 
 class Config:
-    def __init__(self):
+    def __init__(self) -> None:
         self.color = True
         self.cpu_limits = False
 
         # TODO: Move some of these things to default definitions or smth
         self.default_image = "atlassian/default-image:latest"
 
         self.default_caches = {
@@ -24,15 +24,18 @@
             "node": "node_modules",
             "pip": "~/.cache/pip",
             "sbt": "~/.sbt",
         }
 
         self.default_services = {
             "docker": {
-                "image": "atlassian/pipelines-docker-daemon:v20-stable",
+                "image": (
+                    "docker-public.packages.atlassian.com/sox/atlassian"
+                    "/bitbucket-pipelines-docker-daemon:v20.10.24-multiarch-prod-stable"
+                ),
                 "memory": 1024,
             }
         }
 
         self.remote_base_dir = "/opt/atlassian"
         self.remote_workspace_dir = os.path.join(self.remote_base_dir, "workspace")
         self.remote_pipeline_dir = os.path.join(self.remote_base_dir, "pipelines", "agent")
@@ -53,15 +56,15 @@
         self.owner_uuid = "e07413cc-dcd9-4c68-aa2e-08e296b1a8af"
 
         self.bitbucket_build_number = os.getenv("BITBUCKET_BUILD_NUMBER", 0)
 
         self.log_level = logging.getLevelName(os.getenv("PIPELINE_LOG_LEVEL", "DEBUG").upper())
 
     @property
-    def log_config(self) -> Dict:
+    def log_config(self) -> dict[str, Any]:
         log_handler_name = "colored" if self.color and "NO_COLOR" not in os.environ else "default"
         return {
             "version": 1,
             "loggers": {
                 __project_name__: {"handlers": [log_handler_name], "level": config.log_level},
                 "docker": {"handlers": ["default"], "level": "INFO"},
             },
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/container.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,38 +2,44 @@
 import io
 import logging
 import os.path
 import posixpath
 import sys
 import tarfile
 import uuid
+from importlib.resources import as_file, files
+from io import BufferedReader
 from logging import Logger
 from time import time
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Generator, Iterable, Iterator, Optional, Sequence, Union, cast
 
 import boto3
-import docker.errors
-from docker.models.containers import Container, ExecResult
+import docker.errors  # type: ignore
+from docker import DockerClient
+from docker.constants import DEFAULT_DATA_CHUNK_SIZE  # type: ignore
+from docker.models.containers import Container, ExecResult  # type: ignore
+
+import pipeline_runner
 
-from . import utils
 from .config import config
 from .models import Image, Pipe
+from .utils import escape_shell_string, stringify, wrap_in_shell
 
 logger = logging.getLogger(__name__)
 
 
 class ContainerRunner:
     def __init__(
         self,
         name: str,
         image: Image,
         network_name: Optional[str],
         repository_path: str,
         data_volume_name: str,
-        env_vars: Dict[str, str],
+        env_vars: dict[str, str],
         output_logger: Logger,
         mem_limit: int = 512,
         ssh_private_key: Optional[str] = None,
     ):
         self._name = name
         self._image = image
         self._network_name = network_name
@@ -43,112 +49,135 @@
         self._logger = output_logger
         self._mem_limit = mem_limit * 2**20  # MiB to B
         self._ssh_private_key = ssh_private_key
 
         self._client = docker.from_env()
         self._container = None
 
-    def start(self):
+    def start(self) -> None:
         self._start_container()
         self._create_pipeline_directories()
-        self._insert_ssh_key_and_config()
+        self._insert_ssh_private_key()
+        self._insert_ssh_known_hosts()
+
+    def install_docker_client_if_needed(self, services: dict[str, Container]) -> None:
+        if not self._container:
+            # TODO: Refactor
+            raise Exception("called on uninitialized container")
 
-    def install_docker_client_if_needed(self, services: Dict[str, Container]):
         if "docker" not in services:
             return
 
         res = self.run_command("command -v docker")
         if res.exit_code == 0:
             logger.debug("`docker` binary is already present in container.")
             return
 
         docker_service = services["docker"]
         archive, _ = docker_service.get_archive("/usr/local/bin/docker")
         self._container.put_archive("/usr/local/bin", archive)
 
-    def stop(self):
+    def stop(self) -> None:
         if not self._container:
             return
 
         logger.info("Removing container: %s", self._container.name)
         self._container.remove(v=True, force=True)
 
     def run_script(
         self,
-        script: List[Union[str, Pipe]],
+        script: Sequence[Union[str, Pipe]],
         user: Optional[Union[int, str]] = None,
-        env: Optional[Dict[str, Any]] = None,
+        env: Optional[dict[str, Any]] = None,
         exec_time: bool = False,
     ) -> int:
         csr = ContainerScriptRunnerFactory.get(self._container, script, self._logger, user, env, exec_time)
 
         return csr.run()
 
     def run_command(
-        self, command: Union[str, List[str]], wrap_in_shell: bool = True, user: Optional[Union[int, str]] = None
+        self, command: Union[str, list[str]], shell: bool = True, user: Optional[Union[int, str]] = None
     ) -> ExecResult:
-        command = utils.stringify(command)
+        if not self._container:
+            # TODO: Refactor
+            raise Exception("called on uninitialized container")
+
+        command = stringify(command)
 
-        if wrap_in_shell:
-            command = utils.wrap_in_shell(command)
+        if shell:
+            command = wrap_in_shell(command)
 
         if user is not None:
             user = str(user)
 
         return self._container.exec_run(command, user=user)
 
-    def path_exists(self, path) -> bool:
+    def path_exists(self, path: str) -> bool:
         ret, _ = self.run_command(f'[ -e "$(realpath "{path}")" ]')
-        return ret == 0
+        return cast(int, ret) == 0
+
+    # TODO: Validate Typing
+    def get_archive(
+        self, path: str, chunk_size: int = DEFAULT_DATA_CHUNK_SIZE, encode_stream: bool = False
+    ) -> tuple[Generator[bytes, None, None], dict[str, Any]]:
+        if not self._container:
+            # TODO: Refactor
+            raise Exception("called on uninitialized container")
+
+        return self._container.get_archive(path, chunk_size, encode_stream)
 
-    def get_archive(self, *args, **kwargs):
-        return self._container.get_archive(*args, **kwargs)
+    # TODO: Validate Typing
+    def put_archive(self, path: str, data: Union[BufferedReader, bytes]) -> bool:
+        if not self._container:
+            # TODO: Refactor
+            raise Exception("called on uninitialized container")
 
-    def put_archive(self, *args, **kwargs):
-        return self._container.put_archive(*args, **kwargs)
+        return self._container.put_archive(path, data)
 
-    def _start_container(self):
+    def _start_container(self) -> None:
         pull_image(self._client, self._image)
 
         logger.info("Creating container: %s", self._name)
 
         if config.cpu_limits:
             opts = {
                 "cpu_period": 100000,
                 "cpu_quota": 400000,
                 "cpu_shares": 4096,
             }
         else:
             opts = {}
 
-        self._container = self._client.containers.run(
+        container = self._client.containers.run(
             self._image.name,
             name=self._name,
             entrypoint="sh",
             user=self._image.run_as_user or 0,
             working_dir=config.build_dir,
             environment=self._environment,
             volumes=self._get_volumes(),
             mem_limit=self._mem_limit,
             network=self._network_name,
             tty=True,
             detach=True,
             **opts,
         )
 
-        logger.debug("Created container: %s", self._container.name)
+        logger.debug("Created container: %s", container.name)
         logger.debug("Image Used: %s", self._image.name)
 
+        self._container = container
+
     def get_container_name(self) -> Optional[str]:
         if not self._container:
             return None
 
         return self._container.name
 
-    def _create_pipeline_directories(self):
+    def _create_pipeline_directories(self) -> None:
         mkdir_cmd = [
             "install",
             "-dD",
             "-o",
             str(self._image.run_as_user or 0),
             config.build_dir,
             config.scripts_dir,
@@ -157,15 +186,31 @@
             config.ssh_key_dir,
         ]
 
         exit_code, output = self.run_command(mkdir_cmd, user=0)
         if exit_code != 0:
             raise Exception(f"Error creating required directories: {output}")
 
-    def _insert_ssh_key_and_config(self):
+    def _insert_ssh_private_key(self) -> None:
+        static_files = files(pipeline_runner).joinpath("static")
+
+        with as_file(static_files.joinpath("known_hosts")) as p:
+            known_hosts = p.read_text()
+
+        cmd = " && ".join(
+            [
+                "install -d -m 700 ~/.ssh",
+                f"echo '{known_hosts}' >> ~/.ssh/known_hosts",
+            ]
+        )
+        exit_code, output = self.run_command(cmd, user=0)
+        if exit_code != 0:
+            raise Exception(f"Error creating root ssh config: {output}")
+
+    def _insert_ssh_known_hosts(self) -> None:
         if not self._ssh_private_key:
             return
 
         private_key_file_path = os.path.join(config.ssh_key_dir, "id_rsa")
 
         cmd = " && ".join(
             [
@@ -175,62 +220,62 @@
                 f'echo "{self._ssh_private_key}" > {private_key_file_path}',
             ]
         )
         exit_code, output = self.run_command(cmd, user=0)
         if exit_code != 0:
             raise Exception(f"Error creating root ssh config: {output}")
 
-    def _get_volumes(self):
+    def _get_volumes(self) -> dict[str, dict[str, str]]:
         return {
             self._repository_path: {"bind": config.remote_workspace_dir, "mode": "ro"},
             self._data_volume_name: {"bind": config.remote_pipeline_dir},
         }
 
 
 class ContainerScriptRunner:
     def __init__(
         self,
         container: Container,
-        script: List[Union[str, Pipe]],
+        script: Sequence[Union[str, Pipe]],
         output_logger: Optional[Logger] = None,
         user: Optional[Union[int, str]] = None,
-        env: Optional[Dict[str, Any]] = None,
+        env: Optional[dict[str, Any]] = None,
     ):
         self._container = container
         self._script = script
         self._logger = output_logger
         self._user = str(user) if user is not None else None
         self._env = env or {}
 
-        if self._logger:
+        if logger_ := self._logger:
 
-            def stdout_print(msg):
-                self._logger.info(msg)
+            def stdout_print(msg: str) -> None:
+                logger_.info(msg)
 
-            def stderr_print(msg):
-                self._logger.error(msg)
+            def stderr_print(msg: str) -> None:
+                logger_.error(msg)
 
         else:
 
-            def stdout_print(msg):
+            def stdout_print(msg: str) -> None:
                 print(msg, end="")
 
-            def stderr_print(msg):
+            def stderr_print(msg: str) -> None:
                 print(msg, end="", file=sys.stderr)
 
         self._stdout_print = stdout_print
         self._stderr_print = stderr_print
 
     def run(self) -> int:
         entrypoint, exit_code_file_path = self._prepare_script_for_remote_execution()
 
         self._execute_script_on_container(entrypoint)
         return self._get_exit_code_of_command(exit_code_file_path)
 
-    def _prepare_script_for_remote_execution(self) -> Tuple[str, str]:
+    def _prepare_script_for_remote_execution(self) -> tuple[str, str]:
         script = self._add_traces_to_script()
         exit_code_file_path = posixpath.join(config.temp_dir, f"exit_code-{uuid.uuid4().hex}")
 
         sh_script_name = f"shell_script-{uuid.uuid4().hex}.sh"
         sh_script_path = posixpath.join(config.scripts_dir, sh_script_name)
         sh_script = self._wrap_script_in_posix_shell(script)
 
@@ -248,22 +293,22 @@
             (wrapper_script_name, wrapper_script),
         )
 
         self._upload_to_container(scripts)
 
         return wrapper_script_path, exit_code_file_path
 
-    def _execute_script_on_container(self, entrypoint):
+    def _execute_script_on_container(self, entrypoint: str) -> None:
         _, output_stream = self._container.exec_run(
             ["/bin/sh", entrypoint], user=self._user, tty=True, stream=True, demux=True, environment=self._env
         )
 
         self._print_execution_log(output_stream)
 
-    def _print_execution_log(self, output_stream):
+    def _print_execution_log(self, output_stream: Iterator[tuple[bytes, bytes]]) -> None:
         for stdout, stderr in output_stream:
             if stdout:
                 self._stdout_print(stdout.decode())
             if stderr:
                 self._stderr_print(stderr.decode())
 
         self._stdout_print("\n")
@@ -278,46 +323,46 @@
         try:
             exit_code = int(str_code)
         except ValueError:
             raise Exception(f"Invalid exit code: {str_code}") from None
         else:
             return exit_code
 
-    def _add_traces_to_script(self):
+    def _add_traces_to_script(self) -> str:
         script_lines = map(self._add_trace_to_script_line, self._script)
 
         return '\nprintf "\\n"\n'.join(line for line in script_lines if line)
 
-    def _add_trace_to_script_line(self, line: Union[str, Pipe]):
+    def _add_trace_to_script_line(self, line: Union[str, Pipe]) -> Optional[str]:
         if isinstance(line, Pipe):
             line = line.as_cmd()
         else:
             line = line.strip()
 
         if not line:
             return None
 
         return f"{self._add_group_separator(line)}\n{line}"
 
     @staticmethod
-    def _add_group_separator(value):
-        value = utils.escape_shell_string(value)
+    def _add_group_separator(value: str) -> str:
+        value = escape_shell_string(value)
 
         return f'printf "\\x1d+ {value}\\n"'
 
     @staticmethod
-    def _wrap_script_in_posix_shell(script):
+    def _wrap_script_in_posix_shell(script: str) -> str:
         return "\n".join(["#! /bin/sh", "set -e", script])
 
     @staticmethod
-    def _wrap_script_in_bash(script):
+    def _wrap_script_in_bash(script: str) -> str:
         return "\n".join(["#! /bin/bash", "set -e", "set +H", script])
 
     @staticmethod
-    def _make_wrapper_script(sh_script_path, bash_script_path, exit_code_file_path):
+    def _make_wrapper_script(sh_script_path: str, bash_script_path: str, exit_code_file_path: str) -> str:
         return "\n".join(
             [
                 "#! /bin/sh",
                 "if [ -f /bin/bash ]; then",
                 f"    /bin/bash -i {bash_script_path}",
                 f"    echo $? > {exit_code_file_path}",
                 "    exit $?",
@@ -325,15 +370,15 @@
                 f"    /bin/sh {sh_script_path}",
                 f"    echo $? > {exit_code_file_path}",
                 "    exit $?",
                 "fi",
             ]
         )
 
-    def _upload_to_container(self, scripts: Iterable[Tuple[str, str]]):
+    def _upload_to_container(self, scripts: Iterable[tuple[str, str]]) -> None:
         tar_data = io.BytesIO()
 
         with tarfile.open(fileobj=tar_data, mode="w|") as tar:
             for name, script in scripts:
                 ti = tarfile.TarInfo(name)
                 script_data = script.encode()
                 ti.size = len(script_data)
@@ -346,67 +391,69 @@
             raise Exception("Error uploading scripts to container")
 
 
 class ContainerScriptRunnerWithExecTime(ContainerScriptRunner):
     def __init__(
         self,
         container: Container,
-        script: List[Union[str, Pipe]],
+        script: Sequence[Union[str, Pipe]],
         output_logger: Optional[Logger] = None,
         user: Optional[Union[int, str]] = None,
-        env: Optional[Dict[str, Any]] = None,
+        env: Optional[dict[str, Any]] = None,
     ):
         super().__init__(container, script, output_logger, user, env)
-        self._timestamp = None
+        self._timestamp: Optional[float] = None
 
-    def _print_execution_log(self, output_stream):
+    def _print_execution_log(self, output_stream: Iterator[tuple[bytes, bytes]]) -> None:
         for stdout, stderr in output_stream:
             if stdout:
                 chunks = iter(stdout.decode().split("\x1d"))
 
                 self._stdout_print(next(chunks))
 
                 for c in chunks:
                     self._print_timing()
                     self._stdout_print(c)
             if stderr:
                 self._stderr_print(stderr.decode())
 
         self._print_timing()
 
-    def _print_timing(self):
+    def _print_timing(self) -> None:
         now = time()
         if self._timestamp:
             self._stdout_print(f"\n>>> Execution time: {now - self._timestamp:.3f}s\n\n")
 
         self._timestamp = now
 
 
 class ContainerScriptRunnerFactory:
     @staticmethod
     def get(
         container: Container,
-        script: List[Union[str, Pipe]],
+        script: Sequence[Union[str, Pipe]],
         output_logger: Optional[Logger] = None,
         user: Optional[Union[int, str]] = None,
-        env: Optional[Dict[str, Any]] = None,
+        env: Optional[dict[str, Any]] = None,
         exec_time: bool = False,
-    ):
+    ) -> ContainerScriptRunner:
+        cls: type[Union[ContainerScriptRunner, ContainerScriptRunnerWithExecTime]]
+
         if exec_time:
             cls = ContainerScriptRunnerWithExecTime
         else:
             cls = ContainerScriptRunner
 
         return cls(container, script, output_logger, user, env)
 
 
 _pulled_images = set()
 
 
-def pull_image(client, image):
+def pull_image(client: DockerClient, image: Image) -> None:
     global _pulled_images
 
     if image.name in _pulled_images:
         logger.info("Image already pulled: %s", image.name)
         return
 
     logger.info("Pulling image: %s", image.name)
@@ -424,15 +471,15 @@
             logger.warning("Error fetching new version of image, falling back to curent one: %s", image.name)
         else:
             raise
 
     _pulled_images.add(image.name)
 
 
-def get_image_authentication(image: Image):
+def get_image_authentication(image: Image) -> Optional[dict[str, str]]:
     if image.aws:
         aws_access_key_id = image.aws.access_key_id
         aws_secret_access_key = image.aws.secret_access_key
         aws_session_token = os.getenv("AWS_SESSION_TOKEN")
         aws_region = os.getenv("AWS_DEFAULT_REGION", "us-east-1")
 
         client = boto3.client(
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/context.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 import logging
 import os
 import uuid
-from typing import Dict, List, Optional
+from typing import TYPE_CHECKING, Optional
 
 from dotenv import dotenv_values
 from slugify import slugify
 
 from . import utils
 from .config import config
-from .models import CloneSettings, Image, Pipeline, ProjectMetadata, Service, Step
+from .models import CloneSettings, Image, Pipeline, ProjectMetadata, Repository, Service, Step
 from .parse import parse_pipeline_file
-from .repository import Repository
 
 logger = logging.getLogger(__name__)
 
+if TYPE_CHECKING:
+    from .runner import PipelineRunRequest
+
 
 class PipelineRunContext:
     def __init__(
         self,
         pipeline_name: str,
         pipeline: Pipeline,
-        caches: Dict[str, str],
-        services: Dict[str, Service],
+        caches: dict[str, str],
+        services: dict[str, Service],
         clone_settings: CloneSettings,
         default_image: Optional[Image],
         project_metadata: ProjectMetadata,
         repository: Repository,
-        env_vars: Optional[Dict[str, str]] = None,
-        selected_steps: Optional[List[str]] = None,
+        env_vars: Optional[dict[str, str]] = None,
+        selected_steps: Optional[list[str]] = None,
     ):
         self.pipeline_name = pipeline_name
         self.pipeline = pipeline
         self.caches = self._merge_default_caches(caches)
         self.services = self._merge_default_services(services)
         self.clone_settings = clone_settings
         self.default_image = default_image
         self.project_metadata = project_metadata
         self.repository = repository
         self.env_vars = env_vars or {}
         self.selected_steps = selected_steps or []
 
         self.pipeline_uuid = uuid.uuid4()
-        self.pipeline_variables = {}
+        self.pipeline_variables: dict[str, str] = {}
 
         self._data_directory = self.get_pipeline_data_directory()
         self._cache_directory = utils.get_project_cache_directory(project_metadata.path_slug)
 
     @classmethod
-    def from_run_request(cls, req) -> "PipelineRunContext":
+    def from_run_request(cls, req: "PipelineRunRequest") -> "PipelineRunContext":
         env_vars = cls._load_env_vars(req.env_files)
         spec = parse_pipeline_file(req.pipeline_file_path)
         spec.expand_env_vars(env_vars)
 
         pipeline_name = req.pipeline_name
         pipeline_to_run = spec.get_pipeline(pipeline_name)
 
@@ -74,33 +76,35 @@
             project_meta,
             repository,
             env_vars,
             req.selected_steps,
         )
 
     @staticmethod
-    def _load_env_vars(env_files: List[str]) -> Dict[str, str]:
-        envvars = {}
+    def _load_env_vars(env_files: list[str]) -> dict[str, str]:
+        envvars: dict[str, Optional[str]] = {}
         # TODO: Load env file in the repo if exists
         logger.debug("Loading .env file (if exists)")
         envvars.update(dotenv_values(".env"))
 
         for env_file in env_files:
             if not os.path.exists(env_file):
                 raise ValueError(f"Invalid env file: {env_file}")
 
             logger.debug("Loading env file: %s", env_file)
             envvars.update(dotenv_values(env_file))
 
-        os.environ.update(envvars)
+        sanitized_env_vars = {k: v or "" for k, v in envvars.items()}
+
+        os.environ.update(sanitized_env_vars)
 
-        return envvars
+        return sanitized_env_vars
 
     @staticmethod
-    def _merge_default_services(services: Dict[str, Service]) -> Dict[str, Service]:
+    def _merge_default_services(services: dict[str, Service]) -> dict[str, Service]:
         for name, definition in config.default_services.items():
             default_service = Service.parse_obj(definition)
 
             if name in services:
                 service = services[name]
                 service.image = default_service.image
 
@@ -110,27 +114,27 @@
                     service.memory = default_service.memory
             else:
                 services[name] = default_service
 
         return services
 
     @staticmethod
-    def _merge_default_caches(caches: Dict[str, str]) -> Dict[str, str]:
+    def _merge_default_caches(caches: dict[str, str]) -> dict[str, str]:
         all_caches = config.default_caches.copy()
         all_caches.update(caches)
 
         return all_caches
 
-    def get_log_directory(self):
+    def get_log_directory(self) -> str:
         return utils.ensure_directory(os.path.join(self._data_directory, "logs"))
 
-    def get_artifact_directory(self):
+    def get_artifact_directory(self) -> str:
         return utils.ensure_directory(os.path.join(self._data_directory, "artifacts"))
 
-    def get_cache_directory(self):
+    def get_cache_directory(self) -> str:
         return utils.ensure_directory(os.path.join(self._cache_directory, "caches"))
 
     def get_pipeline_data_directory(self) -> str:
         project_data_dir = utils.get_project_data_directory(self.project_metadata.path_slug)
         pipeline_id = f"{self.project_metadata.build_number}-{self.pipeline_uuid}"
 
         return os.path.join(project_data_dir, "pipelines", pipeline_id)
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/models.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,106 +1,101 @@
 import os.path
 from enum import Enum
 from string import Template
-from typing import Dict, List, Optional, Union
+from typing import Any, Generic, Iterator, Optional, Sequence, SupportsIndex, TypeVar, Union
 from uuid import UUID, uuid4
 
-from git import Repo
+from git.repo import Repo
 from pydantic import BaseModel as PydanticBaseModel
-from pydantic import Extra, Field, ValidationError, conlist, root_validator, validator
+from pydantic import Extra, Field, ValidationError, root_validator, validator
 from pydantic.error_wrappers import ErrorWrapper
 from slugify import slugify
 
 from . import utils
 from .config import config
 from .utils import generate_ssh_rsa_key
 
 
 class BaseModel(PydanticBaseModel):
-    __env_var_expand_fields__ = []
+    __env_var_expand_fields__: Sequence[str]
 
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    def expand_env_vars(self, variables: Dict[str, str]):
+    def expand_env_vars(self, variables: dict[str, str]) -> None:
         for attr in self.__env_var_expand_fields__:
             value = getattr(self, attr)
             if value is None:
                 continue
 
             if isinstance(value, str):
                 value = Template(value).substitute(variables)
                 setattr(self, attr, value)
             elif isinstance(value, BaseModel):
                 value.expand_env_vars(variables)
 
 
-# noinspection PyMethodParameters
 class AwsCredentials(BaseModel):
-    access_key_id: str = Field(None, alias="access-key")
-    secret_access_key: str = Field(None, alias="secret-key")
-    oidc_role: str = Field(None, alias="oidc-role")
+    access_key_id: str = Field(alias="access-key")
+    secret_access_key: str = Field(alias="secret-key")
+    oidc_role: Optional[str] = Field(alias="oidc-role")
 
-    __env_var_expand_fields__ = ["access_key_id", "secret_access_key", "oidc_role"]
+    __env_var_expand_fields__: Sequence[str] = ["access_key_id", "secret_access_key", "oidc_role"]
 
     @validator("oidc_role")
-    def oidc_role_not_supported(cls, v):
+    def oidc_role_not_supported(cls, v: Optional[str]) -> Optional[str]:
         if v is not None:
             raise ValueError("aws oidc-role not supported")
 
         return v
 
 
-# noinspection PyMethodParameters
 class Image(BaseModel):
     name: str
     username: Optional[str] = None
     password: Optional[str] = None
     email: Optional[str] = None
-    run_as_user: Optional[int] = Field(None, alias="run-as-user")
+    run_as_user: Optional[str] = Field(None, alias="run-as-user")
     aws: Optional[AwsCredentials] = None
 
-    __env_var_expand_fields__ = ["username", "password", "email", "aws"]
+    __env_var_expand_fields__: Sequence[str] = ["username", "password", "email", "aws"]
 
 
 ImageType = Optional[Union[str, Image]]
 
 
 class Service(BaseModel):
-    image: ImageType = None
-    variables: Dict[str, str] = Field(default_factory=dict, alias="environment")
-    memory: Optional[int] = 1024
-
-    # noinspection PyMethodParameters
-    @validator("image")
-    def convert_str_image_to_object(cls, value):
+    image: Optional[Image] = None
+    variables: dict[str, str] = Field(default_factory=dict, alias="environment")
+    memory: int = 1024
+
+    @validator("image", pre=True)
+    def convert_str_image_to_object(cls, value: Union[Image, str]) -> Image:
         if isinstance(value, str):
             return Image(name=value)
 
         return value
 
-    def expand_env_vars(self, variables: Dict[str, str]):
+    def expand_env_vars(self, variables: dict[str, str]) -> None:
         if self.image:
             self.image.expand_env_vars(variables)
 
         for k, v in self.variables.items():
             self.variables[k] = Template(v).substitute(variables)
 
 
-# noinspection PyMethodParameters
 class Definitions(BaseModel):
-    caches: Dict[str, str] = Field(default_factory=dict)
-    services: Dict[str, Service] = Field(default_factory=dict)
+    caches: dict[str, str] = Field(default_factory=dict)
+    services: dict[str, Service] = Field(default_factory=dict)
 
     @validator("services")
-    def ensure_default_services_have_no_image_and_non_default_services_have_an_image(cls, value):
-        if value is None:
-            return None
-
+    def ensure_default_services_have_no_image_and_non_default_services_have_an_image(
+        cls, value: dict[str, Service]
+    ) -> dict[str, Service]:
         errors = []
 
         for service_name, service in value.items():
             if service_name in config.default_services and service.image is not None:
                 errors.append(
                     ErrorWrapper(ValueError(f"Default service {service_name} can't have an image"), loc=service_name)
                 )
@@ -108,31 +103,30 @@
                 errors.append(ErrorWrapper(ValueError(f"Service {service_name} must have an image"), loc=service_name))
 
         if errors:
             raise ValidationError(errors, cls)
 
         return value
 
-    def expand_env_vars(self, variables: Dict[str, str]):
+    def expand_env_vars(self, variables: dict[str, str]) -> None:
         for s in self.services.values():
             s.expand_env_vars(variables)
 
 
-# noinspection PyMethodParameters
 class CloneSettings(BaseModel):
     depth: Optional[Union[str, int]] = 50
     lfs: Optional[bool] = False
     enabled: Optional[bool] = True
 
     @classmethod
-    def empty(cls):
+    def empty(cls) -> "CloneSettings":
         return CloneSettings(depth=None, lfs=None, enabled=None)
 
     @validator("depth")
-    def validate_depth(cls, value):
+    def validate_depth(cls, value: Optional[Union[str, int]]) -> Optional[Union[str, int]]:
         if value is None:
             return None
 
         if isinstance(value, str):
             if value == "full":
                 return 0
 
@@ -157,100 +151,102 @@
 
     def as_int(self) -> int:
         return {self.Simple: 1, self.Double: 2}[self]
 
 
 class Pipe(BaseModel):
     pipe: str
-    variables: Optional[Dict[str, Union[str, List[str]]]] = Field(default=dict)
+    variables: dict[str, str] = Field(default_factory=dict)
 
     def as_cmd(self) -> str:
-        variables = " ".join(f'-e {k}="{self._escape_value(v)}"' for k, v in self.variables.items())
-        return f"docker run --rm {variables} {self.get_image()}"
+        cmd = "docker run --rm"
+        if self.variables:
+            cmd += " " + " ".join(f'-e {k}="{self._escape_value(v)}"' for k, v in self.variables.items())
+
+        return f"{cmd} {self.get_image()}"
 
     @staticmethod
-    def _escape_value(v):
+    def _escape_value(v: str) -> str:
         return v.replace('"', '\\"')
 
     def get_image(self) -> str:
         if self.pipe.startswith("atlassian/"):
             return self.pipe.replace("atlassian/", "bitbucketpipelines/", 1)
 
         return self.pipe
 
 
 class Step(BaseModel):
-    name: Optional[str] = "<unnamed>"
-    script: List[Union[str, Pipe]]
-    image: ImageType = None
-    caches: Optional[List[str]] = Field(default_factory=list)
-    services: Optional[List[str]] = Field(default_factory=list)
-    artifacts: Optional[List[str]] = Field(default_factory=list)
-    after_script: Optional[List[Union[str, Pipe]]] = Field(default_factory=list, alias="after-script")
-    size: Optional[StepSize] = StepSize.Simple
-    clone_settings: Optional[CloneSettings] = Field(default_factory=CloneSettings.empty, alias="clone")
+    name: str = "<unnamed>"
+    script: list[Union[str, Pipe]]
+    image: Optional[Image] = None
+    caches: list[str] = Field(default_factory=list)
+    services: list[str] = Field(default_factory=list)
+    artifacts: list[str] = Field(default_factory=list)
+    after_script: list[Union[str, Pipe]] = Field(default_factory=list, alias="after-script")
+    size: StepSize = StepSize.Simple
+    clone_settings: CloneSettings = Field(default_factory=CloneSettings.empty, alias="clone")
     deployment: Optional[str] = None
     trigger: Trigger = Trigger.Automatic
     max_time: Optional[int] = Field(None, alias="max-time")
 
-    __env_var_expand_fields__ = ["image"]
+    __env_var_expand_fields__: Sequence[str] = ["image"]
 
-    # noinspection PyMethodParameters
-    @validator("image")
-    def convert_str_image_to_object(cls, value):
+    @validator("image", pre=True)
+    def convert_str_image_to_object(cls, value: Union[Image, str]) -> Image:
         if isinstance(value, str):
             return Image(name=value)
 
         return value
 
 
-# noinspection PyUnresolvedReferences
-class WrapperModel(BaseModel):
-    wrapped: BaseModel
+T = TypeVar("T")
 
-    def __getattr__(self, item):
-        if item in self.__dict__:
-            return self.__dict__[item]
-        else:
-            return getattr(self.wrapped, item)
 
-    def __iter__(self):
+class ListWrapper(BaseModel, Generic[T]):
+    wrapped: list[T]
+
+    def __iter__(self) -> Iterator[T]:  # type: ignore[override]
         return iter(self.wrapped)
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: SupportsIndex) -> T:
         return self.wrapped[item]
 
-    def __len__(self):
-        # noinspection PyTypeChecker
+    def __len__(self) -> int:
         return len(self.wrapped)
 
 
-class StepWrapper(WrapperModel):
-    wrapped: Step = Field(alias="step")
+class StepWrapper(BaseModel):
+    step: Step = Field(alias="step")
 
-    def expand_env_vars(self, variables: Dict[str, str]):
-        self.wrapped.expand_env_vars(variables)
+    def expand_env_vars(self, variables: dict[str, str]) -> None:
+        self.step.expand_env_vars(variables)
 
+    def __getattr__(self, item: str) -> Any:
+        if item in self.__dict__:
+            return self.__dict__[item]
+        else:
+            return getattr(self.step, item)
 
-class ParallelStep(WrapperModel):
-    wrapped: conlist(StepWrapper, min_items=2) = Field(alias="parallel")
 
-    def expand_env_vars(self, variables: Dict[str, str]):
+class ParallelStep(ListWrapper[StepWrapper]):
+    wrapped: list[StepWrapper] = Field(alias="parallel", min_items=2)
+
+    def expand_env_vars(self, variables: dict[str, str]) -> None:
         for s in self.wrapped:
             s.expand_env_vars(variables)
 
 
 class Variable(BaseModel):
     name: str
     default: Optional[str]
-    allowed_values: Optional[List[str]] = Field(alias="allowed-values")
+    allowed_values: Optional[list[str]] = Field(alias="allowed-values")
 
-    # noinspection PyMethodParameters
     @root_validator
-    def validate_var_with_allowed_values_must_have_a_default_value(cls, values):
+    def validate_var_with_allowed_values_must_have_a_default_value(cls, values: dict[str, Any]) -> dict[str, Any]:
         allowed_values = values["allowed_values"]
         default = values["default"]
 
         if allowed_values:
             if not default:
                 raise ValueError(
                     "The variable default value is not provided. "
@@ -259,122 +255,124 @@
 
             if default not in allowed_values:
                 raise ValueError(f'The variable allowed values list doesn\'t contain a default value "{default}".')
 
         return values
 
 
-class Variables(WrapperModel):
-    wrapped: List[Variable] = Field(alias="variables")
+class Variables(ListWrapper[Variable]):
+    wrapped: list[Variable] = Field(alias="variables")
+
+
+PipelineElement = Union[StepWrapper, ParallelStep, Variables]
 
 
 class Pipeline(BaseModel):
-    __root__: conlist(Union[StepWrapper, ParallelStep, Variables], min_items=1)
+    __root__: list[PipelineElement] = Field(min_items=1)
 
-    # noinspection PyMethodParameters
     @validator("__root__")
-    def validate_variables_must_be_first_element_of_list_if_present(cls, pipeline_items):
+    def validate_variables_must_be_first_element_of_list_if_present(
+        cls, pipeline_items: list[PipelineElement]
+    ) -> list[PipelineElement]:
         if any(i for i in pipeline_items[1:] if isinstance(i, Variables)):
             raise ValueError("'variables' can only be the first element of the list.")
 
         return pipeline_items
 
-    def get_variables(self) -> Optional[Variables]:
+    def get_variables(self) -> Variables:
         if isinstance(self.__root__[0], Variables):
             return self.__root__[0]
 
-        return Variables(variables=[])
+        return Variables(wrapped=[])
 
-    def get_steps(self) -> List[Union[StepWrapper, ParallelStep]]:
+    def get_steps(self) -> list[Union[StepWrapper, ParallelStep]]:
         return [i for i in self.__root__ if not isinstance(i, Variables)]
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[PipelineElement]:  # type: ignore[override]
         return iter(self.__root__)
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: SupportsIndex) -> PipelineElement:
         return self.__root__[item]
 
-    def expand_env_vars(self, variables: Dict[str, str]):
+    def expand_env_vars(self, variables: dict[str, str]) -> None:
         for s in self.get_steps():
             s.expand_env_vars(variables)
 
 
 class Pipelines(BaseModel):
     default: Optional[Pipeline] = None
-    branches: Optional[Dict[str, Pipeline]] = Field(default_factory=list)
-    pull_requests: Optional[Dict[str, Pipeline]] = Field(default_factory=list, alias="pull-requests")
-    custom: Optional[Dict[str, Pipeline]] = Field(default_factory=list)
+    branches: dict[str, Pipeline] = Field(default_factory=dict)
+    pull_requests: dict[str, Pipeline] = Field(default_factory=dict, alias="pull-requests")
+    custom: dict[str, Pipeline] = Field(default_factory=dict)
 
-    def get_all(self) -> Dict[str, Pipeline]:
+    def get_all(self) -> dict[str, Pipeline]:
         pipelines = {}
         for attr in self.__annotations__.keys():
             value = getattr(self, attr)
             if isinstance(value, Pipeline):
                 pipelines[attr] = value
             elif isinstance(value, dict):
                 for k, v in value.items():
                     pipelines[f"{attr}.{k}"] = v
 
         return pipelines
 
-    # noinspection PyMethodParameters
     @root_validator
-    def ensure_at_least_one_pipeline(cls, values: dict):
+    def ensure_at_least_one_pipeline(cls, values: dict[str, Any]) -> dict[str, Any]:
         if not any(bool(v) for v in values.values()):
             raise ValueError("There must be at least one pipeline")
 
         return values
 
-    def expand_env_vars(self, variables: Dict[str, str]):
+    def expand_env_vars(self, variables: dict[str, str]) -> None:
         for p in self.get_all().values():
             p.expand_env_vars(variables)
 
 
 class PipelineSpec(BaseModel):
-    image: ImageType = None
-    definitions: Optional[Definitions] = Field(default_factory=Definitions.construct)
-    clone_settings: Optional[CloneSettings] = Field(default_factory=CloneSettings.empty, alias="clone")
+    image: Optional[Image] = None
+    definitions: Definitions = Field(default_factory=Definitions.construct)
+    clone_settings: CloneSettings = Field(default_factory=CloneSettings.empty, alias="clone")
     pipelines: Pipelines
 
-    __env_var_expand_fields__ = ["image", "definitions", "pipelines"]
+    __env_var_expand_fields__: Sequence[str] = ["image", "definitions", "pipelines"]
 
     class Config:
         extra = Extra.ignore
 
     @property
-    def caches(self):
+    def caches(self) -> dict[str, str]:
         return self.definitions.caches
 
     @property
-    def services(self):
+    def services(self) -> dict[str, Service]:
         return self.definitions.services
 
     def get_pipeline(self, name: str) -> Optional[Pipeline]:
         return self.pipelines.get_all().get(name)
 
-    def get_available_pipelines(self) -> List[str]:
+    def get_available_pipelines(self) -> list[str]:
         return list(self.pipelines.get_all().keys())
 
-    # noinspection PyMethodParameters
-    @validator("image")
-    def convert_str_image_to_object(cls, value):
+    @validator("image", pre=True)
+    def convert_str_image_to_object(cls, value: Union[Image, str]) -> Image:
         if isinstance(value, str):
             return Image(name=value)
 
         return value
 
 
 class ProjectMetadata(BaseModel):
     name: str
     path_slug: str
     slug: str
     key: str
     project_uuid: UUID = Field(default_factory=uuid4)
     repo_uuid: UUID = Field(default_factory=uuid4)
-    build_number: Optional[int] = 0
+    build_number: int = 0
     ssh_key: str = Field(default_factory=generate_ssh_rsa_key)
 
     @classmethod
     def load_from_file(cls, project_directory: str) -> "ProjectMetadata":
         path_slug = utils.hashify_path(project_directory)
 
         project_data_dir = utils.get_project_data_directory(path_slug)
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/repository.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import logging
-from typing import Dict, Optional, Union
+from typing import Optional, TypeVar, Union, cast
 
 from .config import config
 from .models import CloneSettings, Image, Repository
 
 logger = logging.getLogger(__name__)
 
 
+T = TypeVar("T")
+
+
 class RepositoryCloner:
     def __init__(
         self,
         repository: Repository,
         step_clone_settings: CloneSettings,
         global_clone_settings: CloneSettings,
-        environment: Dict[str, str],
+        environment: dict[str, str],
         user: Optional[Union[int, str]],
         parent_container_name: str,
         data_volume_name: str,
         output_logger: logging.Logger,
     ):
         self._repository = repository
         self._step_clone_settings = step_clone_settings
@@ -26,15 +29,15 @@
         self._user = str(user) if user is not None else None
         self._name = f"{parent_container_name}-clone"
         self._data_volume_name = data_volume_name
         self._output_logger = output_logger
 
         self._container = None
 
-    def clone(self):
+    def clone(self) -> None:
         # TODO: Fix cyclic import
         from .container import ContainerRunner
 
         if not self._should_clone():
             logger.info("Clone disabled: skipping")
             return
 
@@ -55,15 +58,15 @@
             exit_code = runner.run_script(clone_script)
 
             if exit_code:
                 raise Exception("Error setting up repository")
         finally:
             runner.stop()
 
-    def _get_clone_script(self) -> [str]:
+    def _get_clone_script(self) -> list[str]:
         origin = self._get_origin()
         git_clone_cmd = self._get_clone_command(origin)
 
         return [
             git_clone_cmd,
             "git reset --hard $BITBUCKET_COMMIT",
             "git config user.name bitbucket-pipelines",
@@ -76,15 +79,15 @@
         ]
 
     @staticmethod
     def _get_origin() -> str:
         # https://x-token-auth:$REPOSITORY_OAUTH_ACCESS_TOKEN@bitbucket.org/$BITBUCKET_REPO_FULL_NAME.git
         return f"file://{config.remote_workspace_dir}"
 
-    def _get_clone_command(self, origin) -> str:
+    def _get_clone_command(self, origin: str) -> str:
         git_clone_cmd = []
 
         if not self._should_clone_lfs():
             git_clone_cmd += ["GIT_LFS_SKIP_SMUDGE=1"]
 
         # TODO: Add `retry n`
         branch = self._repository.get_current_branch()
@@ -112,17 +115,19 @@
             self._first_non_none_value(
                 self._step_clone_settings.lfs,
                 self._global_clone_settings.lfs,
                 CloneSettings.construct().lfs,
             )
         )
 
-    def _get_clone_depth(self) -> Optional[int]:
-        return self._first_non_none_value(
+    def _get_clone_depth(self) -> Optional[Union[str, int]]:
+        depth = self._first_non_none_value(
             self._step_clone_settings.depth,
             self._global_clone_settings.depth,
             CloneSettings.construct().depth,
         )
 
+        return cast(Optional[Union[str, int]], depth)
+
     @staticmethod
-    def _first_non_none_value(*args) -> Optional[object]:
+    def _first_non_none_value(*args: Optional[T]) -> Optional[T]:
         return next((v for v in args if v is not None), None)
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/runner.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import logging
 import os
 import sys
+from abc import ABC, abstractmethod
 from time import time as ts
-from typing import Dict, List, Optional, Union
+from typing import Optional, Union
 
-import docker
-from docker.models.networks import Network
+import docker  # type: ignore
+from docker.models.networks import Network  # type: ignore
 
 from . import utils
 from .artifacts import ArtifactManager
 from .cache import CacheManager
 from .config import config
 from .container import ContainerRunner
 from .context import PipelineRunContext, StepRunContext
-from .models import Image, ParallelStep, Pipe, PipelineResult, Step, Trigger, Variable
+from .models import Image, ParallelStep, Pipe, PipelineResult, Step, StepWrapper, Trigger, Variable
 from .repository import RepositoryCloner
 from .service import ServicesManager
 
 logger = logging.getLogger(__name__)
 
 
 class PipelineRunRequest:
     def __init__(
         self,
         pipeline_name: str,
         repository_path: Optional[str] = None,
-        selected_steps: List[str] = None,
-        env_files: List[str] = None,
+        selected_steps: Optional[list[str]] = None,
+        env_files: Optional[list[str]] = None,
     ):
         self.pipeline_name = pipeline_name
         self.selected_steps = selected_steps or []
         self.env_files = env_files or []
         self.repository_path = os.path.abspath(repository_path or ".")
 
     @property
@@ -56,15 +57,15 @@
         if exit_code:
             logger.error("Pipeline '%s': Failed", self._ctx.pipeline_name)
         else:
             logger.info("Pipeline '%s': Successful", self._ctx.pipeline_name)
 
         return PipelineResult(exit_code, self._ctx.project_metadata.build_number, self._ctx.pipeline_uuid)
 
-    def _ask_for_variables(self) -> Dict[str, str]:
+    def _ask_for_variables(self) -> dict[str, str]:
         pipeline_variables = {}
         for var in self._pipeline.get_variables():
             pipeline_variables[var.name] = self._read_user_variable_from_stdin(var)
 
         return pipeline_variables
 
     @classmethod
@@ -91,103 +92,111 @@
         else:
             var = sys.stdin.readline()
             if not var:
                 raise IOError("Unable to read from stdin")
 
         return var.rstrip()
 
-    def _execute_pipeline(self):
+    def _execute_pipeline(self) -> int:
         for step in self._pipeline.get_steps():
             runner = StepRunnerFactory.get(step, self._ctx)
 
             exit_code = runner.run()
 
             if exit_code:
                 return exit_code
 
         return 0
 
 
-class StepRunner:
+class BaseStepRunner(ABC):
+    @abstractmethod
+    def run(self) -> Optional[int]:
+        """Run the step."""
+
+
+class StepRunner(BaseStepRunner):
     def __init__(self, step_run_context: StepRunContext):
         self._ctx = step_run_context
         self._step = step_run_context.step
 
         self._docker_client = docker.from_env()
-        self._services_manager = None
-        self._container_runner = None
+        self._services_manager: Optional[ServicesManager] = None
+        self._container_runner: Optional[ContainerRunner] = None
 
         self._container_name = self._ctx.slug
         self._data_volume_name = f"{self._container_name}-data"
         self._output_logger = utils.get_output_logger(
             self._ctx.pipeline_ctx.get_log_directory(), f"{self._container_name}"
         )
 
     # TODO: Decomplexify
-    def run(self) -> Optional[int]:  # noqa: C901: Too complex (11)
+    def run(self) -> Optional[int]:
         if not self._should_run():
             logger.info("Skipping step: %s", self._step.name)
-            return
+            return None
 
         logger.info("Running step: %s", self._step.name)
         logger.debug("Step ID: %s", self._ctx.step_uuid)
 
         if self._step.trigger == Trigger.Manual:
             input("Press enter to run step ")
 
         s = ts()
 
         network = None
 
+        exit_code: int
+
         try:
             if "docker" not in self._step.services and self._docker_is_needed():
                 logger.debug("Docker service is needed, but wasn't requested. Adding it.")
                 self._step.services.append("docker")
 
             image = self._get_image()
             network = self._create_network()
             environment = self._get_step_env_vars()
 
-            self._services_manager = ServicesManager(
+            services_manager = ServicesManager(
                 self._step.services,
                 self._ctx.pipeline_ctx.services,
                 self._step.size.as_int(),
                 self._data_volume_name,
                 self._ctx.pipeline_ctx.project_metadata.path_slug,
                 self._ctx.pipeline_ctx.get_cache_directory(),
             )
+            self._services_manager = services_manager
 
-            mem_limit = self._get_build_container_memory_limit(self._services_manager.get_memory_usage())
+            mem_limit = self._get_build_container_memory_limit(services_manager.get_memory_usage())
 
-            self._container_runner = ContainerRunner(
+            container_runner = ContainerRunner(
                 self._container_name,
                 image,
                 network.name,
                 self._ctx.pipeline_ctx.repository.path,
                 self._data_volume_name,
                 environment,
                 self._output_logger,
                 mem_limit,
                 self._ctx.pipeline_ctx.project_metadata.ssh_key,
             )
+            self._container_runner = container_runner
 
-            self._container_runner.start()
+            container_runner.start()
 
-            self._services_manager.start_services(f"container:{self._container_runner.get_container_name()}")
+            services_manager.start_services(f"container:{container_runner.get_container_name()}")
 
-            services = self._services_manager.get_services_containers()
-            self._container_runner.install_docker_client_if_needed(services)
+            services = services_manager.get_services_containers()
+            container_runner.install_docker_client_if_needed(services)
 
             self._build_setup()
 
-            exit_code = self._container_runner.run_script(self._step.script, exec_time=True)
+            exit_code = container_runner.run_script(self._step.script, exec_time=True)
 
-            self._container_runner.run_script(
-                self._step.after_script, env={"BITBUCKET_EXIT_CODE": exit_code}, exec_time=True
-            )
+            container_runner.run_script(self._step.after_script, env={"BITBUCKET_EXIT_CODE": exit_code}, exec_time=True)
 
             if exit_code:
                 logger.error("Step '%s': FAIL", self._step.name)
 
             self._build_teardown(exit_code)
         except Exception as e:
             logger.exception("Error during pipeline execution: %s", e)
@@ -207,15 +216,15 @@
                 logger.info("Removing volume: %s", volume.name)
                 volume.remove()
 
         logger.info("Step '%s' executed in %.3fs with exit code: %s", self._step.name, ts() - s, exit_code)
 
         return exit_code
 
-    def _should_run(self):
+    def _should_run(self) -> bool:
         if self._ctx.pipeline_ctx.selected_steps and self._step.name not in self._ctx.pipeline_ctx.selected_steps:
             return False
 
         return True
 
     def _get_image(self) -> Image:
         if self._step.image:
@@ -228,66 +237,70 @@
 
     def _create_network(self) -> Network:
         name = f"{self._ctx.pipeline_ctx.project_metadata.slug}-network"
         network = self._docker_client.networks.create(name, driver="bridge")
 
         return network
 
-    def _get_step_env_vars(self) -> Dict[str, str]:
+    def _get_step_env_vars(self) -> dict[str, str]:
         env_vars = self._get_bitbucket_env_vars()
 
         if "docker" in self._step.services:
             env_vars["DOCKER_HOST"] = "tcp://localhost:2375"
 
         env_vars.update(self._ctx.pipeline_ctx.env_vars)
         env_vars.update(self._ctx.pipeline_ctx.pipeline_variables)
 
         return env_vars
 
-    def _get_bitbucket_env_vars(self) -> Dict[str, str]:
+    def _get_bitbucket_env_vars(self) -> dict[str, str]:
         project_slug = self._ctx.pipeline_ctx.project_metadata.slug
         git_branch = self._ctx.pipeline_ctx.repository.get_current_branch()
         git_commit = self._ctx.pipeline_ctx.repository.get_current_commit()
 
-        env_vars = {
+        env_vars: dict[str, str] = {
             "CI": "true",
             "BUILD_DIR": config.build_dir,
             "BITBUCKET_BRANCH": git_branch,
-            "BITBUCKET_BUILD_NUMBER": self._ctx.pipeline_ctx.project_metadata.build_number,
+            "BITBUCKET_BUILD_NUMBER": str(self._ctx.pipeline_ctx.project_metadata.build_number),
             "BITBUCKET_PROJECT_KEY": self._ctx.pipeline_ctx.project_metadata.key,
-            "BITBUCKET_PROJECT_UUID": self._ctx.pipeline_ctx.project_metadata.project_uuid,
+            "BITBUCKET_PROJECT_UUID": str(self._ctx.pipeline_ctx.project_metadata.project_uuid),
             "BITBUCKET_CLONE_DIR": config.build_dir,
             "BITBUCKET_COMMIT": git_commit,
-            "BITBUCKET_PIPELINE_UUID": self._ctx.pipeline_ctx.pipeline_uuid,
+            "BITBUCKET_PIPELINE_UUID": str(self._ctx.pipeline_ctx.pipeline_uuid),
             "BITBUCKET_REPO_FULL_NAME": f"{project_slug}/{project_slug}",
             "BITBUCKET_REPO_IS_PRIVATE": "true",
             "BITBUCKET_REPO_OWNER": config.username,
             "BITBUCKET_REPO_OWNER_UUID": config.owner_uuid,
             "BITBUCKET_REPO_SLUG": project_slug,
-            "BITBUCKET_REPO_UUID": self._ctx.pipeline_ctx.project_metadata.repo_uuid,
-            "BITBUCKET_STEP_UUID": self._ctx.step_uuid,
+            "BITBUCKET_REPO_UUID": str(self._ctx.pipeline_ctx.project_metadata.repo_uuid),
+            "BITBUCKET_STEP_UUID": str(self._ctx.step_uuid),
             "BITBUCKET_WORKSPACE": project_slug,
         }
 
         if self._ctx.is_parallel():
-            env_vars["BITBUCKET_PARALLEL_STEP"] = self._ctx.parallel_step_index
-            env_vars["BITBUCKET_PARALLEL_STEP_COUNT"] = self._ctx.parallel_step_count
+            env_vars["BITBUCKET_PARALLEL_STEP"] = str(self._ctx.parallel_step_index)
+            env_vars["BITBUCKET_PARALLEL_STEP_COUNT"] = str(self._ctx.parallel_step_count)
 
         if self._step.deployment:
             env_vars["BITBUCKET_DEPLOYMENT_ENVIRONMENT"] = self._step.deployment
 
         return env_vars
 
     def _get_build_container_memory_limit(self, services_memory_usage: int) -> int:
         return config.total_memory_limit * self._step.size.as_int() - services_memory_usage
 
     def _docker_is_needed(self) -> bool:
         return any(i for i in self._step.script + self._step.after_script if isinstance(i, Pipe))
 
-    def _build_setup(self):
+    def _build_setup(self) -> None:
+        if not self._services_manager:
+            # TODO: Refactor
+            raise Exception("called on uninitialized runner")
+
         logger.info("Build setup: '%s'", self._step.name)
         s = ts()
 
         self._clone_repository()
         self._upload_artifacts()
         self._upload_caches()
 
@@ -303,73 +316,90 @@
         self._output_logger.info("\tbuild: %s@%s\n", docker_image.tags[0].split(":")[0], docker_image.id)
         for name, container in self._services_manager.get_services_containers().items():
             self._output_logger.info("\t%s: %s@%s\n", name, container.image.tags[0].split(":")[0], container.image.id)
         self._output_logger.info("\n")
 
         logger.info("Build setup finished in %.3fs: '%s'", ts() - s, self._step.name)
 
-    def _upload_artifacts(self):
+    def _upload_artifacts(self) -> None:
+        if not self._container_runner:
+            # TODO: Refactor
+            raise Exception("called on uninitialized runner")
+
         am = ArtifactManager(
             self._container_runner, self._ctx.pipeline_ctx.get_artifact_directory(), self._ctx.step_uuid
         )
         am.upload()
 
-    def _upload_caches(self):
+    def _upload_caches(self) -> None:
+        if not self._container_runner:
+            # TODO: Refactor
+            raise Exception("called on uninitialized runner")
+
         cm = CacheManager(
             self._container_runner, self._ctx.pipeline_ctx.get_cache_directory(), self._ctx.pipeline_ctx.caches
         )
         cm.upload(self._step.caches)
 
-    def _clone_repository(self):
+    def _clone_repository(self) -> None:
         image = self._get_image()
 
         rc = RepositoryCloner(
             self._ctx.pipeline_ctx.repository,
             self._step.clone_settings,
             self._ctx.pipeline_ctx.clone_settings,
             self._get_bitbucket_env_vars(),
             image.run_as_user,
             self._container_name,
             self._data_volume_name,
             self._output_logger,
         )
         rc.clone()
 
-    def _build_teardown(self, exit_code):
+    def _build_teardown(self, exit_code: int) -> None:
         logger.info("Build teardown: '%s'", self._step.name)
         s = ts()
 
         self._download_caches(exit_code)
         self._download_artifacts()
         self._stop_services()
 
         logger.info("Build teardown finished in %.3fs: '%s'", ts() - s, self._step.name)
 
-    def _download_caches(self, exit_code):
+    def _download_caches(self, exit_code: int) -> None:
+        if not self._container_runner:
+            # TODO: Refactor
+            raise Exception("called on uninitialized runner")
+
         if exit_code == 0:
             cm = CacheManager(
                 self._container_runner,
                 self._ctx.pipeline_ctx.get_cache_directory(),
                 self._ctx.pipeline_ctx.caches,
             )
             cm.download(self._step.caches)
         else:
             logger.warning("Skipping caches for failed step")
 
-    def _download_artifacts(self):
+    def _download_artifacts(self) -> None:
+        if not self._container_runner:
+            # TODO: Refactor
+            raise Exception("called on uninitialized runner")
+
         am = ArtifactManager(
             self._container_runner, self._ctx.pipeline_ctx.get_artifact_directory(), self._ctx.step_uuid
         )
         am.download(self._step.artifacts)
 
-    def _stop_services(self):
+    def _stop_services(self) -> None:
+        # TODO: Remove
         pass
 
 
-class ParallelStepRunner:
+class ParallelStepRunner(BaseStepRunner):
     def __init__(self, parallel_step: ParallelStep, pipeline_run_context: PipelineRunContext):
         self._parallel_step = parallel_step
         self._pipeline_ctx = pipeline_run_context
 
     def run(self) -> Optional[int]:
         return_code = 0
         step_count = len(self._parallel_step)
@@ -384,16 +414,17 @@
 
         return return_code
 
 
 class StepRunnerFactory:
     @staticmethod
     def get(
-        step: Union[Step, ParallelStep],
+        step: Union[Step, StepWrapper, ParallelStep],
         pipeline_run_context: PipelineRunContext,
         parallel_step_index: Optional[int] = None,
         parallel_step_count: Optional[int] = None,
-    ):
+    ) -> BaseStepRunner:
         if isinstance(step, ParallelStep):
             return ParallelStepRunner(step, pipeline_run_context)
-        else:
-            return StepRunner(StepRunContext(step, pipeline_run_context, parallel_step_index, parallel_step_count))
+
+        s = step.step if isinstance(step, StepWrapper) else step
+        return StepRunner(StepRunContext(s, pipeline_run_context, parallel_step_index, parallel_step_count))
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/service.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from importlib.resources import as_file, files
-from typing import Dict, List
+from typing import Union
 
-import docker
+import docker  # type: ignore
 from docker import DockerClient
-from docker.models.containers import Container
-from docker.models.volumes import Volume
+from docker.models.containers import Container  # type: ignore
+from docker.models.volumes import Volume  # type: ignore
 from slugify import slugify
 from tenacity import retry, retry_if_exception_type, stop_after_delay, wait_fixed
 
 import pipeline_runner
 
 from .config import config
 from .container import ContainerScriptRunner, pull_image
@@ -25,32 +25,32 @@
 class ServiceUnhealthyError(Exception):
     pass
 
 
 class ServicesManager:
     def __init__(
         self,
-        service_names: List[str],
-        service_definitions: Dict[str, Service],
+        service_names: list[str],
+        service_definitions: dict[str, Service],
         memory_multiplier: int,
         shared_data_volume_name: str,
         repository_slug: str,
         pipeline_cache_directory: str,
     ):
         self._services_by_name = self._get_services(service_names, service_definitions)
         self._memory_multiplier = memory_multiplier
         self._shared_data_volume_name = shared_data_volume_name
         self._repository_slug = repository_slug
         self._pipeline_cache_directory = pipeline_cache_directory
 
         self._client = docker.from_env()
 
-        self._service_runners = {}
+        self._service_runners: dict[str, ServiceRunner] = {}
 
-    def start_services(self, network_name: str):
+    def start_services(self, network_name: str) -> None:
         self._ensure_memory_for_services()
 
         for service_name, service in self._services_by_name.items():
             sr = ServiceRunnerFactory.get(
                 self._client,
                 service_name,
                 service,
@@ -58,39 +58,39 @@
                 self._shared_data_volume_name,
                 self._repository_slug,
                 self._pipeline_cache_directory,
             )
             sr.start()
             self._service_runners[sr.slug] = sr
 
-    def stop_services(self):
+    def stop_services(self) -> None:
         for s, sr in self._service_runners.items():
             try:
                 sr.stop()
             except Exception as e:
                 logger.exception("Error removing service '%s': %s", s, e)
 
-    def get_services_containers(self) -> Dict[str, Container]:
+    def get_services_containers(self) -> dict[str, Container]:
         return {name: runner.container for name, runner in self._service_runners.items()}
 
     def get_memory_usage(self) -> int:
         return sum(s.memory for s in self._services_by_name.values())
 
     @staticmethod
-    def _get_services(service_names, service_definitions) -> Dict[str, Service]:
+    def _get_services(service_names: list[str], service_definitions: dict[str, Service]) -> dict[str, Service]:
         services = {}
         for service_name in service_names:
             if service_name not in service_definitions:
                 raise ValueError(f"Invalid service: {service_name}")
 
             services[service_name] = service_definitions[service_name]
 
         return services
 
-    def _ensure_memory_for_services(self):
+    def _ensure_memory_for_services(self) -> None:
         requested_mem = self.get_memory_usage()
         available_mem = self._get_service_containers_memory_limit()
         if requested_mem > available_mem:
             raise ValueError(
                 f"Not enough memory to run all services. Requested: {requested_mem}MiB / Available: {available_mem}MiB"
             )
 
@@ -117,114 +117,120 @@
         self._project_slug = project_slug
         self._pipeline_cache_directory = pipeline_cache_directory
         self._container = None
 
         self._slug = slugify(self._service_name)
 
     @property
-    def slug(self):
+    def slug(self) -> str:
         return self._slug
 
     @property
-    def container(self):
+    def container(self) -> Container:
         return self._container
 
-    def start(self):
+    def start(self) -> None:
+        if not self._service.image:
+            raise ValueError("Service has no image.")
+
         logger.info("Starting service: %s", self._service_name)
         pull_image(self._client, self._service.image)
 
         self._container = self._start_container()
         self._ensure_container_ready(self._container)
 
     def _start_container(self) -> Container:
+        if not self._service.image:
+            raise ValueError("Service has no image.")
+
         container = self._client.containers.run(
             self._service.image.name,
             name=self._get_container_name(),
             environment=self._service.variables,
             network=self._network_name,
             mem_limit=self._get_mem_limit(),
             detach=True,
         )
 
         return container
 
-    def _ensure_container_ready(self, container: Container):
+    def _ensure_container_ready(self, container: Container) -> None:
         pass
 
-    def _get_container_name(self):
+    def _get_container_name(self) -> str:
         return f"{self._project_slug}-service-{self._slug}"
 
-    def stop(self):
+    def stop(self) -> None:
+        if not self._container:
+            # TODO: Refactor
+            raise Exception("called on uninitialized service")
+
         logger.info("Removing service: %s", self._service_name)
 
         self._teardown()
 
         self._container.remove(v=True, force=True)
 
     def _get_mem_limit(self) -> int:
         return self._service.memory * 2**20
 
-    def _teardown(self):
+    def _teardown(self) -> None:
         pass
 
 
 class DockerServiceRunner(ServiceRunner):
     def _start_container(self) -> Container:
+        if not self._service.image:
+            raise ValueError("Service has no image.")
+
         environment = self._service.variables
         environment["DOCKER_TLS_CERTDIR"] = ""
 
         container = self._client.containers.run(
             self._service.image.name,
             name=self._get_container_name(),
-            command=["runit.sh", "--tls=false"],
+            command=["--tls=false"],
             environment=environment,
             network=self._network_name,
             privileged=True,
             volumes=self._get_volumes(),
             mem_limit=self._get_mem_limit(),
             detach=True,
             healthcheck={
-                "test": ["CMD", "docker", "ps"],
-                "interval": 5_000_000_000,
                 "start_period": 30_000_000_000,
                 "timeout": 1_000_000_000,
             },
         )
 
         return container
 
     @retry(wait=wait_fixed(1), stop=stop_after_delay(30), retry=retry_if_exception_type(ServiceNotReadyError))
-    def _ensure_container_ready(self, container: Container):
+    def _ensure_container_ready(self, container: Container) -> None:
         # Refresh container to ensure we have its health status
         container = self._client.containers.get(container.name)
         health = container.attrs["State"]["Health"]["Status"]
         if health == "healthy":
             return
         elif health == "unhealthy":
             raise ServiceUnhealthyError()
         else:
             raise ServiceNotReadyError()
 
-    def _get_volumes(self) -> Dict[str, Dict[str, str]]:
+    def _get_volumes(self) -> dict[str, dict[str, str]]:
         static_files = files(pipeline_runner).joinpath("static")
 
-        with as_file(static_files.joinpath("dind")) as p:
-            dind_script_path = p
-
         with as_file(static_files.joinpath("runit.sh")) as p:
             runit_script_path = p
 
         cache_volume = self._get_cache_volume()
 
         return {
             cache_volume.name: {"bind": "/var/lib/docker"},
             self._shared_data_volume_name: {"bind": config.remote_pipeline_dir},
-            # https://github.com/moby/moby/pull/42331
-            dind_script_path: {"bind": "/usr/local/bin/dind"},
-            runit_script_path: {"bind": "/usr/local/bin/runit.sh"},
+            str(runit_script_path): {"bind": "/usr/local/bin/runit.sh"},
         }
 
     def _get_cache_volume(self) -> Volume:
         label_name = "org.acidrain.pipeline_runner.project"
         label_value = self._project_slug
 
         volumes = self._client.volumes.list(filters={"label": f"{label_name}={label_value}"})
@@ -236,15 +242,15 @@
         elif len(volumes) == 1:
             volume = volumes[0]
         else:
             raise Exception("Found more than one cache volume")
 
         return volume
 
-    def _teardown(self):
+    def _teardown(self) -> None:
         logger.info("Executing teardown for service: %s", self._service_name)
 
         script = [
             "docker ps -q | xargs -r docker kill",
             "docker container prune -f",
             "docker volume prune -f",
         ]
@@ -259,14 +265,16 @@
         service_name: str,
         service_def: Service,
         network_name: str,
         shared_data_volume_name: str,
         repository_slug: str,
         pipeline_cache_directory: str,
     ) -> ServiceRunner:
+        cls: type[Union[ServiceRunner, DockerServiceRunner]]
+
         if service_name == "docker":
             cls = DockerServiceRunner
         else:
             cls = ServiceRunner
 
         return cls(
             docker_client,
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pipeline_runner/utils.py` & `bitbucket_pipeline_runner-0.3.8/pipeline_runner/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import base64
 import hashlib
 import logging
 import os
 import sys
-from typing import List, Union
+from logging import Logger
+from tarfile import TarFile
+from typing import IO, Iterator, Union
 
 from appdirs import user_cache_dir, user_data_dir
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from slugify import slugify
 
 from . import APP_NAME
 
 logger = logging.getLogger(__name__)
 
 
-def get_output_logger(output_directory: str, name: str) -> logging.Logger:
+def get_output_logger(output_directory: str, name: str) -> Logger:
     formatter = logging.Formatter("%(message)s")
 
     stream_handler = logging.StreamHandler(stream=sys.stdout)
     stream_handler.setFormatter(formatter)
     stream_handler.terminator = ""
 
     file_handler = logging.FileHandler(os.path.join(output_directory, f"{name}.txt"))
@@ -38,94 +40,119 @@
     return user_cache_dir(appname=APP_NAME)
 
 
 def get_data_directory() -> str:
     return user_data_dir(appname=APP_NAME)
 
 
-def get_project_cache_directory(project_path_slug):
+def get_project_cache_directory(project_path_slug: str) -> str:
     return ensure_directory(os.path.join(get_cache_directory(), project_path_slug))
 
 
-def get_project_data_directory(project_path_slug):
+def get_project_data_directory(project_path_slug: str) -> str:
     return ensure_directory(os.path.join(get_data_directory(), project_path_slug))
 
 
-def ensure_directory(path) -> str:
+def ensure_directory(path: str) -> str:
     if not os.path.exists(path):
         os.makedirs(path)
 
     return path
 
 
-def stringify(value: Union[str, List[str]], sep: str = " "):
+def stringify(value: Union[str, list[str]], sep: str = " ") -> str:
     if isinstance(value, list):
         value = sep.join(value)
 
     return value
 
 
 def escape_shell_string(value: str) -> str:
     for c in "\\$%{}\"'":
         value = value.replace(c, rf"\x{ord(c):02x}")
 
     return value
 
 
-def get_human_readable_size(num):
-    for unit in ["B", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB"]:
-        if abs(num) < 1024.0:
+def get_human_readable_size(value: int) -> str:
+    if value < 0:
+        raise ValueError("size must be positive")
+
+    num: float = value
+    for unit in ["B", "KiB", "MiB", "GiB"]:
+        if num < 1024:
             return f"{num:3.1f}{unit}"
 
-        num /= 1024.0
+        num /= 1024
 
-    return f"{num:.1f}{unit}"
+    return f"{num:.1f}TiB"
 
 
-def wrap_in_shell(command: Union[str, List[str]], stop_on_error=True):
+def wrap_in_shell(command: Union[str, list[str]], stop_on_error: bool = True) -> list[str]:
     command = stringify(command)
 
     wrapped = ["sh"]
     if stop_on_error:
         wrapped.append("-e")
 
     wrapped += ["-c", command]
 
     return wrapped
 
 
-def hashify_path(path):
+def hashify_path(path: str) -> str:
     slug = slugify(os.path.basename(path))
 
     h = hashlib.sha256(path.encode()).digest()
-    h = base64.urlsafe_b64encode(h).decode()[:8]
+    suffix = base64.urlsafe_b64encode(h).decode()[:8]
 
-    return f"{slug}-{h}"
+    return f"{slug}-{suffix}"
 
 
 def generate_ssh_rsa_key() -> str:
     key = rsa.generate_private_key(public_exponent=65537, key_size=2048)
     private_key = key.private_bytes(
         serialization.Encoding.PEM, serialization.PrivateFormat.PKCS8, serialization.NoEncryption()
     )
     return private_key.decode()
 
 
-class FileStreamer:
-    def __init__(self, it):
+class PathTraversalError(Exception):
+    pass
+
+
+def safe_extract_tar(tar: TarFile, path: str = ".", *, numeric_owner: bool = False) -> None:
+    def _is_within_directory(directory: str, target: str) -> bool:
+        abs_directory = os.path.abspath(directory)
+        abs_target = os.path.abspath(target)
+
+        prefix = os.path.commonprefix([abs_directory, abs_target])
+
+        return prefix == abs_directory
+
+    for member in tar:
+        member_path = os.path.join(path, member.name)
+        if not _is_within_directory(path, member_path):
+            raise PathTraversalError
+
+        tar.extract(member, path, numeric_owner=numeric_owner)
+
+
+class FileStreamer(IO[bytes]):
+    def __init__(self, it: Iterator[bytes]) -> None:
         self._it = it
         self._chunk = b""
         self._has_more_data = True
 
-    def _grow_chunk(self):
+    def _grow_chunk(self) -> None:
         self._chunk = self._chunk + next(self._it)
 
-    def read(self, n):
+    def read(self, n: int = 512) -> bytes:
         if not self._has_more_data:
-            return None
+            return b""
 
         try:
             while len(self._chunk) < n:
                 self._grow_chunk()
             rv = self._chunk[:n]
             self._chunk = self._chunk[n:]
             return rv
```

### Comparing `bitbucket_pipeline_runner-0.3.7/pyproject.toml` & `bitbucket_pipeline_runner-0.3.8/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bitbucket-pipeline-runner"
-version = "0.3.7"
+version = "0.3.8"
 description = "Run a bitbucket pipeline locally"
 authors = ["Mathieu Lemay <acidrain1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mathieu-lemay/pipeline-runner"
 packages = [
     {include = "pipeline_runner"}
@@ -15,43 +15,62 @@
 PyYAML = "^6.0"
 docker = "^6.0.0"
 click = "^8.0.1"
 python-slugify = "^8.0.0"
 # Pin boto3 to a specific version to avoid poetry's resolver
 # to go on forever.
 # https://github.com/python-poetry/poetry/issues/7858
-boto3 = "1.26.135"
+boto3 = "^1.26.162"
 GitPython = "^3.1.12"
 python-dotenv = "^1.0.0"
-requests = "^2.25.1"
+requests = "^2.31.0"
 coloredlogs = "^15.0"
 pyfzf = "^0.3.0"
 pydantic = "^1.8.2"
 appdirs = "^1.4.4"
-cryptography = "^40.0.2"
+cryptography = "^41.0.1"
 tenacity = "^8.0.1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.0.1"
 pytest-mock = "^3.5.1"
 coverage = { version = "^7.0.1", extras = ["toml"] }
+mypy = "^1.4.0"
+types-appdirs = "^1.4.3.5"
+types-setuptools = "^68.0.0.0"
+types-pyyaml = "^6.0.12.10"
+types-python-slugify = "^8.0.0.2"
+types-boto3 = "^1.0.2"
 
 [tool.poetry.scripts]
 pipeline-runner = 'pipeline_runner.cli:main'
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 line_length = 120
 
+[tool.mypy]
+namespace_packages=true
+explicit_package_bases=true
+strict=true
+show_error_codes=true
+plugins=["pydantic.mypy"]
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+warn_untyped_fields = true
+
 [tool.ruff]
 exclude = [".venv"]
 ignore = ["E501"]
 line-length = 120
 select = [
     "A",  # flake8-builtins
     "B",  # flake8-bugbear
```

### Comparing `bitbucket_pipeline_runner-0.3.7/PKG-INFO` & `bitbucket_pipeline_runner-0.3.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipeline-runner
-Version: 0.3.7
+Version: 0.3.8
 Summary: Run a bitbucket pipeline locally
 Home-page: https://github.com/mathieu-lemay/pipeline-runner
 License: MIT
 Author: Mathieu Lemay
 Author-email: acidrain1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.12,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: boto3 (==1.26.135)
+Requires-Dist: boto3 (>=1.26.162,<2.0.0)
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0,<16.0)
-Requires-Dist: cryptography (>=40.0.2,<41.0.0)
+Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: docker (>=6.0.0,<7.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pyfzf (>=0.3.0,<0.4.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-slugify (>=8.0.0,<9.0.0)
-Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Project-URL: Repository, https://github.com/mathieu-lemay/pipeline-runner
 Description-Content-Type: text/markdown
 
 # Bitbucket Pipeline Runner
 
 Tool to run Bitbucket Pipelines locally.
```

