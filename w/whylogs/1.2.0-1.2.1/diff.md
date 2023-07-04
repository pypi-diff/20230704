# Comparing `tmp/whylogs-1.2.0.tar.gz` & `tmp/whylogs-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.2.0.tar", max compression
+gzip compressed data, was "whylogs-1.2.1.tar", max compression
```

## Comparing `whylogs-1.2.0.tar` & `whylogs-1.2.1.tar`

### file list

```diff
@@ -1,215 +1,215 @@
--rw-r--r--   0        0        0     3166 2023-06-27 23:30:31.408861 whylogs-1.2.0/DESCRIPTION.md
--rw-r--r--   0        0        0     5846 2023-06-27 23:31:06.009815 whylogs-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1801 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/annotations.py
--rw-r--r--   0        0        0      120 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     4840 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     1997 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/fugue/registry.py
--rw-r--r--   0        0        0     8157 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/experimental/multi_dataset_logger/__init__.py
--rw-r--r--   0        0        0      468 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/experimental/multi_dataset_logger/future_util.py
--rw-r--r--   0        0        0     2119 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py
--rw-r--r--   0        0        0    15693 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py
--rw-r--r--   0        0        0     3964 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py
--rw-r--r--   0        0        0     4770 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    19765 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     9550 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     2113 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     6333 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      687 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      406 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     4217 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0     7663 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/pyspark/experimental/segmented_profiler.py
--rw-r--r--   0        0        0      465 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     2073 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      237 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4566 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0     1208 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      672 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/store/query.py
--rw-r--r--   0        0        0     5350 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/store/sqlite_store.py
--rw-r--r--   0        0        0     6128 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0       79 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/whylabs/__init__.py
--rw-r--r--   0        0        0     7497 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/whylabs/session/config.py
--rw-r--r--   0        0        0      329 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/whylabs/session/notebook_check.py
--rw-r--r--   0        0        0     3813 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/whylabs/session/notebook_logger.py
--rw-r--r--   0        0        0    10646 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/whylabs/session/session_manager.py
--rw-r--r--   0        0        0      666 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/whylabs/session/session_types.py
--rw-r--r--   0        0        0      947 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     2726 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     1169 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     2084 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0     3408 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    39185 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0     1217 2023-06-27 23:30:31.460863 whylogs-1.2.0/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0     1090 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/__init__.py
--rw-r--r--   0        0        0     3391 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/common.py
--rw-r--r--   0        0        0     1549 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/configs.py
--rw-r--r--   0        0        0      455 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0     1798 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2049 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/constraints/factories/condition_counts.py
--rw-r--r--   0        0        0     2601 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     7063 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0      737 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/constraints/factories/multi_metrics.py
--rw-r--r--   0        0        0     3199 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/constraints/factories/types_metrics.py
--rw-r--r--   0        0        0    30671 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    11486 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4120 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/errors.py
--rw-r--r--   0        0        0     2560 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0     1740 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metric_getters.py
--rw-r--r--   0        0        0      984 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4085 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     5031 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6481 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0     7615 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4840 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    21749 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     8016 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     4517 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5504 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0     8976 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7445 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2837 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     5499 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/predicate_parser.py
--rw-r--r--   0        0        0    14489 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0    12534 2023-06-27 23:31:09.953926 whylogs-1.2.0/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    20212 2023-06-27 23:31:08.669890 whylogs-1.2.0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    21343 2023-06-27 23:31:08.669890 whylogs-1.2.0/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29724 2023-06-27 23:31:08.669890 whylogs-1.2.0/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0    18521 2023-06-27 23:31:10.129931 whylogs-1.2.0/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24739 2023-06-27 23:31:08.669890 whylogs-1.2.0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0    18571 2023-06-27 23:31:08.549886 whylogs-1.2.0/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21840 2023-06-27 23:31:08.549886 whylogs-1.2.0/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     7350 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/relations.py
--rw-r--r--   0        0        0    11101 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/resolvers.py
--rw-r--r--   0        0        0     9526 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/segment.py
--rw-r--r--   0        0        0     2343 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0      826 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/specialized_resolvers.py
--rw-r--r--   0        0        0     2087 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/stubs.py
--rw-r--r--   0        0        0      486 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     3603 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2569 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     1602 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      210 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     4760 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0      508 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     6157 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    17663 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     8747 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      211 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/base.py
--rw-r--r--   0        0        0     6087 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6397 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0     3506 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/descr/employee.rst
--rw-r--r--   0        0        0    11285 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10688 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0    10981 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/employee.py
--rw-r--r--   0        0        0     2349 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11476 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/datasets/weather.py
--rw-r--r--   0        0        0        0 2023-06-27 23:30:31.464863 whylogs-1.2.0/whylogs/experimental/__init__.py
--rw-r--r--   0        0        0     3770 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/constraints_generation/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/constraints_generation/condition_counts.py
--rw-r--r--   0        0        0      846 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/constraints_generation/count_metrics.py
--rw-r--r--   0        0        0     1554 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/constraints_generation/distribution_metrics.py
--rw-r--r--   0        0        0     1011 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/constraints_generation/frequent_items.py
--rw-r--r--   0        0        0      685 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/constraints_generation/multi_metrics.py
--rw-r--r--   0        0        0      973 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/constraints_generation/types_metrics.py
--rw-r--r--   0        0        0    19692 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/core/metrics/udf_metric.py
--rw-r--r--   0        0        0    10230 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/core/udf_schema.py
--rw-r--r--   0        0        0     8861 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/extras/embedding_metric.py
--rw-r--r--   0        0        0      939 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/extras/matrix_component.py
--rwxr-xr-x   0        0        0    16737 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/extras/nlp_metric.py
--rw-r--r--   0        0        0        0 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/performance_estimation/__init__.py
--rw-r--r--   0        0        0     1554 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/performance_estimation/estimation_results.py
--rw-r--r--   0        0        0     8872 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/performance_estimation/estimators.py
--rw-r--r--   0        0        0     3777 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/experimental/preprocess/embeddings/selectors.py
--rw-r--r--   0        0        0    10031 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    15367 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/migration/converters.py
--rw-r--r--   0        0        0     6959 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/__init__.py
--rw-r--r--   0        0        0      168 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/configs.py
--rw-r--r--   0        0        0        0 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/drift/__init__.py
--rw-r--r--   0        0        0    21751 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/drift/column_drift_algorithms.py
--rw-r--r--   0        0        0     1366 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/drift/configs.py
--rw-r--r--   0        0        0        0 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2502 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     3218 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2023-06-27 23:30:31.468863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2023-06-27 23:30:31.472863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2023-06-27 23:30:31.472863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2023-06-27 23:30:31.472863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2023-06-27 23:30:31.472863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2023-06-27 23:30:31.472863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2023-06-27 23:30:31.472863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2023-06-27 23:30:31.472863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2023-06-27 23:30:31.472863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2023-06-27 23:30:31.476863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2023-06-27 23:30:31.476863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2023-06-27 23:30:31.476863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2023-06-27 23:30:31.476863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2023-06-27 23:30:31.476863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2023-06-27 23:30:31.476863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2023-06-27 23:30:31.476863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2023-06-27 23:30:31.476863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2023-06-27 23:30:31.476863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2023-06-27 23:30:31.480863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2023-06-27 23:30:31.480863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2023-06-27 23:30:31.480863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2023-06-27 23:30:31.480863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2023-06-27 23:30:31.480863 whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2023-06-27 23:30:31.480863 whylogs-1.2.0/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2023-06-27 23:30:31.480863 whylogs-1.2.0/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2023-06-27 23:30:31.480863 whylogs-1.2.0/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2023-06-27 23:30:31.480863 whylogs-1.2.0/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2023-06-27 23:30:31.484863 whylogs-1.2.0/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2023-06-27 23:30:31.484863 whylogs-1.2.0/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    52663 2023-06-27 23:30:31.484863 whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2023-06-27 23:30:31.484863 whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    26825 2023-06-27 23:30:31.484863 whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2023-06-27 23:30:31.484863 whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    15177 2023-06-27 23:30:31.484863 whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    18298 2023-06-27 23:30:31.484863 whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41933 2023-06-27 23:30:31.484863 whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    21376 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2466 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0    12576 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3561 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2747 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1060 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0    14298 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3581 2023-06-27 23:30:31.488864 whylogs-1.2.0/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0     6558 1970-01-01 00:00:00.000000 whylogs-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3166 2023-07-04 19:33:28.473857 whylogs-1.2.1/DESCRIPTION.md
+-rw-r--r--   0        0        0     5846 2023-07-04 19:34:03.066201 whylogs-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1801 2023-07-04 19:33:28.525857 whylogs-1.2.1/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-04 19:33:28.525857 whylogs-1.2.1/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-04 19:33:28.525857 whylogs-1.2.1/whylogs/api/annotations.py
+-rw-r--r--   0        0        0      120 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     4840 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     1997 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/fugue/registry.py
+-rw-r--r--   0        0        0     8157 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/experimental/multi_dataset_logger/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/experimental/multi_dataset_logger/future_util.py
+-rw-r--r--   0        0        0     2119 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py
+-rw-r--r--   0        0        0    15693 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py
+-rw-r--r--   0        0        0     3964 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py
+-rw-r--r--   0        0        0     4770 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    19765 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     9550 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     2113 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/segment_cache.py
+-rw-r--r--   0        0        0     6333 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      687 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      406 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     6168 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0     7663 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/pyspark/experimental/segmented_profiler.py
+-rw-r--r--   0        0        0      465 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     2073 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      237 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4566 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0     1208 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      672 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/store/query.py
+-rw-r--r--   0        0        0     5350 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/store/sqlite_store.py
+-rw-r--r--   0        0        0     6128 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/whylabs/__init__.py
+-rw-r--r--   0        0        0     7497 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/whylabs/session/config.py
+-rw-r--r--   0        0        0      329 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/whylabs/session/notebook_check.py
+-rw-r--r--   0        0        0     3813 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/whylabs/session/notebook_logger.py
+-rw-r--r--   0        0        0    10646 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/whylabs/session/session_manager.py
+-rw-r--r--   0        0        0      666 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/whylabs/session/session_types.py
+-rw-r--r--   0        0        0      947 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     2726 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     1169 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     2084 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0     3408 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    39185 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0     1217 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0     1090 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     3391 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/common.py
+-rw-r--r--   0        0        0     1589 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/configs.py
+-rw-r--r--   0        0        0      455 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0     1798 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2049 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/constraints/factories/condition_counts.py
+-rw-r--r--   0        0        0     2601 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     7063 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0      737 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/constraints/factories/multi_metrics.py
+-rw-r--r--   0        0        0     3199 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/constraints/factories/types_metrics.py
+-rw-r--r--   0        0        0    30671 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    11486 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4120 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/errors.py
+-rw-r--r--   0        0        0     2560 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0     1740 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/metric_getters.py
+-rw-r--r--   0        0        0      984 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4085 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     5031 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6481 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0     7615 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4840 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2023-07-04 19:33:28.529857 whylogs-1.2.1/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    21749 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     8016 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     4517 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5504 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0     8976 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7445 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2837 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     5499 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/predicate_parser.py
+-rw-r--r--   0        0        0    14489 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2023-07-04 19:34:07.318235 whylogs-1.2.1/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    20212 2023-07-04 19:34:05.934224 whylogs-1.2.1/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2023-07-04 19:34:05.934224 whylogs-1.2.1/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29724 2023-07-04 19:34:05.934224 whylogs-1.2.1/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2023-07-04 19:34:07.490237 whylogs-1.2.1/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24739 2023-07-04 19:34:05.934224 whylogs-1.2.1/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2023-07-04 19:34:05.814223 whylogs-1.2.1/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21840 2023-07-04 19:34:05.814223 whylogs-1.2.1/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     7350 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/relations.py
+-rw-r--r--   0        0        0    11101 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0    10029 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2343 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      826 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/specialized_resolvers.py
+-rw-r--r--   0        0        0     2087 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      486 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     3603 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2569 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     1602 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      210 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     4760 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0      508 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     6157 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    17663 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     8747 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      211 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     6087 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6397 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0     3506 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/descr/employee.rst
+-rw-r--r--   0        0        0    11285 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10688 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0    10981 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/employee.py
+-rw-r--r--   0        0        0     2349 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11476 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/experimental/__init__.py
+-rw-r--r--   0        0        0     3770 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/experimental/constraints_generation/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/experimental/constraints_generation/condition_counts.py
+-rw-r--r--   0        0        0      846 2023-07-04 19:33:28.533857 whylogs-1.2.1/whylogs/experimental/constraints_generation/count_metrics.py
+-rw-r--r--   0        0        0     1554 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/constraints_generation/distribution_metrics.py
+-rw-r--r--   0        0        0     1011 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/constraints_generation/frequent_items.py
+-rw-r--r--   0        0        0      685 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/constraints_generation/multi_metrics.py
+-rw-r--r--   0        0        0      973 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/constraints_generation/types_metrics.py
+-rw-r--r--   0        0        0    19692 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/core/metrics/udf_metric.py
+-rw-r--r--   0        0        0    13720 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/core/udf_schema.py
+-rw-r--r--   0        0        0     8861 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/extras/embedding_metric.py
+-rw-r--r--   0        0        0      939 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/extras/matrix_component.py
+-rwxr-xr-x   0        0        0    16737 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/extras/nlp_metric.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/performance_estimation/__init__.py
+-rw-r--r--   0        0        0     1554 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/performance_estimation/estimation_results.py
+-rw-r--r--   0        0        0     8872 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/performance_estimation/estimators.py
+-rw-r--r--   0        0        0     3777 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/experimental/preprocess/embeddings/selectors.py
+-rw-r--r--   0        0        0    10031 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    15367 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     6959 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/configs.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/drift/__init__.py
+-rw-r--r--   0        0        0    21751 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/drift/column_drift_algorithms.py
+-rw-r--r--   0        0        0     1366 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/drift/configs.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2502 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     3218 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2023-07-04 19:33:28.537857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2023-07-04 19:33:28.541857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2023-07-04 19:33:28.545857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2023-07-04 19:33:28.545857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2023-07-04 19:33:28.545857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2023-07-04 19:33:28.545857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2023-07-04 19:33:28.545857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2023-07-04 19:33:28.545857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2023-07-04 19:33:28.545857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2023-07-04 19:33:28.545857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2023-07-04 19:33:28.545857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2023-07-04 19:33:28.549857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2023-07-04 19:33:28.549857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2023-07-04 19:33:28.549857 whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2023-07-04 19:33:28.549857 whylogs-1.2.1/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2023-07-04 19:33:28.549857 whylogs-1.2.1/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2023-07-04 19:33:28.549857 whylogs-1.2.1/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2023-07-04 19:33:28.549857 whylogs-1.2.1/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2023-07-04 19:33:28.549857 whylogs-1.2.1/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2023-07-04 19:33:28.549857 whylogs-1.2.1/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    52663 2023-07-04 19:33:28.553857 whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2023-07-04 19:33:28.553857 whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    26825 2023-07-04 19:33:28.553857 whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2023-07-04 19:33:28.553857 whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    15177 2023-07-04 19:33:28.553857 whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    18298 2023-07-04 19:33:28.553857 whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41933 2023-07-04 19:33:28.553857 whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    21376 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0    12576 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3561 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2747 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1060 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0    14298 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3581 2023-07-04 19:33:28.557857 whylogs-1.2.1/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0     6558 1970-01-01 00:00:00.000000 whylogs-1.2.1/PKG-INFO
```

### Comparing `whylogs-1.2.0/DESCRIPTION.md` & `whylogs-1.2.1/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/pyproject.toml` & `whylogs-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.2.0"
+version = "1.2.1"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "DESCRIPTION.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
```

### Comparing `whylogs-1.2.0/whylogs/__init__.py` & `whylogs-1.2.1/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/annotations.py` & `whylogs-1.2.1/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/fugue/profiler.py` & `whylogs-1.2.1/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/fugue/registry.py` & `whylogs-1.2.1/whylogs/api/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/logger/__init__.py` & `whylogs-1.2.1/whylogs/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py` & `whylogs-1.2.1/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py` & `whylogs-1.2.1/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py` & `whylogs-1.2.1/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/logger/logger.py` & `whylogs-1.2.1/whylogs/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/logger/result_set.py` & `whylogs-1.2.1/whylogs/api/logger/result_set.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/logger/rolling.py` & `whylogs-1.2.1/whylogs/api/logger/rolling.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/logger/segment_cache.py` & `whylogs-1.2.1/whylogs/api/logger/segment_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/logger/segment_processing.py` & `whylogs-1.2.1/whylogs/api/logger/segment_processing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/logger/transient.py` & `whylogs-1.2.1/whylogs/api/logger/transient.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.2.1/whylogs/api/pyspark/experimental/profiler.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from functools import partial, reduce
 from logging import getLogger
 from typing import Dict, Iterable, Optional, Tuple
 
 import whylogs as why
 from whylogs.api.usage_stats import emit_usage
 from whylogs.core import DatasetSchema
