# Comparing `tmp/encord-0.1.84.tar.gz` & `tmp/encord-0.1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.84.tar", max compression
+gzip compressed data, was "encord-0.1.85.tar", max compression
```

## Comparing `encord-0.1.84.tar` & `encord-0.1.85.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0    11330 2023-07-03 15:48:01.847013 encord-0.1.84/LICENSE
--rw-r--r--   0        0        0     2037 2023-07-03 15:48:01.847013 encord-0.1.84/README.md
--rw-r--r--   0        0        0       84 2023-07-03 15:48:01.847013 encord-0.1.84/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-07-03 15:48:01.867013 encord-0.1.84/encord/__init__.py
--rw-r--r--   0        0        0      240 2023-07-03 15:48:01.867013 encord-0.1.84/encord/_version.py
--rw-r--r--   0        0        0    49540 2023-07-03 15:48:01.867013 encord-0.1.84/encord/client.py
--rw-r--r--   0        0        0        0 2023-07-03 15:48:01.867013 encord-0.1.84/encord/common/__init__.py
--rw-r--r--   0        0        0       45 2023-07-03 15:48:01.867013 encord-0.1.84/encord/common/constants.py
--rw-r--r--   0        0        0      464 2023-07-03 15:48:01.867013 encord-0.1.84/encord/common/enum.py
--rw-r--r--   0        0        0    10852 2023-07-03 15:48:01.867013 encord-0.1.84/encord/configs.py
--rw-r--r--   0        0        0        0 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/__init__.py
--rw-r--r--   0        0        0      866 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/enums.py
--rw-r--r--   0        0        0     3196 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/model.py
--rw-r--r--   0        0        0     4522 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-07-03 15:48:01.867013 encord-0.1.84/encord/dataset.py
--rw-r--r--   0        0        0     6355 2023-07-03 15:48:01.867013 encord-0.1.84/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/bundle.py
--rw-r--r--   0        0        0      319 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/common.py
--rw-r--r--   0        0        0      535 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/limits.py
--rw-r--r--   0        0        0     7870 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/querier.py
--rw-r--r--   0        0        0      747 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/query_methods.py
--rw-r--r--   0        0        0     1738 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/utils.py
--rw-r--r--   0        0        0        0 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/v2/__init__.py
--rw-r--r--   0        0        0     3447 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/v2/api_client.py
--rw-r--r--   0        0        0      964 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/v2/error_utils.py
--rw-r--r--   0        0        0      216 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/v2/payloads.py
--rw-r--r--   0        0        0     2249 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/v2/request_signer.py
--rw-r--r--   0        0        0      340 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/__init__.py
--rw-r--r--   0        0        0     5164 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/bitmask.py
--rw-r--r--   0        0        0      182 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/classification.py
--rw-r--r--   0        0        0    31763 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/common.py
--rw-r--r--   0        0        0      151 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/constants.py
--rw-r--r--   0        0        0     5748 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3461 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/frames.py
--rw-r--r--   0        0        0    21521 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   144757 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      174 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      185 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/project.py
--rw-r--r--   0        0        0     1504 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-07-03 15:48:01.867013 encord-0.1.84/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/__init__.py
--rw-r--r--   0        0        0      932 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/analytics.py
--rw-r--r--   0        0        0      982 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/api_key.py
--rw-r--r--   0        0        0      626 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/base_dto/__init__.py
--rw-r--r--   0        0        0      337 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/base_dto/base_dto_interface.py
--rw-r--r--   0        0        0     1418 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/base_dto/base_dto_pydantic_v1.py
--rw-r--r--   0        0        0     1366 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/base_dto/base_dto_pydantic_v2.py
--rw-r--r--   0        0        0     5335 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32857 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/dataset.py
--rw-r--r--   0        0        0      829 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      256 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/formatter.py
--rw-r--r--   0        0        0     1146 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/label_log.py
--rw-r--r--   0        0        0    11889 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6679 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/model.py
--rw-r--r--   0        0        0      874 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/ontology.py
--rw-r--r--   0        0        0     8658 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0      314 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/workflow.py
--rw-r--r--   0        0        0    41298 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project.py
--rw-r--r--   0        0        0        0 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    29244 2023-07-03 15:48:01.871013 encord-0.1.84/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1966 2023-07-03 15:48:01.871013 encord-0.1.84/pyproject.toml
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 encord-0.1.84/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-07-04 16:11:17.923206 encord-0.1.85/LICENSE
+-rw-r--r--   0        0        0     2037 2023-07-04 16:11:17.923206 encord-0.1.85/README.md
+-rw-r--r--   0        0        0       84 2023-07-04 16:11:17.923206 encord-0.1.85/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-04 16:11:17.939206 encord-0.1.85/encord/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-04 16:11:17.939206 encord-0.1.85/encord/_version.py
+-rw-r--r--   0        0        0    49540 2023-07-04 16:11:17.939206 encord-0.1.85/encord/client.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/common/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-04 16:11:17.939206 encord-0.1.85/encord/common/constants.py
+-rw-r--r--   0        0        0      464 2023-07-04 16:11:17.939206 encord-0.1.85/encord/common/enum.py
+-rw-r--r--   0        0        0    10852 2023-07-04 16:11:17.939206 encord-0.1.85/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/__init__.py
+-rw-r--r--   0        0        0      866 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/enums.py
+-rw-r--r--   0        0        0     3196 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/model.py
+-rw-r--r--   0        0        0     4522 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-07-04 16:11:17.939206 encord-0.1.85/encord/dataset.py
+-rw-r--r--   0        0        0     6355 2023-07-04 16:11:17.939206 encord-0.1.85/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/bundle.py
+-rw-r--r--   0        0        0      319 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/common.py
+-rw-r--r--   0        0        0      535 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/limits.py
+-rw-r--r--   0        0        0     7870 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/querier.py
+-rw-r--r--   0        0        0      747 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1738 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/utils.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/v2/__init__.py
+-rw-r--r--   0        0        0     3447 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/v2/api_client.py
+-rw-r--r--   0        0        0      964 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/v2/error_utils.py
+-rw-r--r--   0        0        0      216 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/v2/payloads.py
+-rw-r--r--   0        0        0     2249 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/v2/request_signer.py
+-rw-r--r--   0        0        0      340 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/__init__.py
+-rw-r--r--   0        0        0     5164 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/bitmask.py
+-rw-r--r--   0        0        0      182 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/classification.py
+-rw-r--r--   0        0        0    21796 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/common.py
+-rw-r--r--   0        0        0      151 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/constants.py
+-rw-r--r--   0        0        0     5748 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3461 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/frames.py
+-rw-r--r--   0        0        0    21928 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   140254 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      174 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      185 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/project.py
+-rw-r--r--   0        0        0     1622 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-07-04 16:11:17.939206 encord-0.1.85/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/analytics.py
+-rw-r--r--   0        0        0      982 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/api_key.py
+-rw-r--r--   0        0        0      626 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/base_dto/__init__.py
+-rw-r--r--   0        0        0      337 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/base_dto/base_dto_interface.py
+-rw-r--r--   0        0        0     1418 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/base_dto/base_dto_pydantic_v1.py
+-rw-r--r--   0        0        0     1366 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/base_dto/base_dto_pydantic_v2.py
+-rw-r--r--   0        0        0     5335 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32857 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/dataset.py
+-rw-r--r--   0        0        0      829 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      256 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1241 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11889 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6679 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/model.py
+-rw-r--r--   0        0        0      874 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8658 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0      314 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/workflow.py
+-rw-r--r--   0        0        0    41304 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    29244 2023-07-04 16:11:17.943206 encord-0.1.85/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1966 2023-07-04 16:11:17.943206 encord-0.1.85/pyproject.toml
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 encord-0.1.85/PKG-INFO
```

### Comparing `encord-0.1.84/LICENSE` & `encord-0.1.85/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/README.md` & `encord-0.1.85/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/client.py` & `encord-0.1.85/encord/client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/configs.py` & `encord-0.1.85/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/constants/enums.py` & `encord-0.1.85/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/constants/model.py` & `encord-0.1.85/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/constants/model_weights.py` & `encord-0.1.85/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/constants/string_constants.py` & `encord-0.1.85/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/constants/test/test_enums.py` & `encord-0.1.85/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/dataset.py` & `encord-0.1.85/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/exceptions.py` & `encord-0.1.85/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/http/bundle.py` & `encord-0.1.85/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/http/constants.py` & `encord-0.1.85/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/http/error_utils.py` & `encord-0.1.85/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/http/querier.py` & `encord-0.1.85/encord/http/querier.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/http/query_methods.py` & `encord-0.1.85/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/http/request.py` & `encord-0.1.85/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/http/utils.py` & `encord-0.1.85/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/http/v2/api_client.py` & `encord-0.1.85/encord/http/v2/api_client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/http/v2/error_utils.py` & `encord-0.1.85/encord/http/v2/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/http/v2/request_signer.py` & `encord-0.1.85/encord/http/v2/request_signer.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/objects/bitmask.py` & `encord-0.1.85/encord/objects/bitmask.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/objects/common.py` & `encord-0.1.85/encord/objects/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,22 +12,24 @@
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
+    cast,
 )
 
 from encord.common.enum import StringEnum
 from encord.exceptions import OntologyError
 from encord.objects.utils import (
     _decode_nested_uid,
     check_type,
-    filter_by_type,
+    checked_cast,
+    does_type_match,
     short_uuid_str,
 )
 
 NestedID = List[int]
 
 
 class PropertyType(StringEnum):
