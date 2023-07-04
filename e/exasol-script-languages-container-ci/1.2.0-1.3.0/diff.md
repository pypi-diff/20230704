# Comparing `tmp/exasol_script_languages_container_ci-1.2.0.tar.gz` & `tmp/exasol_script_languages_container_ci-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_script_languages_container_ci-1.2.0.tar", max compression
+gzip compressed data, was "exasol_script_languages_container_ci-1.3.0.tar", max compression
```

## Comparing `exasol_script_languages_container_ci-1.2.0.tar` & `exasol_script_languages_container_ci-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
--rw-r--r--   0        0        0     1063 2023-06-28 11:15:33.086414 exasol_script_languages_container_ci-1.2.0/LICENSE
--rw-r--r--   0        0        0       95 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/cli/__init__.py
--rw-r--r--   0        0        0       50 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/cli/cli.py
--rw-r--r--   0        0        0        0 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/cli/commands/__init__.py
--rw-r--r--   0        0        0     1658 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/cli/commands/run_ci.py
--rw-r--r--   0        0        0     2566 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/cli/commands/run_release.py
--rw-r--r--   0        0        0        0 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/__init__.py
--rw-r--r--   0        0        0     1304 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/asset_uploader.py
--rw-r--r--   0        0        0     1677 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/branch_config.py
--rw-r--r--   0        0        0     4992 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci.py
--rw-r--r--   0        0        0     2674 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_build.py
--rw-r--r--   0        0        0      944 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_export.py
--rw-r--r--   0        0        0     1157 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_push.py
--rw-r--r--   0        0        0     1071 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_security_scan.py
--rw-r--r--   0        0        0     1309 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_step_output_printer.py
--rw-r--r--   0        0        0     4816 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_test.py
--rw-r--r--   0        0        0      334 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/common.py
--rw-r--r--   0        0        0     1501 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/git_access.py
--rw-r--r--   0        0        0     1223 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py
--rw-r--r--   0        0        0     2786 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/release.py
--rw-r--r--   0        0        0     2443 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/release_uploader.py
--rwxr-xr-x   0        0        0      125 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/main.py
--rw-r--r--   0        0        0      785 2023-06-28 11:15:33.090414 exasol_script_languages_container_ci-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 exasol_script_languages_container_ci-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/LICENSE
+-rw-r--r--   0        0        0       95 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/__init__.py
+-rw-r--r--   0        0        0       50 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1926 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/commands/run_ci.py
+-rw-r--r--   0        0        0     2703 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/commands/run_release.py
+-rw-r--r--   0        0        0        0 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/__init__.py
+-rw-r--r--   0        0        0     1304 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/asset_uploader.py
+-rw-r--r--   0        0        0     1677 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/branch_config.py
+-rw-r--r--   0        0        0     4940 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci.py
+-rw-r--r--   0        0        0     2674 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_build.py
+-rw-r--r--   0        0        0      944 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_export.py
+-rw-r--r--   0        0        0     1157 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_push.py
+-rw-r--r--   0        0        0     1071 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_security_scan.py
+-rw-r--r--   0        0        0     1309 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_step_output_printer.py
+-rw-r--r--   0        0        0     4816 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_test.py
+-rw-r--r--   0        0        0      334 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/common.py
+-rw-r--r--   0        0        0        0 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/config/__init__.py
+-rw-r--r--   0        0        0      584 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/config/config_data_model.py
+-rw-r--r--   0        0        0     2153 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/config/data_model_generator.py
+-rw-r--r--   0        0        0     1501 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/git_access.py
+-rw-r--r--   0        0        0     1223 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py
+-rw-r--r--   0        0        0     2890 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/release.py
+-rw-r--r--   0        0        0     2443 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/release_uploader.py
+-rw-r--r--   0        0        0      321 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/render_template.py
+-rwxr-xr-x   0        0        0      125 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/main.py
+-rw-r--r--   0        0        0      950 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/templates/config_schema.json
+-rw-r--r--   0        0        0      822 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 exasol_script_languages_container_ci-1.3.0/PKG-INFO
```

### Comparing `exasol_script_languages_container_ci-1.2.0/LICENSE` & `exasol_script_languages_container_ci-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/cli/commands/run_ci.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/commands/run_ci.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 import click
 
 from exasol_script_languages_container_ci.cli.cli import cli
 from exasol_script_languages_container_ci.lib.ci import ci
