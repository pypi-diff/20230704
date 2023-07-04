# Comparing `tmp/akerbp.mlops-3.2.1a2.tar.gz` & `tmp/akerbp.mlops-3.2.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-fyic18c8/akerbp.mlops-3.2.1a2.tar", last modified: Wed Jun 28 12:09:31 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-pi4ck2bb/akerbp.mlops-3.2.1a5.tar", last modified: Mon Jul  3 13:12:01 2023, max compression
```

## Comparing `akerbp.mlops-3.2.1a2.tar` & `akerbp.mlops-3.2.1a5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.080246 akerbp.mlops-3.2.1a2/
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    48989 2023-06-28 12:09:31.080246 akerbp.mlops-3.2.1a2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35467 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     4229 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.072246 akerbp.mlops-3.2.1a2/bitbucket_pipeline_helpers/
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1247 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/build.sh
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/increment_package_version.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/install.sh
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/mlops_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.072246 akerbp.mlops-3.2.1a2/model_artifact/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/model_artifact/README.md
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/model_artifact/mlpet_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.072246 akerbp.mlops-3.2.1a2/model_code/
--rw-rw-rw-   0 root         (0) root         (0)     9932 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/model_code/model.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/model_code/requirements.model
--rw-rw-rw-   0 root         (0) root         (0)     5427 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/model_code/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-28 12:09:31.080246 akerbp.mlops-3.2.1a2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.068246 akerbp.mlops-3.2.1a2/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.068246 akerbp.mlops-3.2.1a2/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.072246 akerbp.mlops-3.2.1a2/src/akerbp/mlops/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-28 12:09:30.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.072246 akerbp.mlops-3.2.1a2/src/akerbp/mlops/cdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/cdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/cdf/download_function_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/cdf/handler.py
--rw-rw-rw-   0 root         (0) root         (0)    38715 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/cdf/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.076246 akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16504 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/logger_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/mappings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.076246 akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     5828 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/deploy_prediction_service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/deploy_training_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21239 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/platforms.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.076246 akerbp.mlops-3.2.1a2/src/akerbp/mlops/model_manager/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/model_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22835 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/model_manager/model_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.076246 akerbp.mlops-3.2.1a2/src/akerbp/mlops/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8607 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/services/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/services/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/src/akerbp/mlops/services/training.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.072246 akerbp.mlops-3.2.1a2/src/akerbp.mlops.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    48989 2023-06-28 12:09:31.000000 akerbp.mlops-3.2.1a2/src/akerbp.mlops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-06-28 12:09:31.000000 akerbp.mlops-3.2.1a2/src/akerbp.mlops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-28 12:09:31.000000 akerbp.mlops-3.2.1a2/src/akerbp.mlops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-28 12:09:31.000000 akerbp.mlops-3.2.1a2/src/akerbp.mlops.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-28 12:09:31.000000 akerbp.mlops-3.2.1a2/src/akerbp.mlops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-06-28 12:09:31.000000 akerbp.mlops-3.2.1a2/src/akerbp.mlops.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.076246 akerbp.mlops-3.2.1a2/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_data_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_install_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_metadata_validation.py
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 12:09:31.080246 akerbp.mlops-3.2.1a2/test/test_settings/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_settings/installing_reqs_in_venv.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_settings/multiple_models_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_settings/multiple_models_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_settings/single_model_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_settings/single_model_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_settings/single_model_missing_petrel_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_settings/single_model_no_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_settings/single_model_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3562 2023-06-28 12:08:59.000000 akerbp.mlops-3.2.1a2/test/test_version_increment.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35467 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4303 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.709831 akerbp.mlops-3.2.1a5/bitbucket_pipeline_helpers/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/increment_package_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/install.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/mlops_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.713832 akerbp.mlops-3.2.1a5/model_artifact/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/model_artifact/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/model_artifact/mlpet_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.713832 akerbp.mlops-3.2.1a5/model_code/
+-rw-rw-rw-   0 root         (0) root         (0)     9932 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/model_code/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/model_code/requirements.model
+-rw-rw-rw-   0 root         (0) root         (0)     5427 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/model_code/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.705831 akerbp.mlops-3.2.1a5/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.705831 akerbp.mlops-3.2.1a5/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.713832 akerbp.mlops-3.2.1a5/src/akerbp/mlops/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.713832 akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/download_function_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    38715 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.717831 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16504 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/logger_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/mappings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.717831 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5828 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/deploy_prediction_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/deploy_training_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    21411 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/platforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.717831 akerbp.mlops-3.2.1a5/src/akerbp/mlops/model_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/model_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22835 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/model_manager/model_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8620 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/training.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.713832 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_data_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_install_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_metadata_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/test/test_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/installing_reqs_in_venv.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/multiple_models_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/multiple_models_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/single_model_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/single_model_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/single_model_missing_petrel_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/single_model_no_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/single_model_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3562 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_version_increment.py
```

### Comparing `akerbp.mlops-3.2.1a2/.flake8` & `akerbp.mlops-3.2.1a5/.flake8`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/.pre-commit-config.yaml` & `akerbp.mlops-3.2.1a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/LICENSE` & `akerbp.mlops-3.2.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/PKG-INFO` & `akerbp.mlops-3.2.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.2.1a2
+Version: 3.2.1a5
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.2.1a2/README.md` & `akerbp.mlops-3.2.1a5/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.1a5/bitbucket-pipelines.yml`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
       - step:
           name: Promote Artifacts to Test and Prod
           script:
             - *set-environment-dev
             - *install-mlops
             - python bitbucket_pipeline_helpers/upload_dummy_artifacts.py
             - python bitbucket_pipeline_helpers/promote_dummy_artifacts.py
