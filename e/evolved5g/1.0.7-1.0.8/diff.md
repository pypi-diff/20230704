# Comparing `tmp/evolved5g-1.0.7.tar.gz` & `tmp/evolved5g-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evolved5g-1.0.7.tar", last modified: Thu Jun 15 13:02:27 2023, max compression
+gzip compressed data, was "evolved5g-1.0.8.tar", last modified: Tue Jul  4 14:59:17 2023, max compression
```

## Comparing `evolved5g-1.0.7.tar` & `evolved5g-1.0.8.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:02:27.599353 evolved5g-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-15 13:01:43.000000 evolved5g-1.0.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-15 13:01:43.000000 evolved5g-1.0.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-15 13:01:43.000000 evolved5g-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-15 13:01:43.000000 evolved5g-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-06-15 13:02:27.599353 evolved5g-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-15 13:01:43.000000 evolved5g-1.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:02:27.583353 evolved5g-1.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:02:27.587353 evolved5g-1.0.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/cli.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:02:27.587353 evolved5g-1.0.7/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    26395 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/dummy_html_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/generate.gif
--rw-r--r--   0 runner    (1001) docker     (123)    65839 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/generate_execution.png
--rw-r--r--   0 runner    (1001) docker     (123)    54245 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/netapp_creation.gif
--rw-r--r--   0 runner    (1001) docker     (123)   347578 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/netapp_repo.gif
--rw-r--r--   0 runner    (1001) docker     (123)    55213 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/repo_creation.png
--rw-r--r--   0 runner    (1001) docker     (123)    56898 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/repo_structure.png
--rw-r--r--   0 runner    (1001) docker     (123)   159902 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/ssh_gpg.png
--rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/ssh_key.png
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/ssh_key_button.png
--rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/token1.png
--rw-r--r--   0 runner    (1001) docker     (123)    60688 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/token2.png
--rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/images/token3.png
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/information.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/libraries.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-15 13:01:43.000000 evolved5g-1.0.7/docs/source/pre_requisites.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:02:27.587353 evolved5g-1.0.7/evolved5g/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21200 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/cli_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/nef_and_tsn_api_service_validation_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    91551 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:02:27.591353 evolved5g-1.0.7/evolved5g/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:02:27.591353 evolved5g-1.0.7/evolved5g/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/cells_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/g_n_bs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/location_frontend_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/login_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26635 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/monitoring_event_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/paths_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/qo_s_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27983 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/session_with_qo_s_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27373 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/u_es_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27801 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/ui_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api/utils_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:02:27.599353 evolved5g-1.0.7/evolved5g/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/accumulated_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/all_of_u_es_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/all_of_ue_create_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/all_of_ue_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/all_of_ue_update_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/cell_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/cell_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/gnb_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/gnb_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/location_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_event_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_event_report_received.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_event_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_event_subscription_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/path_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/path_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/qo_s_monitoring_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/qos_monitoring_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/reporting_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/snssai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/u_es.py
--rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/ue.py
--rw-r--r--   0 runner    (1001) docker     (123)    14566 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/ue_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/ue_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/usage_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/user_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/user_plane_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/user_plane_event_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/user_plane_notification_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/user_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-15 13:01:43.000000 evolved5g-1.0.7/evolved5g/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:02:27.591353 evolved5g-1.0.7/evolved5g.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-06-15 13:02:27.000000 evolved5g-1.0.7/evolved5g.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-15 13:02:27.000000 evolved5g-1.0.7/evolved5g.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:02:27.000000 evolved5g-1.0.7/evolved5g.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 13:02:27.000000 evolved5g-1.0.7/evolved5g.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:02:23.000000 evolved5g-1.0.7/evolved5g.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-15 13:02:27.000000 evolved5g-1.0.7/evolved5g.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 13:02:27.000000 evolved5g-1.0.7/evolved5g.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-15 13:01:43.000000 evolved5g-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 13:02:27.599353 evolved5g-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-15 13:01:43.000000 evolved5g-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:59:17.923067 evolved5g-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-04 14:58:32.000000 evolved5g-1.0.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-07-04 14:58:32.000000 evolved5g-1.0.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-04 14:58:32.000000 evolved5g-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-04 14:58:32.000000 evolved5g-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-04 14:59:17.923067 evolved5g-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-04 14:58:32.000000 evolved5g-1.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:59:17.891066 evolved5g-1.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:59:17.899066 evolved5g-1.0.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/cli.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:59:17.903066 evolved5g-1.0.8/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    26395 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/dummy_html_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/generate.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    65839 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/generate_execution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54245 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/netapp_creation.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   347578 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/netapp_repo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    55213 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/repo_creation.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56898 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/repo_structure.png
+-rw-r--r--   0 runner    (1001) docker     (123)   159902 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/ssh_gpg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/ssh_key.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/ssh_key_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/token1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60688 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/token2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/images/token3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/information.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/libraries.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-04 14:58:32.000000 evolved5g-1.0.8/docs/source/pre_requisites.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:59:17.903066 evolved5g-1.0.8/evolved5g/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21200 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/cli_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/nef_and_tsn_api_service_validation_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91466 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:59:17.903066 evolved5g-1.0.8/evolved5g/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:59:17.907066 evolved5g-1.0.8/evolved5g/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/cells_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/g_n_bs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/location_frontend_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/login_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26635 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/monitoring_event_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/paths_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/qo_s_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27983 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/session_with_qo_s_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27373 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/u_es_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27801 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/ui_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api/utils_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:59:17.923067 evolved5g-1.0.8/evolved5g/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/accumulated_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/all_of_u_es_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/all_of_ue_create_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/all_of_ue_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/all_of_ue_update_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/cell_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/cell_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/gnb_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/gnb_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/location_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_event_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_event_report_received.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_event_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_event_subscription_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/path_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/path_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/qo_s_monitoring_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/qos_monitoring_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/reporting_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/snssai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/u_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/ue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14566 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/ue_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/ue_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/usage_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/user_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/user_plane_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/user_plane_event_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/user_plane_notification_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/user_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-04 14:58:32.000000 evolved5g-1.0.8/evolved5g/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:59:17.903066 evolved5g-1.0.8/evolved5g.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-04 14:59:17.000000 evolved5g-1.0.8/evolved5g.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-04 14:59:17.000000 evolved5g-1.0.8/evolved5g.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:59:17.000000 evolved5g-1.0.8/evolved5g.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 14:59:17.000000 evolved5g-1.0.8/evolved5g.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:59:13.000000 evolved5g-1.0.8/evolved5g.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 14:59:17.000000 evolved5g-1.0.8/evolved5g.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 14:59:17.000000 evolved5g-1.0.8/evolved5g.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 14:58:32.000000 evolved5g-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-04 14:59:17.923067 evolved5g-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-04 14:58:32.000000 evolved5g-1.0.8/setup.py
```

### Comparing `evolved5g-1.0.7/CONTRIBUTING.rst` & `evolved5g-1.0.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/HISTORY.rst` & `evolved5g-1.0.8/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 =======
 History
 =======
 
 -------------------