+from exasol_script_languages_container_ci.lib.config.config_data_model import Config
 from exasol_script_languages_container_ci.lib.git_access import GitAccess
 
 
 @cli.command()
 @click.option('--flavor', required=True, type=str,
               help="Flavor name.")
 @click.option('--branch-name', required=True, type=str,
@@ -31,16 +32,17 @@
            docker_user: str,
            docker_password: str,
            docker_build_repository: str,
            docker_release_repository: str,
            commit_sha: str,
            config_file: str):
     logging.basicConfig(level=logging.INFO)
-    ci(flavor,
-       branch_name,
-       docker_user,
-       docker_password,
-       docker_build_repository,
-       docker_release_repository,
-       commit_sha,
-       config_file,
-       GitAccess())
+    build_config = Config.parse_file(config_file)
+    ci(flavor=flavor,
+       branch_name=branch_name,
+       docker_user=docker_user,
+       docker_password=docker_password,
+       docker_build_repository=docker_build_repository,
+       docker_release_repository=docker_release_repository,
+       commit_sha=commit_sha,
+       build_config=build_config,
+       git_access=GitAccess())
```

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/cli/commands/run_release.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/commands/run_release.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 
 import click
 
 from exasol_script_languages_container_ci.cli.cli import cli
 from exasol_script_languages_container_ci.lib.asset_uploader import AssetUploader
+from exasol_script_languages_container_ci.lib.config.config_data_model import Config
 from exasol_script_languages_container_ci.lib.github_release_asset_uploader import GithubReleaseAssetUploader
 from exasol_script_languages_container_ci.lib.release import release
 from exasol_script_languages_container_ci.lib.release_uploader import ReleaseUploader
 
 
 @cli.command()
 @click.option('--flavor', required=True, type=str,
@@ -38,16 +39,17 @@
                 source_repo_url: str,
                 release_id: int,
                 dry_run: bool):
     logging.basicConfig(level=logging.INFO)
     github_release_asset_uploader = GithubReleaseAssetUploader(os.getenv("GITHUB_TOKEN"))
     asset_uploader = AssetUploader(release_asset_uploader=github_release_asset_uploader)
     release_uploader = ReleaseUploader(asset_uploader=asset_uploader)
+    build_config = Config.parse_file(config_file)
     release(flavor=flavor,
             docker_user=docker_user,
             docker_password=docker_password,
             docker_release_repository=docker_release_repository,
-            config_file=config_file,
+            build_config=build_config,
             source_repo_url=source_repo_url,
             release_id=release_id,
             release_uploader=release_uploader,
             is_dry_run=dry_run)
```

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/asset_uploader.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/asset_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/branch_config.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/branch_config.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 import logging
 import os
 from pathlib import Path
 from typing import Set
 
-import click
+from exasol_integration_test_docker_environment.cli.options.system_options import DEFAULT_OUTPUT_DIRECTORY
 from exasol_integration_test_docker_environment.lib.base import luigi_log_config
-from exasol_integration_test_docker_environment.lib.config import build_config
 
 from exasol_script_languages_container_ci.lib.branch_config import BranchConfig
-from exasol_script_languages_container_ci.lib.common import get_config
 from exasol_script_languages_container_ci.lib.ci_build import CIBuild
 from exasol_script_languages_container_ci.lib.ci_push import CIPush
 from exasol_script_languages_container_ci.lib.ci_security_scan import CISecurityScan
 from exasol_script_languages_container_ci.lib.ci_test import CIExecuteTest