+            - python bitbucket_pipeline_helpers/remove_dummy_artifacts.py
             - *set-environment-test
             - python bitbucket_pipeline_helpers/promote_dummy_artifacts.py
       - step:
           <<: *deploy-dev-prediction-service
           name: Deploy Prediction Service to Test
           deployment: test-prediction
       - step:
```

### Comparing `akerbp.mlops-3.2.1a2/build.sh` & `akerbp.mlops-3.2.1a5/build.sh`

 * *Files 15% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 
     # Build and upload if new tag was applied (or prod)
     if [ "$MODEL_ENV" = "test" ] || [ "$MODEL_ENV" = "prod" ]
     then
         echo "Tag release"
         tag=$(python increment_package_version.py);
         commit=$(git rev-parse --short HEAD);
-        git tag -d $tag
-        git push origin :refs/tags/$tag
         git tag $tag $commit
         git push origin --tags
         echo "Build package"
         python -m build
         echo "Upload package"
         python -m twine upload \
             --disable-progress-bar \
```

### Comparing `akerbp.mlops-3.2.1a2/increment_package_version.py` & `akerbp.mlops-3.2.1a5/increment_package_version.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/mlops_settings.yaml` & `akerbp.mlops-3.2.1a5/mlops_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/model_code/model.py` & `akerbp.mlops-3.2.1a5/model_code/model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/model_code/test_model.py` & `akerbp.mlops-3.2.1a5/model_code/test_model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/pyproject.toml` & `akerbp.mlops-3.2.1a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/cdf/handler.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/handler.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/cdf/helpers.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/config.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/exceptions.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/helpers.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/logger.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/logger.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/logger_config.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/logger_config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/core/mappings.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/deploy.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/helpers.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -477,20 +477,19 @@
                 logger.info(log_line.strip())
         if failed_test:
             raise TestError("Unit tests failed :( See the above traceback")
         if model_input is None and deploy:
             raise TestError(
                 "Test was not able to extract the payload for downstream testing of deployed model"
             )
-        if setup_venv:
-            delete_venv(venv_name=venv_dir.split("/")[-1])
-            logger.info("Ephemeral virtual environment deleted")
         logger.info("Unit tests passed :)")
-
-        return model_input
+        if setup_venv:
+            return model_input, venv_dir
+        else:
+            return model_input
     else:
         logger.warning(
             "No test file specified in 'mlops_settings.yaml', skipping tests"
         )
         return {}
 
 
