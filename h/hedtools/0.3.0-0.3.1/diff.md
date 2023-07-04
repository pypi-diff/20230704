# Comparing `tmp/hedtools-0.3.0.tar.gz` & `tmp/hedtools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hedtools-0.3.0.tar", last modified: Tue Jun 20 20:41:22 2023, max compression
+gzip compressed data, was "dist\hedtools-0.3.1.tar", last modified: Tue Jul  4 17:53:08 2023, max compression
```

## Comparing `hedtools-0.3.0.tar` & `hedtools-0.3.1.tar`

### file list

```diff
@@ -1,149 +1,154 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/
--rw-rw-rw-   0        0        0     1103 2023-06-20 20:23:24.000000 hedtools-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       70 2022-06-20 19:04:23.000000 hedtools-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5981 2023-06-20 20:41:22.000000 hedtools-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5337 2023-06-20 20:23:24.000000 hedtools-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/
--rw-rw-rw-   0        0        0      773 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/__init__.py
--rw-rw-rw-   0        0        0      518 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/_version.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/errors/
--rw-rw-rw-   0        0        0      326 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/errors/__init__.py
--rw-rw-rw-   0        0        0    20119 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/errors/error_messages.py
--rw-rw-rw-   0        0        0    22248 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/errors/error_reporter.py
--rw-rw-rw-   0        0        0     5664 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/errors/error_types.py
--rw-rw-rw-   0        0        0     2079 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/errors/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/models/
--rw-rw-rw-   0        0        0      711 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/__init__.py
--rw-rw-rw-   0        0        0    19941 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/base_input.py
--rw-rw-rw-   0        0        0    17951 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/column_mapper.py
--rw-rw-rw-   0        0        0     5298 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/column_metadata.py
--rw-rw-rw-   0        0        0     8455 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/def_expand_gather.py
--rw-rw-rw-   0        0        0    13845 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/definition_dict.py
--rw-rw-rw-   0        0        0     3044 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/definition_entry.py
--rw-rw-rw-   0        0        0     6302 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/df_util.py
--rw-rw-rw-   0        0        0    15583 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/expression_parser.py
--rw-rw-rw-   0        0        0    18781 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/hed_group.py
--rw-rw-rw-   0        0        0    14042 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/hed_string.py
--rw-rw-rw-   0        0        0     4418 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/hed_string_group.py
--rw-rw-rw-   0        0        0    20438 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/hed_tag.py
--rw-rw-rw-   0        0        0      749 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/model_constants.py
--rw-rw-rw-   0        0        0     9063 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/sidecar.py
--rw-rw-rw-   0        0        0     2704 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/spreadsheet_input.py
--rw-rw-rw-   0        0        0     2974 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/tabular_input.py
--rw-rw-rw-   0        0        0      925 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/timeseries_input.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/schema/
--rw-rw-rw-   0        0        0      563 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/__init__.py
--rw-rw-rw-   0        0        0    19301 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_cache.py
--rw-rw-rw-   0        0        0    30335 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema.py
--rw-rw-rw-   0        0        0     2104 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema_constants.py
--rw-rw-rw-   0        0        0    10197 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema_entry.py
--rw-rw-rw-   0        0        0     6990 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema_group.py
--rw-rw-rw-   0        0        0     7202 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema_io.py
--rw-rw-rw-   0        0        0     8969 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema_section.py
--rw-rw-rw-   0        0        0     9013 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_compliance.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/schema/schema_data/
--rw-rw-rw-   0        0        0   316118 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/schema/schema_data/HED8.0.0.xml
--rw-rw-rw-   0        0        0   335759 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/schema/schema_data/HED8.1.0.xml
--rw-rw-rw-   0        0        0   345995 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_data/HED8.2.0.xml
--rw-rw-rw-   0        0        0   350310 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/schema/schema_data/HED_score_1.0.0.xml
--rw-rw-rw-   0        0        0   316637 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/schema/schema_data/HED_testlib_1.0.2.xml
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/schema/schema_io/
--rw-rw-rw-   0        0        0        0 2022-06-20 19:04:23.000000 hedtools-0.3.0/hed/schema/schema_io/__init__.py
--rw-rw-rw-   0        0        0     5464 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/schema2base.py
--rw-rw-rw-   0        0        0     5847 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/schema2wiki.py
--rw-rw-rw-   0        0        0     5576 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/schema2xml.py
--rw-rw-rw-   0        0        0     3692 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/schema_util.py
--rw-rw-rw-   0        0        0    24745 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/wiki2schema.py
--rw-rw-rw-   0        0        0      945 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/wiki_constants.py
--rw-rw-rw-   0        0        0    14077 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/xml2schema.py
--rw-rw-rw-   0        0        0     2507 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/xml_constants.py
--rw-rw-rw-   0        0        0     6221 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_validation_util.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/
--rw-rw-rw-   0        0        0     3090 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/analysis/
--rw-rw-rw-   0        0        0       29 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/analysis/__init__.py
--rw-rw-rw-   0        0        0     9402 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/analysis_util.py
--rw-rw-rw-   0        0        0    15621 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/analysis/annotation_util.py
--rw-rw-rw-   0        0        0     5505 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/event_manager.py
--rw-rw-rw-   0        0        0     5988 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/analysis/file_dictionary.py
--rw-rw-rw-   0        0        0     5796 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_context_manager.py
--rw-rw-rw-   0        0        0     4987 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_tag_counts.py
--rw-rw-rw-   0        0        0     6314 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_type_counts.py
--rw-rw-rw-   0        0        0     5573 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_type_definitions.py
--rw-rw-rw-   0        0        0     5368 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/analysis/hed_type_factors.py
--rw-rw-rw-   0        0        0     5189 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_type_manager.py
--rw-rw-rw-   0        0        0    12301 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_type_values.py
--rw-rw-rw-   0        0        0     9733 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/key_map.py
--rw-rw-rw-   0        0        0     1615 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/tabular_column_name_summary.py
--rw-rw-rw-   0        0        0    10722 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/tabular_summary.py
--rw-rw-rw-   0        0        0     1077 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/temporal_event.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/bids/
--rw-rw-rw-   0        0        0       42 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/bids/__init__.py
--rw-rw-rw-   0        0        0     4726 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/bids/bids_dataset.py
--rw-rw-rw-   0        0        0     3176 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/bids/bids_file.py
--rw-rw-rw-   0        0        0     9525 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/bids/bids_file_dictionary.py
--rw-rw-rw-   0        0        0     9280 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/bids/bids_file_group.py
--rw-rw-rw-   0        0        0     2960 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/bids/bids_sidecar_file.py
--rw-rw-rw-   0        0        0     8310 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/bids/bids_tabular_dictionary.py
--rw-rw-rw-   0        0        0     1433 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/bids/bids_tabular_file.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/remodeling/
--rw-rw-rw-   0        0        0       67 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/remodeling/__init__.py
--rw-rw-rw-   0        0        0    10544 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/backup_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/remodeling/cli/
--rw-rw-rw-   0        0        0       52 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/remodeling/cli/__init__.py
--rw-rw-rw-   0        0        0     9165 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel.py
--rw-rw-rw-   0        0        0     3738 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel_backup.py
--rw-rw-rw-   0        0        0     2188 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel_restore.py
--rw-rw-rw-   0        0        0    10276 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/remodeling/operations/
--rw-rw-rw-   0        0        0       30 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/remodeling/operations/__init__.py
--rw-rw-rw-   0        0        0     3891 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/operations/base_op.py
--rw-rw-rw-   0        0        0    10985 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/base_summary.py
--rw-rw-rw-   0        0        0     2437 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/convert_columns_op.py
--rw-rw-rw-   0        0        0     3143 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/factor_column_op.py
--rw-rw-rw-   0        0        0     4145 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/factor_hed_tags_op.py
--rw-rw-rw-   0        0        0     3307 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/factor_hed_type_op.py
--rw-rw-rw-   0        0        0     6750 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/merge_consecutive_op.py
--rw-rw-rw-   0        0        0     4716 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/number_groups_op.py
--rw-rw-rw-   0        0        0     3568 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/number_rows_op.py
--rw-rw-rw-   0        0        0     5552 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/remap_columns_op.py
--rw-rw-rw-   0        0        0     2472 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/remove_columns_op.py
--rw-rw-rw-   0        0        0     1988 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/remove_rows_op.py
--rw-rw-rw-   0        0        0     2428 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/rename_columns_op.py
--rw-rw-rw-   0        0        0     2847 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/reorder_columns_op.py
--rw-rw-rw-   0        0        0     5360 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/split_rows_op.py
--rw-rw-rw-   0        0        0     6092 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_column_names_op.py
--rw-rw-rw-   0        0        0    11856 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_column_values_op.py
--rw-rw-rw-   0        0        0     8064 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_definitions_op.py
--rw-rw-rw-   0        0        0     9588 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_tags_op.py
--rw-rw-rw-   0        0        0     9956 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_type_op.py
--rw-rw-rw-   0        0        0    10230 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_validation_op.py
--rw-rw-rw-   0        0        0     7408 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py
--rw-rw-rw-   0        0        0     2660 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/valid_operations.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/util/
--rw-rw-rw-   0        0        0       44 2022-09-12 19:32:19.000000 hedtools-0.3.0/hed/tools/util/__init__.py
--rw-rw-rw-   0        0        0    11413 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/util/data_util.py
--rw-rw-rw-   0        0        0     1546 2023-02-14 21:37:41.000000 hedtools-0.3.0/hed/tools/util/hed_logger.py
--rw-rw-rw-   0        0        0    11590 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/util/io_util.py
--rw-rw-rw-   0        0        0     1266 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/util/schema_util.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/validator/
--rw-rw-rw-   0        0        0      298 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/__init__.py
--rw-rw-rw-   0        0        0     5053 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/def_validator.py
--rw-rw-rw-   0        0        0     8849 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/hed_validator.py
--rw-rw-rw-   0        0        0     4563 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/onset_validator.py
--rw-rw-rw-   0        0        0    13152 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/sidecar_validator.py
--rw-rw-rw-   0        0        0     5618 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/spreadsheet_validator.py
--rw-rw-rw-   0        0        0    30296 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/tag_validator.py
--rw-rw-rw-   0        0        0     1849 2023-02-14 21:37:41.000000 hedtools-0.3.0/hed/validator/tag_validator_util.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hedtools.egg-info/
--rw-rw-rw-   0        0        0     5981 2023-06-20 20:41:21.000000 hedtools-0.3.0/hedtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9254 2023-06-20 20:41:22.000000 hedtools-0.3.0/hedtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 20:41:21.000000 hedtools-0.3.0/hedtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      216 2023-06-20 20:41:21.000000 hedtools-0.3.0/hedtools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      112 2023-06-20 20:41:21.000000 hedtools-0.3.0/hedtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 20:41:21.000000 hedtools-0.3.0/hedtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2022-06-20 19:04:23.000000 hedtools-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-06-20 20:23:26.000000 hedtools-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0     1350 2023-06-20 20:41:22.000000 hedtools-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      199 2022-06-20 19:04:23.000000 hedtools-0.3.0/setup.py
--rw-rw-rw-   0        0        0    81180 2022-06-20 19:04:23.000000 hedtools-0.3.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/
+-rw-rw-rw-   0        0        0     1113 2023-07-04 17:44:16.000000 hedtools-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       70 2022-06-20 19:04:23.000000 hedtools-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5981 2023-07-04 17:53:08.000000 hedtools-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5337 2023-06-20 20:23:24.000000 hedtools-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/
+-rw-rw-rw-   0        0        0      773 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/errors/
+-rw-rw-rw-   0        0        0      326 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/errors/__init__.py
+-rw-rw-rw-   0        0        0    20119 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/errors/error_messages.py
+-rw-rw-rw-   0        0        0    22248 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/errors/error_reporter.py
+-rw-rw-rw-   0        0        0     5664 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/errors/error_types.py
+-rw-rw-rw-   0        0        0     2162 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/errors/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/models/
+-rw-rw-rw-   0        0        0      711 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/models/__init__.py
+-rw-rw-rw-   0        0        0    20277 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/models/base_input.py
+-rw-rw-rw-   0        0        0    17951 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/models/column_mapper.py
+-rw-rw-rw-   0        0        0     5298 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/models/column_metadata.py
+-rw-rw-rw-   0        0        0     8455 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/models/def_expand_gather.py
+-rw-rw-rw-   0        0        0    13845 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/models/definition_dict.py
+-rw-rw-rw-   0        0        0     3044 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/models/definition_entry.py
+-rw-rw-rw-   0        0        0     6302 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/models/df_util.py
+-rw-rw-rw-   0        0        0    15583 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/models/expression_parser.py
+-rw-rw-rw-   0        0        0    18781 2023-06-20 20:23:24.000000 hedtools-0.3.1/hed/models/hed_group.py
+-rw-rw-rw-   0        0        0    14042 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/models/hed_string.py
+-rw-rw-rw-   0        0        0     4418 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/models/hed_string_group.py
+-rw-rw-rw-   0        0        0    20639 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/models/hed_tag.py
+-rw-rw-rw-   0        0        0      749 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/models/model_constants.py
+-rw-rw-rw-   0        0        0     8942 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/models/sidecar.py
+-rw-rw-rw-   0        0        0     2704 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/models/spreadsheet_input.py
+-rw-rw-rw-   0        0        0     2990 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/models/tabular_input.py
+-rw-rw-rw-   0        0        0      925 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/models/timeseries_input.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/schema/
+-rw-rw-rw-   0        0        0      563 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/__init__.py
+-rw-rw-rw-   0        0        0    19301 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/hed_cache.py
+-rw-rw-rw-   0        0        0    31244 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/schema/hed_schema.py
+-rw-rw-rw-   0        0        0     2104 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/hed_schema_constants.py
+-rw-rw-rw-   0        0        0    10197 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/hed_schema_entry.py
+-rw-rw-rw-   0        0        0     6990 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/hed_schema_group.py
+-rw-rw-rw-   0        0        0     7202 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/hed_schema_io.py
+-rw-rw-rw-   0        0        0     8969 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/hed_schema_section.py
+-rw-rw-rw-   0        0        0     2975 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/schema/schema_attribute_validators.py
+-rw-rw-rw-   0        0        0     5977 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/schema/schema_compliance.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/schema/schema_data/
+-rw-rw-rw-   0        0        0   316118 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/schema/schema_data/HED8.0.0.xml
+-rw-rw-rw-   0        0        0   335759 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/schema/schema_data/HED8.1.0.xml
+-rw-rw-rw-   0        0        0   345995 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/schema_data/HED8.2.0.xml
+-rw-rw-rw-   0        0        0   350310 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/schema/schema_data/HED_score_1.0.0.xml
+-rw-rw-rw-   0        0        0   316637 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/schema/schema_data/HED_testlib_1.0.2.xml
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/schema/schema_io/
+-rw-rw-rw-   0        0        0        0 2022-06-20 19:04:23.000000 hedtools-0.3.1/hed/schema/schema_io/__init__.py
+-rw-rw-rw-   0        0        0     5464 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/schema_io/schema2base.py
+-rw-rw-rw-   0        0        0     5847 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/schema_io/schema2wiki.py
+-rw-rw-rw-   0        0        0     5576 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/schema_io/schema2xml.py
+-rw-rw-rw-   0        0        0     3692 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/schema_io/schema_util.py
+-rw-rw-rw-   0        0        0    24873 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/schema/schema_io/wiki2schema.py
+-rw-rw-rw-   0        0        0      904 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/schema/schema_io/wiki_constants.py
+-rw-rw-rw-   0        0        0    14077 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/schema_io/xml2schema.py
+-rw-rw-rw-   0        0        0     2507 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/schema/schema_io/xml_constants.py
+-rw-rw-rw-   0        0        0     8262 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/schema/schema_validation_util.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/tools/
+-rw-rw-rw-   0        0        0     3090 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/tools/analysis/
+-rw-rw-rw-   0        0        0       29 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/tools/analysis/__init__.py
+-rw-rw-rw-   0        0        0     9402 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/analysis/analysis_util.py
+-rw-rw-rw-   0        0        0    15621 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/tools/analysis/annotation_util.py
+-rw-rw-rw-   0        0        0     1608 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/analysis/column_name_summary.py
+-rw-rw-rw-   0        0        0     5505 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/analysis/event_manager.py
+-rw-rw-rw-   0        0        0     5988 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/tools/analysis/file_dictionary.py
+-rw-rw-rw-   0        0        0     5823 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/analysis/hed_context_manager.py
+-rw-rw-rw-   0        0        0     5717 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/analysis/hed_tag_counts.py
+-rw-rw-rw-   0        0        0     6314 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/analysis/hed_type_counts.py
+-rw-rw-rw-   0        0        0     5573 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/analysis/hed_type_definitions.py
+-rw-rw-rw-   0        0        0     5320 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/analysis/hed_type_factors.py
+-rw-rw-rw-   0        0        0     5257 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/analysis/hed_type_manager.py
+-rw-rw-rw-   0        0        0    12301 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/analysis/hed_type_values.py
+-rw-rw-rw-   0        0        0     9733 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/analysis/key_map.py
+-rw-rw-rw-   0        0        0    11973 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/analysis/tabular_summary.py
+-rw-rw-rw-   0        0        0     1077 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/analysis/temporal_event.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/tools/bids/
+-rw-rw-rw-   0        0        0       42 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/tools/bids/__init__.py
+-rw-rw-rw-   0        0        0     4726 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/bids/bids_dataset.py
+-rw-rw-rw-   0        0        0     3176 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/tools/bids/bids_file.py
+-rw-rw-rw-   0        0        0     9525 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/bids/bids_file_dictionary.py
+-rw-rw-rw-   0        0        0     9280 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/bids/bids_file_group.py
+-rw-rw-rw-   0        0        0     2960 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/tools/bids/bids_sidecar_file.py
+-rw-rw-rw-   0        0        0     8310 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/bids/bids_tabular_dictionary.py
+-rw-rw-rw-   0        0        0     1433 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/tools/bids/bids_tabular_file.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/tools/remodeling/
+-rw-rw-rw-   0        0        0       67 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/tools/remodeling/__init__.py
+-rw-rw-rw-   0        0        0    10544 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/remodeling/backup_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/tools/remodeling/cli/
+-rw-rw-rw-   0        0        0       52 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/tools/remodeling/cli/__init__.py
+-rw-rw-rw-   0        0        0     9165 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/remodeling/cli/run_remodel.py
+-rw-rw-rw-   0        0        0     3738 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/remodeling/cli/run_remodel_backup.py
+-rw-rw-rw-   0        0        0     2188 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/remodeling/cli/run_remodel_restore.py
+-rw-rw-rw-   0        0        0    10276 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/remodeling/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/tools/remodeling/operations/
+-rw-rw-rw-   0        0        0       30 2023-02-14 21:37:40.000000 hedtools-0.3.1/hed/tools/remodeling/operations/__init__.py
+-rw-rw-rw-   0        0        0     3891 2023-06-20 20:23:25.000000 hedtools-0.3.1/hed/tools/remodeling/operations/base_op.py
+-rw-rw-rw-   0        0        0    11167 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/remodeling/operations/base_summary.py
+-rw-rw-rw-   0        0        0     2437 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/convert_columns_op.py
+-rw-rw-rw-   0        0        0     3143 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/factor_column_op.py
+-rw-rw-rw-   0        0        0     4145 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/factor_hed_tags_op.py
+-rw-rw-rw-   0        0        0     3321 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/remodeling/operations/factor_hed_type_op.py
+-rw-rw-rw-   0        0        0     6750 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/merge_consecutive_op.py
+-rw-rw-rw-   0        0        0     4716 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/number_groups_op.py
+-rw-rw-rw-   0        0        0     3568 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/number_rows_op.py
+-rw-rw-rw-   0        0        0     5552 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/remap_columns_op.py
+-rw-rw-rw-   0        0        0     2472 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/remove_columns_op.py
+-rw-rw-rw-   0        0        0     1988 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/remove_rows_op.py
+-rw-rw-rw-   0        0        0     2428 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/rename_columns_op.py
+-rw-rw-rw-   0        0        0     2847 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/reorder_columns_op.py
+-rw-rw-rw-   0        0        0     5360 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/split_rows_op.py
+-rw-rw-rw-   0        0        0     6458 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/remodeling/operations/summarize_column_names_op.py
+-rw-rw-rw-   0        0        0    12571 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/remodeling/operations/summarize_column_values_op.py
+-rw-rw-rw-   0        0        0     8186 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/remodeling/operations/summarize_definitions_op.py
+-rw-rw-rw-   0        0        0     9731 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/remodeling/operations/summarize_hed_tags_op.py
+-rw-rw-rw-   0        0        0    10497 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/remodeling/operations/summarize_hed_type_op.py
+-rw-rw-rw-   0        0        0    11063 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/remodeling/operations/summarize_hed_validation_op.py
+-rw-rw-rw-   0        0        0     7804 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py
+-rw-rw-rw-   0        0        0     2660 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/remodeling/operations/valid_operations.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/tools/util/
+-rw-rw-rw-   0        0        0       44 2022-09-12 19:32:19.000000 hedtools-0.3.1/hed/tools/util/__init__.py
+-rw-rw-rw-   0        0        0    11413 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/util/data_util.py
+-rw-rw-rw-   0        0        0     1546 2023-02-14 21:37:41.000000 hedtools-0.3.1/hed/tools/util/hed_logger.py
+-rw-rw-rw-   0        0        0    11590 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/util/io_util.py
+-rw-rw-rw-   0        0        0     1266 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/tools/util/schema_util.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/tools/visualization/
+-rw-rw-rw-   0        0        0       62 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/visualization/__init__.py
+-rw-rw-rw-   0        0        0     4412 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/visualization/tag_word_cloud.py
+-rw-rw-rw-   0        0        0     3721 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/tools/visualization/word_cloud_util.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hed/validator/
+-rw-rw-rw-   0        0        0      298 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/validator/__init__.py
+-rw-rw-rw-   0        0        0     6347 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/validator/def_validator.py
+-rw-rw-rw-   0        0        0     8849 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/validator/hed_validator.py
+-rw-rw-rw-   0        0        0     4563 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/validator/onset_validator.py
+-rw-rw-rw-   0        0        0    13152 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/validator/sidecar_validator.py
+-rw-rw-rw-   0        0        0     5618 2023-06-20 20:23:26.000000 hedtools-0.3.1/hed/validator/spreadsheet_validator.py
+-rw-rw-rw-   0        0        0    30375 2023-07-04 17:44:16.000000 hedtools-0.3.1/hed/validator/tag_validator.py
+-rw-rw-rw-   0        0        0     1849 2023-02-14 21:37:41.000000 hedtools-0.3.1/hed/validator/tag_validator_util.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:53:08.000000 hedtools-0.3.1/hedtools.egg-info/
+-rw-rw-rw-   0        0        0     5981 2023-07-04 17:53:07.000000 hedtools-0.3.1/hedtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9572 2023-07-04 17:53:07.000000 hedtools-0.3.1/hedtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 17:53:07.000000 hedtools-0.3.1/hedtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      216 2023-07-04 17:53:07.000000 hedtools-0.3.1/hedtools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      112 2023-07-04 17:53:07.000000 hedtools-0.3.1/hedtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-04 17:53:07.000000 hedtools-0.3.1/hedtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2022-06-20 19:04:23.000000 hedtools-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      137 2023-07-04 17:44:16.000000 hedtools-0.3.1/requirements.txt
+-rw-rw-rw-   0        0        0     1350 2023-07-04 17:53:08.000000 hedtools-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      199 2022-06-20 19:04:23.000000 hedtools-0.3.1/setup.py
+-rw-rw-rw-   0        0        0    81180 2022-06-20 19:04:23.000000 hedtools-0.3.1/versioneer.py
```

### Comparing `hedtools-0.3.0/LICENSE` & `hedtools-0.3.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MIT License
+The MIT License (MIT)
 
 Copyright (c) 2020+ HED Standard Working Group
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `hedtools-0.3.0/PKG-INFO` & `hedtools-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedtools
-Version: 0.3.0
+Version: 0.3.1
 Summary: HED validation, summary, and analysis tools.
 Home-page: https://github.com/hed-standard/hed-python/
 Author: VisLab, Ian Callanan, Jeremy Cockfield, Alexander Jones, Owen Winterberg, Kay Robbins
 Author-email: Kay.Robbins@utsa.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hedtools-0.3.0/README.md` & `hedtools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/__init__.py` & `hedtools-0.3.1/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/errors/error_messages.py` & `hedtools-0.3.1/hed/errors/error_messages.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/errors/error_reporter.py` & `hedtools-0.3.1/hed/errors/error_reporter.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/errors/error_types.py` & `hedtools-0.3.1/hed/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/errors/exceptions.py` & `hedtools-0.3.1/hed/errors/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from hed.errors.error_types import ErrorContext
 
 
 class HedExceptions:
+    GENERIC_ERROR = 'GENERIC_ERROR'
     # A list of all exceptions that can be generated by the hedtools.
     FILE_NOT_FOUND = 'fileNotFound'
     BAD_PARAMETERS = 'badParameters'
     CANNOT_PARSE_XML = 'cannotParseXML'
     CANNOT_PARSE_JSON = 'cannotParseJson'
     INVALID_EXTENSION = 'invalidExtension'
 
     INVALID_DATAFRAME = 'INVALID_DATAFRAME'
-
+    INVALID_FILE_FORMAT = 'INVALID_FILE_FORMAT'
     # These are actual schema issues, not that the file cannot be found or parsed
     SCHEMA_HEADER_MISSING = 'HED_SCHEMA_HEADER_INVALID'
     HED_SCHEMA_HEADER_INVALID = 'HED_SCHEMA_HEADER_INVALID'
 
     SCHEMA_LIBRARY_INVALID = "SCHEMA_LIBRARY_INVALID"
     BAD_HED_LIBRARY_NAME = 'SCHEMA_LIBRARY_INVALID'
     BAD_WITH_STANDARD = "SCHEMA_LIBRARY_INVALID"
```

