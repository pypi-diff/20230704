# Comparing `tmp/n-profile-sdk-1.9.8.tar.gz` & `tmp/n-profile-sdk-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n-profile-sdk-1.9.8.tar", last modified: Tue Jul  4 04:53:52 2023, max compression
+gzip compressed data, was "n-profile-sdk-2.3.4.tar", last modified: Tue Jul  4 04:45:24 2023, max compression
```

## Comparing `n-profile-sdk-1.9.8.tar` & `n-profile-sdk-2.3.4.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:53:52.282599 n-profile-sdk-1.9.8/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4817 2023-07-04 04:53:52.282599 n-profile-sdk-1.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4592 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:53:52.161595 n-profile-sdk-1.9.8/ctddocumentation/
--rw-r--r--   0 root         (0) root         (0)      154 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:53:52.176596 n-profile-sdk-1.9.8/ctddocumentation/controllers/
--rw-r--r--   0 root         (0) root         (0)      462 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5954 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/activities_controller.py
--rw-r--r--   0 root         (0) root         (0)    13390 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/alerts_controller.py
--rw-r--r--   0 root         (0) root         (0)    31715 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/assets_controller.py
--rw-r--r--   0 root         (0) root         (0)     1974 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/custom_attributes_categories_controller.py
--rw-r--r--   0 root         (0) root         (0)     5934 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/events_controller.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/groups_controller.py
--rw-r--r--   0 root         (0) root         (0)     8535 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/insights_controller.py
--rw-r--r--   0 root         (0) root         (0)     6074 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/license_controller.py
--rw-r--r--   0 root         (0) root         (0)     2689 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/login_controller.py
--rw-r--r--   0 root         (0) root         (0)    10643 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/queries_controller.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/sensors_controller.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/sites_controller.py
--rw-r--r--   0 root         (0) root         (0)    12351 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/tasks_controller.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/tasks_queries_controller.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/controllers/users_controller.py
--rw-r--r--   0 root         (0) root         (0)     5617 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/ctddocumentation_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:53:52.181596 n-profile-sdk-1.9.8/ctddocumentation/exceptions/
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/exceptions/api_exception.py
--rw-r--r--   0 root         (0) root         (0)     1678 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/exceptions/auth_authenticate_401_error_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:53:52.183596 n-profile-sdk-1.9.8/ctddocumentation/http/
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:53:52.186596 n-profile-sdk-1.9.8/ctddocumentation/http/auth/
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/http/auth/custom_header_authentication.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:53:52.271599 n-profile-sdk-1.9.8/ctddocumentation/models/
--rw-r--r--   0 root         (0) root         (0)     2449 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2435 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/actionable.py
--rw-r--r--   0 root         (0) root         (0)     2924 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/actionable_asset.py
--rw-r--r--   0 root         (0) root         (0)     2816 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/actionable_cap.py
--rw-r--r--   0 root         (0) root         (0)     2968 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/actionable_information.py
--rw-r--r--   0 root         (0) root         (0)    13915 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/actionable_policy.py
--rw-r--r--   0 root         (0) root         (0)     4885 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/actionable_related_asset.py
--rw-r--r--   0 root         (0) root         (0)    10401 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/active_history.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/activities_object.py
--rw-r--r--   0 root         (0) root         (0)     3617 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/activities_response.py
--rw-r--r--   0 root         (0) root         (0)     5304 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/activity.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/add_license_response.py
--rw-r--r--   0 root         (0) root         (0)    17213 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/alert.py
--rw-r--r--   0 root         (0) root         (0)      786 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/alert_severity_enum.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/asset.py
--rw-r--r--   0 root         (0) root         (0)     9049 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/assets_with_insights.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/assets_with_insights_response.py
--rw-r--r--   0 root         (0) root         (0)     1717 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/authenticate.py
--rw-r--r--   0 root         (0) root         (0)     6441 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/base_task.py
--rw-r--r--   0 root         (0) root         (0)     2989 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/cap.py
--rw-r--r--   0 root         (0) root         (0)     2240 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/code_sections.py
--rw-r--r--   0 root         (0) root         (0)      413 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/content_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     1801 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/create_a_new_query.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/create_a_new_query_response.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/create_group_response.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/create_user_response.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/createanewtask.py
--rw-r--r--   0 root         (0) root         (0)     1700 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/createanewtask_response.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/ctd_login_exception.py
--rw-r--r--   0 root         (0) root         (0)     3419 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/ctd_login_response.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/custom_attribute_category.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/db_statistics.py
--rw-r--r--   0 root         (0) root         (0)     1459 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/delete_a_query_response.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/delete_a_task_response.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/destination_virtual_zone.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/detail.py
--rw-r--r--   0 root         (0) root         (0)     2886 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/discovery_params.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/entity.py
--rw-r--r--   0 root         (0) root         (0)     5422 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/event.py
--rw-r--r--   0 root         (0) root         (0)    20380 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/find_asset_by_id_response.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/format_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/format_enum.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_active_detection_history_response.py
--rw-r--r--   0 root         (0) root         (0)     3040 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_alerts_response.py
--rw-r--r--   0 root         (0) root         (0)     3042 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_all_sites_response.py
--rw-r--r--   0 root         (0) root         (0)     3040 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_assets_response.py
--rw-r--r--   0 root         (0) root         (0)     3184 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_custom_attribute_categories_response.py
--rw-r--r--   0 root         (0) root         (0)     3040 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_events_response.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_license_details_response.py
--rw-r--r--   0 root         (0) root         (0)     2411 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_queries_ids_and_assigned_task_response.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_queries_response.py
--rw-r--r--   0 root         (0) root         (0)     3033 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_tasks_response.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/get_types_response.py
--rw-r--r--   0 root         (0) root         (0)     2429 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/group.py
--rw-r--r--   0 root         (0) root         (0)     2285 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/identifiable.py
--rw-r--r--   0 root         (0) root         (0)     2947 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/indicator_info.py
--rw-r--r--   0 root         (0) root         (0)     4466 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/indicators.py
--rw-r--r--   0 root         (0) root         (0)     6675 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/information.py
--rw-r--r--   0 root         (0) root         (0)      676 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/insight_status_enum.py
--rw-r--r--   0 root         (0) root         (0)      629 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/insight_status_exact_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/insight_status_exact_enum.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/license_request.py
--rw-r--r--   0 root         (0) root         (0)     2586 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/network.py
--rw-r--r--   0 root         (0) root         (0)     6774 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/new_queryobject.py
--rw-r--r--   0 root         (0) root         (0)     6767 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/new_taskobject.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/object.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/paginated_response.py
--rw-r--r--   0 root         (0) root         (0)    12691 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/policy.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/queryextraparams.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/ranger_system_check_response.py
--rw-r--r--   0 root         (0) root         (0)     2742 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/risk_vector.py
--rw-r--r--   0 root         (0) root         (0)     1910 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/selection_params.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/selection_params_1.py
--rw-r--r--   0 root         (0) root         (0)     9791 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/site.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/site_list_slim_enum.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/slim_insight.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/sort_1_enum.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/sort_31_enum.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/sort_3_enum.py
--rw-r--r--   0 root         (0) root         (0)     1062 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/sort_41_enum.py
--rw-r--r--   0 root         (0) root         (0)     1055 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/sort_4_enum.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/sort_5_enum.py
--rw-r--r--   0 root         (0) root         (0)     1037 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/sort_6_enum.py
--rw-r--r--   0 root         (0) root         (0)     3405 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/sort_enum.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/source_virtual_zone.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/special_hint_enum.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/special_hint_exact_enum.py
--rw-r--r--   0 root         (0) root         (0)      423 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/status_enum.py
--rw-r--r--   0 root         (0) root         (0)      622 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/status_exact_enum.py
--rw-r--r--   0 root         (0) root         (0)     1545 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/subnet.py
--rw-r--r--   0 root         (0) root         (0)     9300 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/task.py
--rw-r--r--   0 root         (0) root         (0)     2504 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/taskextraparams.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/update_a_single_query_response.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/update_a_single_task_response.py
--rw-r--r--   0 root         (0) root         (0)     2599 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/update_license_response.py
--rw-r--r--   0 root         (0) root         (0)     2853 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/user.py
--rw-r--r--   0 root         (0) root         (0)     4661 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/models/virtual_zones.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:53:52.273599 n-profile-sdk-1.9.8/ctddocumentation/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/ctddocumentation/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:53:52.279599 n-profile-sdk-1.9.8/n_profile_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4817 2023-07-04 04:53:52.000000 n-profile-sdk-1.9.8/n_profile_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6071 2023-07-04 04:53:52.000000 n-profile-sdk-1.9.8/n_profile_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 04:53:52.000000 n-profile-sdk-1.9.8/n_profile_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-07-04 04:53:52.000000 n-profile-sdk-1.9.8/n_profile_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-04 04:53:52.000000 n-profile-sdk-1.9.8/n_profile_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      602 2023-07-04 04:53:24.000000 n-profile-sdk-1.9.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-07-04 04:53:52.283599 n-profile-sdk-1.9.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:45:24.748082 n-profile-sdk-2.3.4/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-07-04 04:45:24.749082 n-profile-sdk-2.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:45:24.647082 n-profile-sdk-2.3.4/ctddocumentation/
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:45:24.653082 n-profile-sdk-2.3.4/ctddocumentation/controllers/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/activities_controller.py
+-rw-r--r--   0 root         (0) root         (0)    13390 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/alerts_controller.py
+-rw-r--r--   0 root         (0) root         (0)    31715 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/assets_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/custom_attributes_categories_controller.py
+-rw-r--r--   0 root         (0) root         (0)     5934 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/events_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/groups_controller.py
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/insights_controller.py
+-rw-r--r--   0 root         (0) root         (0)     6074 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/license_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/login_controller.py
+-rw-r--r--   0 root         (0) root         (0)    10643 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/queries_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/sensors_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/sites_controller.py
+-rw-r--r--   0 root         (0) root         (0)    12351 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/tasks_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/tasks_queries_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/controllers/users_controller.py
+-rw-r--r--   0 root         (0) root         (0)     5617 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/ctddocumentation_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:45:24.655082 n-profile-sdk-2.3.4/ctddocumentation/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/exceptions/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/exceptions/auth_authenticate_401_error_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:45:24.658082 n-profile-sdk-2.3.4/ctddocumentation/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:45:24.659082 n-profile-sdk-2.3.4/ctddocumentation/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/http/auth/custom_header_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:45:24.742082 n-profile-sdk-2.3.4/ctddocumentation/models/
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/actionable.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/actionable_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/actionable_cap.py
+-rw-r--r--   0 root         (0) root         (0)     2968 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/actionable_information.py
+-rw-r--r--   0 root         (0) root         (0)    13915 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/actionable_policy.py
+-rw-r--r--   0 root         (0) root         (0)     4885 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/actionable_related_asset.py
+-rw-r--r--   0 root         (0) root         (0)    10401 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/active_history.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/activities_object.py
+-rw-r--r--   0 root         (0) root         (0)     3617 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/activities_response.py
+-rw-r--r--   0 root         (0) root         (0)     5304 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/activity.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/add_license_response.py
+-rw-r--r--   0 root         (0) root         (0)    17213 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/alert.py
+-rw-r--r--   0 root         (0) root         (0)      786 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/alert_severity_enum.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/asset.py
+-rw-r--r--   0 root         (0) root         (0)     9049 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/assets_with_insights.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/assets_with_insights_response.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/authenticate.py
+-rw-r--r--   0 root         (0) root         (0)     6441 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/base_task.py
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/cap.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/code_sections.py
+-rw-r--r--   0 root         (0) root         (0)      413 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/content_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/create_a_new_query.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/create_a_new_query_response.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/create_group_response.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/create_user_response.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/createanewtask.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/createanewtask_response.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/ctd_login_exception.py
+-rw-r--r--   0 root         (0) root         (0)     3419 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/ctd_login_response.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/custom_attribute_category.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/db_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/delete_a_query_response.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/delete_a_task_response.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/destination_virtual_zone.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/detail.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/discovery_params.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/entity.py
+-rw-r--r--   0 root         (0) root         (0)     5422 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/event.py
+-rw-r--r--   0 root         (0) root         (0)    20380 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/find_asset_by_id_response.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/format_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/format_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_active_detection_history_response.py
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_alerts_response.py
+-rw-r--r--   0 root         (0) root         (0)     3042 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_all_sites_response.py
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_assets_response.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_custom_attribute_categories_response.py
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_events_response.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_license_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     2411 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_queries_ids_and_assigned_task_response.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_queries_response.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_tasks_response.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/get_types_response.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/group.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/identifiable.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/indicator_info.py
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/indicators.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/information.py
+-rw-r--r--   0 root         (0) root         (0)      676 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/insight_status_enum.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/insight_status_exact_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      512 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/insight_status_exact_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/license_request.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/network.py
+-rw-r--r--   0 root         (0) root         (0)     6774 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/new_queryobject.py
+-rw-r--r--   0 root         (0) root         (0)     6767 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/new_taskobject.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/object.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/paginated_response.py
+-rw-r--r--   0 root         (0) root         (0)    12691 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/policy.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/queryextraparams.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/ranger_system_check_response.py
+-rw-r--r--   0 root         (0) root         (0)     2742 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/risk_vector.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/selection_params.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/selection_params_1.py
+-rw-r--r--   0 root         (0) root         (0)     9791 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/site.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/site_list_slim_enum.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/slim_insight.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/sort_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/sort_31_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/sort_3_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/sort_41_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/sort_4_enum.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/sort_5_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/sort_6_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3405 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/sort_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/source_virtual_zone.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/special_hint_enum.py
+-rw-r--r--   0 root         (0) root         (0)      636 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/special_hint_exact_enum.py
+-rw-r--r--   0 root         (0) root         (0)      423 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)      622 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/status_exact_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/subnet.py
+-rw-r--r--   0 root         (0) root         (0)     9300 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/task.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/taskextraparams.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/update_a_single_query_response.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/update_a_single_task_response.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/update_license_response.py
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/models/virtual_zones.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:45:24.743082 n-profile-sdk-2.3.4/ctddocumentation/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/ctddocumentation/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:45:24.748082 n-profile-sdk-2.3.4/n_profile_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-07-04 04:45:24.000000 n-profile-sdk-2.3.4/n_profile_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6071 2023-07-04 04:45:24.000000 n-profile-sdk-2.3.4/n_profile_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 04:45:24.000000 n-profile-sdk-2.3.4/n_profile_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-04 04:45:24.000000 n-profile-sdk-2.3.4/n_profile_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-04 04:45:24.000000 n-profile-sdk-2.3.4/n_profile_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      602 2023-07-04 04:44:55.000000 n-profile-sdk-2.3.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-04 04:45:24.750082 n-profile-sdk-2.3.4/setup.cfg
```

### Comparing `n-profile-sdk-1.9.8/LICENSE` & `n-profile-sdk-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/PKG-INFO` & `n-profile-sdk-2.3.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,85 @@
-Metadata-Version: 2.1
-Name: n-profile-sdk
-Version: 1.9.8
-Summary: this is testing
-Author-email: Subtain <Subtain@gmail.com>
-Project-URL: Documentation, https://subtain.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testutils
-License-File: LICENSE
-
-
-# Getting Started with CTD - Documentation
-
-## Install the Package
-
+
+# Getting Started with CTD - Documentation
+
+## Install the Package
+
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
-Install the package from PyPi using the following pip command:
-
-```python
-pip install n-profile-sdk==1.9.8
-```
-
+Install the package from PyPi using the following pip command:
+
+```python
+pip install n-profile-sdk==2.3.4
+```
+
 You can also view the package at:
-https://pypi.python.org/pypi/n-profile-sdk/1.9.8
-
-## Test the SDK
-
-You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
-
+https://pypi.python.org/pypi/n-profile-sdk/2.3.4
+
+## Test the SDK
+
+You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
+
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
-```
-
-## Initialize the API Client
-
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/client.md)
-
-The following parameters are configurable for the API Client:
-
-| Parameter | Type | Description |
-|  --- | --- | --- |
-| `host` | `string` | *Default*: `'HostValue'` |
-| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
-| `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
-| `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
-| `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
-| `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
-| `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
-| `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
-| `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
-| `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
-| `authorization` | `string` |  |
-
-The API client can be initialized as follows:
-
-```python
-from ctddocumentation.ctddocumentation_client import CtddocumentationClient
+```
+
+## Initialize the API Client
+
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/client.md)
+
+The following parameters are configurable for the API Client:
+
+| Parameter | Type | Description |
+|  --- | --- | --- |
+| `host` | `string` | *Default*: `'HostValue'` |
+| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
+| `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
+| `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
+| `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
+| `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
+| `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
+| `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
+| `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
+| `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
+| `authorization` | `string` |  |
+
+The API client can be initialized as follows:
+
+```python
+from ctddocumentation.ctddocumentation_client import CtddocumentationClient
 from ctddocumentation.configuration import Environment