+1.0.8 (2023-07-04)
+-------------------
+* Bug fix on CAPIFConnector.offboard_and_deregister_netapp method
+* Update on documentation
+
+-------------------
 1.0.7 (2023-06-15)
 -------------------
 * Bug fix on CLI method register_and_onboard_to_capif: Now accepts a second parameter --environment that takes values "production" or "development".
 If this parameter is set to production then validation tests are running in the background, just after the registration and onboarding of the network app finishes.
 
 
 -------------------
```

### Comparing `evolved5g-1.0.7/LICENSE` & `evolved5g-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/PKG-INFO` & `evolved5g-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolved5g
-Version: 1.0.7
+Version: 1.0.8
 Summary: Evolved5G CLI prototype 
 Home-page: https://github.com/EVOLVED-5G/SDK-CLI
 Author: EVOLVED5G project
 License: Apache Software License 2.0
 Description: *******************
         Evolved5G CLI & SDK
         *******************
@@ -54,14 +54,20 @@
         
         
         =======
         History
         =======
         
         -------------------
+        1.0.8 (2023-07-04)
+        -------------------
+        * Bug fix on CAPIFConnector.offboard_and_deregister_netapp method
+        * Update on documentation
+        
+        -------------------
         1.0.7 (2023-06-15)
         -------------------
         * Bug fix on CLI method register_and_onboard_to_capif: Now accepts a second parameter --environment that takes values "production" or "development".
         If this parameter is set to production then validation tests are running in the background, just after the registration and onboarding of the network app finishes.
         
         
         -------------------