+from whylogs.core.metrics.metrics import conf
 from whylogs.core.stubs import pd
 from whylogs.core.view.column_profile_view import ColumnProfileView
 from whylogs.core.view.dataset_profile_view import DatasetProfileView
 
 logger = getLogger(__name__)
 emit_usage("pyspark")
 
@@ -61,24 +62,67 @@
         col_name for col_name in input_df.schema.names if isinstance(input_df.schema[col_name].dataType, VectorUDT)
     ]
     input_df_arrays = input_df
     for col_name in vector_columns:
         input_df_arrays = input_df_arrays.withColumn(col_name, vector_to_array(input_df_arrays[col_name]))
     cp = f"{COL_NAME_FIELD} string, {COL_PROFILE_FIELD} binary"
     whylogs_pandas_map_profiler_with_schema = partial(whylogs_pandas_map_profiler, schema=schema)
+
     profile_bytes_df = input_df_arrays.mapInPandas(whylogs_pandas_map_profiler_with_schema, schema=cp)  # type: ignore
     column_profiles = profile_bytes_df.groupby(COL_NAME_FIELD).applyInPandas(  # linebreak
         column_profile_bytes_aggregator, schema=cp
     )
     collected_profile_views = {
         row.col_name: ColumnProfileView.from_bytes(row.col_profile) for row in column_profiles.collect()
     }
     return collected_profile_views
 
 