### Comparing `hedtools-0.3.0/hed/models/__init__.py` & `hedtools-0.3.1/hed/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/base_input.py` & `hedtools-0.3.1/hed/models/base_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,20 +39,18 @@
             allow_blank_names(bool): If True, column names can be blank
 
         :raises HedFileError:
             - file is blank
             - An invalid dataframe was passed with size 0
             - An invalid extension was provided
             - A duplicate or empty column name appears
-
-        :raises OSError:
             - Cannot open the indicated file
-
-        :raises KeyError:
             - The specified worksheet name does not exist
+            - If the sidecar file or tabular file had invalid format and could not be read.
+
          """
         if mapper is None:
             mapper = ColumnMapper()
         self._mapper = mapper
         self._has_column_names = has_column_names
         self._name = name
         # This is the loaded workbook if we loaded originally from an Excel file.
@@ -73,32 +71,38 @@
 
         if isinstance(file, pandas.DataFrame):
             self._dataframe = file
             self._has_column_names = self._dataframe_has_names(self._dataframe)
         elif not file:
             raise HedFileError(HedExceptions.FILE_NOT_FOUND, "Empty file passed to BaseInput.", file)
         elif input_type in self.TEXT_EXTENSION:
-            self._dataframe = pandas.read_csv(file, delimiter='\t', header=pandas_header,
-                                              dtype=str, keep_default_na=True, na_values=None)
+            try:
+                self._dataframe = pandas.read_csv(file, delimiter='\t', header=pandas_header,
+                                                  dtype=str, keep_default_na=True, na_values=None)
+            except Exception as e:
+                raise HedFileError(HedExceptions.INVALID_FILE_FORMAT, str(e), self.name) from e
             # Convert nan values to a known value
             self._dataframe = self._dataframe.fillna("n/a")
         elif input_type in self.EXCEL_EXTENSION:
-            self._loaded_workbook = openpyxl.load_workbook(file)
-            loaded_worksheet = self.get_worksheet(self._worksheet_name)
-            self._dataframe = self._get_dataframe_from_worksheet(loaded_worksheet, has_column_names)
+            try:
+                self._loaded_workbook = openpyxl.load_workbook(file)
+                loaded_worksheet = self.get_worksheet(self._worksheet_name)
+                self._dataframe = self._get_dataframe_from_worksheet(loaded_worksheet, has_column_names)
+            except Exception as e:
+                raise HedFileError(HedExceptions.GENERIC_ERROR, str(e), self.name) from e
         else:
             raise HedFileError(HedExceptions.INVALID_EXTENSION, "", file)
 
         if self._dataframe.size == 0:
             raise HedFileError(HedExceptions.INVALID_DATAFRAME, "Invalid dataframe(malformed datafile, etc)", file)
 
         # todo: Can we get rid of this behavior now that we're using pandas?
         column_issues = ColumnMapper.check_for_blank_names(self.columns, allow_blank_names=allow_blank_names)
         if column_issues:
-            raise HedFileError(HedExceptions.BAD_COLUMN_NAMES, "Duplicate or blank columns found.  See issues.",
+            raise HedFileError(HedExceptions.BAD_COLUMN_NAMES, "Duplicate or blank columns found. See issues.",
                                self.name, issues=column_issues)
 
         self.reset_mapper(mapper)
 
     def reset_mapper(self, new_mapper):
         """ Set mapper to a different view of the file.
 
@@ -281,15 +285,15 @@
             row_number (int):    The row number of the spreadsheet to set.
             column_number (int): The column number of the spreadsheet to set.
             new_string_obj (HedString): Object with text to put in the given cell.
             tag_form (str): Version of the tags (short_tag, long_tag, base_tag, etc)
 
         Notes:
              Any attribute of a HedTag that returns a string is a valid value of tag_form.
-             
+
         :raises ValueError:
             - There is not a loaded dataframe
 
         :raises KeyError:
             - the indicated row/column does not exist
 
         :raises AttributeError:
```

### Comparing `hedtools-0.3.0/hed/models/column_mapper.py` & `hedtools-0.3.1/hed/models/column_mapper.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/column_metadata.py` & `hedtools-0.3.1/hed/models/column_metadata.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/def_expand_gather.py` & `hedtools-0.3.1/hed/models/def_expand_gather.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/definition_dict.py` & `hedtools-0.3.1/hed/models/definition_dict.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/definition_entry.py` & `hedtools-0.3.1/hed/models/definition_entry.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/df_util.py` & `hedtools-0.3.1/hed/models/df_util.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/expression_parser.py` & `hedtools-0.3.1/hed/models/expression_parser.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/hed_group.py` & `hedtools-0.3.1/hed/models/hed_group.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/hed_string.py` & `hedtools-0.3.1/hed/models/hed_string.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/hed_string_group.py` & `hedtools-0.3.1/hed/models/hed_string_group.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/hed_tag.py` & `hedtools-0.3.1/hed/models/hed_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -598,18 +598,22 @@
                 return units, value
 
         return None, None
 
     @staticmethod
     def _find_modifier_unit_entry(units, all_valid_unit_permutations):
         possible_match = all_valid_unit_permutations.get(units)
