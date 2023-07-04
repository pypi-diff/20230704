# Comparing `tmp/lusid-notification-sdk-preview-0.1.762.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.762.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.762.tar", last modified: Thu Jun 29 13:40:05 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.762.2.tar", last modified: Tue Jul  4 14:45:06 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.762.tar` & `lusid-notification-sdk-preview-0.1.762.2.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7826 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4279 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      442 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6847 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    13984 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52797 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47803 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27431 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16631 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     2991 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7231 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    11055 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     9333 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/api_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    10618 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    12413 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15029 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/event_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     9778 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8021 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9510 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6425 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9539 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7863 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6827 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7436 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    15651 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)    35621 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7768 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7516 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8104 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     8447 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    11551 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15899 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13560 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2618 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 13:40:05.000000 lusid-notification-sdk-preview-0.1.762/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-06-29 13:38:47.000000 lusid-notification-sdk-preview-0.1.762/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8392 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4898 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6851 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7824 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52809 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47815 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27787 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16637 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5101 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     3608 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9019 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    11057 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     8320 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/amazon_sqs_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     9335 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/api_request_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     7301 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/api_request_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    10620 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15031 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    10459 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/email_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/event_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9780 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8023 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9512 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9541 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10706 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6881 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    16039 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)    35623 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    25118 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     6100 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7770 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8106 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/sms_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    16642 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8449 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    11553 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15901 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13100 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/webhook_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    13562 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2995 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 14:45:06.000000 lusid-notification-sdk-preview-0.1.762.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-07-04 14:44:44.000000 lusid-notification-sdk-preview-0.1.762.2/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.762/README.md` & `lusid-notification-sdk-preview-0.1.762.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.762
-- Package version: 0.1.762
+- API version: 0.1.762.2
+- Package version: 0.1.762.2
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -109,18 +109,21 @@
 
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
  - [AmazonSqsNotificationType](docs/AmazonSqsNotificationType.md)
+ - [AmazonSqsNotificationTypeResponse](docs/AmazonSqsNotificationTypeResponse.md)
  - [ApiRequestNotificationType](docs/ApiRequestNotificationType.md)
+ - [ApiRequestNotificationTypeResponse](docs/ApiRequestNotificationTypeResponse.md)
  - [CreateNotificationRequest](docs/CreateNotificationRequest.md)
  - [CreateSubscription](docs/CreateSubscription.md)
  - [EmailNotificationType](docs/EmailNotificationType.md)
