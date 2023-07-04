# Comparing `tmp/validio_sdk-0.6.0.tar.gz` & `tmp/validio_sdk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_sdk-0.6.0.tar", max compression
+gzip compressed data, was "validio_sdk-0.6.1.tar", max compression
```

## Comparing `validio_sdk-0.6.0.tar` & `validio_sdk-0.6.1.tar`

### file list

```diff
@@ -1,227 +1,227 @@
--rw-r--r--   0        0        0    11340 2023-07-03 15:11:56.619963 validio_sdk-0.6.0/LICENSE
--rw-r--r--   0        0        0      308 2023-07-03 15:11:56.619963 validio_sdk-0.6.0/README_PUBLIC.md
--rw-r--r--   0        0        0     5010 2023-07-03 15:12:08.951918 validio_sdk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      588 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/code/__init__.py
--rw-r--r--   0        0        0      551 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/code/apply.py
--rw-r--r--   0        0        0     4767 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/code/plan.py
--rw-r--r--   0        0        0     1565 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/code/scaffold.py
--rw-r--r--   0        0        0      305 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/code/settings.py
--rw-r--r--   0        0        0     5891 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/config.py
--rw-r--r--   0        0        0   261486 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/__init__.py
--rw-r--r--   0        0        0      573 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/apply_validator_recommendation.py
--rw-r--r--   0        0        0     7319 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/async_base_client.py
--rw-r--r--   0        0        0      526 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/aws_credential_secret_changed.py
--rw-r--r--   0        0        0      613 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
--rw-r--r--   0        0        0      614 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/backfill_source.py
--rw-r--r--   0        0        0     1899 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/base_model.py
--rw-r--r--   0        0        0   654498 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/client.py
--rw-r--r--   0        0        0      506 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_athena_credential.py
--rw-r--r--   0        0        0      458 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_athena_source.py
--rw-r--r--   0        0        0      445 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_credential.py
--rw-r--r--   0        0        0      528 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py
--rw-r--r--   0        0        0      468 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_kinesis_source.py
--rw-r--r--   0        0        0      526 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_redshift_credential.py
--rw-r--r--   0        0        0      480 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_redshift_source.py
--rw-r--r--   0        0        0      418 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_s3_source.py
--rw-r--r--   0        0        0      843 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      823 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      455 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_demo_credential.py
--rw-r--r--   0        0        0      407 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_demo_source.py
--rw-r--r--   0        0        0      407 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_file_window.py
--rw-r--r--   0        0        0      468 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_fixed_batch_window.py
--rw-r--r--   0        0        0      702 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      682 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      539 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py
--rw-r--r--   0        0        0      481 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_big_query_source.py
--rw-r--r--   0        0        0      445 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_credential.py
--rw-r--r--   0        0        0      500 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      459 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      468 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_storage_source.py
--rw-r--r--   0        0        0      557 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_kafka_sasl_plain_credential.py
--rw-r--r--   0        0        0      417 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_kafka_source.py
--rw-r--r--   0        0        0      498 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_kafka_ssl_credential.py
--rw-r--r--   0        0        0      487 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_notification_rule.py
--rw-r--r--   0        0        0      753 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      803 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      783 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      823 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      682 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      662 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      702 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      516 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_postgre_sql_credential.py
--rw-r--r--   0        0        0      468 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_postgre_sql_source.py
--rw-r--r--   0        0        0      733 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      713 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      753 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      753 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      528 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_saml_identity_provider.py
--rw-r--r--   0        0        0      438 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_segmentation.py
--rw-r--r--   0        0        0      477 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_sessionized_window.py
--rw-r--r--   0        0        0      429 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_slack_channel.py
--rw-r--r--   0        0        0      505 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_snowflake_credential.py
--rw-r--r--   0        0        0      517 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_snowflake_destination.py
--rw-r--r--   0        0        0      457 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_snowflake_source.py
--rw-r--r--   0        0        0      447 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_tumbling_window.py
--rw-r--r--   0        0        0      328 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_user.py
--rw-r--r--   0        0        0      672 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      652 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      449 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_webhook_channel.py
--rw-r--r--   0        0        0      364 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_channel.py
--rw-r--r--   0        0        0      614 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_credential.py
--rw-r--r--   0        0        0      622 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_credentials.py
--rw-r--r--   0        0        0      630 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_destination.py
--rw-r--r--   0        0        0      638 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_destinations.py
--rw-r--r--   0        0        0      376 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_identity.py
--rw-r--r--   0        0        0      487 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_identity_provider.py
--rw-r--r--   0        0        0      487 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_notification_rule.py
--rw-r--r--   0        0        0      646 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_segmentation.py
--rw-r--r--   0        0        0      536 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_source.py
--rw-r--r--   0        0        0      544 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_sources.py
--rw-r--r--   0        0        0      328 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_user.py
--rw-r--r--   0        0        0      606 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_validators.py
--rw-r--r--   0        0        0      536 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_window.py
--rw-r--r--   0        0        0      544 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_windows.py
--rw-r--r--   0        0        0      589 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py
--rw-r--r--   0        0        0     3127 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/enums.py
--rw-r--r--   0        0        0     2314 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/exceptions.py
--rw-r--r--   0        0        0   188660 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/fragments.py
--rw-r--r--   0        0        0      526 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py
--rw-r--r--   0        0        0     2896 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_channel_by_resource_name.py
--rw-r--r--   0        0        0     2427 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_channels.py
--rw-r--r--   0        0        0     8124 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_credential_by_resource_name.py
--rw-r--r--   0        0        0     5997 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_destination_by_resource_name.py
--rw-r--r--   0        0        0     2218 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
--rw-r--r--   0        0        0     2033 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_identity_providers.py
--rw-r--r--   0        0        0     5368 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_incidents.py
--rw-r--r--   0        0        0      627 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
--rw-r--r--   0        0        0      480 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_notification_rules.py
--rw-r--r--   0        0        0     2245 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_recommendation.py
--rw-r--r--   0        0        0      460 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_segment_incidents.py
--rw-r--r--   0        0        0      357 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_segmentation.py
--rw-r--r--   0        0        0      572 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
--rw-r--r--   0        0        0    23998 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_source.py
--rw-r--r--   0        0        0    29447 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_by_resource_name.py
--rw-r--r--   0        0        0     1727 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_incidents.py
--rw-r--r--   0        0        0    25201 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_recommended_validators.py
--rw-r--r--   0        0        0      476 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_user_by_resource_name.py
--rw-r--r--   0        0        0      300 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_users.py
--rw-r--r--   0        0        0    40168 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator.py
--rw-r--r--   0        0        0    48254 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_by_resource_name.py
--rw-r--r--   0        0        0      480 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_incidents.py
--rw-r--r--   0        0        0      551 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_segment_incidents.py
--rw-r--r--   0        0        0     3986 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_segment_metrics.py
--rw-r--r--   0        0        0     5711 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_window_by_resource_name.py
--rw-r--r--   0        0        0      286 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_aws_athena_schema.py
--rw-r--r--   0        0        0      290 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
--rw-r--r--   0        0        0      308 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_aws_redshift_schema.py
--rw-r--r--   0        0        0      270 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_aws_s3_schema.py
--rw-r--r--   0        0        0      265 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_demo_schema.py
--rw-r--r--   0        0        0      309 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
--rw-r--r--   0        0        0      318 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
--rw-r--r--   0        0        0      287 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
--rw-r--r--   0        0        0      290 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_gcp_storage_schema.py
--rw-r--r--   0        0        0      269 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_kafka_schema.py
--rw-r--r--   0        0        0      290 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_postgre_sql_schema.py
--rw-r--r--   0        0        0      285 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_snowflake_schema.py
--rw-r--r--   0        0        0    39472 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/input_types.py
--rw-r--r--   0        0        0      644 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/kafka_sasl_plain_credential_secret_changed.py
--rw-r--r--   0        0        0      583 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py
--rw-r--r--   0        0        0     7067 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_credentials.py
--rw-r--r--   0        0        0     5202 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_destinations.py
--rw-r--r--   0        0        0      457 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_segmentations.py
--rw-r--r--   0        0        0    25314 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_sources.py
--rw-r--r--   0        0        0    42237 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_validators.py
--rw-r--r--   0        0        0     4976 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_windows.py
--rw-r--r--   0        0        0      603 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
--rw-r--r--   0        0        0      594 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/scalars.py
--rw-r--r--   0        0        0      288 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/segments.py
--rw-r--r--   0        0        0      499 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/segments_by_resource_name.py
--rw-r--r--   0        0        0      592 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
--rw-r--r--   0        0        0      566 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/start_source.py
--rw-r--r--   0        0        0      550 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/stop_source.py
--rw-r--r--   0        0        0      502 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_athena_credential.py
--rw-r--r--   0        0        0      454 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_athena_source.py
--rw-r--r--   0        0        0      441 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_credential.py
--rw-r--r--   0        0        0      524 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py
--rw-r--r--   0        0        0      464 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_kinesis_source.py
--rw-r--r--   0        0        0      522 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_redshift_credential.py
--rw-r--r--   0        0        0      476 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_redshift_source.py
--rw-r--r--   0        0        0      414 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_s3_source.py
--rw-r--r--   0        0        0      636 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py
--rw-r--r--   0        0        0      469 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_channel_namespace.py
--rw-r--r--   0        0        0      499 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_credential_namespace.py
--rw-r--r--   0        0        0      509 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_destination_namespace.py
--rw-r--r--   0        0        0      464 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_fixed_batch_window.py
--rw-r--r--   0        0        0      491 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_freshness_validator.py
--rw-r--r--   0        0        0      535 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py
--rw-r--r--   0        0        0      477 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_big_query_source.py
--rw-r--r--   0        0        0      441 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_credential.py
--rw-r--r--   0        0        0      496 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      455 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      464 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_storage_source.py
--rw-r--r--   0        0        0      560 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_identity_provider_namespace.py
--rw-r--r--   0        0        0      553 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_kafka_sasl_plain_credential.py
--rw-r--r--   0        0        0      413 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_kafka_source.py
--rw-r--r--   0        0        0      494 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_kafka_ssl_credential.py
--rw-r--r--   0        0        0      534 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_local_identity_provider.py
--rw-r--r--   0        0        0      483 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_notification_rule.py
--rw-r--r--   0        0        0      560 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_notification_rule_namespace.py
--rw-r--r--   0        0        0      540 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
--rw-r--r--   0        0        0      596 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py
--rw-r--r--   0        0        0      469 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_numeric_validator.py
--rw-r--r--   0        0        0      512 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_postgre_sql_credential.py
--rw-r--r--   0        0        0      464 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_postgre_sql_source.py
--rw-r--r--   0        0        0      520 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_relative_time_validator.py
--rw-r--r--   0        0        0      540 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_relative_volume_validator.py
--rw-r--r--   0        0        0      524 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_saml_identity_provider.py
--rw-r--r--   0        0        0      519 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_segmentation_namespace.py
--rw-r--r--   0        0        0      473 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_sessionized_window.py
--rw-r--r--   0        0        0      425 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_slack_channel.py
--rw-r--r--   0        0        0      501 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_snowflake_credential.py
--rw-r--r--   0        0        0      513 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_snowflake_destination.py
--rw-r--r--   0        0        0      453 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_snowflake_source.py
--rw-r--r--   0        0        0      459 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_source_namespace.py
--rw-r--r--   0        0        0      443 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_tumbling_window.py
--rw-r--r--   0        0        0      324 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_user.py
--rw-r--r--   0        0        0      439 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_user_namespace.py
--rw-r--r--   0        0        0      491 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_namespace.py
--rw-r--r--   0        0        0    57176 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0    56052 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0    58306 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      459 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_volume_validator.py
--rw-r--r--   0        0        0      445 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_webhook_channel.py
--rw-r--r--   0        0        0      459 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_window_namespace.py
--rw-r--r--   0        0        0      265 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/metadata.py
--rw-r--r--   0        0        0        0 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/py.typed
--rw-r--r--   0        0        0      135 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/__init__.py
--rw-r--r--   0        0        0    21078 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_diff.py
--rw-r--r--   0        0        0     1505 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_diff_util.py
--rw-r--r--   0        0        0     1657 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_diffable.py
--rw-r--r--   0        0        0     1579 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_errors.py
--rw-r--r--   0        0        0     4002 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_field_selector.py
--rw-r--r--   0        0        0    17790 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_resource.py
--rw-r--r--   0        0        0     1355 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_resource_graph.py
--rw-r--r--   0        0        0     5366 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_serde.py
--rw-r--r--   0        0        0    21679 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_server_resources.py
--rw-r--r--   0        0        0      847 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_util.py
--rw-r--r--   0        0        0     5027 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/channels.py
--rw-r--r--   0        0        0     7692 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/credentials.py
--rw-r--r--   0        0        0     5601 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/destinations.py
--rw-r--r--   0        0        0     6262 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/filters.py
--rw-r--r--   0        0        0     4846 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/notification_rules.py
--rw-r--r--   0        0        0     2040 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/segmentations.py
--rw-r--r--   0        0        0    25888 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/sources.py
--rw-r--r--   0        0        0        0 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/tests/__init__.py
--rw-r--r--   0        0        0    15408 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/tests/test__diff.py
--rw-r--r--   0        0        0     1905 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/tests/test__field_selector.py
--rw-r--r--   0        0        0    16357 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/tests/test__resource.py
--rw-r--r--   0        0        0     5638 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/thresholds.py
--rw-r--r--   0        0        0    32563 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/validators.py
--rw-r--r--   0        0        0     5995 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/windows.py
--rw-r--r--   0        0        0     1377 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/scalars.py
--rw-r--r--   0        0        0     1813 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/util.py
--rw-r--r--   0        0        0     2382 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/validio_client.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 validio_sdk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-07-04 10:01:27.318835 validio_sdk-0.6.1/LICENSE
+-rw-r--r--   0        0        0      308 2023-07-04 10:01:27.318835 validio_sdk-0.6.1/README_PUBLIC.md
+-rw-r--r--   0        0        0     5010 2023-07-04 10:01:47.646540 validio_sdk-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      588 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/code/__init__.py
+-rw-r--r--   0        0        0      551 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/code/apply.py
+-rw-r--r--   0        0        0     4767 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/code/plan.py
+-rw-r--r--   0        0        0     1565 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/code/scaffold.py
+-rw-r--r--   0        0        0      305 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/code/settings.py
+-rw-r--r--   0        0        0     5891 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/config.py
+-rw-r--r--   0        0        0   261486 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/apply_validator_recommendation.py
+-rw-r--r--   0        0        0     7319 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      526 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/aws_credential_secret_changed.py
+-rw-r--r--   0        0        0      613 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
+-rw-r--r--   0        0        0      614 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/backfill_source.py
+-rw-r--r--   0        0        0     1899 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/base_model.py
+-rw-r--r--   0        0        0   654498 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/client.py
+-rw-r--r--   0        0        0      506 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_aws_athena_credential.py
+-rw-r--r--   0        0        0      458 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_aws_athena_source.py
+-rw-r--r--   0        0        0      445 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_aws_credential.py
+-rw-r--r--   0        0        0      528 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      468 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_aws_kinesis_source.py
+-rw-r--r--   0        0        0      526 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_aws_redshift_credential.py
+-rw-r--r--   0        0        0      480 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_aws_redshift_source.py
+-rw-r--r--   0        0        0      418 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_aws_s3_source.py
+-rw-r--r--   0        0        0      843 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      823 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      455 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_demo_credential.py
+-rw-r--r--   0        0        0      407 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_demo_source.py
+-rw-r--r--   0        0        0      407 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_file_window.py
+-rw-r--r--   0        0        0      468 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_fixed_batch_window.py
+-rw-r--r--   0        0        0      702 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      682 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      539 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      481 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_gcp_big_query_source.py
+-rw-r--r--   0        0        0      445 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_gcp_credential.py
+-rw-r--r--   0        0        0      500 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      459 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      468 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_gcp_storage_source.py
+-rw-r--r--   0        0        0      557 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_kafka_sasl_plain_credential.py
+-rw-r--r--   0        0        0      417 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_kafka_source.py
+-rw-r--r--   0        0        0      498 2023-07-04 10:01:27.322835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_kafka_ssl_credential.py
+-rw-r--r--   0        0        0      487 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_notification_rule.py
+-rw-r--r--   0        0        0      753 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      803 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      783 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      823 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      682 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      662 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      702 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      516 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_postgre_sql_credential.py
+-rw-r--r--   0        0        0      468 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_postgre_sql_source.py
+-rw-r--r--   0        0        0      733 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      713 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      753 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      753 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      528 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_saml_identity_provider.py
+-rw-r--r--   0        0        0      438 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_segmentation.py
+-rw-r--r--   0        0        0      477 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_sessionized_window.py
+-rw-r--r--   0        0        0      429 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_slack_channel.py
+-rw-r--r--   0        0        0      505 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_snowflake_credential.py
+-rw-r--r--   0        0        0      517 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_snowflake_destination.py
+-rw-r--r--   0        0        0      457 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_snowflake_source.py
+-rw-r--r--   0        0        0      447 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_tumbling_window.py
+-rw-r--r--   0        0        0      328 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_user.py
+-rw-r--r--   0        0        0      672 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      652 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      449 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/create_webhook_channel.py
+-rw-r--r--   0        0        0      364 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_channel.py
+-rw-r--r--   0        0        0      614 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_credential.py
+-rw-r--r--   0        0        0      622 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_credentials.py
+-rw-r--r--   0        0        0      630 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_destination.py
+-rw-r--r--   0        0        0      638 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_destinations.py
+-rw-r--r--   0        0        0      376 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_identity.py
+-rw-r--r--   0        0        0      487 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_identity_provider.py
+-rw-r--r--   0        0        0      487 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_notification_rule.py
+-rw-r--r--   0        0        0      646 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_segmentation.py
+-rw-r--r--   0        0        0      536 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_source.py
+-rw-r--r--   0        0        0      544 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_sources.py
+-rw-r--r--   0        0        0      328 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_user.py
+-rw-r--r--   0        0        0      606 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_validators.py
+-rw-r--r--   0        0        0      536 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_window.py
+-rw-r--r--   0        0        0      544 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/delete_windows.py
+-rw-r--r--   0        0        0      589 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/dismiss_validator_recommendation.py
+-rw-r--r--   0        0        0     3127 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/enums.py
+-rw-r--r--   0        0        0     2314 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/exceptions.py
+-rw-r--r--   0        0        0   188660 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/fragments.py
+-rw-r--r--   0        0        0      526 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/gcp_credential_secret_changed.py
+-rw-r--r--   0        0        0     2896 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_channel_by_resource_name.py
+-rw-r--r--   0        0        0     2427 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_channels.py
+-rw-r--r--   0        0        0     8124 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_credential_by_resource_name.py
+-rw-r--r--   0        0        0     5997 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_destination_by_resource_name.py
+-rw-r--r--   0        0        0     2218 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
+-rw-r--r--   0        0        0     2033 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_identity_providers.py
+-rw-r--r--   0        0        0     5368 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_incidents.py
+-rw-r--r--   0        0        0      627 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_notification_rules.py
+-rw-r--r--   0        0        0     2245 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_recommendation.py
+-rw-r--r--   0        0        0      460 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_segment_incidents.py
+-rw-r--r--   0        0        0      357 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_segmentation.py
+-rw-r--r--   0        0        0      572 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
+-rw-r--r--   0        0        0    23998 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_source.py
+-rw-r--r--   0        0        0    29447 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_source_by_resource_name.py
+-rw-r--r--   0        0        0     1727 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_source_incidents.py
+-rw-r--r--   0        0        0    25201 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_source_recommended_validators.py
+-rw-r--r--   0        0        0      476 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_user_by_resource_name.py
+-rw-r--r--   0        0        0      300 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_users.py
+-rw-r--r--   0        0        0    40168 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_validator.py
+-rw-r--r--   0        0        0    48254 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_validator_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_validator_incidents.py
+-rw-r--r--   0        0        0      551 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_validator_segment_incidents.py
+-rw-r--r--   0        0        0     3986 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_validator_segment_metrics.py
+-rw-r--r--   0        0        0     5711 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/get_window_by_resource_name.py
+-rw-r--r--   0        0        0      286 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_aws_athena_schema.py
+-rw-r--r--   0        0        0      290 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
+-rw-r--r--   0        0        0      308 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_aws_redshift_schema.py
+-rw-r--r--   0        0        0      270 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_aws_s3_schema.py
+-rw-r--r--   0        0        0      265 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_demo_schema.py
+-rw-r--r--   0        0        0      309 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
+-rw-r--r--   0        0        0      318 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
+-rw-r--r--   0        0        0      287 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
+-rw-r--r--   0        0        0      290 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_gcp_storage_schema.py
+-rw-r--r--   0        0        0      269 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_kafka_schema.py
+-rw-r--r--   0        0        0      290 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_postgre_sql_schema.py
+-rw-r--r--   0        0        0      285 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/infer_snowflake_schema.py
+-rw-r--r--   0        0        0    39472 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/input_types.py
+-rw-r--r--   0        0        0      644 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/kafka_sasl_plain_credential_secret_changed.py
+-rw-r--r--   0        0        0      583 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py
+-rw-r--r--   0        0        0     7067 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/list_credentials.py
+-rw-r--r--   0        0        0     5202 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/list_destinations.py
+-rw-r--r--   0        0        0      457 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/list_segmentations.py
+-rw-r--r--   0        0        0    25314 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/list_sources.py
+-rw-r--r--   0        0        0    42237 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/list_validators.py
+-rw-r--r--   0        0        0     4976 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/list_windows.py
+-rw-r--r--   0        0        0      603 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
+-rw-r--r--   0        0        0      594 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/scalars.py
+-rw-r--r--   0        0        0      288 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/segments.py
+-rw-r--r--   0        0        0      499 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/segments_by_resource_name.py
+-rw-r--r--   0        0        0      592 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
+-rw-r--r--   0        0        0      566 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/start_source.py
+-rw-r--r--   0        0        0      550 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/stop_source.py
+-rw-r--r--   0        0        0      502 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_aws_athena_credential.py
+-rw-r--r--   0        0        0      454 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_aws_athena_source.py
+-rw-r--r--   0        0        0      441 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_aws_credential.py
+-rw-r--r--   0        0        0      524 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      464 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_aws_kinesis_source.py
+-rw-r--r--   0        0        0      522 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_aws_redshift_credential.py
+-rw-r--r--   0        0        0      476 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_aws_redshift_source.py
+-rw-r--r--   0        0        0      414 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_aws_s3_source.py
+-rw-r--r--   0        0        0      636 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_categorical_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_channel_namespace.py
+-rw-r--r--   0        0        0      499 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_credential_namespace.py
+-rw-r--r--   0        0        0      509 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_destination_namespace.py
+-rw-r--r--   0        0        0      464 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_fixed_batch_window.py
+-rw-r--r--   0        0        0      491 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_freshness_validator.py
+-rw-r--r--   0        0        0      535 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      477 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_gcp_big_query_source.py
+-rw-r--r--   0        0        0      441 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_gcp_credential.py
+-rw-r--r--   0        0        0      496 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      455 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      464 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_gcp_storage_source.py
+-rw-r--r--   0        0        0      560 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_identity_provider_namespace.py
+-rw-r--r--   0        0        0      553 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_kafka_sasl_plain_credential.py
+-rw-r--r--   0        0        0      413 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_kafka_source.py
+-rw-r--r--   0        0        0      494 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_kafka_ssl_credential.py
+-rw-r--r--   0        0        0      534 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_local_identity_provider.py
+-rw-r--r--   0        0        0      483 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_notification_rule.py
+-rw-r--r--   0        0        0      560 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_notification_rule_namespace.py
+-rw-r--r--   0        0        0      540 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
+-rw-r--r--   0        0        0      596 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_numeric_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_numeric_validator.py
+-rw-r--r--   0        0        0      512 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_postgre_sql_credential.py
+-rw-r--r--   0        0        0      464 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_postgre_sql_source.py
+-rw-r--r--   0        0        0      520 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_relative_time_validator.py
+-rw-r--r--   0        0        0      540 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_relative_volume_validator.py
+-rw-r--r--   0        0        0      524 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_saml_identity_provider.py
+-rw-r--r--   0        0        0      519 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_segmentation_namespace.py
+-rw-r--r--   0        0        0      473 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_sessionized_window.py
+-rw-r--r--   0        0        0      425 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_slack_channel.py
+-rw-r--r--   0        0        0      501 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_snowflake_credential.py
+-rw-r--r--   0        0        0      513 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_snowflake_destination.py
+-rw-r--r--   0        0        0      453 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_snowflake_source.py
+-rw-r--r--   0        0        0      459 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_source_namespace.py
+-rw-r--r--   0        0        0      443 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_tumbling_window.py
+-rw-r--r--   0        0        0      324 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_user.py
+-rw-r--r--   0        0        0      439 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_user_namespace.py
+-rw-r--r--   0        0        0      491 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_validator_namespace.py
+-rw-r--r--   0        0        0    57176 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0    56052 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0    58306 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      459 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_volume_validator.py
+-rw-r--r--   0        0        0      445 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_webhook_channel.py
+-rw-r--r--   0        0        0      459 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/graphql_client/update_window_namespace.py
+-rw-r--r--   0        0        0      265 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/metadata.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/py.typed
+-rw-r--r--   0        0        0      135 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/__init__.py
+-rw-r--r--   0        0        0    21078 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/_diff.py
+-rw-r--r--   0        0        0     1505 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/_diff_util.py
+-rw-r--r--   0        0        0     1657 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/_diffable.py
+-rw-r--r--   0        0        0     1579 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/_errors.py
+-rw-r--r--   0        0        0     4002 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/_field_selector.py
+-rw-r--r--   0        0        0    17790 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/_resource.py
+-rw-r--r--   0        0        0     1355 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/_resource_graph.py
+-rw-r--r--   0        0        0     5366 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/_serde.py
+-rw-r--r--   0        0        0    21679 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/_server_resources.py
+-rw-r--r--   0        0        0      847 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/_util.py
+-rw-r--r--   0        0        0     5027 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/channels.py
+-rw-r--r--   0        0        0     7692 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/credentials.py
+-rw-r--r--   0        0        0     5601 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/destinations.py
+-rw-r--r--   0        0        0     6262 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/filters.py
+-rw-r--r--   0        0        0     4846 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/notification_rules.py
+-rw-r--r--   0        0        0     2040 2023-07-04 10:01:27.326835 validio_sdk-0.6.1/validio_sdk/resource/segmentations.py
+-rw-r--r--   0        0        0    25888 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/resource/sources.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/resource/tests/__init__.py
+-rw-r--r--   0        0        0    15408 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/resource/tests/test__diff.py
+-rw-r--r--   0        0        0     1905 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/resource/tests/test__field_selector.py
+-rw-r--r--   0        0        0    16357 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/resource/tests/test__resource.py
+-rw-r--r--   0        0        0     5638 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/resource/thresholds.py
+-rw-r--r--   0        0        0    32563 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/resource/validators.py
+-rw-r--r--   0        0        0     5995 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/resource/windows.py
+-rw-r--r--   0        0        0     1377 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/scalars.py
+-rw-r--r--   0        0        0     1813 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/util.py
+-rw-r--r--   0        0        0     2382 2023-07-04 10:01:27.330835 validio_sdk-0.6.1/validio_sdk/validio_client.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 validio_sdk-0.6.1/PKG-INFO
```

### Comparing `validio_sdk-0.6.0/LICENSE` & `validio_sdk-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/pyproject.toml` & `validio_sdk-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "validio-sdk"
 # This version does not represent the released version or any tag. For each
 # release we automatically bump this before building and publishing so this
 # should be kept at 0.0.1dev1