-        if not possible_match or not possible_match.has_attribute(HedKey.UnitSymbol):
-            possible_match = all_valid_unit_permutations.get(units.lower())
-            if possible_match and possible_match.has_attribute(HedKey.UnitSymbol):
-                possible_match = None
+        # If we have a match that's a unit symbol, we're done, return it.
+        if possible_match and possible_match.has_attribute(HedKey.UnitSymbol):
+            return possible_match
+
+        possible_match = all_valid_unit_permutations.get(units.lower())
+        # Unit symbols must match including case, a match of a unit symbol now is something like M becoming m.
+        if possible_match and possible_match.has_attribute(HedKey.UnitSymbol):
+            possible_match = None
 
         return possible_match
 
     def is_placeholder(self):
         if "#" in self.org_tag or "#" in self._extension_value:
             return True
         return False
```

### Comparing `hedtools-0.3.0/hed/models/model_constants.py` & `hedtools-0.3.1/hed/models/model_constants.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/sidecar.py` & `hedtools-0.3.1/hed/models/sidecar.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,23 +123,21 @@
         :raises HedFileError:
             - If the file was not found or could not be parsed into JSON.
             
         """
         if not file:
             return {}
         elif isinstance(file, str):
+            if not self.name:
+                self.name = file
             try:
                 with open(file, "r") as fp:
-                    if not self.name:
-                        self.name = file
                     return self._load_json_file(fp)
-            except FileNotFoundError as e:
-                raise HedFileError(HedExceptions.FILE_NOT_FOUND, e.strerror, file)
-            except TypeError as e:
-                raise HedFileError(HedExceptions.FILE_NOT_FOUND, str(e), file)
+            except OSError as e:
+                raise HedFileError(HedExceptions.FILE_NOT_FOUND, e.strerror, file) from e
         else:
             return self._load_json_file(file)
 
     def load_sidecar_files(self, files):
         """ Load json from a given file or list
 
         Parameters:
@@ -185,20 +183,19 @@
         """ Load the raw json of a given file
 
         Parameters:
             fp (File-like): The JSON source stream.
 
         :raises HedFileError:
             - If the file cannot be parsed.
-            
         """
         try:
             return json.load(fp)
-        except json.decoder.JSONDecodeError as e:
-            raise HedFileError(HedExceptions.CANNOT_PARSE_JSON, str(e), self.name)
+        except (json.decoder.JSONDecodeError, AttributeError) as e:
+            raise HedFileError(HedExceptions.CANNOT_PARSE_JSON, str(e), self.name) from e
 
     def extract_definitions(self, hed_schema=None, error_handler=None):
         """ Gather and validate definitions in metadata.
 
         Parameters:
             hed_schema (HedSchema or None): The schema to used to identify tags.
             error_handler (ErrorHandler or None): The error handler to use for context, uses a default one if None.
```

### Comparing `hedtools-0.3.0/hed/models/spreadsheet_input.py` & `hedtools-0.3.1/hed/models/spreadsheet_input.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/models/tabular_input.py` & `hedtools-0.3.1/hed/models/tabular_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     HED_COLUMN_NAME = "HED"
 
     def __init__(self, file=None, sidecar=None, name=None):
 
         """ Constructor for the TabularInput class.
 
         Parameters:
-            file (str or file like): A tsv file to open.
-            sidecar (str or Sidecar): A Sidecar filename or Sidecar
+            file (str or FileLike): A tsv file to open.
+            sidecar (str or Sidecar or FileLike): A Sidecar or source file/filename.
             name (str): The name to display for this file for error purposes.
 
         :raises HedFileError:
             - file is blank
             - An invalid dataframe was passed with size 0
             - An invalid extension was provided
             - A duplicate or empty column name appears
```

### Comparing `hedtools-0.3.0/hed/models/timeseries_input.py` & `hedtools-0.3.1/hed/models/timeseries_input.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/__init__.py` & `hedtools-0.3.1/hed/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/hed_cache.py` & `hedtools-0.3.1/hed/schema/hed_cache.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/hed_schema.py` & `hedtools-0.3.1/hed/schema/hed_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -505,31 +505,47 @@
         Notes:
             Works left to right (which is mostly relevant for errors).
 
         """
         clean_tag = str(tag)
         namespace = schema_namespace
         clean_tag = clean_tag[len(namespace):]
-        prefix_tag_adj = len(namespace)
         working_tag = clean_tag.lower()
 
         # Most tags are in the schema directly, so test that first
         found_entry = self._get_tag_entry(working_tag)
         if found_entry:
             # this handles the one special case where the actual tag contains "/#" instead of something specific.
             if working_tag.endswith("/#"):
                 remainder = working_tag[-2:]
             else:
                 remainder = ""
 
             return found_entry, remainder, []
 
+        prefix_tag_adj = len(namespace)
+
+        try:
+            found_entry, current_slash_index = self._find_tag_subfunction(tag, working_tag, prefix_tag_adj)
+        except self._TagIdentifyError as e:
+            issue = e.issue
+            return None, None, issue
+
+        remainder = None
+        if current_slash_index != -1:
+            remainder = clean_tag[current_slash_index:]
+        if remainder and found_entry.takes_value_child_entry:
+            found_entry = found_entry.takes_value_child_entry
+
+        return found_entry, remainder, []
+
+    def _find_tag_subfunction(self, tag, working_tag, prefix_tag_adj):
+        """Finds the base tag and remainder from the left, raising exception on issues"""
         current_slash_index = -1
         current_entry = None
-
         # Loop left to right, checking each word.  Once we find an invalid word, we stop.
         while True:
             next_index = working_tag.find("/", current_slash_index + 1)
             if next_index == -1:
                 next_index = len(working_tag)
             parent_name = working_tag[:next_index]
             parent_entry = self._get_tag_entry(parent_name)
@@ -537,44 +553,45 @@
             if not parent_entry:
                 # We haven't found any tag at all yet
                 if current_entry is None:
                     error = ErrorHandler.format_error(ValidationErrors.NO_VALID_TAG_FOUND,
                                                       tag,
                                                       index_in_tag=prefix_tag_adj,
                                                       index_in_tag_end=prefix_tag_adj + next_index)
-                    return None, None, error
+                    raise self._TagIdentifyError(error)
                 # If this is not a takes value node, validate each term in the remainder.
                 if not current_entry.takes_value_child_entry:
-                    child_names = working_tag[current_slash_index + 1:].split("/")
-                    word_start_index = current_slash_index + 1 + prefix_tag_adj
-                    for name in child_names:
-                        if self._get_tag_entry(name):
-                            error = ErrorHandler.format_error(ValidationErrors.INVALID_PARENT_NODE,
-                                                              tag,
-                                                              index_in_tag=word_start_index,
-                                                              index_in_tag_end=word_start_index + len(name),
-                                                              expected_parent_tag=self.all_tags[name].name)
-                            return None, None, error
-                        word_start_index += len(name) + 1
+                    # This will raise _TagIdentifyError on any issues
+                    self._validate_remaining_terms(tag, working_tag, prefix_tag_adj, current_slash_index)
                 break
 
             current_entry = parent_entry
             current_slash_index = next_index
             if next_index == len(working_tag):
                 break
-            continue
 
-        remainder = None
-        if current_slash_index != -1:
-            remainder = clean_tag[current_slash_index:]
-        if remainder and current_entry.takes_value_child_entry:
-            current_entry = current_entry.takes_value_child_entry
-        found_entry = current_entry
+        return current_entry, current_slash_index
 
-        return found_entry, remainder, []
+    def _validate_remaining_terms(self, tag, working_tag, prefix_tag_adj, current_slash_index):
+        """ Validates the terms past current_slash_index.
+        
+        :raises _TagIdentifyError:
+            - One of the extension terms already exists as a schema term.
+        """
+        child_names = working_tag[current_slash_index + 1:].split("/")
+        word_start_index = current_slash_index + 1 + prefix_tag_adj
+        for name in child_names:
+            if self._get_tag_entry(name):
+                error = ErrorHandler.format_error(ValidationErrors.INVALID_PARENT_NODE,
+                                                  tag,
+                                                  index_in_tag=word_start_index,
+                                                  index_in_tag_end=word_start_index + len(name),
+                                                  expected_parent_tag=self.all_tags[name].name)
+                raise self._TagIdentifyError(error)
+            word_start_index += len(name) + 1
 
     # ===============================================
     # Semi-private creation finalizing functions
     # ===============================================
     def finalize_dictionaries(self):
         """ Call to finish loading. """
         self._is_hed3_schema = self.is_hed3_schema
@@ -797,7 +814,12 @@
 
         section = self._sections[key_class]
         return section._add_to_dict(long_tag_name, new_entry)
 
     def _create_tag_entry(self, long_tag_name, key_class):
         section = self._sections[key_class]
         return section._create_tag_entry(long_tag_name)
+
+    class _TagIdentifyError(Exception):
+        """Used internally to note when a tag cannot be identified."""
+        def __init__(self, issue):
+            self.issue = issue
```

### Comparing `hedtools-0.3.0/hed/schema/hed_schema_constants.py` & `hedtools-0.3.1/hed/schema/hed_schema_constants.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/hed_schema_entry.py` & `hedtools-0.3.1/hed/schema/hed_schema_entry.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/hed_schema_group.py` & `hedtools-0.3.1/hed/schema/hed_schema_group.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/hed_schema_io.py` & `hedtools-0.3.1/hed/schema/hed_schema_io.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/hed_schema_section.py` & `hedtools-0.3.1/hed/schema/hed_schema_section.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_compliance.py` & `hedtools-0.3.1/hed/schema/schema_validation_util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,173 +1,177 @@
-""" Utilities for HED schema checking. """
+"""Utilities used in HED validation/loading using a HED schema."""
+from semantic_version import Version
 
-from hed.errors import error_reporter
-from hed.errors.error_types import SchemaWarnings, ErrorContext, SchemaErrors, ErrorSeverity, ValidationErrors
-from hed.errors.error_reporter import ErrorHandler
-from hed.schema.hed_schema import HedSchema, HedKey
+from hed.errors import ErrorHandler, SchemaWarnings
+from hed.schema import hed_schema_constants as constants
+from hed.errors.exceptions import HedExceptions, HedFileError
 
 ALLOWED_TAG_CHARS = "-"
 ALLOWED_DESC_CHARS = "-_:;,./()+ ^"
 
 
-def check_compliance(hed_schema, check_for_warnings=True, name=None, error_handler=None):
-    """ Check for hed3 compliance of a schema object.
+def validate_library_name(library_name):
+    """ Check the validity of the library name.
 
     Parameters:
-        hed_schema (HedSchema): HedSchema object to check for hed3 compliance.
-        check_for_warnings (bool): If True, check for formatting issues like invalid characters, capitalization, etc.
-        name (str): If present, will use as filename for context.
-        error_handler (ErrorHandler or None): Used to report errors. Uses a default one if none passed in.
+        library_name (str): Name of the library.
 
     Returns:
-        list: A list of all warnings and errors found in the file. Each issue is a dictionary.
+        bool or str:  If not False, string indicates the issue.
 
-    :raises ValueError:
-        - Trying to validate a HedSchemaGroup directly
     """
-    if not isinstance(hed_schema, HedSchema):
-        raise ValueError("To check compliance of a HedGroupSchema, call self.check_compliance on the schema itself.")
+    for i, character in enumerate(library_name):
+        if not character.isalpha():
+            return f"Non alpha character '{character}' at position {i} in '{library_name}'"
+        if character.isupper():
+            return f"Non lowercase character '{character}' at position {i} in '{library_name}'"
 
-    if error_handler is None:
-        error_handler = error_reporter.ErrorHandler()
-    issues_list = []
-
-    if not name:
-        name = hed_schema.filename
-    error_handler.push_error_context(ErrorContext.FILE_NAME, name)
-
-    unknown_attributes = hed_schema.get_unknown_attributes()
-    if unknown_attributes:
-        for attribute_name, source_tags in unknown_attributes.items():
-            for tag in source_tags:
-                issues_list += error_handler.format_error_with_context(SchemaErrors.SCHEMA_ATTRIBUTE_INVALID,
-                                                                       attribute_name,
-                                                                       source_tag=tag)
-
-    schema_attribute_validators = {
-        HedKey.SuggestedTag: tag_exists_check,
-        HedKey.RelatedTag: tag_exists_check,
-        HedKey.UnitClass: tag_is_placeholder_check,
-        HedKey.ValueClass: tag_is_placeholder_check,
-        HedKey.Rooted: tag_exists_base_schema_check,
-    }
 
-    # Check attributes
-    for section_key in hed_schema._sections:
-        error_handler.push_error_context(ErrorContext.SCHEMA_SECTION, section_key)
-        # Check attributes
-        for tag_entry in hed_schema[section_key].values():
-            error_handler.push_error_context(ErrorContext.SCHEMA_TAG, tag_entry.name)
-            for attribute_name in tag_entry.attributes:
-                validator = schema_attribute_validators.get(attribute_name)
-                if validator:
-                    error_handler.push_error_context(ErrorContext.SCHEMA_ATTRIBUTE, attribute_name)
-                    new_issues = validator(hed_schema, tag_entry, attribute_name)
-                    # if force_issues_as_warnings:
-                    for issue in new_issues:
-                        issue['severity'] = ErrorSeverity.WARNING
-                    error_handler.add_context_and_filter(new_issues)
-                    issues_list += new_issues
-                    error_handler.pop_error_context()
-            error_handler.pop_error_context()
-
-        # Check duplicate names
-        for name, duplicate_entries in hed_schema[section_key].duplicate_names.items():
-            values = set(entry.has_attribute(HedKey.InLibrary) for entry in duplicate_entries)
-            error_code = SchemaErrors.HED_SCHEMA_DUPLICATE_NODE
-            if len(values) == 2:
-                error_code = SchemaErrors.HED_SCHEMA_DUPLICATE_FROM_LIBRARY
-            issues_list += error_handler.format_error_with_context(error_code, name,
-                                                                   duplicate_tag_list=[entry.name for entry in duplicate_entries],
-                                                                   section=section_key)
-
-        error_handler.pop_error_context()
-
-    if check_for_warnings:
-        hed_terms = hed_schema.get_all_schema_tags(True)
-        for hed_term in hed_terms:
-            issues_list += validate_schema_term(hed_term)
-
-        for tag_name, desc in hed_schema.get_desc_iter():
-            issues_list += validate_schema_description(tag_name, desc)
-
-    error_handler.pop_error_context()
-    return issues_list
-
-# attribute_checker_template(hed_schema, tag_entry, attribute_name, possible_values):
-#     hed_schema (HedSchema): The schema to use for validation
-#     tag_entry (HedSchemaEntry): The schema entry for this tag.
-#     attribute_name (str): The name of this attribute
-
-
-def tag_is_placeholder_check(hed_schema, tag_entry, attribute_name):
-    """ Check if comma separated list has valid HedTags.
-
-    Parameters:
-        hed_schema (HedSchema): The schema to use for validation
-        tag_entry (HedSchemaEntry): The schema entry for this tag.
-        attribute_name (str): The name of this attribute
+def validate_version_string(version_string):
+    """ Check validity of the version.
+
+    Parameters:
+        version_string (str):  A version string.
 
     Returns:
-        list: A list of issues. Each issue is a dictionary.
+        bool or str:  If not False, string indicates the issue.
 
     """
-    issues = []
-    if not tag_entry.name.endswith("/#"):
-        issues += ErrorHandler.format_error(SchemaWarnings.NON_PLACEHOLDER_HAS_CLASS, tag_entry.name,
-                                            attribute_name)
+    try:
+        Version(version_string)
+    except ValueError as e:
+        return str(e)
+    return False
 
-    return issues
 
+def is_hed3_version_number(version_string):
+    """ Check validity of the version.
 