+ - [EmailNotificationTypeResponse](docs/EmailNotificationTypeResponse.md)
  - [EventFieldDefinition](docs/EventFieldDefinition.md)
  - [EventTypeSchema](docs/EventTypeSchema.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [Link](docs/Link.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
@@ -128,30 +131,36 @@
  - [ManualEventBody](docs/ManualEventBody.md)
  - [ManualEventHeader](docs/ManualEventHeader.md)
  - [ManualEventRequest](docs/ManualEventRequest.md)
  - [MatchingPattern](docs/MatchingPattern.md)
  - [Notification](docs/Notification.md)
  - [NotificationStatus](docs/NotificationStatus.md)
  - [NotificationType](docs/NotificationType.md)
+ - [NotificationTypeResponse](docs/NotificationTypeResponse.md)
  - [ResourceId](docs/ResourceId.md)
  - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
  - [ResourceListOfEventTypeSchema](docs/ResourceListOfEventTypeSchema.md)
  - [ResourceListOfNotification](docs/ResourceListOfNotification.md)
  - [ResourceListOfSubscription](docs/ResourceListOfSubscription.md)
  - [SmsNotificationType](docs/SmsNotificationType.md)
+ - [SmsNotificationTypeResponse](docs/SmsNotificationTypeResponse.md)
  - [Subscription](docs/Subscription.md)
  - [UpdateNotificationRequest](docs/UpdateNotificationRequest.md)
  - [UpdateSubscription](docs/UpdateSubscription.md)
  - [WebhookNotificationType](docs/WebhookNotificationType.md)
+ - [WebhookNotificationTypeResponse](docs/WebhookNotificationTypeResponse.md)
 
 
+<a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
 
-## oauth2
+Authentication schemes defined for the API:
+<a id="oauth2"></a>
+### oauth2
 
 - **Type**: OAuth
 - **Flow**: implicit
 - **Authorization URL**: https://lusid.okta.com/oauth2/default/v1/authorize
 - **Scopes**: N/A
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.762"
+__version__ = "0.1.762.2"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
 from lusid_notification.api.subscriptions_api import SubscriptionsApi
@@ -33,18 +33,21 @@
 from lusid_notification.exceptions import ApiKeyError
 from lusid_notification.exceptions import ApiException
 # import models into sdk package
 from lusid_notification.models.access_controlled_action import AccessControlledAction
 from lusid_notification.models.access_controlled_resource import AccessControlledResource
 from lusid_notification.models.action_id import ActionId
 from lusid_notification.models.amazon_sqs_notification_type import AmazonSqsNotificationType
+from lusid_notification.models.amazon_sqs_notification_type_response import AmazonSqsNotificationTypeResponse
 from lusid_notification.models.api_request_notification_type import ApiRequestNotificationType
+from lusid_notification.models.api_request_notification_type_response import ApiRequestNotificationTypeResponse
 from lusid_notification.models.create_notification_request import CreateNotificationRequest
 from lusid_notification.models.create_subscription import CreateSubscription
 from lusid_notification.models.email_notification_type import EmailNotificationType
+from lusid_notification.models.email_notification_type_response import EmailNotificationTypeResponse
 from lusid_notification.models.event_field_definition import EventFieldDefinition
 from lusid_notification.models.event_type_schema import EventTypeSchema
 from lusid_notification.models.id_selector_definition import IdSelectorDefinition
 from lusid_notification.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notification.models.link import Link
 from lusid_notification.models.lusid_problem_details import LusidProblemDetails
 from lusid_notification.models.lusid_validation_problem_details import LusidValidationProblemDetails
@@ -52,24 +55,27 @@
 from lusid_notification.models.manual_event_body import ManualEventBody
 from lusid_notification.models.manual_event_header import ManualEventHeader
 from lusid_notification.models.manual_event_request import ManualEventRequest
 from lusid_notification.models.matching_pattern import MatchingPattern
 from lusid_notification.models.notification import Notification
 from lusid_notification.models.notification_status import NotificationStatus
 from lusid_notification.models.notification_type import NotificationType
+from lusid_notification.models.notification_type_response import NotificationTypeResponse
 from lusid_notification.models.resource_id import ResourceId
 from lusid_notification.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from lusid_notification.models.resource_list_of_event_type_schema import ResourceListOfEventTypeSchema
 from lusid_notification.models.resource_list_of_notification import ResourceListOfNotification
 from lusid_notification.models.resource_list_of_subscription import ResourceListOfSubscription
 from lusid_notification.models.sms_notification_type import SmsNotificationType
+from lusid_notification.models.sms_notification_type_response import SmsNotificationTypeResponse
 from lusid_notification.models.subscription import Subscription
 from lusid_notification.models.update_notification_request import UpdateNotificationRequest
 from lusid_notification.models.update_subscription import UpdateSubscription
 from lusid_notification.models.webhook_notification_type import WebhookNotificationType
+from lusid_notification.models.webhook_notification_type_response import WebhookNotificationTypeResponse
 
 # import utilities into sdk package
 from fbnsdkutilities.utilities.api_client_builder import ApiClientBuilder
 from fbnsdkutilities.utilities.api_configuration import ApiConfiguration
 from fbnsdkutilities.utilities.api_configuration_loader import ApiConfigurationLoader
 from fbnsdkutilities.utilities.refreshing_token import RefreshingToken
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/event_types_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/manual_event_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api/subscriptions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.762'
+        header_params['X-LUSID-SDK-Version'] = '0.1.762.2'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.762/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.762.2/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -193,27 +193,27 @@
 
         self.last_response = response_data
 
         return_data = response_data
 
         if not _preload_content:
             return return_data
-        
+
         response_type = response_types_map.get(response_data.status, None)
 
         if six.PY3 and response_type not in ["file", "bytes"]:
             match = None
             content_type = response_data.getheader('content-type')
             if content_type is not None:
                 match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
             encoding = match.group(1) if match else "utf-8"
             response_data.data = response_data.data.decode(encoding)
 
         # deserialize response data
-        
+
         if response_type:
             return_data = self.deserialize(response_data, response_type)
         else:
             return_data = None
 
         if _return_http_data_only:
             return (return_data)
@@ -298,16 +298,16 @@
 
         if type(klass) == str:
             if klass.startswith('list['):
                 sub_kls = re.match(r'list\[(.*)\]', klass).group(1)
                 return [self.__deserialize(sub_data, sub_kls)
                         for sub_data in data]
 
-            if klass.startswith('dict('):
-                sub_kls = re.match(r'dict\(([^,]*), (.*)\)', klass).group(2)
+            if klass.startswith('dict['):
+                sub_kls = re.match(r'dict\[([^,]*), (.*)\]', klass).group(2)
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in six.iteritems(data)}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
@@ -518,65 +518,72 @@
         accepts = [x.lower() for x in accepts]
 
         if 'application/json' in accepts:
             return 'application/json'
         else:
             return ', '.join(accepts)
 
-    def select_header_content_type(self, content_types):
+    def select_header_content_type(self, content_types, method=None, body=None):
         """Returns `Content-Type` based on an array of content_types provided.
 
         :param content_types: List of content-types.
+        :param method: http method (e.g. POST, PATCH).
+        :param body: http body to send.
         :return: Content-Type (e.g. application/json).
         """
         if not content_types:
-            return 'application/json'
+            return None
 
         content_types = [x.lower() for x in content_types]
 
+        if (method == 'PATCH' and
+                'application/json-patch+json' in content_types and
+                isinstance(body, list)):
+            return 'application/json-patch+json'
+
         if 'application/json' in content_types or '*/*' in content_types:
             return 'application/json'
         else:
             return content_types[0]
 
-    def update_params_for_auth(self, headers, querys, auth_settings,
+    def update_params_for_auth(self, headers, queries, auth_settings,
                                request_auth=None):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
-        :param querys: Query parameters tuple list to be updated.
+        :param queries: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
         :param request_auth: if set, the provided settings will
                              override the token in the configuration.
         """
         if not auth_settings:
             return
 
         if request_auth:
-            self._apply_auth_params(headers, querys, request_auth)
+            self._apply_auth_params(headers, queries, request_auth)
             return
 
         for auth in auth_settings:
             auth_setting = self.configuration.auth_settings().get(auth)
             if auth_setting:
-                self._apply_auth_params(headers, querys, auth_setting)
+                self._apply_auth_params(headers, queries, auth_setting)
 
-    def _apply_auth_params(self, headers, querys, auth_setting):
+    def _apply_auth_params(self, headers, queries, auth_setting):
         """Updates the request parameters based on a single auth_setting
 
         :param headers: Header parameters dict to be updated.
-        :param querys: Query parameters tuple list to be updated.
+        :param queries: Query parameters tuple list to be updated.
         :param auth_setting: auth settings for the endpoint
         """
         if auth_setting['in'] == 'cookie':
             headers['Cookie'] = auth_setting['value']
         elif auth_setting['in'] == 'header':
             headers[auth_setting['key']] = auth_setting['value']
         elif auth_setting['in'] == 'query':
-            querys.append((auth_setting['key'], auth_setting['value']))
+            queries.append((auth_setting['key'], auth_setting['value']))
         else:
             raise ApiValueError(
                 'Authentication token must be in `query` or `header`'
             )
 
     def __deserialize_file(self, response):
         """Deserializes body to file
@@ -681,14 +688,15 @@
                 klass.openapi_types is not None and
                 isinstance(data, (list, dict))):
             for attr, attr_type in six.iteritems(klass.openapi_types):
                 if klass.attribute_map[attr] in data:
                     value = data[klass.attribute_map[attr]]
                     kwargs[attr] = self.__deserialize(value, attr_type)
 
+        kwargs["local_vars_configuration"] = self.configuration
         instance = klass(**kwargs)
 
         if has_discriminator:
             klass_name = instance.get_real_child_model(data)
             if klass_name:
                 instance = self.__deserialize(data, klass_name)
         return instance
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.762\n"\
-               "SDK Package Version: 0.1.762".\
+               "Version of the API: 0.1.762.2\n"\
+               "SDK Package Version: 0.1.762.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/api_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/api_request_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/create_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/email_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/event_field_definition.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/event_field_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/id_selector_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,15 +35,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'identifier': 'dict(str, str)',
+        'identifier': 'dict[str, str]',
         'actions': 'list[ActionId]',
         'name': 'str',
         'description': 'str'
     }
 
     attribute_map = {
         'identifier': 'identifier',
@@ -59,15 +59,15 @@
         'description': 'optional'
     }
 
     def __init__(self, identifier=None, actions=None, name=None, description=None, local_vars_configuration=None):  # noqa: E501
         """IdSelectorDefinition - a model defined in OpenAPI"
         
         :param identifier:  (required)
-        :type identifier: dict(str, str)
+        :type identifier: dict[str, str]
         :param actions:  (required)
         :type actions: list[lusid_notification.ActionId]
         :param name: 
         :type name: str
         :param description: 
         :type description: str
 
@@ -89,25 +89,25 @@
 
     @property
     def identifier(self):
         """Gets the identifier of this IdSelectorDefinition.  # noqa: E501
 
 
         :return: The identifier of this IdSelectorDefinition.  # noqa: E501