```

### Comparing `evolved5g-1.0.7/README.rst` & `evolved5g-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/Makefile` & `evolved5g-1.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/make.bat` & `evolved5g-1.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/cli.rst` & `evolved5g-1.0.8/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/conf.py` & `evolved5g-1.0.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/dummy_html_example.png` & `evolved5g-1.0.8/docs/source/images/dummy_html_example.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/generate.gif` & `evolved5g-1.0.8/docs/source/images/generate.gif`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/generate_execution.png` & `evolved5g-1.0.8/docs/source/images/generate_execution.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/netapp_creation.gif` & `evolved5g-1.0.8/docs/source/images/netapp_creation.gif`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/netapp_repo.gif` & `evolved5g-1.0.8/docs/source/images/netapp_repo.gif`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/repo_creation.png` & `evolved5g-1.0.8/docs/source/images/repo_creation.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/repo_structure.png` & `evolved5g-1.0.8/docs/source/images/repo_structure.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/ssh_gpg.png` & `evolved5g-1.0.8/docs/source/images/ssh_gpg.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/ssh_key.png` & `evolved5g-1.0.8/docs/source/images/ssh_key.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/ssh_key_button.png` & `evolved5g-1.0.8/docs/source/images/ssh_key_button.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/token1.png` & `evolved5g-1.0.8/docs/source/images/token1.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/token2.png` & `evolved5g-1.0.8/docs/source/images/token2.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/images/token3.png` & `evolved5g-1.0.8/docs/source/images/token3.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/index.rst` & `evolved5g-1.0.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/information.rst` & `evolved5g-1.0.8/docs/source/information.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/installation.rst` & `evolved5g-1.0.8/docs/source/installation.rst`

 * *Files 13% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
 The sources for Evolved5G_CLI can be downloaded from the `Github repo`_.
 
 You can either clone the public repository:
 
 .. code-block:: console
 
-    $ git clone git://github.com/EVOLVED-5G/SDK-CLI
+    $ git clone git@github.com:EVOLVED-5G/SDK-CLI.git
+    $ git clone https://github.com/EVOLVED-5G/SDK-CLI.git
 
 Or download the `tarball`_.
 
 .. code-block:: console
 
     $ curl -OJL https://github.com/EVOLVED-5G/SDK-CLI/tarball/master
```

### Comparing `evolved5g-1.0.7/docs/source/libraries.rst` & `evolved5g-1.0.8/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/pipelines.rst` & `evolved5g-1.0.8/docs/source/pipelines.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/docs/source/pre_requisites.rst` & `evolved5g-1.0.8/docs/source/pre_requisites.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/cli.py` & `evolved5g-1.0.8/evolved5g/cli.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/cli_helper.py` & `evolved5g-1.0.8/evolved5g/cli_helper.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/nef_and_tsn_api_service_validation_pipeline.py` & `evolved5g-1.0.8/evolved5g/nef_and_tsn_api_service_validation_pipeline.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/sdk.py` & `evolved5g-1.0.8/evolved5g/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1066,16 +1066,14 @@
             "DELETE",
             url,
             headers={"Content-Type": "application/json"},
             data=json.dumps(payload)
         )
         response.raise_for_status()
 