-def tag_exists_check(hed_schema, tag_entry, attribute_name):
-    """ Check if the list of possible tags exists in the schema.
+    Parameters:
+        version_string (str):  A version string.
+
+    Returns:
+        bool:  If True the version corresponds to a HED3 schema.
+
+    """
+    try:
+        version = Version(version_string)
+        if version.major >= 8:
+            return True
+    except ValueError:
+        return False
+    return False
+
+
+header_attribute_validators = {
+        constants.VERSION_ATTRIBUTE: (validate_version_string, HedExceptions.HED_SCHEMA_VERSION_INVALID),
+        constants.LIBRARY_ATTRIBUTE: (validate_library_name, HedExceptions.BAD_HED_LIBRARY_NAME)
+    }
+
+
+def validate_present_attributes(attrib_dict, filename):
+    """ Validate combinations of attributes
+
+        Parameters:
+            attrib_dict (dict): Dictionary of attributes to be evaluated.
+            filename (str):  File name to use in reporting errors.
+
+        Returns:
+            list: List of issues. Each issue is a dictionary.
+
+        :raises  HedFileError:
+            - withStandard is found in th header, but a library attribute is not specified
+        """
+    if constants.WITH_STANDARD_ATTRIBUTE in attrib_dict and constants.LIBRARY_ATTRIBUTE not in attrib_dict:
+        raise HedFileError(HedExceptions.BAD_WITH_STANDARD,
+                           "withStandard header attribute found, but no library attribute is present",
+                           filename)
+
+
+def validate_attributes(attrib_dict, filename):
+    """ Validate attributes in the dictionary.
 
     Parameters:
-        hed_schema (HedSchema): The schema to use for validation
-        tag_entry (HedSchemaEntry): The schema entry for this tag.
-        attribute_name (str): The name of this attribute
+        attrib_dict (dict): Dictionary of attributes to be evaluated.
+        filename (str):  File name to use in reporting errors.
 
     Returns:
-        list: A list of issues. Each issue is a dictionary.
+        list: List of issues. Each issue is a dictionary.
 
+    :raises  HedFileError:
+        - Invalid library name
+        - Version not present
+        - Invalid combinations of attributes in header
     """
-    issues = []
-    possible_tags = tag_entry.attributes.get(attribute_name, "")
-    split_tags = possible_tags.split(",")
-    for org_tag in split_tags:
-        if org_tag and org_tag not in hed_schema.all_tags:
-            issues += ErrorHandler.format_error(ValidationErrors.NO_VALID_TAG_FOUND,
-                                                org_tag,
-                                                index_in_tag=0,
-                                                index_in_tag_end=len(org_tag))
-
-    return issues
-
-
-def tag_exists_base_schema_check(hed_schema, tag_entry, attribute_name):
-    """ Check if the single tag is a partnered schema tag
-
-    Parameters:
-        hed_schema (HedSchema): The schema to use for validation
-        tag_entry (HedSchemaEntry): The schema entry for this tag.
-        attribute_name (str): The name of this attribute
+    validate_present_attributes(attrib_dict, filename)
+
+    for attribute_name, attribute_value in attrib_dict.items():
+        if attribute_name in header_attribute_validators:
+            validator, error_code = header_attribute_validators[attribute_name]
+            had_error = validator(attribute_value)
+            if had_error:
+                raise HedFileError(error_code, had_error, filename)
+
+    if constants.VERSION_ATTRIBUTE not in attrib_dict:
+        raise HedFileError(HedExceptions.HED_SCHEMA_VERSION_INVALID,
+                           "No version attribute found in header", filename=filename)
+
+
+# Might move this to a baseclass version if one is ever made for wiki2schema/xml2schema
+def find_rooted_entry(tag_entry, schema, loading_merged):
+    """ This semi-validates rooted tags, raising an exception on major errors
+
+    Parameters:
+        tag_entry(HedTagEntry): the possibly rooted tag
+        schema(HedSchema): The schema being loaded
+        loading_merged(bool): If this schema was already merged before loading
 
     Returns:
-        list: A list of issues. Each issue is a dictionary.
+        rooted_tag(HedTagEntry or None): The base tag entry from the standard schema
+            Returns None if this tag isn't rooted
+
+    :raises HedFileError:
+        - A rooted attribute is found in a non-paired schema
+        - A rooted attribute is not a string
+        - A rooted attribute was found on a non-root node in an unmerged schema.
+        - A rooted attribute is found on a root node in a merged schema.
+        - A rooted attribute indicates a tag that doesn't exist in the base schema.
     """
-    issues = []
-    rooted_tag = tag_entry.attributes.get(attribute_name, "")
-    if rooted_tag and rooted_tag not in hed_schema.all_tags:
-        issues += ErrorHandler.format_error(ValidationErrors.NO_VALID_TAG_FOUND,
-                                            rooted_tag,
-                                            index_in_tag=0,
-                                            index_in_tag_end=len(rooted_tag))
+    rooted_tag = tag_entry.has_attribute(constants.HedKey.Rooted, return_value=True)
+    if rooted_tag is not None:
+        if not schema.with_standard:
+            raise HedFileError(HedExceptions.ROOTED_TAG_INVALID,
+                               f"Rooted tag attribute found on '{tag_entry.short_tag_name}' in a standard schema.",
+                               schema.filename)
+
+        if not isinstance(rooted_tag, str):
+            raise HedFileError(HedExceptions.ROOTED_TAG_INVALID,
+                               f'Rooted tag \'{tag_entry.short_tag_name}\' is not a string."',
+                               schema.filename)
+
+        if tag_entry.parent_name and not loading_merged:
+            raise HedFileError(HedExceptions.ROOTED_TAG_INVALID,
+                               f'Found rooted tag \'{tag_entry.short_tag_name}\' as a non root node.',
+                               schema.filename)
+
+        if not tag_entry.parent_name and loading_merged:
+            raise HedFileError(HedExceptions.ROOTED_TAG_INVALID,
+                               f'Found rooted tag \'{tag_entry.short_tag_name}\' as a root node in a merged schema.',
+                               schema.filename)
+
+        rooted_entry = schema.all_tags.get(rooted_tag)
+        if not rooted_entry or rooted_entry.has_attribute(constants.HedKey.InLibrary):
+            raise HedFileError(HedExceptions.ROOTED_TAG_DOES_NOT_EXIST,
+                               f"Rooted tag '{tag_entry.short_tag_name}' not found in paired standard schema",
+                               schema.filename)
+
+        if loading_merged:
+            return None
 
-    return issues
+        return rooted_entry
 
 
 def validate_schema_term(hed_term):
     """ Check short tag for capitalization and illegal characters.
 
     Parameters:
         hed_term (str): A single hed term.
```

### Comparing `hedtools-0.3.0/hed/schema/schema_data/HED8.0.0.xml` & `hedtools-0.3.1/hed/schema/schema_data/HED8.0.0.xml`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_data/HED8.1.0.xml` & `hedtools-0.3.1/hed/schema/schema_data/HED8.1.0.xml`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_data/HED8.2.0.xml` & `hedtools-0.3.1/hed/schema/schema_data/HED8.2.0.xml`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_data/HED_score_1.0.0.xml` & `hedtools-0.3.1/hed/schema/schema_data/HED_score_1.0.0.xml`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_data/HED_testlib_1.0.2.xml` & `hedtools-0.3.1/hed/schema/schema_data/HED_testlib_1.0.2.xml`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_io/schema2base.py` & `hedtools-0.3.1/hed/schema/schema_io/schema2base.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_io/schema2wiki.py` & `hedtools-0.3.1/hed/schema/schema_io/schema2wiki.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_io/schema2xml.py` & `hedtools-0.3.1/hed/schema/schema_io/schema2xml.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_io/schema_util.py` & `hedtools-0.3.1/hed/schema/schema_io/schema_util.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_io/wiki2schema.py` & `hedtools-0.3.1/hed/schema/schema_io/wiki2schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,63 +151,68 @@
             if section not in wiki_lines_by_section:
                 error_code = HedExceptions.INVALID_SECTION_SEPARATOR
                 if section in ErrorsBySection:
                     error_code = ErrorsBySection[section]
                 msg = f"Required section separator '{SectionNames[section]}' not found in file"
                 raise HedFileError(error_code, msg, filename=self.filename)
 
+    def _check_for_new_section(self, line, strings_for_section, current_section):
+        new_section = None
+        for key, section_string in SectionStarts.items():
+            if line.startswith(section_string):
+                if key in strings_for_section:
+                    msg = f"Found section {SectionNames[key]} twice"
+                    raise HedFileError(HedExceptions.INVALID_SECTION_SEPARATOR,
+                                       msg, filename=self.filename)
+                if current_section < key:
+                    new_section = key
+                else:
+                    error_code = HedExceptions.INVALID_SECTION_SEPARATOR
+                    if key in ErrorsBySection:
+                        error_code = ErrorsBySection[key]
+                    msg = f"Found section {SectionNames[key]} out of order in file"
+                    raise HedFileError(error_code, msg, filename=self.filename)
+                break
+        return new_section
+
+    def _handle_bad_section_sep(self, line, current_section):
+        if current_section != HedWikiSection.Schema and line.startswith(wiki_constants.ROOT_TAG):
+            msg = f"Invalid section separator '{line.strip()}'"
+            raise HedFileError(HedExceptions.INVALID_SECTION_SEPARATOR, msg, filename=self.filename)
+
+        if line.startswith("!#"):
+            msg = f"Invalid section separator '{line.strip()}'"
+            raise HedFileError(HedExceptions.INVALID_SECTION_SEPARATOR, msg, filename=self.filename)
+
     def _split_lines_into_sections(self, wiki_lines):
-        """
-            Takes a list of lines, and splits it into valid wiki sections.
+        """ Takes a list of lines, and splits it into valid wiki sections.
+
+        Parameters:
+           wiki_lines : [str]
 
-        Parameters
-        ----------
-        wiki_lines : [str]
-
-        Returns
-        -------
-        sections: {str: [str]}
+        Returns:
+            sections: {str: [str]}
             A list of lines for each section of the schema(not including the identifying section line)
         """
-        # We start having found the header and may still be in it
         current_section = HedWikiSection.HeaderLine
-        found_section = True
         strings_for_section = {}
+        strings_for_section[HedWikiSection.HeaderLine] = []
         for line_number, line in enumerate(wiki_lines):
-            for key, section_string in SectionStarts.items():
-                if line.startswith(section_string):
-                    if key in strings_for_section:
-                        msg = f"Found section {SectionNames[key]} twice"
-                        raise HedFileError(HedExceptions.INVALID_SECTION_SEPARATOR,
-                                           msg, filename=self.filename)
-
-                    if current_section < key:
-                        current_section = key
-                        found_section = True
-                        break
-                    else:
-                        error_code = HedExceptions.INVALID_SECTION_SEPARATOR
-                        if key in ErrorsBySection:
-                            error_code = ErrorsBySection[key]
-                        msg = f"Found section {SectionNames[key]} out of order in file"
-                        raise HedFileError(error_code, msg, filename=self.filename)
-
-            if found_section:
-                strings_for_section[current_section] = []
-                found_section = False
+            # Header is handled earlier
+            if line_number == 0:
+                continue
+
+            new_section = self._check_for_new_section(line, strings_for_section, current_section)
+
+            if new_section:
+                strings_for_section[new_section] = []
+                current_section = new_section
                 continue
 
-            if (current_section != HedWikiSection.Schema and line.startswith(wiki_constants.ROOT_TAG) and
-                    not (line.startswith(wiki_constants.OLD_SYNTAX_SECTION_NAME) and not self._schema.is_hed3_schema)):
-                msg = f"Invalid section separator '{line.strip()}'"
-                raise HedFileError(HedExceptions.INVALID_SECTION_SEPARATOR, msg, filename=self.filename)
-
-            if line.startswith("!#"):
-                msg = f"Invalid section separator '{line.strip()}'"
-                raise HedFileError(HedExceptions.INVALID_SECTION_SEPARATOR, msg, filename=self.filename)
+            self._handle_bad_section_sep(line, current_section)
 
             if current_section == HedWikiSection.Prologue or current_section == HedWikiSection.Epilogue:
                 strings_for_section[current_section].append((line_number + 1, line))
             else:
                 line = self._remove_nowiki_tag_from_line(line_number + 1, line.strip())
                 if line:
                     strings_for_section[current_section].append((line_number + 1, line))
```

### Comparing `hedtools-0.3.0/hed/schema/schema_io/wiki_constants.py` & `hedtools-0.3.1/hed/schema/schema_io/wiki_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 UNIT_CLASS_STRING = "'''Unit classes'''"
 UNIT_MODIFIER_STRING = "'''Unit modifiers'''"
 ATTRIBUTE_DEFINITION_STRING = "'''Schema attributes'''"
 ATTRIBUTE_PROPERTY_STRING = "'''Properties'''"
 VALUE_CLASS_STRING = "'''Value classes'''"
 PROLOGUE_SECTION_ELEMENT = "'''Prologue'''"
 EPILOGUE_SECTION_ELEMENT = "'''Epilogue'''"