-        :rtype: dict(str, str)
+        :rtype: dict[str, str]
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier):
         """Sets the identifier of this IdSelectorDefinition.
 
 
         :param identifier: The identifier of this IdSelectorDefinition.  # noqa: E501
-        :type identifier: dict(str, str)
+        :type identifier: dict[str, str]
         """
         if self.local_vars_configuration.client_side_validation and identifier is None:  # noqa: E501
             raise ValueError("Invalid value for `identifier`, must not be `None`")  # noqa: E501
 
         self._identifier = identifier
 
     @property
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/lusid_problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -36,15 +36,15 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'name': 'str',
-        'error_details': 'list[dict(str, str)]',
+        'error_details': 'list[dict[str, str]]',
         'code': 'int',
         'type': 'str',
         'title': 'str',
         'status': 'int',
         'detail': 'str',
         'instance': 'str'
     }
@@ -73,15 +73,15 @@
 
     def __init__(self, name=None, error_details=None, code=None, type=None, title=None, status=None, detail=None, instance=None, local_vars_configuration=None):  # noqa: E501
         """LusidProblemDetails - a model defined in OpenAPI"
         
         :param name:  (required)
         :type name: str
         :param error_details: 
-        :type error_details: list[dict(str, str)]
+        :type error_details: list[dict[str, str]]
         :param code:  (required)
         :type code: int
         :param type: 
         :type type: str
         :param title: 
         :type title: str
         :param status: 
@@ -143,25 +143,25 @@
 
     @property
     def error_details(self):
         """Gets the error_details of this LusidProblemDetails.  # noqa: E501
 
 
         :return: The error_details of this LusidProblemDetails.  # noqa: E501