+def _collect_column_profile_views_batched(
+    batch_size: int, input_df: SparkDataFrame, schema: Optional[DatasetSchema] = None
+) -> Dict[str, ColumnProfileView]:
+    if batch_size <= 0:
+        logger.warning(
+            f"Batched pyspark column processing was called with batch_size of {batch_size}, falling back to non-batched profiling."
+        )
+        return collect_column_profile_views(input_df=input_df, schema=schema)
+
+    columns = input_df.columns
+    num_batches = len(columns) // batch_size  # Total number of batches
+
+    # Initialize an empty dataset_profile
+    combined_column_views = dict()
+
+    # process the column profiles in batches
+    for batch_num in range(num_batches):
+        start_idx = batch_num * batch_size
+        end_idx = (batch_num + 1) * batch_size
+        selected_columns = columns[start_idx:end_idx]
+        column_partitioned_batch_df = input_df.select(*selected_columns)
+        column_views_dict = collect_column_profile_views(input_df=column_partitioned_batch_df, schema=schema)
+        combined_column_views.update(column_views_dict)
+
+    # Handle the last batch (if any) that may have fewer columns
+    last_batch_columns = columns[num_batches * batch_size :]
+    if last_batch_columns:
+        column_partitioned_batch_df = input_df.select(*last_batch_columns)
+        # Process the last batch DataFrame
+        column_views_dict = collect_column_profile_views(input_df=column_partitioned_batch_df, schema=schema)
+        combined_column_views.update(column_views_dict)
+
+    return combined_column_views
+
+
+def _get_column_batch_size() -> Optional[int]:
+    if conf.column_batch_size:
+        return conf.column_batch_size
+    else:
+        return None
+
+
 def collect_dataset_profile_view(
     input_df: SparkDataFrame,
     dataset_timestamp: Optional[int] = None,
     creation_timestamp: Optional[int] = None,
     schema: Optional[DatasetSchema] = None,
 ) -> DatasetProfileView:
     now = datetime.now(timezone.utc)