@@ -43,116 +45,139 @@
     SKELETON = "skeleton"
     POLYLINE = "polyline"
     ROTATABLE_BOUNDING_BOX = "rotatable_bounding_box"
     BITMASK = "bitmask"
 
 
 OptionType = TypeVar("OptionType", bound="Option")
+OntologyNestedElementT = TypeVar("OntologyNestedElementT", bound="OntologyNestedElement")
 
 
-class Attribute(ABC, Generic[OptionType]):
-    """
-    Base class for shared Attribute fields
-    """
-
-    uid: NestedID
+@dataclass
+class OntologyElement(ABC):
     feature_node_hash: str
-    name: str
-    required: bool
-    dynamic: bool
-    """
-    The `dynamic` member is part of every attribute. However it can only be true for top level (not nested) attributes
-    that are part of an :class:`encord.objects.ontology_object.Object`.
-    """
-
-    def __init__(self, uid: NestedID, feature_node_hash: str, name: str, required: bool, dynamic: bool):
-        self.uid = uid
-        self.feature_node_hash = feature_node_hash
-        self.name = name
-        self.required = required
-        self.dynamic = dynamic
 
     @property
-    def options(self) -> Sequence[OptionType]:
+    def children(self) -> Sequence[OntologyElement]:
         return []
 
-    @staticmethod
-    @abstractmethod
-    def get_property_type() -> PropertyType:
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def _get_property_type_name() -> str:
-        pass
-
+    @property
     @abstractmethod
-    def _encode_options(self) -> Optional[List[dict]]:
-        pass
+    def title(self) -> str:
+        raise NotImplementedError("This method is not implemented for this class")
 