-        :rtype: list[dict(str, str)]
+        :rtype: list[dict[str, str]]
         """
         return self._error_details
 
     @error_details.setter
     def error_details(self, error_details):
         """Sets the error_details of this LusidProblemDetails.
 
 
         :param error_details: The error_details of this LusidProblemDetails.  # noqa: E501
-        :type error_details: list[dict(str, str)]
+        :type error_details: list[dict[str, str]]
         """
 
         self._error_details = error_details
 
     @property
     def code(self):
         """Gets the code of this LusidProblemDetails.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -36,17 +36,17 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'name': 'str',
-        'error_details': 'list[dict(str, str)]',
+        'error_details': 'list[dict[str, str]]',
         'code': 'int',
-        'errors': 'dict(str, list[str])',
+        'errors': 'dict[str, list[str]]',
         'type': 'str',
         'title': 'str',
         'status': 'int',
         'detail': 'str',
         'instance': 'str'
     }
 
@@ -76,19 +76,19 @@
 
     def __init__(self, name=None, error_details=None, code=None, errors=None, type=None, title=None, status=None, detail=None, instance=None, local_vars_configuration=None):  # noqa: E501
         """LusidValidationProblemDetails - a model defined in OpenAPI"
         
         :param name:  (required)
         :type name: str
         :param error_details: 
-        :type error_details: list[dict(str, str)]
+        :type error_details: list[dict[str, str]]
         :param code:  (required)
         :type code: int
         :param errors: 
-        :type errors: dict(str, list[str])
+        :type errors: dict[str, list[str]]
         :param type: 
         :type type: str
         :param title: 
         :type title: str
         :param status: 
         :type status: int
         :param detail: 
@@ -150,25 +150,25 @@
 
     @property
     def error_details(self):
         """Gets the error_details of this LusidValidationProblemDetails.  # noqa: E501
 
 
         :return: The error_details of this LusidValidationProblemDetails.  # noqa: E501