+from exasol_script_languages_container_ci.lib.config.config_data_model import Config
 from exasol_script_languages_container_ci.lib.git_access import GitAccess
 
 
 def get_all_affected_files(git_access: GitAccess, base_branch: str) -> Set[str]:
     base_last_commit_sha = git_access.get_head_commit_sha_of_branch(base_branch)
     changed_files = set()
     for commit in git_access.get_last_commits():
         if commit == base_last_commit_sha:
             break
         changed_files.update(git_access.get_files_of_commit(commit))
     return changed_files
 
 
-def check_if_need_to_build(branch_name: str, config_file: str, flavor: str, git_access: GitAccess):
+def check_if_need_to_build(branch_name: str, config: Config, flavor: str, git_access: GitAccess):
     if BranchConfig.build_always(branch_name):
         return True
     if "[rebuild]" in git_access.get_last_commit_message():
         return True
-    with get_config(config_file) as config:
-        affected_files = list(get_all_affected_files(git_access, config["base_branch"]))
-        logging.debug(f"check_if_need_to_build: Found files of last commits: {affected_files}")
-        for ignore_path in config["build_ignore"]["ignored_paths"]:
-            affected_files = list(filter(lambda file: not file.startswith(ignore_path), affected_files))
+    affected_files = list(get_all_affected_files(git_access, config.build.base_branch))
+    logging.debug(f"check_if_need_to_build: Found files of last commits: {affected_files}")
+    for ignore_path in config.build.ignore.paths:
+        affected_files = list(filter(lambda file: not file.startswith(ignore_path), affected_files))
 
     if len(affected_files) > 0:
         # Now filter out also other flavor folders
         this_flavor_path = f"flavors/{flavor}"
         affected_files = list(filter(lambda file: not file.startswith("flavors") or file.startswith(this_flavor_path),
                                      affected_files))
     logging.debug(f"check_if_need_to_build: filtered files: {affected_files}")
@@ -49,15 +47,15 @@
 def ci(flavor: str,
        branch_name: str,
        docker_user: str,
        docker_password: str,
        docker_build_repository: str,
        docker_release_repository: str,
        commit_sha: str,
-       config_file: str,
+       build_config: Config,
        git_access: GitAccess,
        ci_build: CIBuild = CIBuild(),
        ci_execute_tests: CIExecuteTest = CIExecuteTest(),
        ci_push: CIPush = CIPush(),
        ci_security_scan: CISecurityScan = CISecurityScan()):
     """
     Run CI build:
@@ -67,17 +65,17 @@
     4. Push to docker repositories
     """
     logging.info(f"Running CI build for parameters: {locals()}")
 
     flavor_path = (f"flavors/{flavor}",)
     test_container_folder = "test_container"
     rebuild = BranchConfig.rebuild(branch_name)
-    needs_to_build = check_if_need_to_build(branch_name, config_file, flavor, git_access)
+    needs_to_build = check_if_need_to_build(branch_name, build_config, flavor, git_access)
     if needs_to_build:
-        log_path = Path(build_config.DEFAULT_OUTPUT_DIRECTORY) / "jobs" / "logs" / "main.log"
+        log_path = Path(DEFAULT_OUTPUT_DIRECTORY) / "jobs" / "logs" / "main.log"
         os.environ[luigi_log_config.LOG_ENV_VARIABLE_NAME] = f"{log_path.absolute()}"
 
         ci_build.build(flavor_path=flavor_path,
                        rebuild=rebuild,
                        build_docker_repository=docker_build_repository,
                        commit_sha=commit_sha,
                        docker_user=docker_user,
```

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_build.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_export.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_export.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_push.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_push.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_security_scan.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_step_output_printer.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_step_output_printer.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/ci_test.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_test.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/git_access.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/git_access.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/release.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/release.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import logging
 import os
 from pathlib import Path
 
+from exasol_integration_test_docker_environment.cli.options.system_options import DEFAULT_OUTPUT_DIRECTORY
 from exasol_integration_test_docker_environment.lib.base import luigi_log_config
-from exasol_integration_test_docker_environment.lib.config import build_config
 
 from exasol_script_languages_container_ci.lib.ci_build import CIBuild
 from exasol_script_languages_container_ci.lib.ci_push import CIPush
 from exasol_script_languages_container_ci.lib.ci_security_scan import CISecurityScan
 from exasol_script_languages_container_ci.lib.ci_test import CIExecuteTest
+from exasol_script_languages_container_ci.lib.config.config_data_model import Config
 from exasol_script_languages_container_ci.lib.release_uploader import ReleaseUploader
 
 
 def release(flavor: str,
             docker_user: str,
             docker_password: str,
             docker_release_repository: str,
-            config_file: str,
+            build_config: Config,
             source_repo_url: str,
             release_id: int,
             is_dry_run: bool,
             release_uploader: ReleaseUploader,
             ci_build: CIBuild = CIBuild(),
             ci_execute_tests: CIExecuteTest = CIExecuteTest(),
             ci_push: CIPush = CIPush(),
@@ -32,15 +33,15 @@
     3. Push to docker release repository
     4. Upload to GH release url
     """
     logging.info(f"Running Release build for parameters: {locals()}")
 
     flavor_path = (f"flavors/{flavor}",)
     test_container_folder = "test_container"
-    log_path = Path(build_config.DEFAULT_OUTPUT_DIRECTORY) / "jobs" / "logs" / "main.log"
+    log_path = Path(DEFAULT_OUTPUT_DIRECTORY) / "jobs" / "logs" / "main.log"
     os.environ[luigi_log_config.LOG_ENV_VARIABLE_NAME] = f"{log_path.absolute()}"
 
     ci_build.build(flavor_path=flavor_path, rebuild=True,
                    build_docker_repository=None,
                    commit_sha="",
                    docker_user=None,
                    docker_password=None,
```

### Comparing `exasol_script_languages_container_ci-1.2.0/exasol_script_languages_container_ci/lib/release_uploader.py` & `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/release_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.2.0/pyproject.toml` & `exasol_script_languages_container_ci-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exasol-script-languages-container-ci"
-version = "1.2.0"
+version = "1.3.0"
 description = "Implements CI builds for script-language-container."
 
 license = "MIT"
 
 authors = [
     "Thomas Uebensee <ext.thomas.uebensee@exasol.com>"
 ]
@@ -12,15 +12,16 @@
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4.0"
 click = "^8.0.3"
 GitPython = ">=3.1.0"
 exasol-script-languages-container-tool = "^0.18.0"
 exasol-integration-test-docker-environment = "^1.7.1"
 PyGithub = "^1.55.0"
-setuptools = "^67.6.0"
+setuptools = "^68.0.0"
+datamodel-code-generator = "^0.21.0"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dev-dependencies]
 toml = ">=0.10.2"
```

### Comparing `exasol_script_languages_container_ci-1.2.0/PKG-INFO` & `exasol_script_languages_container_ci-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: exasol-script-languages-container-ci
-Version: 1.2.0
+Version: 1.3.0
 Summary: Implements CI builds for script-language-container.
 License: MIT
 Author: Thomas Uebensee
 Author-email: ext.thomas.uebensee@exasol.com
 Requires-Python: >=3.8.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.0)
 Requires-Dist: PyGithub (>=1.55.0,<2.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
+Requires-Dist: datamodel-code-generator (>=0.21.0,<0.22.0)
 Requires-Dist: exasol-integration-test-docker-environment (>=1.7.1,<2.0.0)
 Requires-Dist: exasol-script-languages-container-tool (>=0.18.0,<0.19.0)
-Requires-Dist: setuptools (>=67.6.0,<68.0.0)
+Requires-Dist: setuptools (>=68.0.0,<69.0.0)
```