-    @abstractmethod
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
+        type_: Optional[Type[OntologyNestedElementT]] = None,
+    ) -> OntologyNestedElementT:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         Args:
             feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
             type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
         """
-        raise NotImplementedError("This method is not implemented for this class")
+        found_item = _get_element_by_hash(feature_node_hash, self.children)
+        if found_item is None:
+            raise OntologyError("Item not found.")
+        check_type(found_item, type_)
+        return found_item
+
+    def get_children_by_title(
+        self,
+        title: str,
+        type_: Optional[Type[OntologyNestedElementT]] = None,
+    ) -> List[OntologyNestedElementT]:
+        """
+        Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
+        Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
+
+        Args:
+            title: The exact title of the child node to search for in the ontology.
+            type_: The expected type of the item. Only nodes that match this type will be returned.
+        """
+        return _get_elements_by_title(title, self.children, type_=type_)
 
     def get_child_by_title(
         self,
         title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
+        type_: Optional[Type[OntologyNestedElementT]] = None,
+    ) -> OntologyNestedElementT:
         """
         Returns a child node of this ontology tree node with the matching title and matching type if specified. If more
         than one child in this Object have the same title, then an error will be thrown. If no item is found, an error
         will be thrown as well.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the child node. Only a node that matches this type will be returned.
         """
         found_items = self.get_children_by_title(title, type_)
         _handle_wrong_number_of_found_items(found_items, title, type_)
         return found_items[0]
 
+
+@dataclass
+class OntologyNestedElement(OntologyElement):
+    uid: NestedID
+
+
+class Attribute(OntologyNestedElement, Generic[OptionType]):
+    """
+    Base class for shared Attribute fields
+    """
+
+    name: str
+    required: bool
+    dynamic: bool
+    """
+    The `dynamic` member is part of every attribute. However it can only be true for top level (not nested) attributes
+    that are part of an :class:`encord.objects.ontology_object.Object`.
+    """
+
+    def __init__(self, uid: NestedID, feature_node_hash: str, name: str, required: bool, dynamic: bool):
+        super().__init__(uid=uid, feature_node_hash=feature_node_hash)
+        self.name = name
+        self.required = required
+        self.dynamic = dynamic
+
+    @property
+    def options(self) -> Sequence[OptionType]:
+        return []
+
+    @property
+    def title(self) -> str:
+        return self.name
+
+    @staticmethod
+    @abstractmethod
+    def get_property_type() -> PropertyType:
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def _get_property_type_name() -> str:
+        pass
+
+    @abstractmethod
+    def _encode_options(self) -> Optional[List[dict]]:
+        pass
+
     def to_dict(self) -> Dict[str, Any]:
         ret = self._encode_base()
 
         options = self._encode_options()
         if options is not None:
             ret["options"] = options
 
         return ret
 
-    @abstractmethod
-    def get_children_by_title(
-        self,
-        title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> List[OntologyElement]:
-        """
-        Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
-        Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the item. Only nodes that match this type will be returned.
-        """
-        raise NotImplementedError("This method is not implemented for this class")
-
     @classmethod
     def from_dict(cls, d: Dict[str, Any]) -> Attribute:
         property_type = d["type"]
         common_attribute_fields = cls._decode_common_attribute_fields(d)
         if property_type == RadioAttribute._get_property_type_name():
             return RadioAttribute(
                 **common_attribute_fields,
@@ -199,18 +224,14 @@
     def __eq__(self, other: object):
         return (
             isinstance(other, Attribute) and self.uid == other.uid and self.feature_node_hash == other.feature_node_hash
         )
 
 
 class RadioAttribute(Attribute["NestableOption"]):
-    """
-    This class is currently in BETA. Its API might change in future minor version releases.
-    """
-
     _options: List[NestableOption]
 
     def __init__(
         self,
         uid: NestedID,
         feature_node_hash: str,
         name: str,
@@ -221,63 +242,31 @@
         super().__init__(uid, feature_node_hash, name, required, dynamic)
         self._options = options if options is not None else []
 
     @property
     def options(self) -> Sequence[NestableOption]:
         return self._options
 
+    @property
+    def children(self) -> Sequence[OntologyElement]:
+        return self._options
+
     @staticmethod
     def get_property_type() -> PropertyType:
         return PropertyType.RADIO
 
     @staticmethod
     def _get_property_type_name() -> str:
         return PropertyType.RADIO.value
 
     def _encode_options(self) -> Optional[List[Dict[str, Any]]]:
         if len(self._options) == 0:
             return None
         return [option.to_dict() for option in self._options]
 
-    def get_child_by_hash(
-        self,
-        feature_node_hash: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns the first child node of this ontology tree node with the matching feature node hash. If there is
-        more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
-        an invalid state. Throws if nothing is found or if the type is not matched.
-
-        Args:
-            feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
-            type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
-        """
-        found_item = _get_option_by_hash(feature_node_hash, self._options)
-        if found_item is None:
-            raise OntologyError("Item not found.")
-        check_type(found_item, type_)
-        return found_item
-
-    def get_children_by_title(
-        self,
-        title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> List[OntologyElement]:
-        """
-        Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
-        Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the item. Only nodes that match this type will be returned.
-        """
-        found_items = _get_options_by_title(title, self.options)
-        return filter_by_type(found_items, type_)
-
     def add_option(
         self,
         label: str,
         value: Optional[str] = None,
         local_uid: Optional[int] = None,
         feature_node_hash: Optional[str] = None,
     ) -> NestableOption:
@@ -293,18 +282,14 @@
         Returns:
             a `NestableOption` instance attached to the attribute. This can be further specified by adding nested attributes.
         """
         return _add_option(self._options, NestableOption, label, self.uid, local_uid, feature_node_hash, value)
 
 
 class ChecklistAttribute(Attribute["FlatOption"]):
-    """
-    This class is currently in BETA. Its API might change in future minor version releases.
-    """
-
     _options: List[FlatOption]
 
     def __init__(
         self,
         uid: NestedID,
         feature_node_hash: str,
         name: str,
@@ -328,45 +313,17 @@
             return None
         return [option.to_dict() for option in self._options]
 
     @property
     def options(self) -> Sequence[FlatOption]:
         return self._options
 
-    def get_child_by_hash(
-        self,
-        feature_node_hash: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns the first child node of this ontology tree node with the matching feature node hash. If there is
-        more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
-        an invalid state. Throws if nothing is found or if the type is not matched.
-
-        Args:
-            feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
-            type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
-        """
-        found_item = _get_option_by_hash(feature_node_hash, self._options)
-        if found_item is None:
-            raise OntologyError("Item not found.")
-        check_type(found_item, type_)
-        return found_item
-
-    def get_children_by_title(self, title: str, type_: Optional[OntologyElementType] = None) -> List[OntologyElement]:
-        """
-        Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
-        Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the item. Only nodes that match this type will be returned.
-        """
-        found_items = _get_options_by_title(title, self.options)
-        return filter_by_type(found_items, type_)
+    @property
+    def children(self) -> Sequence[OntologyElement]:
+        return self._options
 
     def add_option(
         self,
         label: str,
         value: Optional[str] = None,
         local_uid: Optional[int] = None,
         feature_node_hash: Optional[str] = None,
@@ -382,72 +339,28 @@
         Returns:
             a `FlatOption` instance attached to the attribute.
         """
         return _add_option(self._options, FlatOption, label, self.uid, local_uid, feature_node_hash, value)
 
 
 class TextAttribute(Attribute["FlatOption"]):
-    """
-    This class is currently in BETA. Its API might change in future minor version releases.
-    """
-
     def __init__(self, uid: NestedID, feature_node_hash: str, name: str, required: bool, dynamic: bool):
         super().__init__(uid, feature_node_hash, name, required, dynamic)
 
     @staticmethod
     def get_property_type() -> PropertyType:
         return PropertyType.TEXT
 
     @staticmethod
     def _get_property_type_name() -> str:
         return PropertyType.TEXT.value
 
     def _encode_options(self) -> Optional[List[Dict[str, Any]]]:
         return None
 
-    def get_child_by_hash(
-        self,
-        feature_node_hash: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns the first child node of this ontology tree node with the matching feature node hash. If there is
-        more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
-        an invalid state. Throws if nothing is found or if the type is not matched.
-
-        For TextAttributes this will always throw as they have no children.
-
-        Args:
-            feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
-            type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
-        """
-        raise OntologyError("No nested options available for text attributes.")
-
-    def get_children_by_title(
-        self,
-        title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> List[OntologyElement]:
-        """
-        Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
-        Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
-
-        For TextAttributes this will always return an empty list.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the item. Only nodes that match this type will be returned.
-        """
-        return []
-
-
-"""
-This class is currently in BETA. Its API might change in future minor version releases. 
-"""
-
 
 def _attribute_id_from_json_str(attribute_id: str) -> NestedID:
     nested_ids = attribute_id.split(".")
     return [int(x) for x in nested_ids]
 
 
 def attribute_from_dict(d: Dict[str, Any]) -> Attribute:
@@ -460,73 +373,33 @@
     for attribute in attributes:
         attributes_list.append(attribute.to_dict())
 
     return attributes_list
 
 
 @dataclass
-class Option(ABC):
+class Option(OntologyNestedElement):
     """
     Base class for shared Option fields
     """
 
-    uid: NestedID
-    feature_node_hash: str
     label: str
     value: str
 
-    @abstractmethod
-    def is_nestable(self) -> bool:
-        pass
+    @property
+    def title(self) -> str:
+        return self.label
 
     @abstractmethod
-    def get_child_by_hash(
-        self,
-        feature_node_hash: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns the first child node of this ontology tree node with the matching feature node hash. If there is
-        more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
-        an invalid state. Throws if nothing is found or if the type is not matched.
-
-        Args:
-            feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
-            type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
-        """
+    def is_nestable(self) -> bool:
         raise NotImplementedError("This method is not implemented for this class")
 
-    def get_child_by_title(
-        self,
-        title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns a child node of this ontology tree node with the matching title and matching type if specified. If more
-        than one child in this Object have the same title, then an error will be thrown. If no item is found, an error
-        will be thrown as well.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the child node. Only a node that matches this type will be returned.
-        """
-        found_items = self.get_children_by_title(title, type_)
-        _handle_wrong_number_of_found_items(found_items, title, type_)
-        return found_items[0]
-
+    @property
     @abstractmethod
-    def get_children_by_title(self, title: str, type_: Optional[OntologyElementType] = None) -> List[OntologyElement]:
-        """
-        Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
-        Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the item. Only nodes that match this type will be returned.
-        """
+    def attributes(self) -> List[Attribute]:
         raise NotImplementedError("This method is not implemented for this class")
 
     def to_dict(self) -> Dict[str, Any]:
         ret: Dict[str, Any] = dict()
         ret["id"] = _decode_nested_uid(self.uid)
         ret["label"] = self.label
         ret["value"] = self.value
@@ -550,110 +423,43 @@
             "value": option_dict["value"],
             "feature_node_hash": option_dict["featureNodeHash"],
         }
 
 
 @dataclass
 class FlatOption(Option):
-    """
-    This class is currently in BETA. Its API might change in future minor version releases.
-    """
-
     def is_nestable(self) -> bool:
         return False
 
-    def get_child_by_hash(
-        self,
-        feature_node_hash: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns the first child node of this ontology tree node with the matching feature node hash. If there is
-        more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
-        an invalid state. Throws if nothing is found or if the type is not matched.
-
-        For FlatOptions this will always throw as they have no children.
-
-        Args:
-            feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
-            type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
-        """
-        raise OntologyError("No nested attributes for flat options.")
-
-    def get_children_by_title(
-        self,
-        title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> List[OntologyElement]:
-        """
-        Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
-        Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
-
-        For FlatOptions this will always return an empty list.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the item. Only nodes that match this type will be returned.
-        """
+    @property
+    def attributes(self) -> List[Attribute]:
         return []
 
     @classmethod
     def from_dict(cls, d: dict) -> FlatOption:
         return FlatOption(**cls._decode_common_option_fields(d))
 
     def _encode_nested_options(self) -> list:
         return []
 
 
 @dataclass
 class NestableOption(Option):
-    """
-    This class is currently in BETA. Its API might change in future minor version releases.
-    """
-
     nested_options: List[Attribute] = field(default_factory=list)
 
     def is_nestable(self) -> bool:
         return True
 
-    def get_child_by_hash(
-        self,
-        feature_node_hash: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns the first child node of this ontology tree node with the matching feature node hash. If there is
-        more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
-        an invalid state. Throws if nothing is found or if the type is not matched.
-
-        Args:
-            feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
-            type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
-        """
-        found_item = _get_attribute_by_hash(feature_node_hash, self.nested_options)
-        if found_item is None:
-            raise OntologyError("Item not found.")
-        check_type(found_item, type_)
-        return found_item
-
-    def get_children_by_title(
-        self,
-        title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> List[OntologyElement]:
-        """
-        Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
-        Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
+    @property
+    def attributes(self) -> List[Attribute]:
+        return self.nested_options
 
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the item. Only nodes that match this type will be returned.
-        """
-        found_items = _get_attributes_by_title(title, self.nested_options)
-        return filter_by_type(found_items, type_)
+    @property
+    def children(self) -> Sequence[OntologyElement]:
+        return self.nested_options
 
     def _encode_nested_options(self) -> list:
         return attributes_to_list_dict(self.nested_options)
 
     @classmethod
     def from_dict(cls, d: dict) -> NestableOption:
         nested_options_ret: List[Attribute] = list()
@@ -694,15 +500,15 @@
         return _add_attribute(self.nested_options, cls, name, self.uid, local_uid, feature_node_hash, required)
 
     def __hash__(self):
         return hash(self.feature_node_hash)
 
 
 def __build_identifiers(
-    existent_items: Iterable[OntologyElement],
+    existent_items: Iterable[OntologyNestedElement],
     local_uid: Optional[int] = None,
     feature_node_hash: Optional[str] = None,
 ) -> Tuple[int, str]:
     if local_uid is None:
         if existent_items:
             local_uid = max([item.uid[-1] for item in existent_items]) + 1
         else:
@@ -752,92 +558,78 @@
     local_uid: Optional[int] = None,
     feature_node_hash: Optional[str] = None,
     value: Optional[str] = None,
 ) -> OT:
     local_uid, feature_node_hash = __build_identifiers(options, local_uid, feature_node_hash)
     if not value:
         value = re.sub(r"[\s]", "_", label).lower()
-    option = cls(parent_uid + [local_uid], feature_node_hash, label, value)
+    option = cls(uid=parent_uid + [local_uid], feature_node_hash=feature_node_hash, label=label, value=value)
     options.append(option)
     return option
 
 
-def _get_option_by_hash(feature_node_hash: str, options: Iterable[Option]) -> Optional[OntologyElement]:
-    for option_ in options:
-        if option_.feature_node_hash == feature_node_hash:
-            return option_
-
-        if option_.is_nestable():
-            found_item = _get_attribute_by_hash(feature_node_hash, option_.nested_options)
-            if found_item is not None:
-                return found_item
-
-    return None
+def _get_element_by_hash(
+    feature_node_hash: str, elements: Iterable[OntologyElement], type_: Optional[Type[OntologyNestedElementT]] = None
+) -> Optional[OntologyNestedElementT]:
+    for element in elements:
+        if element.feature_node_hash == feature_node_hash:
+            return checked_cast(element, type_)
 
-
-def _get_attribute_by_hash(feature_node_hash: str, attributes: List[Attribute]) -> Optional[OntologyElement]:
-    for attribute in attributes:
-        if attribute.feature_node_hash == feature_node_hash:
-            return attribute
-
-        found_item = _get_option_by_hash(feature_node_hash, attribute.options)
+        found_item = _get_element_by_hash(feature_node_hash, element.children, type_=type_)
         if found_item is not None:
             return found_item
+
     return None
 
 
-def _get_options_by_title(title: str, options: Iterable[Option]) -> List[OntologyElement]:
-    ret: List[OntologyElement] = []
-    for option_ in options:
-        if option_.label == title:
-            ret.append(option_)
+def _get_elements_by_title(
+    title: str, elements: Iterable[OntologyElement], type_: Optional[Type[OntologyNestedElementT]] = None
+) -> List[OntologyNestedElementT]:
+    res: List[OntologyNestedElementT] = []
+    for element in elements:
+        if element.title == title and does_type_match(element, type_):
+            res.append(cast(OntologyNestedElementT, element))
 
-        if option_.is_nestable():
-            found_items = _get_attributes_by_title(title, option_.nested_options)
-            ret.extend(found_items)
+        found_items = _get_elements_by_title(title, element.children, type_=type_)
+        res.extend(found_items)
 
-    return ret
+    return res
 
 
-def _get_attributes_by_title(title: str, attributes: List[Attribute]) -> List[OntologyElement]:
-    ret: List[OntologyElement] = []
-    for attribute in attributes:
-        if attribute.name == title:
-            ret.append(attribute)
+def _get_option_by_hash(feature_node_hash: str, options: Iterable[Option]) -> Optional[Option]:
+    return _get_element_by_hash(feature_node_hash, options, type_=Option)
+
 
-        found_items = _get_options_by_title(title, attribute.options)
-        ret.extend(found_items)
-    return ret
+def _get_attribute_by_hash(feature_node_hash: str, attributes: List[Attribute]) -> Optional[Attribute]:
+    return _get_element_by_hash(feature_node_hash, attributes, type_=Attribute)
 
 
 def _handle_wrong_number_of_found_items(
-    found_items: List[OntologyElement],
+    found_items: Sequence[OntologyElement],
     title: str,
     type_: Any,
 ) -> None:
     if len(found_items) == 0:
         raise OntologyError(f"No item was found in the ontology with the given title `{title}` and type `{type_}`")
     elif len(found_items) > 1:
         raise OntologyError(
             f"More than one item was found in the ontology with the given title `{title}` and type `{type_}`. "
             f"Use the `get_children_by_title` or `get_child_by_hash` function instead. "
             f"The found items are `{found_items}`."
         )
 
 
 OptionAttribute = Union[RadioAttribute, ChecklistAttribute]
-OntologyElement = Union[Attribute, Option]
 AttributeTypes = Union[
     Type[RadioAttribute],
     Type[ChecklistAttribute],
     Type[TextAttribute],
     Type[Attribute],
 ]
 OptionTypes = Union[Type[FlatOption], Type[NestableOption], Type[Option]]
-OntologyElementType = Union[AttributeTypes, OptionTypes]
 
 # Two types below are kept for the backwards compatibility
 # Please don't use them, as they are going to be removed in the future versions
 AttributeClasses = Union[RadioAttribute, ChecklistAttribute, TextAttribute, Attribute]
 OptionClasses = Union[FlatOption, NestableOption, Option]
```

### Comparing `encord-0.1.84/encord/objects/coordinates.py` & `encord-0.1.85/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/objects/frames.py` & `encord-0.1.85/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/objects/internal_helpers.py` & `encord-0.1.85/encord/objects/internal_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Attribute,
     ChecklistAttribute,
     FlatOption,
     NestableOption,
     Option,
     RadioAttribute,
     TextAttribute,
-    _get_option_by_hash,
+    _get_element_by_hash,
 )
 from encord.objects.constants import DEFAULT_MANUAL_ANNOTATION
 from encord.objects.frames import Ranges, ranges_to_list
 from encord.objects.utils import _lower_snake_case, short_uuid_str
 
 ValueType = TypeVar("ValueType")
 AttributeType = TypeVar("AttributeType", bound=Attribute)
@@ -250,15 +250,20 @@
             raise ValueError("Cannot set the value of a TextAnswer based on a different ontology attribute.")
 
         answers = d["answers"]
         if len(answers) != 1:
             raise ValueError("RadioAnswers must have exactly one answer.")
 
         answer = answers[0]
-        nestable_option = _get_option_by_hash(answer["featureHash"], self.ontology_attribute.options)
+        nestable_option = _get_element_by_hash(
+            answer["featureHash"], self.ontology_attribute.options, type_=NestableOption
+        )
+        if nestable_option is None:
+            raise ValueError(f"Item not found: can't find an option with a feature hash {answer['featureHash']}")
+
         self.set(nestable_option)
         self.is_manual_annotation = d["manualAnnotation"]
 
     def __hash__(self):
         return hash((self.ontology_attribute.feature_node_hash, self._value, type(self).__name__))
 
     def __eq__(self, other: object) -> bool:
@@ -351,15 +356,17 @@
             )
         other_is_answered = checklist_answer.is_answered()
         if not other_is_answered:
             self.unset()
         else:
             self._answered = True
             for feature_node_hash in self._feature_hash_to_answer_map.keys():
-                option = _get_option_by_hash(feature_node_hash, self.ontology_attribute.options)
+                option = _get_element_by_hash(feature_node_hash, self.ontology_attribute.options, type_=FlatOption)
+                if option is None:
+                    raise RuntimeError(f"Item not found: can't find an option with a feature hash {feature_node_hash}")
                 other_answer = checklist_answer.get_option_value(option)
                 self._feature_hash_to_answer_map[feature_node_hash] = other_answer
 
     def _initialise_feature_hash_to_answer_map(self) -> Dict[str, bool]:
         ret: Dict[str, bool] = {}
         for child in self._ontology_attribute.options:
             ret[child.feature_node_hash] = False
@@ -407,15 +414,18 @@
             raise ValueError("Cannot set the value of a ChecklistAnswer based on a different ontology attribute.")
 
         answers = d["answers"]
         if len(answers) == 0:
             return
 
         for answer in answers:
-            flat_option = _get_option_by_hash(answer["featureHash"], self.ontology_attribute.options)
+            flat_option = _get_element_by_hash(answer["featureHash"], self.ontology_attribute.options, type_=FlatOption)
+            if flat_option is None:
+                raise ValueError(f"Item not found: can't find an option with a feature hash {answer['featureHash']}")
+
             self.check_options([flat_option])
 
         self.is_manual_annotation = d["manualAnnotation"]
         self._answered = True
 
     def __hash__(self):
         flat_values = [(key, value) for key, value in self._feature_hash_to_answer_map.items()]
@@ -450,17 +460,16 @@
     ret: List[Answer] = list()
     for attribute in attributes:
         if not attribute.dynamic:
             answer = get_default_answer_from_attribute(attribute)
             ret.append(answer)
 
         for option in attribute.options:
-            if option.is_nestable():
-                other_attributes = _get_default_static_answers_from_attributes(option.nested_options)
-                ret.extend(other_attributes)
+            other_attributes = _get_default_static_answers_from_attributes(option.attributes)
+            ret.extend(other_attributes)
 
     return ret
 
 
 def _get_static_answer_map(attributes: List[Attribute]) -> Dict[str, Answer]:
     answers = _get_default_static_answers_from_attributes(attributes)
     answer_map = {answer.ontology_attribute.feature_node_hash: answer for answer in answers}
@@ -492,30 +501,29 @@
 
 
 def _search_for_parent(passed_option: Option, attributes: List[Attribute]) -> Optional[Attribute]:
     for attribute in attributes:
         for option in attribute.options:
             if option == passed_option:
                 return attribute
-            if option.is_nestable():
-                attribute_opt = _search_for_parent(passed_option, option.nested_options)
-                if attribute_opt is not None:
-                    return attribute_opt
+
+            attribute_opt = _search_for_parent(passed_option, option.attributes)
+            if attribute_opt is not None:
+                return attribute_opt
     return None
 
 
-def _search_for_text_attributes(attributes: List[Attribute]) -> List[Attribute]:
-    text_attributes: List[Attribute] = list()
+def _search_for_text_attributes(attributes: List[Attribute]) -> List[TextAttribute]:
+    text_attributes: List[TextAttribute] = list()
     for attribute in attributes:
         if isinstance(attribute, TextAttribute):
             text_attributes.append(attribute)
 
         for option in attribute.options:
-            if option.is_nestable():
-                text_attributes.extend(_search_for_text_attributes(option.nested_options))
+            text_attributes.extend(_search_for_text_attributes(option.attributes))
     return text_attributes
 
 
 def _infer_attribute_from_answer(
     attributes: List[Attribute], answer: Union[str, Option, Sequence[Option]]
 ) -> Attribute:
     if isinstance(answer, Option):
```

### Comparing `encord-0.1.84/encord/objects/ontology_labels_impl.py` & `encord-0.1.85/encord/objects/ontology_labels_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
+    cast,
 )
 from uuid import uuid4
 
 from dateutil.parser import parse
 
 from encord.client import EncordClientProject
 from encord.client import LabelRow as OrmLabelRow
@@ -38,22 +39,22 @@
 from encord.objects.common import AttributeTypes  # pylint: disable=unused-import
 from encord.objects.common import OptionClasses  # pylint: disable=unused-import
 from encord.objects.common import OptionTypes  # pylint: disable=unused-import
 from encord.objects.common import (
     Attribute,
     ChecklistAttribute,
     OntologyElement,
-    OntologyElementType,
+    OntologyNestedElement,
     Option,
     RadioAttribute,
     Shape,
     TextAttribute,
     _add_attribute,
     _get_attribute_by_hash,
-    _get_attributes_by_title,
+    _get_element_by_hash,
     _get_option_by_hash,
     _handle_wrong_number_of_found_items,
     attribute_from_dict,
     attributes_to_list_dict,
 )
 from encord.objects.constants import (
     DATETIME_LONG_STRING_FORMAT,
@@ -85,101 +86,50 @@
     _infer_attribute_from_answer,
     _search_child_attributes,
     get_default_answer_from_attribute,
 )
 from encord.objects.utils import (
     _lower_snake_case,
     check_email,
-    check_type,
+    checked_cast,
     does_type_match,
-    filter_by_type,
     short_uuid_str,
 )
 from encord.orm.formatter import Formatter
 from encord.orm.label_row import (
     AnnotationTaskStatus,
     LabelRowMetadata,
     LabelStatus,
     WorkflowGraphNode,
 )
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
-class Object:
-    """
-    This class is currently in BETA. Its API might change in future minor version releases.
-    """
-
+class Object(OntologyElement):
     uid: int
     name: str
     color: str
     shape: Shape
     feature_node_hash: str
     attributes: List[Attribute] = field(default_factory=list)
 
+    @property
+    def title(self) -> str:
+        return self.name
+
+    @property
+    def children(self) -> Sequence[OntologyElement]:
+        return self.attributes
+
     def create_instance(self) -> ObjectInstance:
         """Create a :class:`encord.objects.ObjectInstance` to be used with a label row."""
         return ObjectInstance(self)
 
-    def get_child_by_hash(
-        self,
-        feature_node_hash: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns the first child node of this ontology tree node with the matching feature node hash. If there is
-        more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
-        an invalid state. Throws if nothing is found or if the type is not matched.
-
-        Args:
-            feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
-            type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
-        """
-        found_item = _get_attribute_by_hash(feature_node_hash, self.attributes)
-        if found_item is None:
-            raise OntologyError("Item not found.")
-        check_type(found_item, type_)
-        return found_item
-
-    def get_child_by_title(
-        self,
-        title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns a child node of this ontology tree node with the matching title and matching type if specified. If more
-        than one child in this Object have the same title, then an error will be thrown. If no item is found, an error
-        will be thrown as well.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the child node. Only a node that matches this type will be returned.
-        """
-        found_items = self.get_children_by_title(title, type_)
-        _handle_wrong_number_of_found_items(found_items, title, type_)
-        return found_items[0]
-
-    def get_children_by_title(
-        self,
-        title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> List[OntologyElement]:
-        """
-        Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
-        Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the item. Only nodes that match this type will be returned.
-        """
-        found_items = _get_attributes_by_title(title, self.attributes)
-        return filter_by_type(found_items, type_)
-
     @classmethod
     def from_dict(cls, d: dict) -> Object:
         shape_opt = Shape.from_string(d["shape"])
         if shape_opt is None:
             raise TypeError(f"The shape '{d['shape']}' of the object '{d}' is not recognised")
 
         attributes_ret: List[Attribute] = list()
@@ -242,84 +192,36 @@
         Raises:
             ValueError: if specified `local_uid` or `feature_node_hash` violate uniqueness constraints
         """
         return _add_attribute(self.attributes, cls, name, [self.uid], local_uid, feature_node_hash, required, dynamic)
 
 
 @dataclass
-class Classification:
+class Classification(OntologyElement):
     """
-    This class is currently in BETA. Its API might change in future minor version releases.
-
     Represents a whole-image classification as part of Ontology structure. Wraps a single Attribute that describes
-    the image in general rather then individual object.
+    the image in general rather than an individual object.
     """
 
     uid: int
     feature_node_hash: str
     attributes: List[Attribute]
 
+    @property
+    def title(self) -> str:
+        return self.attributes[0].name
+
+    @property
+    def children(self) -> Sequence[OntologyElement]:
+        return self.attributes
+
     def create_instance(self) -> ClassificationInstance:
         """Create a :class:`encord.objects.ClassificationInstance` to be used with a label row."""
         return ClassificationInstance(self)
 
-    def get_child_by_hash(
-        self,
-        feature_node_hash: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns the first child node of this ontology tree node with the matching feature node hash. If there is
-        more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
-        an invalid state. Throws if nothing is found or if the type is not matched.
-
-        Args:
-            feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
-            type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
-        """
-        found_item = _get_attribute_by_hash(feature_node_hash, self.attributes)
-        if found_item is None:
-            raise OntologyError("Item not found.")
-        check_type(found_item, type_)
-        return found_item
-
-    def get_child_by_title(
-        self,
-        title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
-        """
-        Returns a child node of this ontology tree node with the matching title and matching type if specified. If more
-        than one child in this Object have the same title, then an error will be thrown. If no item is found, an error
-        will be thrown as well.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the child node. Only a node that matches this type will be returned.
-        """
-        found_items = self.get_children_by_title(title, type_)
-        _handle_wrong_number_of_found_items(found_items, title, type_)
-        return found_items[0]
-
-    def get_children_by_title(
-        self,
-        title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> List[OntologyElement]:
-        """
-        Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
-        Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
-
-        Args:
-            title: The exact title of the child node to search for in the ontology.
-            type_: The expected type of the item. Only nodes that match this type will be returned.
-        """
-        found_items = _get_attributes_by_title(title, self.attributes)
-        return filter_by_type(found_items, type_)
-
     @classmethod
     def from_dict(cls, d: dict) -> Classification:
         attributes_ret: List[Attribute] = list()
         for attribute_dict in d["attributes"]:
             attributes_ret.append(attribute_from_dict(attribute_dict))
 
         return Classification(
@@ -1921,15 +1823,15 @@
         frame: int,
     ) -> Dict[str, Any]:
         ret: Dict[str, Any] = {}
 
         object_instance_annotation = object_.get_annotation(frame)
         coordinates = object_instance_annotation.coordinates
         ontology_hash = object_.ontology_item.feature_node_hash
-        ontology_object = self._ontology.structure.get_child_by_hash(ontology_hash)
+        ontology_object = self._ontology.structure.get_child_by_hash(ontology_hash, type_=Object)
 
         ret["name"] = ontology_object.name
         ret["color"] = ontology_object.color
         ret["shape"] = ontology_object.shape.value
         ret["value"] = _lower_snake_case(ontology_object.name)
         ret["createdAt"] = object_instance_annotation.created_at.strftime(DATETIME_LONG_STRING_FORMAT)
         ret["createdBy"] = object_instance_annotation.created_by
@@ -1984,17 +1886,19 @@
         return ret
 
     def _to_encord_classification(self, classification: ClassificationInstance, frame: int) -> Dict[str, Any]:
         ret: Dict[str, Any] = {}
 
         annotation = classification.get_annotation(frame)
         classification_feature_hash = classification.ontology_item.feature_node_hash
-        ontology_classification = self._ontology.structure.get_child_by_hash(classification_feature_hash)
+        ontology_classification = self._ontology.structure.get_child_by_hash(
+            classification_feature_hash, type_=Classification
+        )
         attribute_hash = classification.ontology_item.attributes[0].feature_node_hash
-        ontology_attribute = self._ontology.structure.get_child_by_hash(attribute_hash)
+        ontology_attribute = self._ontology.structure.get_child_by_hash(attribute_hash, type_=Attribute)
 
         ret["name"] = ontology_attribute.name
         ret["value"] = _lower_snake_case(ontology_attribute.name)
         ret["createdAt"] = annotation.created_at.strftime(DATETIME_LONG_STRING_FORMAT)
         ret["createdBy"] = annotation.created_by
         ret["confidence"] = annotation.confidence
         ret["featureHash"] = ontology_classification.feature_node_hash
@@ -2168,15 +2072,15 @@
             object_instance.set_answer_from_list(answer_list)
 
     def _create_new_object_instance(self, frame_object_label: dict, frame: int) -> ObjectInstance:
         ontology = self._ontology.structure
         feature_hash = frame_object_label["featureHash"]
         object_hash = frame_object_label["objectHash"]
 
-        label_class = ontology.get_child_by_hash(feature_hash)
+        label_class = ontology.get_child_by_hash(feature_hash, type_=Object)
         object_instance = ObjectInstance(label_class, object_hash=object_hash)
 
         coordinates = self._get_coordinates(frame_object_label)
         object_frame_instance_info = ObjectInstance.FrameInfo.from_dict(frame_object_label)
 
         object_instance.set_for_frames(coordinates=coordinates, frames=frame, **asdict(object_frame_instance_info))
         return object_instance
@@ -2243,15 +2147,15 @@
 
     def _create_new_classification_instance(
         self, frame_classification_label: dict, frame: int, classification_answers: dict
     ) -> ClassificationInstance:
         feature_hash = frame_classification_label["featureHash"]
         classification_hash = frame_classification_label["classificationHash"]
 
-        label_class = self._ontology.structure.get_child_by_hash(feature_hash)
+        label_class = self._ontology.structure.get_child_by_hash(feature_hash, type_=Classification)
         classification_instance = ClassificationInstance(label_class, classification_hash=classification_hash)
 
         frame_view = ClassificationInstance.FrameData.from_dict(frame_classification_label)
         classification_instance.set_for_frames(frame, **asdict(frame_view))
         answers_dict = classification_answers[classification_hash]["classifications"]
         self._add_static_answers_from_dict(classification_instance, answers_dict)
 
@@ -3085,62 +2989,58 @@
     "#0C797D",
     "#0062B1",
     "#653294",
     "#AB149E",
 )
 
 
+OntologyElementT = TypeVar("OntologyElementT", bound=OntologyElement)
+
+
 @dataclass
 class OntologyStructure:
-    """
-    This class is currently in BETA. Its API might change in future minor version releases.
-    """
-
     objects: List[Object] = field(default_factory=list)
     classifications: List[Classification] = field(default_factory=list)
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
+        type_: Optional[Type[OntologyElementT]] = None,
+    ) -> OntologyElementT:
         """
         Returns the first child node of this ontology tree node with the matching feature node hash. If there is
         more than one child with the same feature node hash in the ontology tree node, then the ontology would be in
         an invalid state. Throws if nothing is found or if the type is not matched.
 
         Args:
             feature_node_hash: the feature_node_hash of the child node to search for in the ontology.
             type_: The expected type of the item. If the found child does not match the type, an error will be thrown.
         """
         for object_ in self.objects:
             if object_.feature_node_hash == feature_node_hash:
-                check_type(object_, type_)
-                return object_
-            found_item = _get_attribute_by_hash(feature_node_hash, object_.attributes)
+                return checked_cast(object_, type_)
+
+            found_item = _get_element_by_hash(feature_node_hash, object_.attributes)
             if found_item is not None:
-                check_type(found_item, type_)
-                return found_item
+                return checked_cast(found_item, type_)
 
         for classification in self.classifications:
             if classification.feature_node_hash == feature_node_hash:
-                check_type(classification, type_)
-                return classification
-            found_item = _get_attribute_by_hash(feature_node_hash, classification.attributes)
+                return checked_cast(classification, type_)
+            found_item = _get_element_by_hash(feature_node_hash, classification.attributes)
             if found_item is not None:
-                check_type(found_item, type_)
-                return found_item
+                return checked_cast(found_item, type_)
 
-        raise OntologyError("Item not found.")
+        raise OntologyError(f"Item not found: can't find an item with a hash {feature_node_hash} in the ontology.")
 
     def get_child_by_title(
         self,
         title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> OntologyElement:
+        type_: Optional[Type[OntologyElementT]] = None,
+    ) -> OntologyElementT:
         """
         Returns a child node of this ontology tree node with the matching title and matching type if specified. If more
         than one child in this Object have the same title, then an error will be thrown. If no item is found, an error
         will be thrown as well.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
@@ -3149,42 +3049,44 @@
         found_items = self.get_children_by_title(title, type_)
         _handle_wrong_number_of_found_items(found_items, title, type_)
         return found_items[0]
 
     def get_children_by_title(
         self,
         title: str,
-        type_: Optional[OntologyElementType] = None,
-    ) -> List[OntologyElement]:
+        type_: Optional[Type[OntologyElementT]] = None,
+    ) -> List[OntologyElementT]:
         """
         Returns all the child nodes of this ontology tree node with the matching title and matching type if specified.
         Title in ontologies do not need to be unique, however, we recommend unique titles when creating ontologies.
 
         Args:
             title: The exact title of the child node to search for in the ontology.
             type_: The expected type of the item. Only nodes that match this type will be returned.
         """
         ret: List[OntologyElement] = []
         for object_ in self.objects:
-            if object_.name == title:
-                if does_type_match(object_, type_):
-                    ret.append(object_)
-            found_items = _get_attributes_by_title(title, object_.attributes)
-            filtered_items = filter_by_type(found_items, type_)
-            ret.extend(filtered_items)
+            if object_.title == title and does_type_match(object_, type_):
+                ret.append(object_)
+
+            if type_ is None or issubclass(type_, OntologyNestedElement):
+                found_items = object_.get_children_by_title(title, type_=type_)
+                ret.extend(found_items)
 
         for classification in self.classifications:
-            if classification.attributes[0].name == title:
-                if does_type_match(classification, type_):
-                    ret.append(classification)
-            found_items = _get_attributes_by_title(title, classification.attributes)
-            filtered_items = filter_by_type(found_items, type_)
-            ret.extend(filtered_items)
+            if classification.title == title and does_type_match(classification, type_):
+                ret.append(classification)
 
-        return ret
+            if type_ is None or issubclass(type_, OntologyNestedElement):
+                found_items = classification.get_children_by_title(title, type_=type_)
+                ret.extend(found_items)
+
+        # type checks in the code above guarantee the type conformity of the return value
+        # but there is no obvious way to tell that to mypy, so just casting here for now
+        return cast(List[OntologyElementT], ret)
 
     @classmethod
     def from_dict(cls, d: Dict[str, Any]) -> OntologyStructure:
         """
         Args:
             d: a JSON blob of an "ontology structure" (e.g. from Encord web app)
 
@@ -3283,15 +3185,15 @@
 
         if feature_node_hash is None:
             feature_node_hash = str(uuid4())[:8]
 
         if any([obj.feature_node_hash == feature_node_hash for obj in self.objects]):
             raise ValueError(f"Duplicate feature_node_hash '{feature_node_hash}'")
 
-        obj = Object(uid, name, color, shape, feature_node_hash)
+        obj = Object(uid=uid, name=name, color=color, shape=shape, feature_node_hash=feature_node_hash)
         self.objects.append(obj)
         return obj
 
     def add_classification(
         self,
         uid: Optional[int] = None,
         feature_node_hash: Optional[str] = None,
@@ -3333,15 +3235,15 @@
 
         if feature_node_hash is None:
             feature_node_hash = str(uuid4())[:8]
 
         if any([cls.feature_node_hash == feature_node_hash for cls in self.classifications]):
             raise ValueError(f"Duplicate feature_node_hash '{feature_node_hash}'")
 
-        cls = Classification(uid, feature_node_hash, list())
+        cls = Classification(uid=uid, feature_node_hash=feature_node_hash, attributes=list())
         self.classifications.append(cls)
         return cls
 
 
 class OntologyUserRole(IntEnum):
     ADMIN = 0
     USER = 1
```

### Comparing `encord-0.1.84/encord/objects/project.py` & `encord-0.1.85/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/objects/utils.py` & `encord-0.1.85/encord/objects/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import base64
 import re
 import uuid
-from typing import Any, Iterable, List, Optional, Type, TypeVar
+from typing import Any, Iterable, List, Optional, Type, TypeVar, cast
 
 
 def _decode_nested_uid(nested_uid: list) -> str:
     return ".".join([str(uid) for uid in nested_uid])
 
 
 def short_uuid_str() -> str:
@@ -36,14 +36,19 @@
         return False
     return True
 
 
 T = TypeVar("T")
 
 
+def checked_cast(obj: Any, type_: Optional[Type[T]]) -> T:
+    check_type(obj, type_)
+    return cast(T, obj)
+
+
 def filter_by_type(objects: Iterable[Any], type_: Optional[Type[T]]) -> List[T]:
     return [object_ for object_ in objects if does_type_match(object_, type_)]
 
 
 def is_valid_email(email: str) -> bool:
     """
     Validate that an email is a valid one
```

### Comparing `encord-0.1.84/encord/ontology.py` & `encord-0.1.85/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/analytics.py` & `encord-0.1.85/encord/orm/analytics.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/api_key.py` & `encord-0.1.85/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/base_dto/__init__.py` & `encord-0.1.85/encord/orm/base_dto/__init__.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/base_dto/base_dto_pydantic_v1.py` & `encord-0.1.85/encord/orm/base_dto/base_dto_pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/base_dto/base_dto_pydantic_v2.py` & `encord-0.1.85/encord/orm/base_dto/base_dto_pydantic_v2.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/base_orm.py` & `encord-0.1.85/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/dataset.py` & `encord-0.1.85/encord/orm/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/dataset_with_user_role.py` & `encord-0.1.85/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/label_log.py` & `encord-0.1.85/encord/orm/label_log.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,7 +47,10 @@
     ADD_ATTRIBUTE = 23
     EDIT_ATTRIBUTE = 24
     DELETE_ATTRIBUTE = 25
     APPROVE_NESTED_ATTRIBUTE = 26
     REJECT_NESTED_ATTRIBUTE = 27
     SUBMIT_LABEL = 28
     SUBMIT_NESTED_ATTRIBUTE = 29
+    BUFFERING_OVERLAY_SHOWN = 30
+    BITRATE_WARNING_SHOWN = 31
+    SEEKING_OVERLAY_SHOWN = 32
```

### Comparing `encord-0.1.84/encord/orm/label_row.py` & `encord-0.1.85/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/labeling_algorithm.py` & `encord-0.1.85/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/model.py` & `encord-0.1.85/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/ontology.py` & `encord-0.1.85/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/project.py` & `encord-0.1.85/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/project_api_key.py` & `encord-0.1.85/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/project_with_user_role.py` & `encord-0.1.85/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/orm/test/test_dataset.py` & `encord-0.1.85/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/project.py` & `encord-0.1.85/encord/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         return project_instance.last_edited_at
 
     @property
     def ontology(self) -> dict:
         """
         Get the ontology of the project.
 
-        BETA: Prefer using the :class:`encord.objects.ontology_structure.OntologyStructure` class to work with the data.
+        DEPRECATED: Prefer using the :class:`encord.objects.ontology_structure.OntologyStructure` class to work with the data.
 
         .. code::
 
             from encord.objects.ontology_structure import OntologyStructure
 
             project = user_client.get_project("<project_hash>")
```

### Comparing `encord-0.1.84/encord/project_ontology/classification_attribute.py` & `encord-0.1.85/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/project_ontology/classification_option.py` & `encord-0.1.85/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/project_ontology/ontology.py` & `encord-0.1.85/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/project_ontology/ontology_classification.py` & `encord-0.1.85/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/project_ontology/ontology_object.py` & `encord-0.1.85/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/user_client.py` & `encord-0.1.85/encord/user_client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/utilities/client_utilities.py` & `encord-0.1.85/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/utilities/label_utilities.py` & `encord-0.1.85/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/encord/utilities/project_user.py` & `encord-0.1.85/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.84/pyproject.toml` & `encord-0.1.85/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.84"
+version = "0.1.85"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
```

### Comparing `encord-0.1.84/PKG-INFO` & `encord-0.1.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.84
+Version: 0.1.85
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.84 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.85 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