-        :rtype: list[dict(str, str)]
+        :rtype: list[dict[str, str]]
         """
         return self._error_details
 
     @error_details.setter
     def error_details(self, error_details):
         """Sets the error_details of this LusidValidationProblemDetails.
 
 
         :param error_details: The error_details of this LusidValidationProblemDetails.  # noqa: E501
-        :type error_details: list[dict(str, str)]
+        :type error_details: list[dict[str, str]]
         """
 
         self._error_details = error_details
 
     @property
     def code(self):
         """Gets the code of this LusidValidationProblemDetails.  # noqa: E501
@@ -194,25 +194,25 @@
 
     @property
     def errors(self):
         """Gets the errors of this LusidValidationProblemDetails.  # noqa: E501
 
 
         :return: The errors of this LusidValidationProblemDetails.  # noqa: E501
-        :rtype: dict(str, list[str])
+        :rtype: dict[str, list[str]]
         """
         return self._errors
 
     @errors.setter
     def errors(self, errors):
         """Sets the errors of this LusidValidationProblemDetails.
 
 
         :param errors: The errors of this LusidValidationProblemDetails.  # noqa: E501
-        :type errors: dict(str, list[str])
+        :type errors: dict[str, list[str]]
         """
 
         self._errors = errors
 
     @property
     def type(self):
         """Gets the type of this LusidValidationProblemDetails.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/manual_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/manual_event_header.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,64 +35,87 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'event_type': 'str',
         'timestamp': 'datetime',
-        'event_id': 'str',
         'user_id': 'str',
         'request_id': 'str'
     }
 
     attribute_map = {
+        'event_type': 'eventType',
         'timestamp': 'timestamp',
-        'event_id': 'eventId',
         'user_id': 'userId',
         'request_id': 'requestId'
     }
 
     required_map = {
+        'event_type': 'optional',
         'timestamp': 'optional',
-        'event_id': 'optional',
         'user_id': 'optional',
         'request_id': 'optional'
     }
 
-    def __init__(self, timestamp=None, event_id=None, user_id=None, request_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, event_type=None, timestamp=None, user_id=None, request_id=None, local_vars_configuration=None):  # noqa: E501
         """ManualEventHeader - a model defined in OpenAPI"
         
+        :param event_type:  The event type of the manual event
+        :type event_type: str
         :param timestamp:  The timestamp of the manual event
         :type timestamp: datetime
-        :param event_id:  The event ID of the manual event
-        :type event_id: str
         :param user_id:  The user ID of the manual event
         :type user_id: str
         :param request_id:  The request ID of the manual event
         :type request_id: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._event_type = None
         self._timestamp = None
-        self._event_id = None
         self._user_id = None
         self._request_id = None
         self.discriminator = None
 
+        self.event_type = event_type
         if timestamp is not None:
             self.timestamp = timestamp
-        self.event_id = event_id
         self.user_id = user_id
         self.request_id = request_id
 
     @property