@@ -87,15 +131,18 @@
     _creation_timestamp = creation_timestamp or now
     if schema and schema.segments:
         raise ValueError(
             "collect_dataset_profile_view returns a single DatasetProfileView but segmentation was defined, "
             f": {schema.segments} may return multiple segmented profiles. Please use `collect_segmented_results` if you want to profile"
             " in spark with segments defined."
         )
-
-    column_views_dict = collect_column_profile_views(input_df=input_df, schema=schema)
+    batch_size = _get_column_batch_size()
+    if batch_size is not None:
+        column_views_dict = _collect_column_profile_views_batched(batch_size, input_df=input_df, schema=schema)
+    else:
+        column_views_dict = collect_column_profile_views(input_df=input_df, schema=schema)
 
     profile_view = DatasetProfileView(
         columns=column_views_dict, dataset_timestamp=_dataset_timestamp, creation_timestamp=_creation_timestamp
     )
 
     return profile_view
```

### Comparing `whylogs-1.2.0/whylogs/api/pyspark/experimental/segmented_profiler.py` & `whylogs-1.2.1/whylogs/api/pyspark/experimental/segmented_profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/reader/local.py` & `whylogs-1.2.1/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/reader/reader.py` & `whylogs-1.2.1/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/reader/s3.py` & `whylogs-1.2.1/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/store/local_store.py` & `whylogs-1.2.1/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/store/profile_store.py` & `whylogs-1.2.1/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/store/query.py` & `whylogs-1.2.1/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/store/sqlite_store.py` & `whylogs-1.2.1/whylogs/api/store/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/usage_stats/__init__.py` & `whylogs-1.2.1/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/whylabs/session/config.py` & `whylogs-1.2.1/whylogs/api/whylabs/session/config.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/whylabs/session/notebook_logger.py` & `whylogs-1.2.1/whylogs/api/whylabs/session/notebook_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/whylabs/session/session_manager.py` & `whylogs-1.2.1/whylogs/api/whylabs/session/session_manager.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/whylabs/session/session_types.py` & `whylogs-1.2.1/whylogs/api/whylabs/session/session_types.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/writer/__init__.py` & `whylogs-1.2.1/whylogs/api/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/writer/gcs.py` & `whylogs-1.2.1/whylogs/api/writer/gcs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/writer/local.py` & `whylogs-1.2.1/whylogs/api/writer/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/writer/mlflow.py` & `whylogs-1.2.1/whylogs/api/writer/mlflow.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/writer/s3.py` & `whylogs-1.2.1/whylogs/api/writer/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/writer/whylabs.py` & `whylogs-1.2.1/whylogs/api/writer/whylabs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/api/writer/writer.py` & `whylogs-1.2.1/whylogs/api/writer/writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/__init__.py` & `whylogs-1.2.1/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/column_profile.py` & `whylogs-1.2.1/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/configs.py` & `whylogs-1.2.1/whylogs/core/configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "basic-latin": (0x00, 0x7F),
     "extended-latin": (0x0080, 0x02AF),
 }
 lower_case: bool = True  # Convert Unicode characters to lower-case before counting Unicode ranges
 normalize: bool = True  # Unicode normalize strings before counting Unicode ranges
 max_frequent_item_size: int = 128
 identity_column: Optional[str] = None