-
+
 client = CtddocumentationClient(
     authorization='Authorization'
-)
-```
-
-## Authorization
-
-This API uses `Custom Header Signature`.
-
-## List of APIs
-
-* [Tasks Queries](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/tasks-queries.md)
-* [Custom Attributes Categories](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/custom-attributes-categories.md)
-* [Login](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/login.md)
-* [Assets](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/assets.md)
-* [Alerts](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/alerts.md)
-* [Tasks](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/tasks.md)
-* [Queries](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/queries.md)
-* [Insights](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/insights.md)
-* [Sites](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/sites.md)
-* [Activities](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/activities.md)
-* [License](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/license.md)
-* [Users](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/users.md)
-* [Groups](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/groups.md)
-* [Sensors](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/sensors.md)
-* [Events](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/events.md)
-
-## Classes Documentation
-
-* [Utility Classes](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/http-request.md)
-
+)
+```
+
+## Authorization
+
+This API uses `Custom Header Signature`.
+
+## List of APIs
+
+* [Tasks Queries](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/tasks-queries.md)
+* [Custom Attributes Categories](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/custom-attributes-categories.md)
+* [Login](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/login.md)
+* [Assets](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/assets.md)
+* [Alerts](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/alerts.md)
+* [Tasks](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/tasks.md)
+* [Queries](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/queries.md)
+* [Insights](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/insights.md)
+* [Sites](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/sites.md)
+* [Activities](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/activities.md)
+* [License](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/license.md)
+* [Users](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/users.md)
+* [Groups](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/groups.md)
+* [Sensors](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/sensors.md)
+* [Events](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/events.md)
+
+## Classes Documentation
+
+* [Utility Classes](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/http-request.md)
+
```

### Comparing `n-profile-sdk-1.9.8/README.md` & `n-profile-sdk-2.3.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,96 @@
-
-# Getting Started with CTD - Documentation
-
-## Install the Package
-
+Metadata-Version: 2.1
+Name: n-profile-sdk
+Version: 2.3.4
+Summary: this is testing
+Author-email: Subtain <Subtain@gmail.com>
+Project-URL: Documentation, https://subtain.com
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: testutils
+License-File: LICENSE
+
+
+# Getting Started with CTD - Documentation
+
+## Install the Package
+
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
-Install the package from PyPi using the following pip command:
-
-```python
-pip install n-profile-sdk==1.9.8
-```
-
+Install the package from PyPi using the following pip command:
+
+```python
+pip install n-profile-sdk==2.3.4
+```
+
 You can also view the package at:
-https://pypi.python.org/pypi/n-profile-sdk/1.9.8
-
-## Test the SDK
-
-You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
-
+https://pypi.python.org/pypi/n-profile-sdk/2.3.4
+
+## Test the SDK
+
+You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
+
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
-```
-
-## Initialize the API Client
-
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/client.md)
-
-The following parameters are configurable for the API Client:
-
-| Parameter | Type | Description |
-|  --- | --- | --- |
-| `host` | `string` | *Default*: `'HostValue'` |
-| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
-| `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
-| `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
-| `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
-| `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
-| `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
-| `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
-| `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
-| `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
-| `authorization` | `string` |  |
-
-The API client can be initialized as follows:
-
-```python
-from ctddocumentation.ctddocumentation_client import CtddocumentationClient
+```
+
+## Initialize the API Client
+
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/client.md)
+
+The following parameters are configurable for the API Client:
+
+| Parameter | Type | Description |
+|  --- | --- | --- |
+| `host` | `string` | *Default*: `'HostValue'` |
+| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
+| `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
+| `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
+| `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
+| `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
+| `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
+| `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
+| `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
+| `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
+| `authorization` | `string` |  |
+
+The API client can be initialized as follows:
+
+```python
+from ctddocumentation.ctddocumentation_client import CtddocumentationClient
 from ctddocumentation.configuration import Environment