-OLD_SYNTAX_SECTION_NAME = "'''Syntax'''"
 
 wiki_section_headers = {
     HedSectionKey.AllTags: START_HED_STRING,
     HedSectionKey.UnitClasses: UNIT_CLASS_STRING,
     HedSectionKey.Units: None,
     HedSectionKey.UnitModifiers: UNIT_MODIFIER_STRING,
     HedSectionKey.ValueClasses: VALUE_CLASS_STRING,
```

### Comparing `hedtools-0.3.0/hed/schema/schema_io/xml2schema.py` & `hedtools-0.3.1/hed/schema/schema_io/xml2schema.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/schema/schema_io/xml_constants.py` & `hedtools-0.3.1/hed/schema/schema_io/xml_constants.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/__init__.py` & `hedtools-0.3.1/hed/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/analysis/analysis_util.py` & `hedtools-0.3.1/hed/tools/analysis/analysis_util.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/analysis/annotation_util.py` & `hedtools-0.3.1/hed/tools/analysis/annotation_util.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/analysis/event_manager.py` & `hedtools-0.3.1/hed/tools/analysis/event_manager.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/analysis/file_dictionary.py` & `hedtools-0.3.1/hed/tools/analysis/file_dictionary.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/analysis/hed_context_manager.py` & `hedtools-0.3.1/hed/tools/analysis/hed_context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ Manages context and events of temporal extent. """
 
 from hed.errors.exceptions import HedFileError
 from hed.models import HedGroup, HedString
 from hed.schema import HedSchema, HedSchemaGroup
 from hed.tools.analysis.analysis_util import hed_to_str
 
-#TODO: [Refactor] clean up distinction between hed as strings versus objects -- maybe replace by event manager.
+# TODO: [Refactor] clean up distinction between hed as strings versus objects -- maybe replace by event manager.
+# TODO: Implement insets
 
 class OnsetGroup:
     def __init__(self, name, contents, start_index, end_index=None):
         self.name = name
         self.start_index = start_index
         self.end_index = end_index
         self.contents = hed_to_str(contents, remove_parentheses=True)
```

### Comparing `hedtools-0.3.0/hed/tools/analysis/hed_tag_counts.py` & `hedtools-0.3.1/hed/tools/analysis/hed_tag_counts.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,19 +17,19 @@
         self.tag_terms = hed_tag.tag_terms
         self.events = 1
         self.files = {file_name: ''}
         self.value_dict = {}
         self.set_value(hed_tag)
 
     def set_value(self, hed_tag):
-        """ Update the tag term value counts for a HedTag. 
-        
+        """ Update the tag term value counts for a HedTag.
+
         Parameters:
-            hed_tag (HedTag or None):  Item to use to update the value counts. 
-        
+            hed_tag (HedTag or None):  Item to use to update the value counts.
+
         """
         if not hed_tag:
             return
         value = hed_tag.extension
         if not value:
             value = None
         if value in self.value_dict:
@@ -39,56 +39,55 @@
 
     def get_info(self, verbose=False):
         if verbose:
             files = [name for name in self.files]
         else:
             files = len(self.files)
         return {'tag': self.tag, 'events': self.events, 'files': files}
-    
+
     def get_summary(self):
         """ Return a dictionary summary of the events and files for this tag.
-        
+
         Returns:
             dict:  dictionary summary of events and files that contain this tag.
-        
+
         """
         return {'tag': self.tag, 'events': self.events, 'files': [name for name in self.files]}
 
     def get_empty(self):
         empty = copy.copy(self)
         empty.events = 0
         empty.files = {}
         empty.value_dict = {}
         return empty
 
 
 class HedTagCounts:
     """ Counts of HED tags for a tabular file.
-    
+
     Parameters:
         name (str):  An identifier for these counts (usually the filename of the tabular file)
         total_events (int):  The total number of events in the tabular file.
 
-
     """
 
     def __init__(self, name, total_events=0):
         self.tag_dict = {}
         self.name = name
         self.files = {}
         self.total_events = total_events
-     
+
     def update_event_counts(self, hed_string_obj, file_name, definitions=None):
-        """ Update the tag counts based on a hed string object. 
-        
+        """ Update the tag counts based on a hed string object.
+
         Parameters:
             hed_string_obj (HedString): The HED string whose tags should be counted.
             file_name (str): The name of the file corresponding to these counts.
             definitions (dict): The definitions associated with the HED string.
-            
+
         """
         if file_name not in self.files:
             self.files[file_name] = ""
         tag_list = hed_string_obj.get_all_tags()
         tag_dict = {}
         for tag in tag_list:
             str_tag = tag.short_base_tag.lower()
@@ -96,48 +95,68 @@
                 tag_dict[str_tag] = HedTagCount(tag, file_name)
             else:
                 tag_dict[str_tag].set_value(tag)
 
         self.merge_tag_dicts(tag_dict)
 
     def organize_tags(self, tag_template):
+        """ Organize tags into categories as specified by the tag_template.
+
+        Parameters:
+            tag_template (dict): A dictionary whose keys are titles and values are lists of HED tags (str).
+
+        Returns:
+            dict  - keys are tags (strings) and values are list of HedTagCount for items fitting template.
+            list - of HedTagCount objects corresponding to tags that don't fit the template.
+
+        """
         template = self.create_template(tag_template)
         unmatched = []
-        for key, tag_count in self.tag_dict.items():
-            matched = False
-            for tag in reversed(tag_count.tag_terms):
-                if tag in template:
-                    template[tag].append(tag_count)
-                    matched = True
-                    break
-            if not matched:
-                unmatched.append(tag_count)
+        for tag_count in self.tag_dict.values():
+            self._update_template(tag_count, template, unmatched)
         return template, unmatched
 
     def merge_tag_dicts(self, other_dict):
         for tag, count in other_dict.items():
             if tag not in self.tag_dict:
                 self.tag_dict[tag] = count.get_empty()
             self.tag_dict[tag].events = self.tag_dict[tag].events + count.events
-            value_dict = self.tag_dict[tag].value_dict
-            for value, val_count in count.value_dict.items():
-                if value in value_dict:
-                    value_dict[value] = value_dict[value] + val_count
-                else:
-                    value_dict[value] = val_count
             for file in count.files:
                 self.tag_dict[tag].files[file] = ''
+            if not self.tag_dict[tag].value_dict:
+                continue
+            for value, val_count in count.value_dict.items():
+                if value in self.tag_dict[tag].value_dict:
+                    self.tag_dict[tag].value_dict[value] = self.tag_dict[tag].value_dict + val_count
+                else:
+                    self.tag_dict[tag].value_dict[value] = val_count
 
     def get_summary(self):
         details = {}
         for tag, count in self.tag_dict.items():
             details[tag] = count.get_summary()
-        return {'name': str(self.name), 'type_tag': self.type_tag, 'files': list(self.files.keys()),
+        return {'name': str(self.name), 'files': list(self.files.keys()),
                 'total_events': self.total_events, 'details': details}
 
     @staticmethod
     def create_template(tags):
         template_dict = {}
         for key, key_list in tags.items():
             for element in key_list:
                 template_dict[element.lower()] = []
         return template_dict
+
+    @staticmethod
+    def _update_template(tag_count, template, unmatched):
+        """ Update the template or unmatched with info in the tag_count.
+
+        Parameters:
+            tag_count (HedTagCount): Information for a particular tag.
+            template (dict):  The 
+
+        """
+        tag_list = reversed(list(tag_count.tag_terms))
+        for tkey in tag_list:
+            if tkey in template.keys():
+                template[tkey].append(tag_count)
+                return
+        unmatched.append(tag_count)
```

### Comparing `hedtools-0.3.0/hed/tools/analysis/hed_type_counts.py` & `hedtools-0.3.1/hed/tools/analysis/hed_type_counts.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/analysis/hed_type_definitions.py` & `hedtools-0.3.1/hed/tools/analysis/hed_type_definitions.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/analysis/hed_type_factors.py` & `hedtools-0.3.1/hed/tools/analysis/hed_type_factors.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         Parameters:
             factor_encoding (str):   Specifies type of factor encoding (one-hot or categorical).
 
         Returns:
             DataFrame:   DataFrame containing the factor vectors as the columns.
 
         """
-        df = pd.DataFrame(0, index=range(self.number_elements), columns=[self.type_value])
-        df.loc[list(self.direct_indices.keys()), [self.type_value]] = 1
+
         if not self.levels:
+            df = pd.DataFrame(0, index=range(self.number_elements), columns=[self.type_value])
+            df.loc[list(self.direct_indices.keys()), [self.type_value]] = 1
             return df
 
         levels = list(self.levels.keys())
         levels_list = [f"{self.type_value}.{level}" for level in levels]
-        df_levels = pd.DataFrame(0, index=range(self.number_elements), columns=levels_list)
+        factors = pd.DataFrame(0, index=range(self.number_elements), columns=levels_list)
         for index, level in enumerate(levels):
             index_keys = list(self.levels[level].keys())
-            df_levels.loc[index_keys, [levels_list[index]]] = 1
-        factors = pd.concat([df, df_levels], axis=1)
+            factors.loc[index_keys, [levels_list[index]]] = 1
         if factor_encoding == "one-hot":
             return factors
         sum_factors = factors.sum(axis=1)
         if factor_encoding == "categorical" and sum_factors.max() > 1:
             raise HedFileError("MultipleFactorSameEvent",
                                f"{self.type_value} has multiple occurrences at index {sum_factors.idxmax()}", "")
         elif factor_encoding == "categorical":
```

### Comparing `hedtools-0.3.0/hed/tools/analysis/hed_type_manager.py` & `hedtools-0.3.1/hed/tools/analysis/hed_type_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,29 @@
 
         Parameters:
             type_tag (str):    HED tag to retrieve factors for.
             type_values (list or None):  The values of the tag to create factors for or None if all unique values.
             factor_encoding (str):   Specifies type of factor encoding (one-hot or categorical).
 
         Returns:
-            DataFrame:   DataFrame containing the factor vectors as the columns.
+            DataFrame or None:   DataFrame containing the factor vectors as the columns.
 
         """
-        this_var = self.get_type_variable(type_tag)
+        this_var = self.get_type_variable(type_tag.lower())
         if this_var is None:
             return None
         variables = this_var.get_type_value_names()
-        if variables is None:
-            variables = type_values
-        df_list = [0]*len(variables)
-        for index, variable in enumerate(variables):
+        if not type_values:
+            type_values = variables
+        df_list = [0]*len(type_values)
+        for index, variable in enumerate(type_values):
             var_sum = this_var._type_value_map[variable]
             df_list[index] = var_sum.get_factors(factor_encoding=factor_encoding)
+        if not df_list:
+            return None
         return pd.concat(df_list, axis=1)
 
     def get_type_variable(self, type_tag):
         """
 
         Parameters:
             type_tag (str): Hed tag to retrieve the type for
```

### Comparing `hedtools-0.3.0/hed/tools/analysis/hed_type_values.py` & `hedtools-0.3.1/hed/tools/analysis/hed_type_values.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/analysis/key_map.py` & `hedtools-0.3.1/hed/tools/analysis/key_map.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/analysis/tabular_column_name_summary.py` & `hedtools-0.3.1/hed/tools/analysis/column_name_summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Summarizes the unique column names in a dataset. """
 
 import json
 
 
-class TabularColumnNameSummary:
+class ColumnNameSummary:
     def __init__(self, name=''):
         self.name = name
         self.file_dict = {}
         self.unique_headers = []
 
     def update(self, name, columns):
         position = self.update_headers(columns)
```

### Comparing `hedtools-0.3.0/hed/tools/analysis/tabular_summary.py` & `hedtools-0.3.1/hed/tools/analysis/tabular_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,16 +77,17 @@
             for v_key in sorted_v_keys:
                 val_dict[v_key] = cat_dict[v_key]
             categorical_cols[key] = val_dict
         sorted_cols = sorted(map(str, list(self.value_info)))
         value_cols = {}
         for key in sorted_cols:
             value_cols[key] = self.value_info[key]
-        summary = {"Summary name": self.name, "Total events": self.total_events, "Total files": self.total_files,
-                   "Categorical columns": categorical_cols, "Value columns": value_cols}
+        summary = {"Name": self.name, "Total events": self.total_events, "Total files": self.total_files,
+                   "Categorical columns": categorical_cols, "Value columns": value_cols,
+                   "Skip columns": self.skip_cols, "Files": self.files}
         if as_json:
             return json.dumps(summary, indent=4)
         else:
             return summary
 
     def get_number_unique(self, column_names=None):
         """ Return the number of unique values in columns.
@@ -212,14 +213,38 @@
             elif col not in val_cols:
                 self.value_info[col] = col_dict.value_info[col]
             else:
                 self.value_info[col] = [self.value_info[col][0] + col_dict.value_info[col][0],
                                         self.value_info[col][1] + col_dict.value_info[col][1]]
 
     @staticmethod
+    def extract_summary(summary_info):
+        """ Create a TabularSummary object from a serialized summary
+
+        Parameters:
+            summary_info (dict or str):  A JSON string or a dictionary containing contents of a TabularSummary.
+            
+        Returns:
+            TabularSummary:  contains the information in summary_info as a TabularSummary object.
+        """
+
+        if isinstance(summary_info, str):
+            summary_info = json.loads(summary_info)
+        new_tab = TabularSummary(value_cols=summary_info.get('Value columns', {}).keys(),
+                                 skip_cols=summary_info.get('Skip columns', []),
+                                 name=summary_info.get('Summary name', ''))
+        new_tab.value_info = summary_info.get('Value_columns', {})
+        new_tab.total_files = summary_info.get('Total files', 0)
+        new_tab.total_events = summary_info.get('Total events', 0)
+        new_tab.skip_cols = summary_info.get('Skip columns', [])
+        new_tab.categorical_info = summary_info.get('Categorical columns', {})
+        new_tab.files = summary_info.get('Files', {})
+        return new_tab
+
+    @staticmethod
     def get_columns_info(dataframe, skip_cols=None):
         """ Extract unique value counts for columns.
 
         Parameters:
             dataframe (DataFrame):    The DataFrame to be analyzed.
             skip_cols(list):          List of names of columns to be skipped in the extraction.
```

### Comparing `hedtools-0.3.0/hed/tools/analysis/temporal_event.py` & `hedtools-0.3.1/hed/tools/analysis/temporal_event.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/bids/bids_dataset.py` & `hedtools-0.3.1/hed/tools/bids/bids_dataset.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/bids/bids_file.py` & `hedtools-0.3.1/hed/tools/bids/bids_file.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/bids/bids_file_dictionary.py` & `hedtools-0.3.1/hed/tools/bids/bids_file_dictionary.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/bids/bids_file_group.py` & `hedtools-0.3.1/hed/tools/bids/bids_file_group.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/bids/bids_sidecar_file.py` & `hedtools-0.3.1/hed/tools/bids/bids_sidecar_file.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/bids/bids_tabular_dictionary.py` & `hedtools-0.3.1/hed/tools/bids/bids_tabular_dictionary.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/bids/bids_tabular_file.py` & `hedtools-0.3.1/hed/tools/bids/bids_tabular_file.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/backup_manager.py` & `hedtools-0.3.1/hed/tools/remodeling/backup_manager.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel.py` & `hedtools-0.3.1/hed/tools/remodeling/cli/run_remodel.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel_backup.py` & `hedtools-0.3.1/hed/tools/remodeling/cli/run_remodel_backup.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel_restore.py` & `hedtools-0.3.1/hed/tools/remodeling/cli/run_remodel_restore.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/dispatcher.py` & `hedtools-0.3.1/hed/tools/remodeling/dispatcher.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/base_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/base_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/base_summary.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/base_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
             - The 'Dataset' value is either a string or a dictionary with the overall summary.
             - The 'Individual files' value is dictionary whose keys are file names and values are
                    their corresponding summaries.
 
         Users are expected to provide merge_all_info and get_details_dict to support this.
 
         """
-        merged_summary = self.merge_all_info()
-        if merged_summary:
-            details = self.get_details_dict(merged_summary)
+        merged_counts = self.merge_all_info()
+        if merged_counts:
+            details = self.get_details_dict(merged_counts)
         else:
             details = "Overall summary unavailable"
 
         summary_details = {"Dataset": details, "Individual files": {}}
         if include_individual:
             for name, count in self.summary_dict.items():
                 summary_details["Individual files"][name] = self.get_details_dict(count)
@@ -216,14 +216,19 @@
 
         Returns:
             dict: dictionary with the results.
 
         Notes:
             Abstract method be implemented by each individual summary.
 
+        Notes:
+            The expected return value is a dictionary of the form:
+
+               {"Name": "", "Total events": 0, "Total files": 0, "Files": [], "Specifics": {}}"
+
         """
         raise NotImplementedError
 
     @abstractmethod
     def merge_all_info(self):
         """ Return merged information.
```

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/convert_columns_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/convert_columns_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/factor_column_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/factor_column_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/factor_hed_tags_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/factor_hed_tags_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/factor_hed_type_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/factor_hed_type_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,13 +74,13 @@
         hed_strings, definitions = get_assembled(input_data, sidecar, dispatcher.hed_schema, 
                                                  extra_def_dicts=None, join_columns=True,
                                                  shrink_defs=True, expand_defs=False)
 
         var_manager = HedTypeManager(hed_strings, dispatcher.hed_schema, definitions)
         var_manager.add_type_variable(self.type_tag.lower())
 
-        df_factors = var_manager.get_factor_vectors(self.type_tag, [], factor_encoding="one-hot")
+        df_factors = var_manager.get_factor_vectors(self.type_tag, self.type_values, factor_encoding="one-hot")
         if len(df_factors.columns) > 0:
             df_list.append(df_factors)
         df_new = pd.concat(df_list, axis=1)
         df_new.replace('n/a', np.NaN, inplace=True)
         return df_new
```

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/merge_consecutive_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/merge_consecutive_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/number_groups_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/number_groups_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/number_rows_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/number_rows_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/remap_columns_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/remap_columns_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/remove_columns_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/remove_columns_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/remove_rows_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/remove_rows_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/rename_columns_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/rename_columns_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/reorder_columns_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/reorder_columns_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/split_rows_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/split_rows_op.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_column_names_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/summarize_column_names_op.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """  Summarize the column names in a collection of tabular files. """
 
-from hed.tools.analysis.tabular_column_name_summary import TabularColumnNameSummary
+from hed.tools.analysis.column_name_summary import ColumnNameSummary
 from hed.tools.remodeling.operations.base_op import BaseOp
 from hed.tools.remodeling.operations.base_summary import BaseSummary
 
 
 class SummarizeColumnNamesOp(BaseOp):
     """  Summarize the column names in a collection of tabular files.
 
@@ -63,61 +63,65 @@
         Side-effect:
             Updates the relevant summary.
 
         """
         df_new = df.copy()
         summary = dispatcher.summary_dicts.get(self.summary_name, None)
         if not summary:
-            summary = ColumnNameSummary(self)
+            summary = ColumnNamesSummary(self)
             dispatcher.summary_dicts[self.summary_name] = summary
         summary.update_summary({"name": name, "column_names": list(df_new.columns)})
         return df_new
 
 
-class ColumnNameSummary(BaseSummary):
+class ColumnNamesSummary(BaseSummary):
 
     def __init__(self, sum_op):
         super().__init__(sum_op)
 
     def update_summary(self, new_info):
         """ Update the summary for a given tabular input file.
 
         Parameters:
             new_info (dict):  A dictionary with the parameters needed to update a summary.
 
         Notes:
-            - The summary information is kept in separate TabularColumnNameSummary objects for each file.  
+            - The summary information is kept in separate ColumnNameSummary objects for each file.  
             - The summary needs a "name" str and a "column_names" list.  
-            - The summary uses TabularColumnNameSummary as the summary object.
+            - The summary uses ColumnNameSummary as the summary object.
         """
         name = new_info['name']
         if name not in self.summary_dict:
-            self.summary_dict[name] = TabularColumnNameSummary(name=name)
+            self.summary_dict[name] = ColumnNameSummary(name=name)
         self.summary_dict[name].update(name, new_info["column_names"])
 
     def get_details_dict(self, column_summary):
         """ Return the summary dictionary extracted from a ColumnNameSummary.
 
         Parameters:
-            column_summary (TabularColumnNameSummary):  A column name summary for the data file.
+            column_summary (ColumnNameSummary):  A column name summary for the data file.
 
         Returns:
             dict - a dictionary with the summary information for column names.
 
         """
-        return column_summary.get_summary()
+        summary = column_summary.get_summary()
+        return {"Name": summary['Summary name'], "Total events": "n/a",
+                "Total files": summary['Number files'],
+                "Files": [name for name in column_summary.file_dict.keys()],
+                "Specifics": {"Columns": summary['Columns']}}
 
     def merge_all_info(self):
-        """ Create a TabularColumnNameSummary containing the overall dataset summary.
+        """ Create a ColumnNameSummary containing the overall dataset summary.
 
         Returns:
-            TabularColumnNameSummary - the overall summary object for column names.
+            ColumnNameSummary - the overall summary object for column names.
 
         """
-        all_sum = TabularColumnNameSummary(name='Dataset')
+        all_sum = ColumnNameSummary(name='Dataset')
         for key, counts in self.summary_dict.items():
             for name, pos in counts.file_dict.items():
                 all_sum.update(name, counts.unique_headers[pos])
         return all_sum
 
     def _get_result_string(self, name, result, indent=BaseSummary.DISPLAY_INDENT):
         """ Return a formatted string with the summary for the indicated name.
@@ -132,28 +136,33 @@
 
         Notes:
             This calls _get_dataset_string to get the overall summary string.
 
         """
         if name == "Dataset":
             return self._get_dataset_string(result, indent)
-        columns = result["Columns"][0]
-        return f"{indent}{str(columns['Column names'])}"
+        columns = result.get("Specifics", {}).get("Columns", [])
+        if columns:
+            return f"{indent}{str(columns[0])}"
+        else:
+            return ""
 
     @staticmethod
     def _get_dataset_string(result, indent=BaseSummary.DISPLAY_INDENT):
         """ Return  a string with the overall summary for all of the tabular files.
 
         Parameters:
             result (dict): Dictionary of merged summary information.
             indent (str):  String of blanks used as the amount to indent for readability.
 
         Returns:
             str: Formatted string suitable for saving in a file or printing.
 
         """
-        sum_list = [f"Dataset: Number of files={result.get('Number files', 0)}"]
-        for element in result.get("Columns", []):
+        sum_list = [f"Dataset: Number of files={result.get('Total files', 0)}"]
+        specifics = result.get("Specifics", {})
+        columns = specifics.get("Columns", {})
+        for element in columns:
             sum_list.append(f"{indent}Columns: {str(element['Column names'])}")
             for file in element.get("Files", []):
                 sum_list.append(f"{indent}{indent}{file}")
         return "\n".join(sum_list)
```

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_column_values_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/summarize_column_values_op.py`

 * *Files 7% similar despite different names*

```diff
@@ -124,25 +124,32 @@
         """
         this_summary = summary.get_summary(as_json=False)
         unique_counts = [(key, len(count_dict)) for key, count_dict in this_summary['Categorical columns'].items()]
         this_summary['Categorical counts'] = dict(unique_counts)
         for key, dict_entry in this_summary['Categorical columns'].items():
             num_disp, sorted_tuples = ColumnValueSummary.sort_dict(dict_entry, reverse=True)
             this_summary['Categorical columns'][key] = dict(sorted_tuples[:min(num_disp, self.op.max_categorical)])
-        return this_summary
+        return {"Name": this_summary['Name'], "Total events": this_summary["Total events"],
+                "Total files": this_summary['Total files'],
+                "Files": [name for name in this_summary['Files'].keys()],
+                "Specifics": {"Value columns": this_summary['Value columns'].keys(),
+                              "Skip columns": this_summary['Skip columns'],
+                              "Value columns": this_summary['Value columns'],
+                              "Categorical columns": this_summary['Categorical columns'],
+                              "Categorical counts": this_summary['Categorical counts']}}
 
     def merge_all_info(self):
         """ Create a TabularSummary containing the overall dataset summary.
 
         Returns:
             TabularSummary - the summary object for column values.
 
         """
         all_sum = TabularSummary(value_cols=self.op.value_columns, skip_cols=self.op.skip_columns, name='Dataset')
-        for key, counts in self.summary_dict.items():
+        for counts in self.summary_dict.values():
             all_sum.update_summary(counts)
         return all_sum
 
     def _get_result_string(self, name, result, indent=BaseSummary.DISPLAY_INDENT):
         """ Return a formatted string with the summary for the indicated name.
 
         Parameters:
@@ -194,18 +201,19 @@
 
         Returns:
             str: Formatted string suitable for saving in a file or printing.
 
         """
         sum_list = [f"Dataset: Total events={result.get('Total events', 0)} "
                     f"Total files={result.get('Total files', 0)}"]
-        cat_string = self._get_categorical_string(result, offset="", indent=indent)
+        specifics = result["Specifics"]
+        cat_string = self._get_categorical_string(specifics, offset="", indent=indent)
         if cat_string:
             sum_list.append(cat_string)
-        val_cols = result.get("Value columns", {})
+        val_cols = specifics.get("Value columns", {})
         if val_cols:
             sum_list.append(ColumnValueSummary._get_value_string(val_cols, offset="", indent=indent))
         return "\n".join(sum_list)
 
     def _get_individual_string(self, result, indent=BaseSummary.DISPLAY_INDENT):
 
         """ Return  a string with the summary for an individual tabular file.
@@ -215,14 +223,15 @@
             indent (str):  String of blanks used as the amount to indent for readability.
 
         Returns:
             str: Formatted string suitable for saving in a file or printing.
 
         """
         sum_list = [f"Total events={result.get('Total events', 0)}"]
+        specifics = result.get("Specifics", {})
         cat_cols = result.get("Categorical columns", {})
         if cat_cols:
             sum_list.append(self._get_categorical_string(cat_cols, offset=indent, indent=indent))
         val_cols = result.get("Value columns", {})
         if val_cols:
             sum_list.append(ColumnValueSummary._get_value_string(val_cols, offset=indent, indent=indent))
         return "\n".join(sum_list)
```

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_definitions_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/summarize_definitions_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,16 @@
                                                       display_description=True)
         ambiguous_defs_summary = self._build_summary_dict(def_gatherer.ambiguous_defs, "Ambiguous Definitions",
                                                           def_gatherer.get_ambiguous_group)
         errors_summary = self._build_summary_dict(def_gatherer.errors, "Errors", None)
 
         known_defs_summary.update(ambiguous_defs_summary)
         known_defs_summary.update(errors_summary)
+        return {"Name": "", "Total events": 0, "Total files": 0, "Files": [], "Specifics": known_defs_summary}
+        
         return known_defs_summary
 
     def merge_all_info(self):
         """ Create an Object containing the definition summary.
 
         Returns:
             Object - the overall summary object for definitions.
```

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_tags_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/summarize_hed_tags_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         "required_parameters": {
             "summary_name": str,
             "summary_filename": str,
             "tags": dict
         },
         "optional_parameters": {
             "append_timecode": bool,
+            "expand_definitions": bool,
             "expand_context": bool
         }
     }
 
     SUMMARY_TYPE = "hed_tag_summary"
 
     def __init__(self, parameters):