+column_batch_size: Optional[int] = 1024
 
 
 class FrequentItemsErrorType(int, Enum):
     NO_FALSE_NEGATIVES = 1
     NO_FALSE_POSITIVES = 0
 
     def to_datasketches_type(self) -> ds.frequent_items_error_type:
```

### Comparing `whylogs-1.2.0/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.2.1/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.2.1/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/constraints/factories/condition_counts.py` & `whylogs-1.2.1/whylogs/core/constraints/factories/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.2.1/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.2.1/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.2.1/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/constraints/factories/multi_metrics.py` & `whylogs-1.2.1/whylogs/core/constraints/factories/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/constraints/factories/types_metrics.py` & `whylogs-1.2.1/whylogs/core/constraints/factories/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.2.1/whylogs/core/constraints/metric_constraints.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/dataset_profile.py` & `whylogs-1.2.1/whylogs/core/dataset_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/datatypes.py` & `whylogs-1.2.1/whylogs/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/errors.py` & `whylogs-1.2.1/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/feature_weights.py` & `whylogs-1.2.1/whylogs/core/feature_weights.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/input_resolver.py` & `whylogs-1.2.1/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metric_getters.py` & `whylogs-1.2.1/whylogs/core/metric_getters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/__init__.py` & `whylogs-1.2.1/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/aggregators.py` & `whylogs-1.2.1/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/column_metrics.py` & `whylogs-1.2.1/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/compound_metric.py` & `whylogs-1.2.1/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.2.1/whylogs/core/metrics/condition_count_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/decorators.py` & `whylogs-1.2.1/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/deserializers.py` & `whylogs-1.2.1/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/maths.py` & `whylogs-1.2.1/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/metric_components.py` & `whylogs-1.2.1/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/metrics.py` & `whylogs-1.2.1/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/multimetric.py` & `whylogs-1.2.1/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/serializers.py` & `whylogs-1.2.1/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/metrics/unicode_range.py` & `whylogs-1.2.1/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.2.1/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.2.1/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.2.1/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/predicate_parser.py` & `whylogs-1.2.1/whylogs/core/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/preprocessing.py` & `whylogs-1.2.1/whylogs/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/proto/v0/v0_constraints_pb2.py` & `whylogs-1.2.1/whylogs/core/proto/v0/v0_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.2.1/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/proto/v0/v0_messages_pb2.py` & `whylogs-1.2.1/whylogs/core/proto/v0/v0_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.2.1/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/proto/v0/v0_summaries_pb2.py` & `whylogs-1.2.1/whylogs/core/proto/v0/v0_summaries_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.2.1/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/proto/whylogs_messages_pb2.py` & `whylogs-1.2.1/whylogs/core/proto/whylogs_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.2.1/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/relations.py` & `whylogs-1.2.1/whylogs/core/relations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/resolvers.py` & `whylogs-1.2.1/whylogs/core/resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/schema.py` & `whylogs-1.2.1/whylogs/core/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -234,30 +234,45 @@
         metrics: Optional[List[MetricSpec]] = None,
     ):
         spec = ResolverSpec(column_name=column_name, column_type=column_type, metrics=metrics or [])
         self.add_resolver(spec)
 
     def __init__(
         self,
-        resolvers: List[ResolverSpec],
+        resolvers: Optional[List[ResolverSpec]] = None,
         types: Optional[Dict[str, Any]] = None,
         default_config: Optional[MetricConfig] = None,
         type_mapper: Optional[TypeMapper] = None,
         cache_size: int = 1024,
         schema_based_automerge: bool = False,
         segments: Optional[Dict[str, SegmentationPartition]] = None,
         validators: Optional[Dict[str, List[Validator]]] = None,
     ) -> None:
-        if not resolvers:
-            resolvers = res.DEFAULT_RESOLVERS
+        if resolvers is None:
+            resolvers = res.DEFAULT_RESOLVER
             logger.warning("No columns specified in DeclarativeSchema")
         resolver = DeclarativeResolver(resolvers, default_config)
         super().__init__(
             types=types,
             default_configs=default_config,
             type_mapper=type_mapper,
             resolvers=resolver,
             cache_size=cache_size,
             schema_based_automerge=schema_based_automerge,
             segments=segments,
             validators=validators,
         )
+
+    def copy(self) -> "DeclarativeSchema":
+        copy = DeclarativeSchema(
+            [],
+            deepcopy(self.types),
+            deepcopy(self.default_configs),
+            deepcopy(self.type_mapper),
+            self.cache_size,
+            self.schema_based_automerge,
+            self.segments.copy(),
+            deepcopy(self.validators),
+        )
+        copy.resolvers = deepcopy(self.resolvers)
+        copy._columns = deepcopy(self._columns)
+        return copy
```

### Comparing `whylogs-1.2.0/whylogs/core/segmentation_partition.py` & `whylogs-1.2.1/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/specialized_resolvers.py` & `whylogs-1.2.1/whylogs/core/specialized_resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/stubs.py` & `whylogs-1.2.1/whylogs/core/stubs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.2.1/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/utils/stats_calculations.py` & `whylogs-1.2.1/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/utils/utils.py` & `whylogs-1.2.1/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/validators/condition_validator.py` & `whylogs-1.2.1/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/view/column_profile_view.py` & `whylogs-1.2.1/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.2.1/whylogs/core/view/dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.2.1/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/datasets/base.py` & `whylogs-1.2.1/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/datasets/configs.py` & `whylogs-1.2.1/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.2.1/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/datasets/descr/employee.rst` & `whylogs-1.2.1/whylogs/datasets/descr/employee.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/datasets/descr/weather.rst` & `whylogs-1.2.1/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/datasets/ecommerce.py` & `whylogs-1.2.1/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/datasets/employee.py` & `whylogs-1.2.1/whylogs/datasets/employee.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/datasets/utils.py` & `whylogs-1.2.1/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/datasets/weather.py` & `whylogs-1.2.1/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/constraints_generation/__init__.py` & `whylogs-1.2.1/whylogs/experimental/constraints_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/constraints_generation/condition_counts.py` & `whylogs-1.2.1/whylogs/experimental/constraints_generation/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/constraints_generation/count_metrics.py` & `whylogs-1.2.1/whylogs/experimental/constraints_generation/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/constraints_generation/distribution_metrics.py` & `whylogs-1.2.1/whylogs/experimental/constraints_generation/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/constraints_generation/frequent_items.py` & `whylogs-1.2.1/whylogs/experimental/constraints_generation/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/constraints_generation/multi_metrics.py` & `whylogs-1.2.1/whylogs/experimental/constraints_generation/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/constraints_generation/types_metrics.py` & `whylogs-1.2.1/whylogs/experimental/constraints_generation/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/core/metrics/udf_metric.py` & `whylogs-1.2.1/whylogs/experimental/core/metrics/udf_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/core/udf_schema.py` & `whylogs-1.2.1/whylogs/experimental/core/udf_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,58 +10,72 @@
     List,
     Mapping,
     Optional,
     Tuple,
     Union,
 )
 
-from whylogs.core.datatypes import TypeMapper
+from whylogs.core.datatypes import DataType, TypeMapper
 from whylogs.core.metrics.metrics import Metric, MetricConfig
 from whylogs.core.resolvers import DEFAULT_RESOLVER, MetricSpec, ResolverSpec
-from whylogs.core.schema import DatasetSchema, DeclarativeSchema
+from whylogs.core.schema import DeclarativeSchema
 from whylogs.core.segmentation_partition import SegmentationPartition
 from whylogs.core.stubs import pd
 from whylogs.core.validators.validator import Validator
 from whylogs.experimental.core.metrics.udf_metric import (
     _reset_metric_udfs,
     generate_udf_resolvers,
 )
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class UdfSpec:
     """
-    Defines UDFs to apply to matching input columns. Tthe UDF is
-    passed a dictionary or dataframe with the named columns available (the UDF will
-    not be called unless all the named columns are available). The new column name
-    the key in the udfs dictionary.
+    Defines UDFs to apply to matching input columns.
+
+    For UDFs matched by column_name(s), the function is passed a dictionary or
+    dataframe with the named columns available (the UDF will not be called unless
+    all the named columns are available). The output column name is the key in
+    the udfs dictionary.
+
+    For UDFs matched by column_type, the function is passed the value or Pandas
+    series. The output column name is the key in the udfs dictionary prefixed
+    by the input column name.
+
+    You must specify exactly one of column_names or column_type.
     """
 