-
+
 client = CtddocumentationClient(
     authorization='Authorization'
-)
-```
-
-## Authorization
-
-This API uses `Custom Header Signature`.
-
-## List of APIs
-
-* [Tasks Queries](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/tasks-queries.md)
-* [Custom Attributes Categories](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/custom-attributes-categories.md)
-* [Login](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/login.md)
-* [Assets](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/assets.md)
-* [Alerts](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/alerts.md)
-* [Tasks](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/tasks.md)
-* [Queries](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/queries.md)
-* [Insights](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/insights.md)
-* [Sites](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/sites.md)
-* [Activities](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/activities.md)
-* [License](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/license.md)
-* [Users](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/users.md)
-* [Groups](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/groups.md)
-* [Sensors](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/sensors.md)
-* [Events](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/events.md)
-
-## Classes Documentation
-
-* [Utility Classes](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/http-request.md)
-
+)
+```
+
+## Authorization
+
+This API uses `Custom Header Signature`.
+
+## List of APIs
+
+* [Tasks Queries](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/tasks-queries.md)
+* [Custom Attributes Categories](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/custom-attributes-categories.md)
+* [Login](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/login.md)
+* [Assets](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/assets.md)
+* [Alerts](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/alerts.md)
+* [Tasks](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/tasks.md)
+* [Queries](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/queries.md)
+* [Insights](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/insights.md)
+* [Sites](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/sites.md)
+* [Activities](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/activities.md)
+* [License](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/license.md)
+* [Users](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/users.md)
+* [Groups](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/groups.md)
+* [Sensors](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/sensors.md)
+* [Events](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/events.md)
+
+## Classes Documentation
+
+* [Utility Classes](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/http-request.md)
+
```

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/api_helper.py` & `n-profile-sdk-2.3.4/ctddocumentation/api_helper.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/configuration.py` & `n-profile-sdk-2.3.4/ctddocumentation/configuration.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/activities_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/activities_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/alerts_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/alerts_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/assets_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/assets_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/base_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/custom_attributes_categories_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/custom_attributes_categories_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/events_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/events_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/groups_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/groups_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/insights_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/insights_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/license_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/license_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/login_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/login_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/queries_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/queries_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/sensors_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/sensors_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/sites_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/sites_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/tasks_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/tasks_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/tasks_queries_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/tasks_queries_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/controllers/users_controller.py` & `n-profile-sdk-2.3.4/ctddocumentation/controllers/users_controller.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/ctddocumentation_client.py` & `n-profile-sdk-2.3.4/ctddocumentation/ctddocumentation_client.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/exceptions/api_exception.py` & `n-profile-sdk-2.3.4/ctddocumentation/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/exceptions/auth_authenticate_401_error_exception.py` & `n-profile-sdk-2.3.4/ctddocumentation/exceptions/auth_authenticate_401_error_exception.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/http/auth/custom_header_authentication.py` & `n-profile-sdk-2.3.4/ctddocumentation/http/auth/custom_header_authentication.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/http/http_request.py` & `n-profile-sdk-2.3.4/ctddocumentation/http/http_request.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/http/http_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/http/http_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/__init__.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/__init__.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/actionable.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/actionable.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/actionable_asset.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/actionable_asset.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/actionable_cap.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/actionable_cap.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/actionable_information.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/actionable_information.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/actionable_policy.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/actionable_policy.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/actionable_related_asset.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/actionable_related_asset.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/active_history.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/active_history.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/activities_object.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/activities_object.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/activities_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/activities_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/activity.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/activity.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/add_license_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/add_license_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/alert.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/alert.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/alert_severity_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/alert_severity_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/asset.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/asset.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/assets_with_insights.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/assets_with_insights.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/assets_with_insights_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/assets_with_insights_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/authenticate.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/authenticate.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/base_task.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/base_task.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/cap.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/cap.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/code_sections.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/code_sections.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/create_a_new_query.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/create_a_new_query.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/create_a_new_query_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/create_a_new_query_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/create_group_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/create_group_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/create_user_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/create_user_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/createanewtask.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/createanewtask.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/createanewtask_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/createanewtask_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/ctd_login_exception.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/ctd_login_exception.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/ctd_login_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/ctd_login_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/custom_attribute_category.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/custom_attribute_category.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/db_statistics.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/db_statistics.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/delete_a_query_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/delete_a_query_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/delete_a_task_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/delete_a_task_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/destination_virtual_zone.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/destination_virtual_zone.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/detail.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/detail.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/discovery_params.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/discovery_params.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/entity.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/entity.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/event.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/event.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/find_asset_by_id_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/find_asset_by_id_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/format_1_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/format_1_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/format_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/format_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_active_detection_history_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_active_detection_history_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_alerts_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_alerts_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_all_sites_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_all_sites_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_assets_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_assets_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_custom_attribute_categories_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_custom_attribute_categories_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_events_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_events_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_license_details_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_license_details_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_queries_ids_and_assigned_task_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_queries_ids_and_assigned_task_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_queries_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_queries_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_tasks_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_tasks_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/get_types_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/get_types_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/group.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/group.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/identifiable.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/identifiable.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/indicator_info.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/indicator_info.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/indicators.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/indicators.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/information.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/information.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/insight_status_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/insight_status_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/insight_status_exact_1_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/insight_status_exact_1_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/insight_status_exact_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/insight_status_exact_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/license_request.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/license_request.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/network.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/network.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/new_queryobject.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/new_queryobject.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/new_taskobject.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/new_taskobject.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/object.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/object.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/paginated_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/paginated_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/policy.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/policy.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/queryextraparams.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/queryextraparams.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/ranger_system_check_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/ranger_system_check_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/risk_vector.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/risk_vector.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/selection_params.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/selection_params.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/selection_params_1.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/selection_params_1.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/site.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/site.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/slim_insight.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/slim_insight.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/sort_1_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/sort_1_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/sort_31_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/sort_31_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/sort_3_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/sort_3_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/sort_41_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/sort_41_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/sort_4_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/sort_4_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/sort_5_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/sort_5_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/sort_6_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/sort_6_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/sort_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/sort_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/source_virtual_zone.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/source_virtual_zone.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/special_hint_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/special_hint_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/special_hint_exact_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/special_hint_exact_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/status_exact_enum.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/status_exact_enum.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/subnet.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/subnet.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/task.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/task.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/taskextraparams.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/taskextraparams.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/update_a_single_query_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/update_a_single_query_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/update_a_single_task_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/update_a_single_task_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/update_license_response.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/update_license_response.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/user.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/user.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/ctddocumentation/models/virtual_zones.py` & `n-profile-sdk-2.3.4/ctddocumentation/models/virtual_zones.py`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/n_profile_sdk.egg-info/PKG-INFO` & `n-profile-sdk-2.3.4/n_profile_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n-profile-sdk
-Version: 1.9.8
+Version: 2.3.4
 Summary: this is testing
 Author-email: Subtain <Subtain@gmail.com>
 Project-URL: Documentation, https://subtain.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testutils
 License-File: LICENSE