@@ -114,32 +115,33 @@
                                                  extra_def_dicts=None, join_columns=True,
                                                  shrink_defs=False, expand_defs=True)
         # definitions = input_data.get_definitions().gathered_defs
         for hed in hed_strings:
             counts.update_event_counts(hed, new_info['name'])
         self.summary_dict[new_info["name"]] = counts
 
-    def get_details_dict(self, merge_counts):
+    def get_details_dict(self, tag_counts):
         """ Return the summary-specific information in a dictionary.
 
         Parameters:
-            merge_counts (HedTagCounts):  Contains the counts of tags in the dataset.
+            tag_counts (HedTagCounts):  Contains the counts of tags in the dataset.
 
         Returns:
             dict: dictionary with the summary results.
 
         """
-        template, unmatched = merge_counts.organize_tags(self.tags)
+        template, unmatched = tag_counts.organize_tags(self.tags)
         details = {}
         for key, key_list in self.tags.items():
             details[key] = self._get_details(key_list, template, verbose=True)
         leftovers = [value.get_info(verbose=True) for value in unmatched]
-        return {"name": merge_counts.name, "total_events": merge_counts.total_events,
-                "files": [name for name in merge_counts.files.keys()],
-                "Main tags": details, "Other tags": leftovers}
+        return {"Name": tag_counts.name, "Total events": tag_counts.total_events,
+                "Total files": len(tag_counts.files.keys()),
+                "Files": [name for name in tag_counts.files.keys()],
+                "Specifics": {"Main tags": details, "Other tags": leftovers}}
 
     def _get_result_string(self, name, result, indent=BaseSummary.DISPLAY_INDENT):
         """ Return a formatted string with the summary for the indicated name.
 
         Parameters:
             name (str):  Identifier (usually the filename) of the individual file.
             result (dict): The dictionary of the summary results indexed by name.
@@ -181,16 +183,16 @@
             result (dict): Dictionary of merged summary information.
             indent (str):  String of blanks used as the amount to indent for readability.
 
         Returns:
             str: Formatted string suitable for saving in a file or printing.
 
         """
-        sum_list = [f"Dataset: Total events={result.get('total_events', 0)} "
-                    f"Total files={len(result.get('files', []))}"]
+        sum_list = [f"Dataset: Total events={result.get('Total events', 0)} "
+                    f"Total files={len(result.get('Files', 0))}"]
         sum_list = sum_list + HedTagSummary._get_tag_list(result, indent=indent)
         return "\n".join(sum_list)
 
     @staticmethod
     def _get_individual_string(result, indent=BaseSummary.DISPLAY_INDENT):
         """ Return  a string with the summary for an individual tabular file.
 
@@ -198,27 +200,28 @@
             result (dict): Dictionary of summary information for a particular tabular file.
             indent (str):  String of blanks used as the amount to indent for readability.
 
         Returns:
             str: Formatted string suitable for saving in a file or printing.
 
         """
-        sum_list = [f"Total events={result.get('total_events', 0)}"]
+        sum_list = [f"Total events={result.get('Total events', 0)}"]
         sum_list = sum_list + HedTagSummary._get_tag_list(result, indent=indent)
         return "\n".join(sum_list)
 
     @staticmethod
     def _tag_details(tags):
         tag_list = []
         for tag in tags:
             tag_list.append(f"{tag['tag']}[{tag['events']},{len(tag['files'])}]")
         return tag_list
 
     @staticmethod
-    def _get_tag_list(tag_info, indent=BaseSummary.DISPLAY_INDENT):
+    def _get_tag_list(result, indent=BaseSummary.DISPLAY_INDENT):
+        tag_info = result["Specifics"]
         sum_list = [f"\n{indent}Main tags[events,files]:"]
         for category, tags in tag_info['Main tags'].items():
             sum_list.append(f"{indent}{indent}{category}:")
             if tags:
                 sum_list.append(f"{indent}{indent}{indent}{' '.join(HedTagSummary._tag_details(tags))}")
         if tag_info['Other tags']:
             sum_list.append(f"{indent}Other tags[events,files]:")