-    column_names: List[str]
+    column_names: Optional[List[str]] = None
     udfs: Dict[str, Callable[[Any], Any]] = field(
         default_factory=dict
     )  # new column name -> callable to compute new column value
+    column_type: Optional[DataType] = None
 
     def __post_init__(self):
-        if len(self.column_names) == 0 or not all([isinstance(x, str) for x in self.column_names]):
-            raise ValueError("UdfSpec: column_names must be either a non-empty list of strings")
+        if self.column_type is not None:
+            if self.column_names:
+                raise ValueError("UdfSpec cannot specify both column_names and column_type")
+        elif self.column_names is None:
+            raise ValueError("UdfSpec must specify column_names or column_type")
+        elif len(self.column_names) == 0 or not all([isinstance(x, str) for x in self.column_names]):
+            raise ValueError("UdfSpec column_names must be a non-empty list of strings")
 
 
 def _apply_udfs_on_row(value: Any, udfs: Dict, new_columns: Dict[str, Any], input_cols: Collection[str]) -> None:
     for new_col, udf in udfs.items():
         if new_col in input_cols:
             continue
 
         try:
             new_columns[new_col] = udf(value)
         except Exception:  # noqa
             new_columns[new_col] = None
-            logger.exception(f"Evaluating multi-column UDF {new_col} failed")
+            logger.exception(f"Evaluating UDF {new_col} failed")
 
 
 def _apply_udfs_on_dataframe(
     pandas: pd.DataFrame, udfs: Dict, new_df: pd.DataFrame, input_cols: Collection[str]
 ) -> None:
     for new_col, udf in udfs.items():
         if new_col in input_cols:
@@ -70,23 +84,35 @@
         try:
             new_df[new_col] = udf(pandas)
         except Exception as e:  # noqa
             new_df[new_col] = pd.Series([None])
             logger.exception(f"Evaluating UDF {new_col} failed on columns {pandas.keys()} with error {e}")
 
 
+def _apply_type_udfs(pandas: pd.Series, udfs: Dict, new_df: pd.DataFrame, input_cols: Collection[str]) -> None:
+    for new_col, udf in udfs.items():
+        if new_col in input_cols:
+            continue
+
+        try:
+            new_df[new_col] = udf(pandas)
+        except Exception as e:  # noqa
+            new_df[new_col] = pd.Series([None])
+            logger.exception(f"Evaluating UDF {new_col} failed on column {new_col} with error {e}")
+
+
 class UdfSchema(DeclarativeSchema):
     """
     Subclass of DeclarativeSchema that runs the UDFs specified in udf_specs to
     create new columns before resolving metrics.
     """
 
     def __init__(
         self,
-        resolvers: List[ResolverSpec],
+        resolvers: Optional[List[ResolverSpec]] = None,
         types: Optional[Dict[str, Any]] = None,
         default_config: Optional[MetricConfig] = None,
         type_mapper: Optional[TypeMapper] = None,
         cache_size: int = 1024,
         schema_based_automerge: bool = False,
         segments: Optional[Dict[str, SegmentationPartition]] = None,
         validators: Optional[Dict[str, List[Validator]]] = None,
@@ -99,33 +125,50 @@
             type_mapper=type_mapper,
             cache_size=cache_size,
             schema_based_automerge=schema_based_automerge,
             segments=segments,
             validators=validators,
         )
         udf_specs = udf_specs if udf_specs else []
-        self.multicolumn_udfs = list(udf_specs)
+        self.multicolumn_udfs = [spec for spec in udf_specs if spec.column_names]
+        self.type_udfs = defaultdict(list)
+        for spec in udf_specs:
+            if spec.column_type:
+                self.type_udfs[spec.column_type].append(spec)
 
-    def copy(self) -> DatasetSchema:
+    def copy(self) -> "UdfSchema":
         copy = super().copy()
-        copy.multicolumn_udfs = list(self.multicolumn_udfs)
+        copy.multicolumn_udfs = deepcopy(self.multicolumn_udfs)
+        copy.type_udfs = deepcopy(self.type_udfs)
         return copy
 
     def _run_udfs_on_row(
         self, row: Mapping[str, Any], new_columns: Dict[str, Any], input_cols: Collection[str]
     ) -> None:
         for spec in self.multicolumn_udfs:
-            if set(spec.column_names).issubset(set(row.keys())):
+            if spec.column_names and set(spec.column_names).issubset(set(row.keys())):
                 _apply_udfs_on_row(row, spec.udfs, new_columns, input_cols)
 
+        for column, value in row.items():
+            why_type = type(self.type_mapper(type(value)))
+            for spec in self.type_udfs[why_type]:
+                udfs = {f"{column}.{key}": spec.udfs[key] for key in spec.udfs.keys()}
+                _apply_udfs_on_row(value, udfs, new_columns, input_cols)
+
     def _run_udfs_on_dataframe(self, pandas: pd.DataFrame, new_df: pd.DataFrame, input_cols: Collection[str]) -> None:
         for spec in self.multicolumn_udfs:
-            if set(spec.column_names).issubset(set(pandas.keys())):
+            if spec.column_names and set(spec.column_names).issubset(set(pandas.keys())):
                 _apply_udfs_on_dataframe(pandas[spec.column_names], spec.udfs, new_df, input_cols)
 