@@ -504,15 +503,18 @@
     **kwargs,
 ) -> None:
     # Run unit tests and get test payload before deploying
     logger.info(
         f"Running tests for model {c.human_friendly_model_name} before deploying to {env}"
     )
     setup_venv = kwargs.pop("setup_venv", False)
-    test_payload = run_tests(c, setup_venv=setup_venv)
+    if setup_venv:
+        test_payload, venv_dir = run_tests(c, setup_venv=setup_venv)
+    else:
+        test_payload = run_tests(c, setup_venv=setup_venv)
 
     # Log deployment folder content - at this point we are already inside the deployment folder
     deployment_folder_content = get_deployment_folder_content(
         deployment_folder=Path(".")
     )
     logger.info(
         f"Deployment folder '{deployment_folder}' now contains the following: {deployment_folder_content}"
@@ -593,14 +595,18 @@
         cdf.garbage_collection(
             c,
             function_name,
             env,
             remove_artifacts=c.model_name == "mlopsdemo",
         )
 
+    if setup_venv:
+        delete_venv(venv_name=venv_dir.split("/")[-1])
+        logger.info("Ephemeral virtual environment deleted")
+
 
 def redeploy_model_with_numbered_external_id(
     c: ServiceSettings,
     numbered_external_id: str,
     test_payload: Any,
     info: Dict[str, Union[str, Dict[str, str]]],
     platform_methods: Dict = platform_methods,
```

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/platforms.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/platforms.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/deployment/setup.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/setup.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/model_manager/model_manager.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/model_manager/model_manager.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/services/prediction.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/prediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             mlops_helpers.client_secrets = secrets
             mlops_helpers.set_up_cdf_client(context="write")
         logger.info("Initializing model")
         initialization(secrets)
         logger.info("Model initialized")
 
         try:
-            skip_input_validation = eval(
+            skip_input_validation = ast.literal_eval(
                 c.info["prediction"]["metadata"]["supports_external_retrieval"]
             )
         except KeyError as e:
             raise MissingFieldError(
                 "Field 'supports_external_retrieval' is missing from the metadata specification in mlops_settings.yaml"
             ) from e
         if skip_input_validation:
@@ -101,14 +101,15 @@
         y = predict(data, init_object, secrets)  # type: ignore
         logger.info("Predictions obtained")
         write_predictions_to_file = data.get("return_file", False)
         if write_predictions_to_file:
             logger.info("Writing predictions to file")
             if platform == "cdf":
                 import base64
+
                 public_key = data.get("public_key", None)
                 content = str(json.dumps(y))
                 data_encrypted = False
                 if public_key is None:
                     logger.warning(
                         "Public key is not provided. The predictions will not be encrypted. This is not recommended!"
                     )
```

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/services/test_service.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/test_service.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp/mlops/services/training.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/training.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp.mlops.egg-info/PKG-INFO` & `akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.2.1a2
+Version: 3.2.1a5
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.2.1a2/src/akerbp.mlops.egg-info/SOURCES.txt` & `akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_data_validation.py` & `akerbp.mlops-3.2.1a5/test/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_install_requirements.py` & `akerbp.mlops-3.2.1a5/test/test_install_requirements.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_metadata_validation.py` & `akerbp.mlops-3.2.1a5/test/test_metadata_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_settings/installing_reqs_in_venv.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/installing_reqs_in_venv.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_settings/multiple_models_all_required_fields.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/multiple_models_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_settings/multiple_models_missing_field.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/multiple_models_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_settings/single_model_all_required_fields.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/single_model_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_settings/single_model_missing_field.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/single_model_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_settings/single_model_missing_petrel_field.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/single_model_missing_petrel_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_settings/single_model_no_required_input.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/single_model_no_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_settings/single_model_required_input.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/single_model_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a2/test/test_version_increment.py` & `akerbp.mlops-3.2.1a5/test/test_version_increment.py`

 * *Files identical despite different names*

