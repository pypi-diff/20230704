# Comparing `tmp/akerbp.mlops-3.2.1a8.tar.gz` & `tmp/akerbp.mlops-3.2.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-3zvfa_n9/akerbp.mlops-3.2.1a8.tar", last modified: Tue Jul  4 11:38:20 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-i9kyos4c/akerbp.mlops-3.2.1a9.tar", last modified: Tue Jul  4 12:12:28 2023, max compression
```

## Comparing `akerbp.mlops-3.2.1a8.tar` & `akerbp.mlops-3.2.1a9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.763511 akerbp.mlops-3.2.1a8/
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-04 11:38:20.763511 akerbp.mlops-3.2.1a8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35467 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     4303 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.751511 akerbp.mlops-3.2.1a8/bitbucket_pipeline_helpers/
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/build.sh
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/increment_package_version.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/install.sh
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/mlops_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.755511 akerbp.mlops-3.2.1a8/model_artifact/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/model_artifact/README.md
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/model_artifact/mlpet_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.755511 akerbp.mlops-3.2.1a8/model_code/
--rw-rw-rw-   0 root         (0) root         (0)     9932 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/model_code/model.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/model_code/requirements.model
--rw-rw-rw-   0 root         (0) root         (0)     5427 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/model_code/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)     1643 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-04 11:38:20.763511 akerbp.mlops-3.2.1a8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.751511 akerbp.mlops-3.2.1a8/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.751511 akerbp.mlops-3.2.1a8/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.755511 akerbp.mlops-3.2.1a8/src/akerbp/mlops/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-04 11:38:20.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.755511 akerbp.mlops-3.2.1a8/src/akerbp/mlops/cdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/cdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/cdf/download_function_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/cdf/handler.py
--rw-rw-rw-   0 root         (0) root         (0)    38715 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/cdf/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.759511 akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16504 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/logger_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/mappings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.759511 akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     5828 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/deploy_prediction_service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/deploy_training_service.py
--rw-rw-rw-   0 root         (0) root         (0)    22199 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/platforms.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.759511 akerbp.mlops-3.2.1a8/src/akerbp/mlops/model_manager/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/model_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22835 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/model_manager/model_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.759511 akerbp.mlops-3.2.1a8/src/akerbp/mlops/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8630 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/services/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/services/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/src/akerbp/mlops/services/training.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.755511 akerbp.mlops-3.2.1a8/src/akerbp.mlops.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-04 11:38:20.000000 akerbp.mlops-3.2.1a8/src/akerbp.mlops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-07-04 11:38:20.000000 akerbp.mlops-3.2.1a8/src/akerbp.mlops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-04 11:38:20.000000 akerbp.mlops-3.2.1a8/src/akerbp.mlops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-04 11:38:20.000000 akerbp.mlops-3.2.1a8/src/akerbp.mlops.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-07-04 11:38:20.000000 akerbp.mlops-3.2.1a8/src/akerbp.mlops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-04 11:38:20.000000 akerbp.mlops-3.2.1a8/src/akerbp.mlops.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.759511 akerbp.mlops-3.2.1a8/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_data_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_install_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_metadata_validation.py
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 11:38:20.763511 akerbp.mlops-3.2.1a8/test/test_settings/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_settings/installing_reqs_in_venv.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_settings/multiple_models_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_settings/multiple_models_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_settings/single_model_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_settings/single_model_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_settings/single_model_missing_petrel_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_settings/single_model_no_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_settings/single_model_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3562 2023-07-04 11:37:50.000000 akerbp.mlops-3.2.1a8/test/test_version_increment.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.411518 akerbp.mlops-3.2.1a9/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-04 12:12:28.411518 akerbp.mlops-3.2.1a9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35467 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4303 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.399518 akerbp.mlops-3.2.1a9/bitbucket_pipeline_helpers/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/increment_package_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/install.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/mlops_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.399518 akerbp.mlops-3.2.1a9/model_artifact/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/model_artifact/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/model_artifact/mlpet_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.399518 akerbp.mlops-3.2.1a9/model_code/
+-rw-rw-rw-   0 root         (0) root         (0)     9932 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/model_code/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/model_code/requirements.model
+-rw-rw-rw-   0 root         (0) root         (0)     5427 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/model_code/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1643 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-04 12:12:28.411518 akerbp.mlops-3.2.1a9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.395518 akerbp.mlops-3.2.1a9/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.395518 akerbp.mlops-3.2.1a9/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.403518 akerbp.mlops-3.2.1a9/src/akerbp/mlops/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-04 12:12:28.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.403518 akerbp.mlops-3.2.1a9/src/akerbp/mlops/cdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/cdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/cdf/download_function_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/cdf/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    38715 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/cdf/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.403518 akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16504 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/logger_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/mappings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.407518 akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5828 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/deploy_prediction_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/deploy_training_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    22257 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/platforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.407518 akerbp.mlops-3.2.1a9/src/akerbp/mlops/model_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/model_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22835 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/model_manager/model_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.407518 akerbp.mlops-3.2.1a9/src/akerbp/mlops/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8630 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/services/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/services/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/src/akerbp/mlops/services/training.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.403518 akerbp.mlops-3.2.1a9/src/akerbp.mlops.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-04 12:12:28.000000 akerbp.mlops-3.2.1a9/src/akerbp.mlops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-07-04 12:12:28.000000 akerbp.mlops-3.2.1a9/src/akerbp.mlops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-04 12:12:28.000000 akerbp.mlops-3.2.1a9/src/akerbp.mlops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-04 12:12:28.000000 akerbp.mlops-3.2.1a9/src/akerbp.mlops.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-07-04 12:12:28.000000 akerbp.mlops-3.2.1a9/src/akerbp.mlops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-04 12:12:28.000000 akerbp.mlops-3.2.1a9/src/akerbp.mlops.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.407518 akerbp.mlops-3.2.1a9/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_data_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_install_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_metadata_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-04 12:12:28.411518 akerbp.mlops-3.2.1a9/test/test_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_settings/installing_reqs_in_venv.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_settings/multiple_models_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_settings/multiple_models_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_settings/single_model_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_settings/single_model_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_settings/single_model_missing_petrel_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_settings/single_model_no_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_settings/single_model_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3562 2023-07-04 12:12:00.000000 akerbp.mlops-3.2.1a9/test/test_version_increment.py
```

### Comparing `akerbp.mlops-3.2.1a8/.flake8` & `akerbp.mlops-3.2.1a9/.flake8`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/.pre-commit-config.yaml` & `akerbp.mlops-3.2.1a9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/LICENSE` & `akerbp.mlops-3.2.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/PKG-INFO` & `akerbp.mlops-3.2.1a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.2.1a8
+Version: 3.2.1a9
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.2.1a8/README.md` & `akerbp.mlops-3.2.1a9/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.1a9/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/build.sh` & `akerbp.mlops-3.2.1a9/build.sh`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/increment_package_version.py` & `akerbp.mlops-3.2.1a9/increment_package_version.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/mlops_settings.yaml` & `akerbp.mlops-3.2.1a9/mlops_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/model_code/model.py` & `akerbp.mlops-3.2.1a9/model_code/model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/model_code/test_model.py` & `akerbp.mlops-3.2.1a9/model_code/test_model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/pyproject.toml` & `akerbp.mlops-3.2.1a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/cdf/handler.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/cdf/handler.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/cdf/helpers.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/cdf/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/config.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/exceptions.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/helpers.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/logger.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/logger.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/logger_config.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/logger_config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/core/mappings.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/core/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/deploy.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/helpers.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,21 +521,23 @@
     # Run unit tests and get test payload before deploying
     logger.info(
         f"Running tests for model {c.human_friendly_model_name} before deploying to {env}"
     )
     setup_venv = kwargs.pop("setup_venv", False)
     if setup_venv:
         test_payload, venv_dir = run_tests(c, setup_venv=setup_venv)