+        for column, dtype in pandas.dtypes.items():
+            why_type = type(self.type_mapper(dtype))
+            for spec in self.type_udfs[why_type]:
+                udfs = {f"{column}.{key}": spec.udfs[key] for key in spec.udfs.keys()}
+                _apply_type_udfs(pandas[column], udfs, new_df, input_cols)
+
     def _run_udfs(
         self, pandas: Optional[pd.DataFrame] = None, row: Optional[Dict[str, Any]] = None
     ) -> Tuple[Optional[pd.DataFrame], Optional[Mapping[str, Any]]]:
         new_columns = deepcopy(row) if row else None
         new_df = pd.DataFrame() if pandas is not None else None
         if row is not None:
             self._run_udfs_on_row(row, new_columns, row.keys())  # type: ignore
@@ -194,24 +237,58 @@
             _resolver_specs[schema_name].append(ResolverSpec(name, None, [MetricSpec(m) for m in anti_metrics], True))
 
         return func
 
     return decorator_register
 
 
+def register_type_udf(
+    col_type: DataType,
+    udf_name: Optional[str] = None,
+    namespace: Optional[str] = None,
+    schema_name: str = "",
+) -> Callable[[Any], Any]:
+    """
+    Decorator to easily configure UDFs for your data set. Decorate your UDF
+    functions, then call generate_udf_dataset_schema() to create a UdfSchema
+    that includes the UDFs configured by your decorator parameters. The decorated
+    function will automatically be a UDF in the UdfSchema.
+
+    The registered function will be applied to any columns of the specified type.
+    Specify udf_name to give the output of the UDF a name. udf_name
+    defautls to the name of the decorated function. The output column name is the
+    UDF name prefixed with the input column name. Note that all lambdas are
+    named "lambda", so omitting udf_name on more than one lambda will result
+    in name collisions. If you pass a namespace, it will be prepended to the UDF name.
+    Specifying schema_name will register the UDF in a particular schema. If omitted,
+    it will be registered to the defualt schema.
+
+    """
+
+    def decorator_register(func):
+        global _multicolumn_udfs, _resolver_specs
+        name = udf_name or func.__name__
+        name = f"{namespace}.{name}" if namespace else name
+        _multicolumn_udfs[schema_name].append(UdfSpec(None, {name: func}, col_type))
+
+        return func
+
+    return decorator_register
+
+
 def generate_udf_specs(
     other_udf_specs: Optional[List[UdfSpec]] = None,
     schema_name: Union[str, List[str]] = "",
     include_default_schema: bool = True,
 ) -> List[UdfSpec]:
     """
-    Generates a list UdfSpecs that implement the UDFs specified
-    by the @register_dataset_udf decorators. You can provide a list of
-    other_udf_specs to include in addition to those UDFs registered via
-    the decorator.
+    Generates a list UdfSpecs that implement the UDFs specified by the
+    @register_dataset_udf, @register_type_udf, and @register_metric_udf
+    decorators. You can provide a list of other_udf_specs to include in
+    addition to those UDFs registered via the decorator.
 
     For example:
 
     @register_dataset_udf(col_names=["col1"])
     def add5(x):
         return x + 5
```

### Comparing `whylogs-1.2.0/whylogs/experimental/extras/embedding_metric.py` & `whylogs-1.2.1/whylogs/experimental/extras/embedding_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/extras/matrix_component.py` & `whylogs-1.2.1/whylogs/experimental/extras/matrix_component.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/extras/nlp_metric.py` & `whylogs-1.2.1/whylogs/experimental/extras/nlp_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/performance_estimation/estimation_results.py` & `whylogs-1.2.1/whylogs/experimental/performance_estimation/estimation_results.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/performance_estimation/estimators.py` & `whylogs-1.2.1/whylogs/experimental/performance_estimation/estimators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/experimental/preprocess/embeddings/selectors.py` & `whylogs-1.2.1/whylogs/experimental/preprocess/embeddings/selectors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/extras/image_metric.py` & `whylogs-1.2.1/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/migration/converters.py` & `whylogs-1.2.1/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/migration/uncompound.py` & `whylogs-1.2.1/whylogs/migration/uncompound.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/drift/column_drift_algorithms.py` & `whylogs-1.2.1/whylogs/viz/drift/column_drift_algorithms.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/drift/configs.py` & `whylogs-1.2.1/whylogs/viz/drift/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/enums/enums.py` & `whylogs-1.2.1/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.2.1/whylogs/viz/extensions/reports/html_report.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.2.1/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.2.1/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.2.1/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.2.1/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.2.1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.2.1/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.2.1/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/js/d3.min.js` & `whylogs-1.2.1/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/js/handlebars.js` & `whylogs-1.2.1/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.2.1/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.2.1/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/html/templates/index.html` & `whylogs-1.2.1/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.2.1/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.2.1/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.2.1/whylogs/viz/utils/drift_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.2.1/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.2.1/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.2.1/whylogs/viz/utils/html_template_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.2.1/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.2.1/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.0/PKG-INFO` & `whylogs-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylogs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Profile and monitor your ML data pipeline end-to-end
 Home-page: https://docs.whylabs.ai
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.7.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: whylogs Version: 1.2.0 Summary: Profile and monitor
+Metadata-Version: 2.1 Name: whylogs Version: 1.2.1 Summary: Profile and monitor
 your ML data pipeline end-to-end Home-page: https://docs.whylabs.ai License:
 Apache-2.0 Author: WhyLabs.ai Author-email: support@whylabs.ai Requires-Python:
 >=3.7.1,<4 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: datasets
```