@@ -14,34 +14,34 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install n-profile-sdk==1.9.8
+pip install n-profile-sdk==2.3.4
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/n-profile-sdk/1.9.8
+https://pypi.python.org/pypi/n-profile-sdk/2.3.4
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `host` | `string` | *Default*: `'HostValue'` |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
@@ -68,29 +68,29 @@
 
 ## Authorization
 
 This API uses `Custom Header Signature`.
 
 ## List of APIs
 
-* [Tasks Queries](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/tasks-queries.md)
-* [Custom Attributes Categories](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/custom-attributes-categories.md)
-* [Login](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/login.md)
-* [Assets](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/assets.md)
-* [Alerts](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/alerts.md)
-* [Tasks](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/tasks.md)
-* [Queries](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/queries.md)
-* [Insights](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/insights.md)
-* [Sites](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/sites.md)
-* [Activities](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/activities.md)
-* [License](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/license.md)
-* [Users](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/users.md)
-* [Groups](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/groups.md)
-* [Sensors](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/sensors.md)
-* [Events](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/controllers/events.md)
+* [Tasks Queries](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/tasks-queries.md)
+* [Custom Attributes Categories](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/custom-attributes-categories.md)
+* [Login](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/login.md)
+* [Assets](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/assets.md)
+* [Alerts](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/alerts.md)
+* [Tasks](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/tasks.md)
+* [Queries](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/queries.md)
+* [Insights](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/insights.md)
+* [Sites](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/sites.md)
+* [Activities](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/activities.md)
+* [License](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/license.md)
+* [Users](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/users.md)
+* [Groups](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/groups.md)
+* [Sensors](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/sensors.md)
+* [Events](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/controllers/events.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/Syed-Subtain/testn-profile-python-sdk/tree/1.9.8/doc/http-request.md)
+* [Utility Classes](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/n-profile-python-sdk/tree/2.3.4/doc/http-request.md)
```

### Comparing `n-profile-sdk-1.9.8/n_profile_sdk.egg-info/SOURCES.txt` & `n-profile-sdk-2.3.4/n_profile_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `n-profile-sdk-1.9.8/pyproject.toml` & `n-profile-sdk-2.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "n-profile-sdk"
 description = "this is testing"
-version = "1.9.8"
+version = "2.3.4"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = []
 authors = [{name = "Subtain", email = "Subtain@gmail.com"}]
 urls = {Documentation = "https://subtain.com"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10"]
 classifiers = []
```