```

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_type_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/summarize_hed_type_op.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,24 +91,24 @@
 
     def update_summary(self, new_info):
         """ Update the summary for a given tabular input file.
 
         Parameters:
             new_info (dict):  A dictionary with the parameters needed to update a summary.
 
-        Notes:  
+        Notes:
             - The summary needs a "name" str, a "schema", a "df, and a "Sidecar".
 
         """
 
         sidecar = new_info['sidecar']
         if sidecar and not isinstance(sidecar, Sidecar):
             sidecar = Sidecar(sidecar)
         input_data = TabularInput(new_info['df'], sidecar=sidecar, name=new_info['name'])
-        hed_strings, definitions = get_assembled(input_data, sidecar, new_info['schema'], 
+        hed_strings, definitions = get_assembled(input_data, sidecar, new_info['schema'],
                                                  extra_def_dicts=None, join_columns=True, expand_defs=False)
         context_manager = HedContextManager(hed_strings, new_info['schema'])
         type_values = HedTypeValues(context_manager, definitions, new_info['name'], type_tag=self.type_tag)
 
         counts = HedTypeCounts(new_info['name'], self.type_tag)
         counts.update_summary(type_values.get_summary(), type_values.total_events, new_info['name'])
         counts.add_descriptions(type_values.definitions)
@@ -120,15 +120,20 @@
         Parameters:
             counts (HedTypeCounts):  Contains the counts of the events in which the type occurs.
 
         Returns:
             dict: dictionary with the summary results.
 
         """
-        return counts.get_summary()
+        summary = counts.get_summary()
+        files = summary.get('files', [])
+        return {"Name": summary.get("name", ""), "Total events": summary.get("total_events", 0),
+                "Total files": len(files), "Files": files,
+                "Specifics": {"Type tag": summary.get('type_tag', 'condition-variable'),
+                              "Type info": summary.get('details', {})}}
 
     def merge_all_info(self):
         """ Create a HedTypeCounts containing the overall dataset HED type summary.
 
         Returns:
             HedTypeCounts - the overall dataset summary object for HED type summary.
 
@@ -166,19 +171,20 @@
             result (dict): Dictionary of merged summary information.
             indent (str):  String of blanks used as the amount to indent for readability.
 
         Returns:
             str: Formatted string suitable for saving in a file or printing.
 
         """
-        details = result.get('details', {})
-        sum_list = [f"Dataset: Type={result['type_tag']} Type values={len(details)} "
-                    f"Total events={result.get('total_events', 0)} Total files={len(result.get('files', []))}"]
+        specifics = result.get('Specifics', {})
+        type_info = specifics.get('Type info', {})
+        sum_list = [f"Dataset: Type={specifics.get('Type tag', 'condition-variable')} Type values={len(type_info)} "
+                    f"Total events={result.get('Total events', 0)} Total files={len(result.get('Files', []))}"]
 
-        for key, item in details.items():
+        for key, item in type_info.items():
             str1 = f"{item['events']} event(s) out of {item['total_events']} total events in " + \
                    f"{len(item['files'])} file(s)"
             if item['level_counts']:
                 str1 = f"{len(item['level_counts'])} levels in " + str1
             if item['direct_references']:
                 str1 = str1 + f" Direct references:{item['direct_references']}"
             if item['events_with_multiple_refs']:
@@ -196,19 +202,20 @@
             result (dict): Dictionary of summary information for a particular tabular file.
             indent (str):  String of blanks used as the amount to indent for readability.
 
         Returns:
             str: Formatted string suitable for saving in a file or printing.
 
         """
-        details = result.get('details', {})
-        sum_list = [f"Type={result['type_tag']} Type values={len(details)} "
-                    f"Total events={result.get('total_events', 0)}"]
+        specifics = result.get('Specifics', {})
+        type_info = specifics.get('Type info', {})
+        sum_list = [f"Type={specifics.get('Type tag', 'condition-variable')} Type values={len(type_info)} "
+                    f"Total events={result.get('Total events', 0)}"]
 
-        for key, item in details.items():
+        for key, item in type_info.items():
             sum_list.append(f"{indent*2}{key}: {item['levels']} levels in {item['events']} events")
             str1 = ""
             if item['direct_references']:
                 str1 = str1 + f" Direct references:{item['direct_references']}"
             if item['events_with_multiple_refs']:
                 str1 = str1 + f" (Multiple references:{item['events_with_multiple_refs']})"
             if str1:
```

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_validation_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/summarize_hed_validation_op.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,130 +97,127 @@
         Returns:
             str - The results in a printable format ready to be saved to a text file.
 
         Notes:
             This gets the error list from "sidecar_issues" and "event_issues".
 
         """
-
-        if result["is_merged"]:
-            sum_list = [f"{name}: [{result['total_sidecar_files']} sidecar files, "
-                        f"{result['total_event_files']} event files]"]
-            sum_list = sum_list + self.get_error_list(result['sidecar_issues'], count_only=True, indent=indent)
-            sum_list = sum_list + self.get_error_list(result['event_issues'], count_only=True, indent=indent)
+        specifics = result.get("Specifics", {})
+        sum_list = [f"{name}: [{len(specifics['sidecar_files'])} sidecar files, "
+                    f"{len(specifics['event_files'])} event files]"]
+        if specifics.get('is_merged'):
+            sum_list = sum_list + self.get_error_list(specifics['sidecar_issues'], count_only=True, indent=indent)
+            sum_list = sum_list + self.get_error_list(specifics['event_issues'], count_only=True, indent=indent)
         else:
-            sum_list = [f"{indent}{name}: {result['total_sidecar_files']} sidecar files"]
-            sum_list = sum_list + self.get_error_list(result['sidecar_issues'], indent=indent*2)
-            if result['validation_completed']:
-                sum_list = sum_list + self.get_error_list(result['event_issues'], count_only=False, indent=indent*2)
+            sum_list = sum_list + self.get_error_list(specifics['sidecar_issues'], indent=indent*2)
+            if specifics['sidecar_had_issues']:
+                sum_list = sum_list + self.get_error_list(specifics['event_issues'], count_only=False, indent=indent*2)
             else:
                 sum_list = sum_list + [f"{indent*2}Event file validation was incomplete because of sidecar errors"]
         return "\n".join(sum_list)
 
     def update_summary(self, new_info):
         """ Update the summary for a given tabular input file.
 
         Parameters:
             new_info (dict):  A dictionary with the parameters needed to update a summary.
 
         Notes:
             - The summary needs a "name" str, a schema, a "df", and a "Sidecar".
         """
 
-        results = self.get_empty_results()
-        results["total_event_files"] = 1
-        results["event_issues"][new_info["name"]] = []
-        self.summary_dict[new_info["name"]] = results
         sidecar = new_info.get('sidecar', None)
-        filtered_issues = []
-        if sidecar:
-            if not isinstance(sidecar, Sidecar):
-                sidecar = Sidecar(files=new_info['sidecar'], name=os.path.basename(sidecar))
-            results["sidecar_issues"][sidecar.name] = []
-            sidecar_issues = sidecar.validate(new_info['schema'])
-            filtered_issues = ErrorHandler.filter_issues_by_severity(sidecar_issues, ErrorSeverity.ERROR)
-            if not self.check_for_warnings:
-                sidecar_issues = filtered_issues
-            results['sidecar_issues'][sidecar.name] = sidecar_issues
-            results['total_sidecar_issues'] = len(sidecar_issues)
-            results['total_sidecar_files'] = 1
-        if not filtered_issues:
-            results['validation_completed'] = True
+        if sidecar and not isinstance(sidecar, Sidecar):
+            sidecar = Sidecar(files=new_info['sidecar'], name=os.path.basename(sidecar))
+        results = self._get_sidecar_results(sidecar, new_info, self.check_for_warnings)
+        if not results['sidecar_had_issues']:
             input_data = TabularInput(new_info['df'], sidecar=sidecar)
             issues = input_data.validate(new_info['schema'])
             if not self.check_for_warnings:
                 issues = ErrorHandler.filter_issues_by_severity(issues, ErrorSeverity.ERROR)
             results['event_issues'][new_info["name"]] = issues
             results['total_event_issues'] = len(issues)
+        self.summary_dict[new_info["name"]] = results
 
     def get_details_dict(self, summary_info):
         """Return the summary details from the summary_info.
 
         Parameters:
             summary_info (dict): Dictionary of issues
 
         Returns:
             dict:  Same summary_info as was passed in.
 
         """
-        return summary_info
+
+        return {"Name": "", "Total events": "n/a",
+                "Total files": len(summary_info.get("event_files", [])),
+                "Files": summary_info.get("event_files", []),
+                "Specifics": summary_info}
 
     def merge_all_info(self):
         """ Create a dictionary containing all of the errors in the dataset.
 
         Returns:
             dict - dictionary of issues organized into sidecar_issues and event_issues.
 
         """
-
         results = self.get_empty_results()
         results["is_merged"] = True
         for key, ind_results in self.summary_dict.items():
-            results["total_event_files"] += ind_results["total_event_files"]
-            results["total_event_issues"] += ind_results["total_event_issues"]
-
-            for ikey, errors in ind_results["sidecar_issues"].items():
-                results["sidecar_issues"][ikey] = errors
-            for ikey, errors in ind_results["event_issues"].items():
-                if not ind_results["validation_completed"]:
-                    results["event_issues"][ikey] = \
-                       f"Validation incomplete due to {ind_results['total_sidecar_issues']} sidecar issues"
-                else:
-                    results["event_issues"][ikey] = f"{len(errors)}"
-            results["total_sidecar_files"] += ind_results["total_sidecar_files"]
+            HedValidationSummary._update_sidecar_results(results, ind_results)
+            results["event_files"].append(key)
+            HedValidationSummary._update_events_results(results, ind_results)
         return results
 
     @staticmethod
+    def _update_events_results(results, ind_results):
+        results["total_event_issues"] += ind_results["total_event_issues"]
+        for ikey, errors in ind_results["event_issues"].items():
+            if ind_results["sidecar_had_issues"]:
+                results["event_issues"][ikey] = \
+                    f"Validation incomplete due to {ind_results['total_sidecar_issues']} sidecar issues"
+            else:
+                results["event_issues"][ikey] = f"{len(errors)}"
+
+    @staticmethod
+    def _update_sidecar_results(results, ind_results):
+        results["total_sidecar_issues"] += ind_results["total_sidecar_issues"]
+        results["sidecar_files"] = results["sidecar_files"] + ind_results["sidecar_files"]
+        for ikey, errors in ind_results["sidecar_issues"].items():
+            results["sidecar_issues"][ikey] = errors
+
+    @staticmethod
     def get_empty_results():
-        return {"total_event_files": 0, "total_event_issues": 0, "event_issues": {}, "is_merged": False,
-                "total_sidecar_files": 0, "total_sidecar_issues": 0, "sidecar_issues": {},
-                "validation_completed": False}
+        return {"event_files": [], "total_event_issues": 0, "event_issues": {}, "is_merged": False,
+                "sidecar_files": [], "total_sidecar_issues": 0, "sidecar_issues": {},
+                "sidecar_had_issues": False}
 
     @staticmethod
     def get_error_list(error_dict, count_only=False, indent=BaseSummary.DISPLAY_INDENT):
         error_list = []
         for key, item in error_dict.items():
             if count_only and isinstance(item, list):
                 error_list.append(f"{indent}{key}: {len(item)} issues")
             elif count_only:
                 error_list.append(f"{indent}{key}: {item} issues")
             elif not len(item):
                 error_list.append(f"{indent}{key} has no issues")
             else:
-                error_list.append(f"{indent}{key} issues:")
-                for this_item in item:
-                    error_list.append(f"{indent*2}{HedValidationSummary.format_error(this_item)}")
+                HedValidationSummary._format_errors(error_list, key, item, indent)
         return error_list
 
     @staticmethod
-    def format_errors(error_list):
-        pass
+    def _format_errors(error_list, name, errors, indent):
+        error_list.append(f"{indent}{name} issues:")
+        for this_item in errors:
+            error_list.append(f"{indent * 2}{HedValidationSummary._format_error(this_item)}")
 
     @staticmethod
-    def format_error(error):
+    def _format_error(error):
         error_str = error['code']
         error_locations = []
         HedValidationSummary.update_error_location(error_locations, "row", "ec_row", error)
         HedValidationSummary.update_error_location(error_locations, "column", "ec_column", error)
         HedValidationSummary.update_error_location(error_locations, "sidecar column",
                                                    "ec_sidecarColumnName", error)
         HedValidationSummary.update_error_location(error_locations, "sidecar key", "ec_sidecarKeyName", error)
@@ -230,7 +227,25 @@
         error_str = error_str + f": {error['message']}"
         return error_str
 
     @staticmethod
     def update_error_location(error_locations, location_name, location_key, error):
         if location_key in error:
             error_locations.append(f"{location_name}={error[location_key][0]}")
+
+    @staticmethod
+    def _get_sidecar_results(sidecar, new_info, check_for_warnings):
+        results = HedValidationSummary.get_empty_results()
+        results["event_files"].append(new_info["name"])
+        results["event_issues"][new_info["name"]] = []
+        if sidecar:
+            results["sidecar_files"].append(sidecar.name)
+            results["sidecar_issues"][sidecar.name] = []
+            sidecar_issues = sidecar.validate(new_info['schema'])
+            filtered_issues = ErrorHandler.filter_issues_by_severity(sidecar_issues, ErrorSeverity.ERROR)
+            if filtered_issues:
+                results["sidecar_had_issues"] = True
+            if not check_for_warnings:
+                sidecar_issues = filtered_issues
+            results['sidecar_issues'][sidecar.name] = sidecar_issues
+            results['total_sidecar_issues'] = len(sidecar_issues)
+        return results
```

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,17 +111,21 @@
             summary_info (TabularSummary):  Summary to return info from
 
         Notes:
             Abstract method be implemented by each individual context summary.
 
         """
 
-        return {"files": summary_info.files, "total_files": summary_info.total_files,
-                "total_events": summary_info.total_events, "skip_cols": summary_info.skip_cols,
-                "sidecar": summary_info.extract_sidecar_template()}
+        return {"Name": summary_info.name, "Total events": summary_info.total_events,
+                "Total files": summary_info.total_files,
+                "Files": summary_info.files.keys(),
+                "Specifics": {"Categorical info": summary_info.categorical_info,
+                              "Value info": summary_info.value_info,
+                              "Skip columns": summary_info.skip_cols,
+                              "Sidecar": summary_info.extract_sidecar_template()}}
 
     def merge_all_info(self):
         """ Merge summary information from all of the files
 
         Returns:
            TabularSummary:  Consolidated summary of information.
 
@@ -161,31 +165,33 @@
             result (dict): Dictionary of merged summary information.
             indent (str):  String of blanks used as the amount to indent for readability.
 
         Returns:
             str: Formatted string suitable for saving in a file or printing.
 
         """
-        sum_list = [f"Dataset: Total events={result.get('total_events', 0)} "
-                    f"Total files={result.get('total_files', 0)}",
-                    f"Skip columns: {str(result.get('skip_cols', []))}",
-                    f"Value columns: {str(result.get('value_cols', []))}",
-                    f"Sidecar:\n{json.dumps(result['sidecar'], indent=indent)}"]
+        specifics = result.get("Specifics", {})
+        sum_list = [f"Dataset: Total events={result.get('Total events', 0)} "
+                    f"Total files={result.get('Total files', 0)}",
+                    f"Skip columns: {str(specifics.get('Skip columns', []))}",
+                    f"Value columns: {str(specifics.get('Value info', {}).keys())}",
+                    f"Sidecar:\n{json.dumps(specifics.get('Sidecar', {}), indent=indent)}"]
         return "\n".join(sum_list)
 
     @staticmethod
     def _get_individual_string(result, indent=BaseSummary.DISPLAY_INDENT):
         """ Return  a string with the summary for an individual tabular file.
 
         Parameters:
             result (dict): Dictionary of summary information for a particular tabular file.
             indent (str):  String of blanks used as the amount to indent for readability.
 
         Returns:
             str: Formatted string suitable for saving in a file or printing.
 
         """
-        sum_list = [f"Total events={result.get('total_events', 0)}",
-                    f"Skip columns: {str(result.get('skip_cols', []))}",
-                    f"Value columns: {str(result.get('value_cols', []))}",
-                    f"Sidecar:\n{json.dumps(result['sidecar'], indent=indent)}"]
+        specifics = result.get("Specifics", {})
+        sum_list = [f"Total events={result.get('Total events', 0)}",
+                    f"Skip columns: {str(specifics.get('Slip columns', []))}",
+                    f"Value columns: {str(specifics.get('Value info', {}).keys())}",
+                    f"Sidecar:\n{json.dumps(specifics['Sidecar'], indent=indent)}"]
         return "\n".join(sum_list)
```

### Comparing `hedtools-0.3.0/hed/tools/remodeling/operations/valid_operations.py` & `hedtools-0.3.1/hed/tools/remodeling/operations/valid_operations.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/util/data_util.py` & `hedtools-0.3.1/hed/tools/util/data_util.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/util/hed_logger.py` & `hedtools-0.3.1/hed/tools/util/hed_logger.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/util/io_util.py` & `hedtools-0.3.1/hed/tools/util/io_util.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/tools/util/schema_util.py` & `hedtools-0.3.1/hed/tools/util/schema_util.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/validator/def_validator.py` & `hedtools-0.3.1/hed/validator/def_validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,24 +34,76 @@
         def_issues = []
         # We need to check for labels to expand in ALL groups
         for def_tag, def_expand_group, def_group in hed_string_obj.find_def_tags(recursive=True):
             def_issues += self._validate_def_contents(def_tag, def_expand_group, tag_validator)
 
         return def_issues
 