+        deployment_folder_content = get_deployment_folder_content(
+            deployment_folder=Path("."), venv_dir=Path(venv_dir)
+        )
     else:
         test_payload = run_tests(c, setup_venv=setup_venv)
+        deployment_folder_content = get_deployment_folder_content(
+            deployment_folder=Path(".")
+        )
 
-    # Log deployment folder content - at this point we are already inside the deployment folder
-    deployment_folder_content = get_deployment_folder_content(
-        deployment_folder=Path(".")
-    )
     logger.info(
         f"Deployment folder '{deployment_folder}' now contains the following: {deployment_folder_content}"
     )
     external_id = function_name
     platform = c.platform
     deploy_function, _, test_function = platform_methods[platform]
     logger.info(f"Starting deployment of model {c.model_name} to {env}")
```

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/platforms.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/platforms.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/deployment/setup.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/deployment/setup.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/model_manager/model_manager.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/model_manager/model_manager.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/services/prediction.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/services/prediction.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/services/test_service.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/services/test_service.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp/mlops/services/training.py` & `akerbp.mlops-3.2.1a9/src/akerbp/mlops/services/training.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp.mlops.egg-info/PKG-INFO` & `akerbp.mlops-3.2.1a9/src/akerbp.mlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.2.1a8
+Version: 3.2.1a9
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.2.1a8/src/akerbp.mlops.egg-info/SOURCES.txt` & `akerbp.mlops-3.2.1a9/src/akerbp.mlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_data_validation.py` & `akerbp.mlops-3.2.1a9/test/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_install_requirements.py` & `akerbp.mlops-3.2.1a9/test/test_install_requirements.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_metadata_validation.py` & `akerbp.mlops-3.2.1a9/test/test_metadata_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_settings/installing_reqs_in_venv.yaml` & `akerbp.mlops-3.2.1a9/test/test_settings/installing_reqs_in_venv.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_settings/multiple_models_all_required_fields.yaml` & `akerbp.mlops-3.2.1a9/test/test_settings/multiple_models_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_settings/multiple_models_missing_field.yaml` & `akerbp.mlops-3.2.1a9/test/test_settings/multiple_models_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_settings/single_model_all_required_fields.yaml` & `akerbp.mlops-3.2.1a9/test/test_settings/single_model_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_settings/single_model_missing_field.yaml` & `akerbp.mlops-3.2.1a9/test/test_settings/single_model_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_settings/single_model_missing_petrel_field.yaml` & `akerbp.mlops-3.2.1a9/test/test_settings/single_model_missing_petrel_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_settings/single_model_no_required_input.yaml` & `akerbp.mlops-3.2.1a9/test/test_settings/single_model_no_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_settings/single_model_required_input.yaml` & `akerbp.mlops-3.2.1a9/test/test_settings/single_model_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a8/test/test_version_increment.py` & `akerbp.mlops-3.2.1a9/test/test_version_increment.py`

 * *Files identical despite different names*