+    def event_type(self):
+        """Gets the event_type of this ManualEventHeader.  # noqa: E501
+
+        The event type of the manual event  # noqa: E501
+
+        :return: The event_type of this ManualEventHeader.  # noqa: E501
+        :rtype: str
+        """
+        return self._event_type
+
+    @event_type.setter
+    def event_type(self, event_type):
+        """Sets the event_type of this ManualEventHeader.
+
+        The event type of the manual event  # noqa: E501
+
+        :param event_type: The event_type of this ManualEventHeader.  # noqa: E501
+        :type event_type: str
+        """
+
+        self._event_type = event_type
+
+    @property
     def timestamp(self):
         """Gets the timestamp of this ManualEventHeader.  # noqa: E501
 
         The timestamp of the manual event  # noqa: E501
 
         :return: The timestamp of this ManualEventHeader.  # noqa: E501
         :rtype: datetime
@@ -108,37 +131,14 @@
         :param timestamp: The timestamp of this ManualEventHeader.  # noqa: E501
         :type timestamp: datetime
         """
 
         self._timestamp = timestamp
 
     @property
-    def event_id(self):
-        """Gets the event_id of this ManualEventHeader.  # noqa: E501
-
-        The event ID of the manual event  # noqa: E501
-
-        :return: The event_id of this ManualEventHeader.  # noqa: E501
-        :rtype: str
-        """
-        return self._event_id
-
-    @event_id.setter
-    def event_id(self, event_id):
-        """Sets the event_id of this ManualEventHeader.
-
-        The event ID of the manual event  # noqa: E501
-
-        :param event_id: The event_id of this ManualEventHeader.  # noqa: E501
-        :type event_id: str
-        """
-
-        self._event_id = event_id
-
-    @property
     def user_id(self):
         """Gets the user_id of this ManualEventHeader.  # noqa: E501
 
         The user ID of the manual event  # noqa: E501
 
         :return: The user_id of this ManualEventHeader.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/manual_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/notification.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -38,15 +38,15 @@
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'notification_id': 'str',
         'display_name': 'str',
         'description': 'str',
-        'notification_type': 'object',
+        'notification_type': 'NotificationTypeResponse',
         'created_at': 'datetime',
         'user_id_created': 'str',
         'modified_at': 'datetime',
         'user_id_modified': 'str',
         'href': 'str'
     }
 
@@ -60,35 +60,35 @@
         'modified_at': 'modifiedAt',
         'user_id_modified': 'userIdModified',
         'href': 'href'
     }
 
     required_map = {
         'notification_id': 'required',
-        'display_name': 'optional',
+        'display_name': 'required',
         'description': 'optional',
         'notification_type': 'required',
         'created_at': 'required',
         'user_id_created': 'required',
         'modified_at': 'required',
         'user_id_modified': 'required',
         'href': 'optional'
     }
 
     def __init__(self, notification_id=None, display_name=None, description=None, notification_type=None, created_at=None, user_id_created=None, modified_at=None, user_id_modified=None, href=None, local_vars_configuration=None):  # noqa: E501
         """Notification - a model defined in OpenAPI"
         
         :param notification_id:  The identifier of the notification (required)
         :type notification_id: str
-        :param display_name:  The name of the notification
+        :param display_name:  The name of the notification (required)
         :type display_name: str
         :param description:  The summary of the services provided by the notification
         :type description: str
-        :param notification_type:  The type and contents of the notification (required)
-        :type notification_type: object
+        :param notification_type:  (required)
+        :type notification_type: lusid_notification.NotificationTypeResponse
         :param created_at:  The time at which the subscription was made (required)
         :type created_at: datetime
         :param user_id_created:  The user who made the subscription (required)
         :type user_id_created: str
         :param modified_at:  The time at which the subscription was last modified (required)
         :type modified_at: datetime
         :param user_id_modified:  The user who last modified the subscription (required)
@@ -166,14 +166,16 @@
         """Sets the display_name of this Notification.
 
         The name of the notification  # noqa: E501
 
         :param display_name: The display_name of this Notification.  # noqa: E501
         :type display_name: str
         """