-version = "0.6.0"
+version = "0.6.1"
 description = "SDK to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://dev.validio.io/sdk-docs"
 packages = [{ include = "validio_sdk" }]
 exclude = ["./validio_sdk/bin/pull_graphql.py", "./schema/**", "./plugins/**", "./examples/**"]
```

### Comparing `validio_sdk-0.6.0/validio_sdk/__init__.py` & `validio_sdk-0.6.1/validio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/code/apply.py` & `validio_sdk-0.6.1/validio_sdk/code/apply.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/code/plan.py` & `validio_sdk-0.6.1/validio_sdk/code/plan.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/code/scaffold.py` & `validio_sdk-0.6.1/validio_sdk/code/scaffold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/config.py` & `validio_sdk-0.6.1/validio_sdk/config.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/__init__.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/apply_validator_recommendation.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/apply_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/async_base_client.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/aws_credential_secret_changed.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/aws_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/backfill_source.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/backfill_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/base_model.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/client.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_redshift_credential.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_kafka_sasl_plain_credential.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_kafka_sasl_plain_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_postgre_sql_credential.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_saml_identity_provider.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_snowflake_destination.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_credential.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/delete_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_credentials.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/delete_credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_destination.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/delete_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_destinations.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/delete_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_segmentation.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/delete_segmentation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_source.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/delete_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_sources.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/delete_sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_validators.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/delete_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_window.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/delete_window.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_windows.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/delete_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/dismiss_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/enums.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/enums.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/exceptions.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/fragments.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/fragments.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/gcp_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_channel_by_resource_name.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_channel_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_channels.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_credential_by_resource_name.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_credential_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_destination_by_resource_name.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_destination_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_identity_providers.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_identity_providers.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_incidents.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_recommendation.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_segmentation_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_source.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_by_resource_name.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_source_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_incidents.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_source_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_recommended_validators.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_source_recommended_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_by_resource_name.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_validator_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_segment_incidents.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_validator_segment_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_segment_metrics.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_validator_segment_metrics.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/get_window_by_resource_name.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/get_window_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/input_types.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/input_types.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/kafka_sasl_plain_credential_secret_changed.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/kafka_sasl_plain_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/list_credentials.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/list_credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/list_destinations.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/list_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/list_sources.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/list_sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/list_validators.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/list_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/list_windows.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/list_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/scalars.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/scalars.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/snowflake_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/start_source.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/start_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/stop_source.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/stop_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_redshift_credential.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_categorical_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_identity_provider_namespace.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_identity_provider_namespace.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_kafka_sasl_plain_credential.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_kafka_sasl_plain_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_local_identity_provider.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_local_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_notification_rule_namespace.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_notification_rule_namespace.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_numeric_anomaly_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_numeric_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_postgre_sql_credential.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_relative_time_validator.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_relative_time_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_relative_volume_validator.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_relative_volume_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_saml_identity_provider.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_segmentation_namespace.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_segmentation_namespace.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_snowflake_destination.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.1/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/_diff.py` & `validio_sdk-0.6.1/validio_sdk/resource/_diff.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/_diff_util.py` & `validio_sdk-0.6.1/validio_sdk/resource/_diff_util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/_diffable.py` & `validio_sdk-0.6.1/validio_sdk/resource/_diffable.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/_errors.py` & `validio_sdk-0.6.1/validio_sdk/resource/_errors.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/_field_selector.py` & `validio_sdk-0.6.1/validio_sdk/resource/_field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/_resource.py` & `validio_sdk-0.6.1/validio_sdk/resource/_resource.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/_resource_graph.py` & `validio_sdk-0.6.1/validio_sdk/resource/_resource_graph.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/_serde.py` & `validio_sdk-0.6.1/validio_sdk/resource/_serde.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/_server_resources.py` & `validio_sdk-0.6.1/validio_sdk/resource/_server_resources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/_util.py` & `validio_sdk-0.6.1/validio_sdk/resource/_util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/channels.py` & `validio_sdk-0.6.1/validio_sdk/resource/channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/credentials.py` & `validio_sdk-0.6.1/validio_sdk/resource/credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/destinations.py` & `validio_sdk-0.6.1/validio_sdk/resource/destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/filters.py` & `validio_sdk-0.6.1/validio_sdk/resource/filters.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/notification_rules.py` & `validio_sdk-0.6.1/validio_sdk/resource/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/segmentations.py` & `validio_sdk-0.6.1/validio_sdk/resource/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/sources.py` & `validio_sdk-0.6.1/validio_sdk/resource/sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/tests/test__diff.py` & `validio_sdk-0.6.1/validio_sdk/resource/tests/test__diff.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/tests/test__field_selector.py` & `validio_sdk-0.6.1/validio_sdk/resource/tests/test__field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/tests/test__resource.py` & `validio_sdk-0.6.1/validio_sdk/resource/tests/test__resource.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/thresholds.py` & `validio_sdk-0.6.1/validio_sdk/resource/thresholds.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/validators.py` & `validio_sdk-0.6.1/validio_sdk/resource/validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/resource/windows.py` & `validio_sdk-0.6.1/validio_sdk/resource/windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/scalars.py` & `validio_sdk-0.6.1/validio_sdk/scalars.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/util.py` & `validio_sdk-0.6.1/validio_sdk/util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/validio_sdk/validio_client.py` & `validio_sdk-0.6.1/validio_sdk/validio_client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.0/PKG-INFO` & `validio_sdk-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-sdk
-Version: 0.6.0
+Version: 0.6.1
 Summary: SDK to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