+    @staticmethod
+    def _validate_def_units(def_tag, placeholder_tag, tag_validator, is_def_expand_tag):
+        """Validate units and value classes on def/def-expand tags
+
+        Parameters:
+            def_tag(HedTag): The source tag
+            placeholder_tag(HedTag): The placeholder tag this def fills in
+            tag_validator(TagValidator): Used to validate the units/values
+            is_def_expand_tag(bool): If the given def_tag is a def-expand tag or not.
+
+        Returns:
+            issues(list): Issues found from validating placeholders.
+        """
+        def_issues = []
+        error_code = ValidationErrors.DEF_INVALID
+        if is_def_expand_tag:
+            error_code = ValidationErrors.DEF_EXPAND_INVALID
+        if placeholder_tag.is_unit_class_tag():
+            def_issues += tag_validator.check_tag_unit_class_units_are_valid(placeholder_tag,
+                                                                             report_as=def_tag,
+                                                                             error_code=error_code)
+        elif placeholder_tag.is_value_class_tag():
+            def_issues += tag_validator.check_tag_value_class_valid(placeholder_tag,
+                                                                    report_as=def_tag,
+                                                                    error_code=error_code)
+        return def_issues
+
+    @staticmethod
+    def _report_missing_or_invalid_value(def_tag, def_entry, is_def_expand_tag):
+        """Returns the correct error for this type of def tag
+
+        Parameters:
+            def_tag(HedTag): The source tag
+            def_entry(DefinitionEntry): The entry for this definition
+            is_def_expand_tag(bool): If the given def_tag is a def-expand tag or not.
+
+        Returns:
+            issues(list): Issues found from validating placeholders.
+        """
+        def_issues = []
+        if def_entry.takes_value:
+            error_code = ValidationErrors.HED_DEF_VALUE_MISSING
+            if is_def_expand_tag:
+                error_code = ValidationErrors.HED_DEF_EXPAND_VALUE_MISSING
+        else:
+            error_code = ValidationErrors.HED_DEF_VALUE_EXTRA
+            if is_def_expand_tag:
+                error_code = ValidationErrors.HED_DEF_EXPAND_VALUE_EXTRA
+        def_issues += ErrorHandler.format_error(error_code, tag=def_tag)
+        return def_issues
+
     def _validate_def_contents(self, def_tag, def_expand_group, tag_validator):
         """ Check for issues with expanding a tag from Def to a Def-expand tag group
 
         Parameters:
             def_tag (HedTag): Source hed tag that may be a Def or Def-expand tag.
-            def_expand_group (HedGroup or HedTag):
-            Source group for this def-expand tag.  Same as def_tag if this is not a def-expand tag.
+            def_expand_group (HedGroup or HedTag): Source group for this def-expand tag.
+                                                   Same as def_tag if this is not a def-expand tag.
             tag_validator (TagValidator): Used to validate the placeholder replacement.
+
         Returns:
-            issues
+            issues(list): Issues found from validating placeholders.
         """
         def_issues = []
         is_def_expand_tag = def_expand_group != def_tag
         is_label_tag = def_tag.extension
         placeholder = None
         found_slash = is_label_tag.find("/")
         if found_slash != -1:
@@ -71,31 +123,13 @@
             if def_tag_name:
                 if is_def_expand_tag and def_expand_group != def_contents:
                     def_issues += ErrorHandler.format_error(ValidationErrors.HED_DEF_EXPAND_INVALID,
                                                             tag=def_tag, actual_def=def_contents,
                                                             found_def=def_expand_group)
                 if def_entry.takes_value and tag_validator:
                     placeholder_tag = def_contents.get_first_group().find_placeholder_tag()
-                    error_code = ValidationErrors.DEF_INVALID
-                    if is_def_expand_tag:
-                        error_code = ValidationErrors.DEF_EXPAND_INVALID
-                    if placeholder_tag.is_unit_class_tag():
-                        def_issues += tag_validator.check_tag_unit_class_units_are_valid(placeholder_tag,
-                                                                                         report_as=def_tag,
-                                                                                         error_code=error_code)
-                    elif placeholder_tag.is_value_class_tag():
-                        def_issues += tag_validator.check_tag_value_class_valid(placeholder_tag,
-                                                                                report_as=def_tag,
-                                                                                error_code=error_code)
-
-            elif def_entry.takes_value:
-                error_code = ValidationErrors.HED_DEF_VALUE_MISSING
-                if is_def_expand_tag:
-                    error_code = ValidationErrors.HED_DEF_EXPAND_VALUE_MISSING
-                def_issues += ErrorHandler.format_error(error_code, tag=def_tag)
+                    def_issues += self._validate_def_units(def_tag, placeholder_tag, tag_validator,
+                                                           is_def_expand_tag)
             else:
-                error_code = ValidationErrors.HED_DEF_VALUE_EXTRA
-                if is_def_expand_tag:
-                    error_code = ValidationErrors.HED_DEF_EXPAND_VALUE_EXTRA
-                def_issues += ErrorHandler.format_error(error_code, tag=def_tag)
+                def_issues += self._report_missing_or_invalid_value(def_tag, def_entry, is_def_expand_tag)
 
-        return def_issues
+        return def_issues
```

### Comparing `hedtools-0.3.0/hed/validator/hed_validator.py` & `hedtools-0.3.1/hed/validator/hed_validator.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/validator/onset_validator.py` & `hedtools-0.3.1/hed/validator/onset_validator.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/validator/sidecar_validator.py` & `hedtools-0.3.1/hed/validator/sidecar_validator.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/validator/spreadsheet_validator.py` & `hedtools-0.3.1/hed/validator/spreadsheet_validator.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hed/validator/tag_validator.py` & `hedtools-0.3.1/hed/validator/tag_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,58 +287,64 @@
                                                            actual_error=actual_error)
         else:
             validation_issues += ErrorHandler.format_error(ValidationErrors.TAG_EXTENDED, tag=original_tag,
                                                            index_in_tag=len(original_tag.org_base_tag),
                                                            index_in_tag_end=None)
         return validation_issues
 
+    def _check_value_class(self, original_tag, stripped_value, report_as, error_code=None):
+        """Returns any issues found if this is a value tag"""
+        validation_issues = []
+        if original_tag.is_takes_value_tag() and \
+                not self._validate_value_class_portion(original_tag, stripped_value):
+            validation_issues += ErrorHandler.format_error(ValidationErrors.VALUE_INVALID, report_as)
+            if error_code:
+                validation_issues += ErrorHandler.format_error(ValidationErrors.VALUE_INVALID,
+                                                               report_as, actual_error=error_code)
+        return validation_issues
+
+    def _check_units(self, original_tag, bad_units, report_as):
+        """Returns an issue noting this is either bad units, or missing units"""
+        if bad_units:
+            tag_unit_class_units = original_tag.get_tag_unit_class_units()
+            validation_issue = ErrorHandler.format_error(ValidationErrors.UNITS_INVALID,
+                                                         tag=report_as, units=tag_unit_class_units)
+        else:
+            default_unit = original_tag.get_unit_class_default_unit()
+            validation_issue = ErrorHandler.format_error(ValidationErrors.UNITS_MISSING,
+                                                         tag=report_as, default_unit=default_unit)
+        return validation_issue
+
     def check_tag_unit_class_units_are_valid(self, original_tag, report_as=None, error_code=None):
         """ Report incorrect unit class or units.
 
         Parameters:
             original_tag (HedTag): The original tag that is used to report the error.
             report_as (HedTag): Report errors as coming from this tag, rather than original_tag.
             error_code (str): Override error codes to this
         Returns:
             list: Validation issues. Each issue is a dictionary.
         """
         validation_issues = []
         if original_tag.is_unit_class_tag():
             stripped_value, unit = original_tag.get_stripped_unit_value()
             if not unit:
-                bad_units = " " in original_tag.extension
-                had_error = False
                 # Todo: in theory this should separately validate the number and the units, for units
                 # that are prefixes like $.  Right now those are marked as unit invalid AND value_invalid.
+                bad_units = " " in original_tag.extension
+                report_as = report_as if report_as else original_tag
+
                 if bad_units:
                     stripped_value = stripped_value.split(" ")[0]
-                if original_tag.is_takes_value_tag() and\
-                        not self._validate_value_class_portion(original_tag, stripped_value):
-                    validation_issues += ErrorHandler.format_error(ValidationErrors.VALUE_INVALID,
-                                                                   report_as if report_as else original_tag)
-                    if error_code:
-                        had_error = True
-                        validation_issues += ErrorHandler.format_error(ValidationErrors.VALUE_INVALID,
-                                                                       report_as if report_as else original_tag,
-                                                                       actual_error=error_code)
 
-                if bad_units:
-                    tag_unit_class_units = original_tag.get_tag_unit_class_units()
-                    if tag_unit_class_units:
-                        validation_issues += ErrorHandler.format_error(ValidationErrors.UNITS_INVALID,
-                                                                       tag=report_as if report_as else original_tag,
-                                                                       units=tag_unit_class_units)
-                else:
-                    default_unit = original_tag.get_unit_class_default_unit()
-                    validation_issues += ErrorHandler.format_error(ValidationErrors.UNITS_MISSING,
-                                                                   tag=report_as if report_as else original_tag,
-                                                                   default_unit=default_unit)
+                validation_issues += self._check_value_class(original_tag, stripped_value, report_as, error_code)
+                validation_issues += self._check_units(original_tag, bad_units, report_as)
 
                 # We don't want to give this overall error twice
-                if error_code and not had_error:
+                if error_code and not any(error_code == issue['code'] for issue in validation_issues):
                     new_issue = validation_issues[0].copy()
                     new_issue['code'] = error_code
                     validation_issues += [new_issue]
 
         return validation_issues
 
     def check_tag_value_class_valid(self, original_tag, report_as=None, error_code=None):
```

### Comparing `hedtools-0.3.0/hed/validator/tag_validator_util.py` & `hedtools-0.3.1/hed/validator/tag_validator_util.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/hedtools.egg-info/PKG-INFO` & `hedtools-0.3.1/hedtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedtools
-Version: 0.3.0
+Version: 0.3.1
 Summary: HED validation, summary, and analysis tools.
 Home-page: https://github.com/hed-standard/hed-python/
 Author: VisLab, Ian Callanan, Jeremy Cockfield, Alexander Jones, Owen Winterberg, Kay Robbins
 Author-email: Kay.Robbins@utsa.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hedtools-0.3.0/hedtools.egg-info/SOURCES.txt` & `hedtools-0.3.1/hedtools.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 ./hed/schema/hed_cache.py
 ./hed/schema/hed_schema.py
 ./hed/schema/hed_schema_constants.py
 ./hed/schema/hed_schema_entry.py
 ./hed/schema/hed_schema_group.py
 ./hed/schema/hed_schema_io.py
 ./hed/schema/hed_schema_section.py
+./hed/schema/schema_attribute_validators.py
 ./hed/schema/schema_compliance.py
 ./hed/schema/schema_validation_util.py
 ./hed/schema/schema_data/HED8.0.0.xml
 ./hed/schema/schema_data/HED8.1.0.xml
 ./hed/schema/schema_data/HED8.2.0.xml
 ./hed/schema/schema_data/HED_score_1.0.0.xml
 ./hed/schema/schema_data/HED_testlib_1.0.2.xml
@@ -55,25 +56,25 @@
 ./hed/schema/schema_io/wiki_constants.py
 ./hed/schema/schema_io/xml2schema.py
 ./hed/schema/schema_io/xml_constants.py
 ./hed/tools/__init__.py
 ./hed/tools/analysis/__init__.py
 ./hed/tools/analysis/analysis_util.py
 ./hed/tools/analysis/annotation_util.py
+./hed/tools/analysis/column_name_summary.py
 ./hed/tools/analysis/event_manager.py
 ./hed/tools/analysis/file_dictionary.py
 ./hed/tools/analysis/hed_context_manager.py
 ./hed/tools/analysis/hed_tag_counts.py
 ./hed/tools/analysis/hed_type_counts.py
 ./hed/tools/analysis/hed_type_definitions.py
 ./hed/tools/analysis/hed_type_factors.py
 ./hed/tools/analysis/hed_type_manager.py
 ./hed/tools/analysis/hed_type_values.py
 ./hed/tools/analysis/key_map.py
-./hed/tools/analysis/tabular_column_name_summary.py
 ./hed/tools/analysis/tabular_summary.py
 ./hed/tools/analysis/temporal_event.py
 ./hed/tools/bids/__init__.py
 ./hed/tools/bids/bids_dataset.py
 ./hed/tools/bids/bids_file.py
 ./hed/tools/bids/bids_file_dictionary.py
 ./hed/tools/bids/bids_file_group.py
@@ -112,14 +113,17 @@
 ./hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py
 ./hed/tools/remodeling/operations/valid_operations.py
 ./hed/tools/util/__init__.py
 ./hed/tools/util/data_util.py
 ./hed/tools/util/hed_logger.py
 ./hed/tools/util/io_util.py
 ./hed/tools/util/schema_util.py
+./hed/tools/visualization/__init__.py
+./hed/tools/visualization/tag_word_cloud.py
+./hed/tools/visualization/word_cloud_util.py
 ./hed/validator/__init__.py
 ./hed/validator/def_validator.py
 ./hed/validator/hed_validator.py
 ./hed/validator/onset_validator.py
 ./hed/validator/sidecar_validator.py
 ./hed/validator/spreadsheet_validator.py
 ./hed/validator/tag_validator.py
@@ -153,14 +157,15 @@
 hed/schema/hed_cache.py
 hed/schema/hed_schema.py
 hed/schema/hed_schema_constants.py
 hed/schema/hed_schema_entry.py
 hed/schema/hed_schema_group.py
 hed/schema/hed_schema_io.py
 hed/schema/hed_schema_section.py
+hed/schema/schema_attribute_validators.py
 hed/schema/schema_compliance.py
 hed/schema/schema_validation_util.py
 hed/schema/schema_data/HED8.0.0.xml
 hed/schema/schema_data/HED8.1.0.xml
 hed/schema/schema_data/HED8.2.0.xml
 hed/schema/schema_data/HED_score_1.0.0.xml
 hed/schema/schema_data/HED_testlib_1.0.2.xml
@@ -173,25 +178,25 @@
 hed/schema/schema_io/wiki_constants.py
 hed/schema/schema_io/xml2schema.py
 hed/schema/schema_io/xml_constants.py
 hed/tools/__init__.py
 hed/tools/analysis/__init__.py
 hed/tools/analysis/analysis_util.py
 hed/tools/analysis/annotation_util.py
+hed/tools/analysis/column_name_summary.py
 hed/tools/analysis/event_manager.py
 hed/tools/analysis/file_dictionary.py
 hed/tools/analysis/hed_context_manager.py
 hed/tools/analysis/hed_tag_counts.py
 hed/tools/analysis/hed_type_counts.py
 hed/tools/analysis/hed_type_definitions.py
 hed/tools/analysis/hed_type_factors.py
 hed/tools/analysis/hed_type_manager.py
 hed/tools/analysis/hed_type_values.py
 hed/tools/analysis/key_map.py
-hed/tools/analysis/tabular_column_name_summary.py
 hed/tools/analysis/tabular_summary.py
 hed/tools/analysis/temporal_event.py
 hed/tools/bids/__init__.py
 hed/tools/bids/bids_dataset.py
 hed/tools/bids/bids_file.py
 hed/tools/bids/bids_file_dictionary.py
 hed/tools/bids/bids_file_group.py
@@ -230,14 +235,17 @@
 hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py
 hed/tools/remodeling/operations/valid_operations.py
 hed/tools/util/__init__.py
 hed/tools/util/data_util.py
 hed/tools/util/hed_logger.py
 hed/tools/util/io_util.py
 hed/tools/util/schema_util.py
+hed/tools/visualization/__init__.py
+hed/tools/visualization/tag_word_cloud.py
+hed/tools/visualization/word_cloud_util.py
 hed/validator/__init__.py
 hed/validator/def_validator.py
 hed/validator/hed_validator.py
 hed/validator/onset_validator.py
 hed/validator/sidecar_validator.py
 hed/validator/spreadsheet_validator.py
 hed/validator/tag_validator.py
```

### Comparing `hedtools-0.3.0/setup.cfg` & `hedtools-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hedtools-0.3.0/versioneer.py` & `hedtools-0.3.1/versioneer.py`

 * *Files identical despite different names*