+        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 display_name is not None and len(display_name) > 64):
             raise ValueError("Invalid value for `display_name`, length must be less than or equal to `64`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 display_name is not None and len(display_name) < 0):
             raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `0`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
@@ -214,30 +216,30 @@
 
         self._description = description
 
     @property
     def notification_type(self):
         """Gets the notification_type of this Notification.  # noqa: E501
 
-        The type and contents of the notification  # noqa: E501
 
         :return: The notification_type of this Notification.  # noqa: E501
-        :rtype: object
+        :rtype: lusid_notification.NotificationTypeResponse
         """
         return self._notification_type
 
     @notification_type.setter
     def notification_type(self, notification_type):
         """Sets the notification_type of this Notification.
 
-        The type and contents of the notification  # noqa: E501
 
         :param notification_type: The notification_type of this Notification.  # noqa: E501
-        :type notification_type: object
+        :type notification_type: lusid_notification.NotificationTypeResponse
         """
+        if self.local_vars_configuration.client_side_validation and notification_type is None:  # noqa: E501
+            raise ValueError("Invalid value for `notification_type`, must not be `None`")  # noqa: E501
 
         self._notification_type = notification_type
 
     @property
     def created_at(self):
         """Gets the created_at of this Notification.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/notification_type.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -52,15 +52,15 @@
         'html_body': 'str',
         'email_address_to': 'list[str]',
         'email_address_cc': 'list[str]',
         'email_address_bcc': 'list[str]',
         'recipients': 'list[str]',
         'url': 'str',
         'authentication_type': 'str',
-        'authentication_configuration_item_paths': 'dict(str, str)',
+        'authentication_configuration_item_paths': 'dict[str, str]',
         'content_type': 'str'
     }
 
     attribute_map = {
         'type': 'type',
         'api_key_ref': 'apiKeyRef',
         'api_secret_ref': 'apiSecretRef',
@@ -138,15 +138,15 @@
         :param recipients:  The phone numbers to which the SMS will be sent to (E.164 format) (required)
         :type recipients: list[str]
         :param url:  The URL to send the request to (required)
         :type url: str
         :param authentication_type:  The type of authentication to use on the request (required)
         :type authentication_type: str
         :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
-        :type authentication_configuration_item_paths: dict(str, str)
+        :type authentication_configuration_item_paths: dict[str, str]
         :param content_type:  The type of the content e.g. Json (required)
         :type content_type: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
@@ -697,26 +697,26 @@
     @property
     def authentication_configuration_item_paths(self):
         """Gets the authentication_configuration_item_paths of this NotificationType.  # noqa: E501
 
         The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :return: The authentication_configuration_item_paths of this NotificationType.  # noqa: E501
-        :rtype: dict(str, str)
+        :rtype: dict[str, str]
         """
         return self._authentication_configuration_item_paths
 
     @authentication_configuration_item_paths.setter
     def authentication_configuration_item_paths(self, authentication_configuration_item_paths):
         """Sets the authentication_configuration_item_paths of this NotificationType.
 
         The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :param authentication_configuration_item_paths: The authentication_configuration_item_paths of this NotificationType.  # noqa: E501
-        :type authentication_configuration_item_paths: dict(str, str)
+        :type authentication_configuration_item_paths: dict[str, str]
         """
 
         self._authentication_configuration_item_paths = authentication_configuration_item_paths
 
     @property
     def content_type(self):
         """Gets the content_type of this NotificationType.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/sms_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/update_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/models/webhook_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -39,15 +39,15 @@
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'type': 'str',
         'http_method': 'str',
         'url': 'str',
         'authentication_type': 'str',
-        'authentication_configuration_item_paths': 'dict(str, str)',
+        'authentication_configuration_item_paths': 'dict[str, str]',
         'content_type': 'str',
         'content': 'object'
     }
 
     attribute_map = {
         'type': 'type',
         'http_method': 'httpMethod',
@@ -76,15 +76,15 @@
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
         :type http_method: str
         :param url:  The URL to send the request to (required)
         :type url: str
         :param authentication_type:  The type of authentication to use on the request (required)
         :type authentication_type: str
         :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
-        :type authentication_configuration_item_paths: dict(str, str)
+        :type authentication_configuration_item_paths: dict[str, str]
         :param content_type:  The type of the content e.g. Json (required)
         :type content_type: str
         :param content:  The content of the request
         :type content: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
@@ -232,26 +232,26 @@
     @property
     def authentication_configuration_item_paths(self):
         """Gets the authentication_configuration_item_paths of this WebhookNotificationType.  # noqa: E501
 
         The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :return: The authentication_configuration_item_paths of this WebhookNotificationType.  # noqa: E501
-        :rtype: dict(str, str)
+        :rtype: dict[str, str]
         """
         return self._authentication_configuration_item_paths
 
     @authentication_configuration_item_paths.setter
     def authentication_configuration_item_paths(self, authentication_configuration_item_paths):
         """Sets the authentication_configuration_item_paths of this WebhookNotificationType.
 
         The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :param authentication_configuration_item_paths: The authentication_configuration_item_paths of this WebhookNotificationType.  # noqa: E501
-        :type authentication_configuration_item_paths: dict(str, str)
+        :type authentication_configuration_item_paths: dict[str, str]
         """
 
         self._authentication_configuration_item_paths = authentication_configuration_item_paths
 
     @property
     def content_type(self):
         """Gets the content_type of this WebhookNotificationType.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.762
+    The version of the OpenAPI document: 0.1.762.2
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.762/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.762.2/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 lusid_notification/api/notifications_api.py
 lusid_notification/api/subscriptions_api.py
 lusid_notification/models/__init__.py
 lusid_notification/models/access_controlled_action.py
 lusid_notification/models/access_controlled_resource.py
 lusid_notification/models/action_id.py
 lusid_notification/models/amazon_sqs_notification_type.py
+lusid_notification/models/amazon_sqs_notification_type_response.py
 lusid_notification/models/api_request_notification_type.py
+lusid_notification/models/api_request_notification_type_response.py
 lusid_notification/models/create_notification_request.py
 lusid_notification/models/create_subscription.py
 lusid_notification/models/email_notification_type.py
+lusid_notification/models/email_notification_type_response.py
 lusid_notification/models/event_field_definition.py
 lusid_notification/models/event_type_schema.py
 lusid_notification/models/id_selector_definition.py
 lusid_notification/models/identifier_part_schema.py
 lusid_notification/models/link.py
 lusid_notification/models/lusid_problem_details.py
 lusid_notification/models/lusid_validation_problem_details.py
@@ -33,24 +36,27 @@
 lusid_notification/models/manual_event_body.py
 lusid_notification/models/manual_event_header.py
 lusid_notification/models/manual_event_request.py
 lusid_notification/models/matching_pattern.py
 lusid_notification/models/notification.py
 lusid_notification/models/notification_status.py
 lusid_notification/models/notification_type.py
+lusid_notification/models/notification_type_response.py
 lusid_notification/models/resource_id.py
 lusid_notification/models/resource_list_of_access_controlled_resource.py
 lusid_notification/models/resource_list_of_event_type_schema.py
 lusid_notification/models/resource_list_of_notification.py
 lusid_notification/models/resource_list_of_subscription.py
 lusid_notification/models/sms_notification_type.py
+lusid_notification/models/sms_notification_type_response.py
 lusid_notification/models/subscription.py
 lusid_notification/models/update_notification_request.py
 lusid_notification/models/update_subscription.py
 lusid_notification/models/webhook_notification_type.py
+lusid_notification/models/webhook_notification_type_response.py
 lusid_notification/utilities/__init__.py
 lusid_notification/utilities/config_keys.json
 lusid_notification/utilities/config_keys.py
 lusid_notification_sdk_preview.egg-info/PKG-INFO
 lusid_notification_sdk_preview.egg-info/SOURCES.txt
 lusid_notification_sdk_preview.egg-info/dependency_links.txt
 lusid_notification_sdk_preview.egg-info/requires.txt
```

### Comparing `lusid-notification-sdk-preview-0.1.762/setup.py` & `lusid-notification-sdk-preview-0.1.762.2/setup.py`

 * *Files identical despite different names*