-        response_payload = json.loads(response.text)
-        return response_payload
 
     def __save_capif_ca_root_file_and_get_auth_token(self, role):
 
         url = self.capif_http_url + "getauth"
 
         payload = dict()
         payload["username"] = self.capif_netapp_username
```

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/__init__.py` & `evolved5g-1.0.8/evolved5g/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/__init__.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/cells_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/cells_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/default_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/g_n_bs_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/g_n_bs_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/location_frontend_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/location_frontend_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/login_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/login_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/monitoring_event_api_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/monitoring_event_api_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/paths_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/paths_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/qo_s_information_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/qo_s_information_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/session_with_qo_s_api_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/session_with_qo_s_api_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/u_es_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/u_es_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/ui_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/ui_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/users_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api/utils_api.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api/utils_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/api_client.py` & `evolved5g-1.0.8/evolved5g/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/configuration.py` & `evolved5g-1.0.8/evolved5g/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/__init__.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/accumulated_usage.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/accumulated_usage.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/all_of_u_es_speed.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/all_of_u_es_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/all_of_ue_create_speed.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/all_of_ue_create_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/all_of_ue_speed.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/all_of_ue_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/all_of_ue_update_speed.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/all_of_ue_update_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/cell.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/cell.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/cell_create.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/cell_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/cell_update.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/cell_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/gnb.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/gnb.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/gnb_create.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/gnb_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/gnb_update.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/gnb_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/http_validation_error.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/location_info.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/location_info.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_event_report.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_event_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_event_report_received.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_event_report_received.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_event_subscription.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_event_subscription.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_event_subscription_create.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_event_subscription_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_notification.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_notification.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/monitoring_type.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/monitoring_type.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/msg.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/msg.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/path.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/path.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/path_create.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/path_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/path_update.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/path_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/paths.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/paths.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/point.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/point.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/qo_s_monitoring_report.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/qo_s_monitoring_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/qos_monitoring_information.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/qos_monitoring_information.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/reporting_frequency.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/reporting_frequency.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/snssai.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/snssai.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/speed.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/token.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/token.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/u_es.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/u_es.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/ue.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/ue.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/ue_create.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/ue_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/ue_update.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/ue_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/usage_threshold.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/usage_threshold.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/user.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/user.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/user_create.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/user_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/user_plane_event.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/user_plane_event.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/user_plane_event_report.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/user_plane_event_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/user_plane_notification_data.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/user_plane_notification_data.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/user_update.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/user_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/models/validation_error.py` & `evolved5g-1.0.8/evolved5g/swagger_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g/swagger_client/rest.py` & `evolved5g-1.0.8/evolved5g/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/evolved5g.egg-info/PKG-INFO` & `evolved5g-1.0.8/evolved5g.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolved5g
-Version: 1.0.7
+Version: 1.0.8
 Summary: Evolved5G CLI prototype 
 Home-page: https://github.com/EVOLVED-5G/SDK-CLI
 Author: EVOLVED5G project
 License: Apache Software License 2.0
 Description: *******************
         Evolved5G CLI & SDK
         *******************
@@ -54,14 +54,20 @@
         
         
         =======
         History
         =======
         
         -------------------
+        1.0.8 (2023-07-04)
+        -------------------
+        * Bug fix on CAPIFConnector.offboard_and_deregister_netapp method
+        * Update on documentation
+        
+        -------------------
         1.0.7 (2023-06-15)
         -------------------
         * Bug fix on CLI method register_and_onboard_to_capif: Now accepts a second parameter --environment that takes values "production" or "development".
         If this parameter is set to production then validation tests are running in the background, just after the registration and onboarding of the network app finishes.
         
         
         -------------------
```

### Comparing `evolved5g-1.0.7/evolved5g.egg-info/SOURCES.txt` & `evolved5g-1.0.8/evolved5g.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.7/setup.py` & `evolved5g-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords="evolved5g",
     name="evolved5g",
     packages=find_packages(include=["evolved5g", "evolved5g.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/EVOLVED-5G/SDK-CLI",
-    version="1.0.7",
+    version="1.0.8",
     zip_safe=False,
 )
```

