# Comparing `tmp/akerbp.mlops-3.2.1a6.tar.gz` & `tmp/akerbp.mlops-3.2.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-nx3tpugt/akerbp.mlops-3.2.1a6.tar", last modified: Mon Jul  3 13:20:15 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-w_6dzn6n/akerbp.mlops-3.2.1a7.tar", last modified: Mon Jul  3 13:51:14 2023, max compression
```

## Comparing `akerbp.mlops-3.2.1a6.tar` & `akerbp.mlops-3.2.1a7.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.326672 akerbp.mlops-3.2.1a6/
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-03 13:20:15.322672 akerbp.mlops-3.2.1a6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35467 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     4303 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.314672 akerbp.mlops-3.2.1a6/bitbucket_pipeline_helpers/
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/build.sh
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/increment_package_version.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/install.sh
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/mlops_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.314672 akerbp.mlops-3.2.1a6/model_artifact/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/model_artifact/README.md
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/model_artifact/mlpet_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.314672 akerbp.mlops-3.2.1a6/model_code/
--rw-rw-rw-   0 root         (0) root         (0)     9932 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/model_code/model.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/model_code/requirements.model
--rw-rw-rw-   0 root         (0) root         (0)     5427 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/model_code/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-03 13:20:15.326672 akerbp.mlops-3.2.1a6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.310671 akerbp.mlops-3.2.1a6/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.310671 akerbp.mlops-3.2.1a6/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.314672 akerbp.mlops-3.2.1a6/src/akerbp/mlops/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-03 13:20:15.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.318672 akerbp.mlops-3.2.1a6/src/akerbp/mlops/cdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/cdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/cdf/download_function_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/cdf/handler.py
--rw-rw-rw-   0 root         (0) root         (0)    38715 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/cdf/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.318672 akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16504 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/logger_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/mappings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.318672 akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     5828 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/deploy_prediction_service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/deploy_training_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21411 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/platforms.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.322672 akerbp.mlops-3.2.1a6/src/akerbp/mlops/model_manager/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/model_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22835 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/model_manager/model_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.322672 akerbp.mlops-3.2.1a6/src/akerbp/mlops/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8625 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/services/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/services/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/src/akerbp/mlops/services/training.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.314672 akerbp.mlops-3.2.1a6/src/akerbp.mlops.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-03 13:20:15.000000 akerbp.mlops-3.2.1a6/src/akerbp.mlops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-07-03 13:20:15.000000 akerbp.mlops-3.2.1a6/src/akerbp.mlops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-03 13:20:15.000000 akerbp.mlops-3.2.1a6/src/akerbp.mlops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-03 13:20:15.000000 akerbp.mlops-3.2.1a6/src/akerbp.mlops.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-03 13:20:15.000000 akerbp.mlops-3.2.1a6/src/akerbp.mlops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-03 13:20:15.000000 akerbp.mlops-3.2.1a6/src/akerbp.mlops.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.322672 akerbp.mlops-3.2.1a6/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_data_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_install_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_metadata_validation.py
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:20:15.322672 akerbp.mlops-3.2.1a6/test/test_settings/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_settings/installing_reqs_in_venv.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_settings/multiple_models_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_settings/multiple_models_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_settings/single_model_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_settings/single_model_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_settings/single_model_missing_petrel_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_settings/single_model_no_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_settings/single_model_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3562 2023-07-03 13:19:53.000000 akerbp.mlops-3.2.1a6/test/test_version_increment.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.699759 akerbp.mlops-3.2.1a7/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-03 13:51:14.695759 akerbp.mlops-3.2.1a7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35467 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4303 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.687759 akerbp.mlops-3.2.1a7/bitbucket_pipeline_helpers/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/increment_package_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/install.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/mlops_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.691759 akerbp.mlops-3.2.1a7/model_artifact/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/model_artifact/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/model_artifact/mlpet_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.691759 akerbp.mlops-3.2.1a7/model_code/
+-rw-rw-rw-   0 root         (0) root         (0)     9932 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/model_code/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/model_code/requirements.model
+-rw-rw-rw-   0 root         (0) root         (0)     5427 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/model_code/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1643 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-03 13:51:14.699759 akerbp.mlops-3.2.1a7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.687759 akerbp.mlops-3.2.1a7/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.687759 akerbp.mlops-3.2.1a7/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.691759 akerbp.mlops-3.2.1a7/src/akerbp/mlops/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-03 13:51:14.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.691759 akerbp.mlops-3.2.1a7/src/akerbp/mlops/cdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/cdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/cdf/download_function_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/cdf/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    38715 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/cdf/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.691759 akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16504 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/logger_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/mappings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.695759 akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5828 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/deploy_prediction_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/deploy_training_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    21411 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/platforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.695759 akerbp.mlops-3.2.1a7/src/akerbp/mlops/model_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/model_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22835 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/model_manager/model_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.695759 akerbp.mlops-3.2.1a7/src/akerbp/mlops/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8630 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/services/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/services/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/src/akerbp/mlops/services/training.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.691759 akerbp.mlops-3.2.1a7/src/akerbp.mlops.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-03 13:51:14.000000 akerbp.mlops-3.2.1a7/src/akerbp.mlops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-07-03 13:51:14.000000 akerbp.mlops-3.2.1a7/src/akerbp.mlops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-03 13:51:14.000000 akerbp.mlops-3.2.1a7/src/akerbp.mlops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-03 13:51:14.000000 akerbp.mlops-3.2.1a7/src/akerbp.mlops.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-07-03 13:51:14.000000 akerbp.mlops-3.2.1a7/src/akerbp.mlops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-03 13:51:14.000000 akerbp.mlops-3.2.1a7/src/akerbp.mlops.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.695759 akerbp.mlops-3.2.1a7/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_data_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_install_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_metadata_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:51:14.695759 akerbp.mlops-3.2.1a7/test/test_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_settings/installing_reqs_in_venv.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_settings/multiple_models_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_settings/multiple_models_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_settings/single_model_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_settings/single_model_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_settings/single_model_missing_petrel_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_settings/single_model_no_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_settings/single_model_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3562 2023-07-03 13:50:50.000000 akerbp.mlops-3.2.1a7/test/test_version_increment.py
```

### Comparing `akerbp.mlops-3.2.1a6/.flake8` & `akerbp.mlops-3.2.1a7/.flake8`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/.pre-commit-config.yaml` & `akerbp.mlops-3.2.1a7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/LICENSE` & `akerbp.mlops-3.2.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/PKG-INFO` & `akerbp.mlops-3.2.1a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.2.1a6
+Version: 3.2.1a7
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.2.1a6/README.md` & `akerbp.mlops-3.2.1a7/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.1a7/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/build.sh` & `akerbp.mlops-3.2.1a7/build.sh`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/increment_package_version.py` & `akerbp.mlops-3.2.1a7/increment_package_version.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/mlops_settings.yaml` & `akerbp.mlops-3.2.1a7/mlops_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/model_code/model.py` & `akerbp.mlops-3.2.1a7/model_code/model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/model_code/test_model.py` & `akerbp.mlops-3.2.1a7/model_code/test_model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/pyproject.toml` & `akerbp.mlops-3.2.1a7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 dependencies = [
     "pytest>=6.1.1",
-    "pydantic>=1.7.3",
+    "pydantic>=1.7.3, <2",
     "PyYAML>=5.4.1",
     "setuptools>50.3.0", # nodeenv a dependency of one of our dependencies is installing an old version of setuptools that snyk doesn't like
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
```

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/cdf/handler.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/cdf/handler.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/cdf/helpers.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/cdf/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/config.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/exceptions.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/helpers.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/logger.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/logger.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/logger_config.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/logger_config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/core/mappings.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/core/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/deploy.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/helpers.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/platforms.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/platforms.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/deployment/setup.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/deployment/setup.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/model_manager/model_manager.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/model_manager/model_manager.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/services/prediction.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/services/prediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             )
             logger.info(
                 "Call predict on the initialized model using the retrieved data"
             )
         else:
             logger.info("Performing input data validation")
             required_input = ast.literal_eval(
-                c.info["prediction"]["metadata"]["required_input"]
+                str(c.info["prediction"]["metadata"]["required_input"])
             )
             is_input_data_valid = input_data_validation(
                 required_input=required_input, input=data
             )
             if is_input_data_valid:
                 logger.info("Input data successfully validated")
             else:
```

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/services/test_service.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/services/test_service.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp/mlops/services/training.py` & `akerbp.mlops-3.2.1a7/src/akerbp/mlops/services/training.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp.mlops.egg-info/PKG-INFO` & `akerbp.mlops-3.2.1a7/src/akerbp.mlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.2.1a6
+Version: 3.2.1a7
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.2.1a6/src/akerbp.mlops.egg-info/SOURCES.txt` & `akerbp.mlops-3.2.1a7/src/akerbp.mlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_data_validation.py` & `akerbp.mlops-3.2.1a7/test/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_install_requirements.py` & `akerbp.mlops-3.2.1a7/test/test_install_requirements.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_metadata_validation.py` & `akerbp.mlops-3.2.1a7/test/test_metadata_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_settings/installing_reqs_in_venv.yaml` & `akerbp.mlops-3.2.1a7/test/test_settings/installing_reqs_in_venv.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_settings/multiple_models_all_required_fields.yaml` & `akerbp.mlops-3.2.1a7/test/test_settings/multiple_models_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_settings/multiple_models_missing_field.yaml` & `akerbp.mlops-3.2.1a7/test/test_settings/multiple_models_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_settings/single_model_all_required_fields.yaml` & `akerbp.mlops-3.2.1a7/test/test_settings/single_model_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_settings/single_model_missing_field.yaml` & `akerbp.mlops-3.2.1a7/test/test_settings/single_model_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_settings/single_model_missing_petrel_field.yaml` & `akerbp.mlops-3.2.1a7/test/test_settings/single_model_missing_petrel_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_settings/single_model_no_required_input.yaml` & `akerbp.mlops-3.2.1a7/test/test_settings/single_model_no_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_settings/single_model_required_input.yaml` & `akerbp.mlops-3.2.1a7/test/test_settings/single_model_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a6/test/test_version_increment.py` & `akerbp.mlops-3.2.1a7/test/test_version_increment.py`

 * *Files identical despite different names*

