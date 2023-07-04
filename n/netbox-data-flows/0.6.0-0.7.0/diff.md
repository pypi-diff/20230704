# Comparing `tmp/netbox-data-flows-0.6.0.tar.gz` & `tmp/netbox-data-flows-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-data-flows-0.6.0.tar", last modified: Tue Jun  6 20:55:18 2023, max compression
+gzip compressed data, was "netbox-data-flows-0.7.0.tar", last modified: Tue Jul  4 16:23:31 2023, max compression
```

## Comparing `netbox-data-flows-0.6.0.tar` & `netbox-data-flows-0.7.0.tar`

### file list

```diff
@@ -1,107 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.978301 netbox-data-flows-0.6.0/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.978301 netbox-data-flows-0.6.0/netbox_data_flows/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.978301 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.982302 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/addins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.982302 netbox-data-flows-0.6.0/netbox_data_flows/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.982302 netbox-data-flows-0.6.0/netbox_data_flows/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/graphql/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/graphql/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/graphql/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/graphql/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.982302 netbox-data-flows-0.6.0/netbox_data_flows/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.982302 netbox-data-flows-0.6.0/netbox_data_flows/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.986302 netbox-data-flows-0.6.0/netbox_data_flows/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0002_alter_objectalias_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0007_remove_objectalias_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.986302 netbox-data-flows-0.6.0/netbox_data_flows/models/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/models/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/models/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/models/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/models/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.986302 netbox-data-flows-0.6.0/netbox_data_flows/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/tables/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/tables/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/tables/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/tables/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.974301 netbox-data-flows-0.6.0/netbox_data_flows/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/application.html
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/inc/
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/inc/dataflow_specifications.html
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/objectalias_tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/netbox_data_flows/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/utils/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/netbox_data_flows/views/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.978301 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-06 20:55:18.000000 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-06 20:55:18.000000 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:55:18.000000 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:55:18.000000 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 20:55:18.000000 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.551177 netbox-data-flows-0.7.0/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.551177 netbox-data-flows-0.7.0/netbox_data_flows/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/addins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/graphql/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/graphql/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/graphql/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/graphql/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.559177 netbox-data-flows-0.7.0/netbox_data_flows/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0002_alter_objectalias_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0007_remove_objectalias_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.559177 netbox-data-flows-0.7.0/netbox_data_flows/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/models/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/models/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/models/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/models/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.559177 netbox-data-flows-0.7.0/netbox_data_flows/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/tables/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/tables/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/tables/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/tables/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.551177 netbox-data-flows-0.7.0/netbox_data_flows/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/application.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/netbox_data_flows/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/netbox_data_flows/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/model_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.551177 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-04 16:23:31.000000 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-04 16:23:31.000000 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:23:31.000000 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:23:31.000000 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 16:23:31.000000 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/setup.cfg
```

### Comparing `netbox-data-flows-0.6.0/LICENSE` & `netbox-data-flows-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/PKG-INFO` & `netbox-data-flows-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.6.0
+Version: 0.7.0
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `netbox-data-flows-0.6.0/README.md` & `netbox-data-flows-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/__init__.py` & `netbox-data-flows-0.7.0/netbox_data_flows/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from extras.plugins import PluginConfig
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 
 class DataFlowsConfig(PluginConfig):
     name = "netbox_data_flows"
     verbose_name = "Data Flows"
-    description = "NetBox plugin to document data flows between systems and applications."
+    description = (
+        "NetBox plugin to document data flows between "
+        "systems and applications."
+    )
     version = __version__
     base_url = "data-flows"
     author = "Thomas Fargeix"
     required_settings = []
     default_settings = {}
     min_version = "3.5.0"
     max_version = "3.5.99"
 
     def ready(self):
-        from . import signals
+        from . import signals  # noqa: F401
 
         super().ready()
 
 
 config = DataFlowsConfig
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/applications.py` & `netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from rest_framework import serializers
 
 from netbox.api.serializers import NetBoxModelSerializer
 
-from netbox_data_flows import models, choices
+from netbox_data_flows import models
 
-from .nested import *
+from . import nested
 
 
 __all__ = (
     "ApplicationSerializer",
     "ApplicationRoleSerializer",
 )
 
@@ -37,15 +37,15 @@
 
 
 class ApplicationSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_data_flows-api:application-detail"
     )
     dataflow_count = serializers.IntegerField(read_only=True)
-    role = NestedApplicationRoleSerializer()
+    role = nested.NestedApplicationRoleSerializer()
 
     class Meta:
         model = models.Application
         fields = (
             "id",
             "url",
             "display",
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/dataflows.py` & `netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/groups.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,55 @@
 from rest_framework import serializers
 
-from netbox.api.fields import ChoiceField, SerializedPKRelatedField
+from netbox.api.fields import ChoiceField
 from netbox.api.serializers import NetBoxModelSerializer
 
 from netbox_data_flows import models, choices
 
-from .nested import *
+from . import nested
 
 
-__all__ = ("DataFlowSerializer",)
+__all__ = ("DataFlowGroupSerializer",)
 
 
-class DataFlowSerializer(NetBoxModelSerializer):
+class DataFlowGroupSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_data_flows-api:dataflow-detail"
-    )
-
-    application = NestedApplicationSerializer(
-        required=False, allow_null=True, default=None
-    )
-    group = NestedDataFlowGroupSerializer(
-        required=False, allow_null=True, default=None
-    )
-    recursive_group = NestedDataFlowGroupSerializer(
-        required=False, allow_null=True, default=None
+        view_name="plugins-api:netbox_data_flows-api:dataflowgroup-detail"
     )
 
     status = ChoiceField(choices=choices.DataFlowStatusChoices, required=False)
     inherited_status = ChoiceField(
         choices=choices.DataFlowInheritedStatusChoices,
         required=False,
         read_only=True,
     )
-    protocol = ChoiceField(
-        choices=choices.DataFlowProtocolChoices, required=False
-    )
 
-    sources = SerializedPKRelatedField(
-        queryset=models.ObjectAlias.objects.all(),
-        serializer=NestedObjectAliasSerializer,
-        required=False,
-        many=True,
+    application = nested.NestedApplicationSerializer(
+        required=False, allow_null=True, default=None
     )
-    destinations = SerializedPKRelatedField(
-        queryset=models.ObjectAlias.objects.all(),
-        serializer=NestedObjectAliasSerializer,
-        required=False,
-        many=True,
+    parent = nested.NestedDataFlowGroupSerializer(
+        required=False, allow_null=True, default=None
+    )
+    ancestor = nested.NestedDataFlowGroupSerializer(
+        required=False, allow_null=True, default=None
     )
 
     class Meta:
-        model = models.DataFlow
+        model = models.DataFlowGroup
         fields = (
             "id",
             "url",
             "display",
+            "slug",
             "application",
-            "group",
-            "recursive_group",
+            "parent",
+            "ancestor",
             "name",
             "description",
             "status",
             "inherited_status",
             "comments",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
-            "protocol",
-            "source_ports",
-            "destination_ports",
-            "sources",
-            "destinations",
         )
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/groups.py` & `netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/dataflows.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,75 @@
 from rest_framework import serializers
 
 from netbox.api.fields import ChoiceField, SerializedPKRelatedField
 from netbox.api.serializers import NetBoxModelSerializer
 
 from netbox_data_flows import models, choices
 
-from .nested import *
+from . import nested
 
 
-__all__ = ("DataFlowGroupSerializer",)
+__all__ = ("DataFlowSerializer",)
 
 
-class DataFlowGroupSerializer(NetBoxModelSerializer):
+class DataFlowSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_data_flows-api:dataflowgroup-detail"
+        view_name="plugins-api:netbox_data_flows-api:dataflow-detail"
+    )
+
+    application = nested.NestedApplicationSerializer(
+        required=False, allow_null=True, default=None
+    )
+    group = nested.NestedDataFlowGroupSerializer(
+        required=False, allow_null=True, default=None
+    )
+    recursive_group = nested.NestedDataFlowGroupSerializer(
+        required=False, allow_null=True, default=None
     )
 
     status = ChoiceField(choices=choices.DataFlowStatusChoices, required=False)
     inherited_status = ChoiceField(
         choices=choices.DataFlowInheritedStatusChoices,
         required=False,
         read_only=True,
     )
-
-    application = NestedApplicationSerializer(
-        required=False, allow_null=True, default=None
+    protocol = ChoiceField(
+        choices=choices.DataFlowProtocolChoices, required=False
     )
-    parent = NestedDataFlowGroupSerializer(
-        required=False, allow_null=True, default=None
+
+    sources = SerializedPKRelatedField(
+        queryset=models.ObjectAlias.objects.all(),
+        serializer=nested.NestedObjectAliasSerializer,
+        required=False,
+        many=True,
     )
-    ancestor = NestedDataFlowGroupSerializer(
-        required=False, allow_null=True, default=None
+    destinations = SerializedPKRelatedField(
+        queryset=models.ObjectAlias.objects.all(),
+        serializer=nested.NestedObjectAliasSerializer,
+        required=False,
+        many=True,
     )
 
     class Meta:
-        model = models.DataFlowGroup
+        model = models.DataFlow
         fields = (
             "id",
             "url",
             "display",
-            "slug",
             "application",
-            "parent",
-            "ancestor",
+            "group",
+            "recursive_group",
             "name",
             "description",
             "status",
             "inherited_status",
             "comments",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
+            "protocol",
+            "source_ports",
+            "destination_ports",
+            "sources",
+            "destinations",
         )
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/nested.py` & `netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/nested.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/objectaliases.py` & `netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/objectaliases.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from rest_framework import serializers
 
-from netbox.api.fields import ChoiceField, SerializedPKRelatedField
+from netbox.api.fields import SerializedPKRelatedField
 from netbox.api.serializers import (
     NetBoxModelSerializer,
     GenericObjectSerializer,
 )
 
-from netbox_data_flows import models, choices
-
-from .nested import *
+from netbox_data_flows import models
 
 
 __all__ = (
     "ObjectAliasTargetSerializer",
     "ObjectAliasSerializer",
 )
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/api/urls.py` & `netbox-data-flows-0.7.0/netbox_data_flows/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/api/views.py` & `netbox-data-flows-0.7.0/netbox_data_flows/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from django.db.models import Count
 from rest_framework.routers import APIRootView
-from rest_framework.viewsets import ModelViewSet
 
 from netbox.api.viewsets import NetBoxModelViewSet
 
 from netbox_data_flows import filtersets, models
 
 from . import serializers
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/choices.py` & `netbox-data-flows-0.7.0/netbox_data_flows/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/addins.py` & `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/addins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from django.db.models import Q
 from django_filters import FilterSet
 
 from netbox_data_flows import models, choices
 
 from .filters import ModelMultipleChoiceFilter, ChoiceFilter
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/applications.py` & `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/applications.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     NetBoxModelFilterSet,
     OrganizationalModelFilterSet,
 )
 from tenancy.filtersets import ContactModelFilterSet
 
 from netbox_data_flows import models
 
-from .filters import *
+from .filters import ModelMultipleChoiceFilter
 
 
 __all__ = (
     "ApplicationFilterSet",
     "ApplicationRoleFilterSet",
 )
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/dataflows.py` & `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/dataflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from django.db.models import Q
-from django_filters import FilterSet
 
 from netbox.filtersets import NetBoxModelFilterSet
 
 from dcim.models import Device
 from ipam.models import Prefix, IPRange, IPAddress
 from virtualization.models import VirtualMachine
 
 from netbox_data_flows import models, choices
 
-from .addins import *
-from .filters import *
+from .addins import ApplicationFilterSetAddin, InheritedStatusFilterSetAddin
+from .filters import (
+    ChoiceFilter,
+    ModelMultipleChoiceFilter,
+    MultipleChoiceFilter,
+    MultiValueNumberFilter,
+    MultiValueNumericArrayFilter,
+)
 
 __all__ = ("DataFlowFilterSet",)
 
 
 class DataFlowFilterSet(
     ApplicationFilterSetAddin,
     InheritedStatusFilterSetAddin,
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/filters.py` & `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/groups.py` & `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.db.models import Q
 
 from netbox.filtersets import NetBoxModelFilterSet
 
 from netbox_data_flows import models
 
-from .addins import *
-from .filters import *
+from .addins import ApplicationFilterSetAddin, InheritedStatusFilterSetAddin
+from .filters import ModelMultipleChoiceFilter
 
 __all__ = ("DataFlowGroupFilterSet",)
 
 
 class DataFlowGroupFilterSet(
     ApplicationFilterSetAddin,
     InheritedStatusFilterSetAddin,
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/objectaliases.py` & `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/objectaliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dcim.models import Device
 from ipam.models import Prefix, IPRange, IPAddress
 from virtualization.models import VirtualMachine
 
 from netbox_data_flows import models
 from netbox_data_flows.utils.helpers import get_device_ipaddresses
 
-from .filters import *
+from .filters import ModelMultipleChoiceFilter
 
 
 __all__ = (
     "ObjectAliasTargetFilterSet",
     "ObjectAliasFilterSet",
 )
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/forms/applicationroles.py` & `netbox-data-flows-0.7.0/netbox_data_flows/forms/applicationroles.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     ApplicationRole,
 )
 
 __all__ = (
     "ApplicationRoleForm",
     "ApplicationRoleBulkEditForm",
     "ApplicationRoleImportForm",
+    "ApplicationRoleFilterForm",
 )
 
 #
 # Object forms
 #
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/forms/applications.py` & `netbox-data-flows-0.7.0/netbox_data_flows/forms/applications.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     NetBoxModelImportForm,
 )
 from tenancy.forms import ContactModelFilterForm
 from utilities.forms.fields import (
     CommentField,
     CSVModelChoiceField,
     DynamicModelChoiceField,
-    DynamicModelMultipleChoiceField,
     TagFilterField,
 )
 
 from netbox_data_flows.models import (
     Application,
     ApplicationRole,
 )
@@ -31,15 +30,17 @@
 #
 # Object forms
 #
 
 
 class ApplicationForm(NetBoxModelForm):
     role = DynamicModelChoiceField(
-        queryset=ApplicationRole.objects.all(), required=False
+        queryset=ApplicationRole.objects.all(),
+        required=False,
+        selector=True,
     )
     comments = CommentField()
 
     fieldsets = (
         (
             "Application",
             (
@@ -68,29 +69,33 @@
 
 
 class ApplicationBulkEditForm(NetBoxModelBulkEditForm):
     model = Application
 
     description = forms.CharField(max_length=200, required=False)
     role = DynamicModelChoiceField(
-        queryset=ApplicationRole.objects.all(), required=False
+        queryset=ApplicationRole.objects.all(),
+        required=False,
+        selector=True,
     )
+    comments = CommentField()
 
     fieldsets = (
         (
             "Application",
             (
                 "role",
                 "description",
             ),
         ),
     )
     nullable_fields = (
         "role",
         "description",
+        "comments",
     )
 
 
 class ApplicationImportForm(NetBoxModelImportForm):
     role = CSVModelChoiceField(
         queryset=ApplicationRole.objects.all(),
         required=False,
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/forms/dataflows.py` & `netbox-data-flows-0.7.0/netbox_data_flows/forms/dataflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,38 +39,49 @@
 #
 
 
 class DataFlowForm(NetBoxModelForm):
     application = DynamicModelChoiceField(
         queryset=models.Application.objects.all(),
         required=False,
+        selector=True,
         help_text="Application that this data flow is part of.",
     )
     group = DynamicModelChoiceField(
         queryset=models.DataFlowGroup.objects.all(),
         required=False,
+        selector=True,
         query_params={
             "application_id": "$application",
         },
-        help_text="Parent group of this Data Flow. Disabling the group will disable this data flow.",
+        help_text=(
+            "Parent group of this Data Flow. "
+            "Disabling the group will disable this data flow."
+        ),
     )
 
     comments = CommentField()
     source_ports = NumericArrayField(
         base_field=forms.IntegerField(
             min_value=SERVICE_PORT_MIN, max_value=SERVICE_PORT_MAX
         ),
-        help_text="Comma-separated list of one or more port numbers. A range may be specified using a hyphen.",
+        help_text=(
+            "Comma-separated list of one or more port numbers. "
+            "A range may be specified using a hyphen."
+        ),
         required=False,
     )
     destination_ports = NumericArrayField(
         base_field=forms.IntegerField(
             min_value=SERVICE_PORT_MIN, max_value=SERVICE_PORT_MAX
         ),
-        help_text="Comma-separated list of one or more port numbers. A range may be specified using a hyphen.",
+        help_text=(
+            "Comma-separated list of one or more port numbers. "
+            "A range may be specified using a hyphen."
+        ),
         required=False,
     )
 
     sources = DynamicModelMultipleChoiceField(
         queryset=models.ObjectAlias.objects.all(),
         required=False,
     )
@@ -119,37 +130,42 @@
             "sources",
             "destinations",
         )
         widgets = {
             "protocol": forms.Select(),
         }
         help_texts = {
-            "status": "Status of the data group. If its group is disabled, the data flow will also be disabled."
+            "status": (
+                "Status of the data group. If its group is disabled, "
+                "the data flow will also be disabled."
+            )
         }
 
 
 #
 # Bulk forms
 #
 
 
 class DataFlowBulkEditForm(NetBoxModelBulkEditForm):
     model = models.DataFlow
 
+    description = forms.CharField(max_length=200, required=False)
     application = DynamicModelChoiceField(
         queryset=models.Application.objects.all(),
         required=False,
     )
     group = DynamicModelChoiceField(
         queryset=models.DataFlowGroup.objects.all(),
         required=False,
         query_params={
             "application_id": "$application",
         },
     )
+    comments = CommentField()
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
         widget=forms.Select(),
     )
     protocol = forms.ChoiceField(
@@ -157,22 +173,28 @@
         required=False,
         widget=forms.Select(),
     )
     source_ports = NumericArrayField(
         base_field=forms.IntegerField(
             min_value=SERVICE_PORT_MIN, max_value=SERVICE_PORT_MAX
         ),
-        help_text="Comma-separated list of one or more port numbers. A range may be specified using a hyphen.",
+        help_text=(
+            "Comma-separated list of one or more port numbers. "
+            "A range may be specified using a hyphen."
+        ),
         required=False,
     )
     destination_ports = NumericArrayField(
         base_field=forms.IntegerField(
             min_value=SERVICE_PORT_MIN, max_value=SERVICE_PORT_MAX
         ),
-        help_text="Comma-separated list of one or more port numbers. A range may be specified using a hyphen.",
+        help_text=(
+            "Comma-separated list of one or more port numbers. "
+            "A range may be specified using a hyphen."
+        ),
         required=False,
     )
 
     sources = DynamicModelMultipleChoiceField(
         queryset=models.ObjectAlias.objects.all(),
         required=False,
     )
@@ -183,15 +205,14 @@
 
     fieldsets = (
         (
             "Data Flow",
             (
                 "application",
                 "group",
-                "name",
                 "description",
                 "status",
             ),
         ),
         (
             "Specifications",
             (
@@ -203,14 +224,15 @@
             ),
         ),
     )
     nullable_fields = (
         "application",
         "group",
         "description",
+        "comments",
         "protocol",
         "source_ports",
         "destination_ports",
         "sources",
         "destinations",
     )
 
@@ -235,22 +257,28 @@
         choices=add_blank_choice(choices.DataFlowProtocolChoices),
         required=True,
     )
     source_ports = NumericArrayField(
         base_field=forms.IntegerField(
             min_value=SERVICE_PORT_MIN, max_value=SERVICE_PORT_MAX
         ),
-        help_text="Comma-separated list of one or more port numbers. A range may be specified using a hyphen.",
+        help_text=(
+            "Comma-separated list of one or more port numbers. "
+            "A range may be specified using a hyphen."
+        ),
         required=False,
     )
     destination_ports = NumericArrayField(
         base_field=forms.IntegerField(
             min_value=SERVICE_PORT_MIN, max_value=SERVICE_PORT_MAX
         ),
-        help_text="Comma-separated list of one or more port numbers. A range may be specified using a hyphen.",
+        help_text=(
+            "Comma-separated list of one or more port numbers. "
+            "A range may be specified using a hyphen."
+        ),
         required=False,
     )
 
     sources = CSVModelMultipleChoiceField(
         queryset=models.ObjectAlias.objects.all(),
         required=False,
         to_field_name="name",
@@ -463,15 +491,18 @@
                 "source_ipranges",
                 "source_ipaddresses",
                 "source_devices",
                 "source_virtual_machines",
             ),
         ),
         (
-            "Destinations - all destinations are OR'ed together, any will match",
+            (
+                "Destinations - all destinations are OR'ed together, "
+                "any will match"
+            ),
             (
                 "destination_is_null",
                 "destination_aliases",
                 "destination_prefixes",
                 "destination_ipranges",
                 "destination_ipaddresses",
                 "destination_devices",
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/forms/groups.py` & `netbox-data-flows-0.7.0/netbox_data_flows/forms/groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from utilities.forms import add_blank_choice
 from utilities.forms.fields import (
     CommentField,
     CSVChoiceField,
     CSVModelChoiceField,
     DynamicModelChoiceField,
     DynamicModelMultipleChoiceField,
-    MultipleChoiceField,  # TODO: deprecated, remove for 3.6.0
-    NumericArrayField,
     SlugField,
     TagFilterField,
 )
 
 from netbox_data_flows import models, choices
 
 
@@ -35,19 +33,24 @@
 
 
 class DataFlowGroupForm(NetBoxModelForm):
     slug = SlugField()
     application = DynamicModelChoiceField(
         queryset=models.Application.objects.all(),
         required=False,
-        help_text="Application that this data flow group (and all of its descendants) is part of.",
+        selector=True,
+        help_text=(
+            "Application that this data flow group (and all of its "
+            "descendants) is part of."
+        ),
     )
     parent = DynamicModelChoiceField(
         queryset=models.DataFlowGroup.objects.all(),
         required=False,
+        selector=True,
         help_text="Parent group of this Data Flow Group.",
         query_params={
             "application_id": "$application",
         },
     )
     comments = CommentField()
 
@@ -74,34 +77,41 @@
             "name",
             "description",
             "status",
             "comments",
             "tags",
         )
         help_texts = {
-            "status": "Status of the data flow group. Disabling a parent disables all its descendants and their data flows."
+            "status": (
+                "Status of the data flow group. Disabling a parent disables "
+                "all its descendants and their data flows."
+            )
         }
 
 
 #
 # Bulk forms
 #
 
 
 class DataFlowGroupBulkEditForm(NetBoxModelBulkEditForm):
     model = models.DataFlowGroup
 
+    description = forms.CharField(max_length=200, required=False)
     application = DynamicModelChoiceField(
         queryset=models.Application.objects.all(),
         required=False,
+        selector=True,
     )
     parent = DynamicModelChoiceField(
         queryset=models.DataFlowGroup.objects.all(),
         required=False,
+        selector=True,
     )
+    comments = CommentField()
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
         widget=forms.Select(),
     )
 
@@ -109,21 +119,21 @@
         (
             "Data Flow Groups",
             (
                 "application",
                 "parent",
                 "description",
                 "status",
-                "tags",
             ),
         ),
     )
     nullable_fields = (
         "parent",
         "application",
+        "comments",
     )
 
 
 class DataFlowGroupImportForm(NetBoxModelImportForm):
     application = DynamicModelChoiceField(
         queryset=models.Application.objects.all(),
         required=False,
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/forms/objectaliases.py` & `netbox-data-flows-0.7.0/netbox_data_flows/forms/objectaliases.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,19 @@
                 "tags",
             ),
         ),
     )
 
     class Meta:
         model = models.ObjectAlias
-        fields = ("name", "description", "tags")
+        fields = (
+            "name",
+            "description",
+            "tags",
+        )
 
 
 #
 # Bulk forms
 #
 
 
@@ -145,19 +149,24 @@
     aliased_fields = (
         "aliased_prefixes",
         "aliased_ipranges",
         "aliased_ipaddresses",
     )
 
     aliased_prefixes = DynamicModelMultipleChoiceField(
-        queryset=Prefix.objects.all(), required=False, label="Aliased Prefixes"
+        queryset=Prefix.objects.all(),
+        required=False,
+        selector=True,
+        label="Aliased Prefixes",
     )
     aliased_ipranges = DynamicModelMultipleChoiceField(
         queryset=IPRange.objects.all(),
         required=False,
+        selector=True,
         label="Aliased IP Ranges",
     )
     aliased_ipaddresses = DynamicModelMultipleChoiceField(
         queryset=IPAddress.objects.all(),
         required=False,
+        selector=True,
         label="Aliased IP Addresses",
     )
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/graphql/__init__.py` & `netbox-data-flows-0.7.0/netbox_data_flows/graphql/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from graphene import ObjectType
 
 from netbox.graphql.fields import ObjectField, ObjectListField
 
-from .applications import *
-from .dataflows import *
-from .groups import *
-from .objectaliases import *
+from .applications import ApplicationRoleType, ApplicationType
+from .dataflows import DataFlowType
+from .groups import DataFlowGroupType
+from .objectaliases import ObjectAliasType, ObjectAliasTargetType
 
 
 class Query(ObjectType):
     application_role = ObjectField(ApplicationRoleType)
     application_role_list = ObjectListField(ApplicationRoleType)
 
     application = ObjectField(ApplicationType)
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/graphql/applications.py` & `netbox-data-flows-0.7.0/netbox_data_flows/graphql/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/graphql/objectaliases.py` & `netbox-data-flows-0.7.0/netbox_data_flows/graphql/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py` & `netbox-data-flows-0.7.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
                     f"Identified {len(orphaned)} orphaned aliases."
                 )
                 sys.exit(1)
             else:
                 ObjectAliasTarget.objects.filter(pk__in=orphaned).delete()
                 self.stdout.write(f"Deleted {len(orphaned)} orphaned aliases.")
         else:
-            self.stdout.write(f"No orphaned aliases to delete.")
+            self.stdout.write("No orphaned aliases to delete.")
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/migrations/0001_initial.py` & `netbox-data-flows-0.7.0/netbox_data_flows/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py` & `netbox-data-flows-0.7.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py` & `netbox-data-flows-0.7.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py` & `netbox-data-flows-0.7.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/models/applications.py` & `netbox-data-flows-0.7.0/netbox_data_flows/models/applications.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from django.contrib.contenttypes.fields import GenericRelation
-from django.contrib.postgres.fields import ArrayField
 from django.db import models
 from django.urls import reverse
 
 from netbox.models import NetBoxModel, OrganizationalModel
 
 
 __all__ = (
     "ApplicationRole",
     "Application",
 )
 
 
 class ApplicationRole(OrganizationalModel):
-    """Functional role of an application, e.g.: "Infrastructure", "Management", "Business" """
+    """
+    Functional role of an application,
+    e.g.: "Infrastructure", "Management", "Business"
+    """
 
     # Inherited fields:
     # name - unique
     # slug - unique
     # description
 
     def __str__(self):
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/models/dataflows.py` & `netbox-data-flows-0.7.0/netbox_data_flows/models/dataflows.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,29 +35,41 @@
 
     def only_enabled(self):
         disabled_groups = DataFlowGroup.objects.only_disabled().only("pk")
         return self.filter(
             status=DataFlowStatusChoices.STATUS_ENABLED
         ).exclude(group_id__in=disabled_groups)
 
-    def part_of_group_recursive(self, *dataflowgroups):
+    def part_of_group_recursive(
+        self, *dataflowgroups, include_direct_children=True
+    ):
         group_ids = [getattr(dfg, "pk", dfg) for dfg in dataflowgroups]
         subgroups = (
             DataFlowGroup.objects.filter(pk__in=group_ids)
-            .get_descendants(include_self=True)
+            .get_descendants(include_self=include_direct_children)
             .only("pk")
         )
         return self.filter(group_id__in=subgroups)
 
-    def source_or_destination(self, *targets):
+    def sources_or_destinations(self, *targets):
         return self.filter(
             models.Q(sources__in=ObjectAlias.objects.contains(*targets))
             | models.Q(destinations__in=ObjectAlias.objects.contains(*targets))
         ).distinct()
 
+    def sources(self, *targets):
+        return self.filter(
+            models.Q(sources__in=ObjectAlias.objects.contains(*targets))
+        ).distinct()
+
+    def destinations(self, *targets):
+        return self.filter(
+            models.Q(destinations__in=ObjectAlias.objects.contains(*targets))
+        ).distinct()
+
 
 class DataFlow(NetBoxModel):
     """Representation of a data flow for an application"""
 
     name = models.CharField(max_length=200)
     description = models.CharField(
         max_length=500,
@@ -212,11 +224,17 @@
 
         if self.group and self.group.application != self.application:
             if not self.application:
                 self.application = self.group.application
             else:
                 raise ValidationError(
                     {
-                        "application": "The application of the data flow must match the application of its group.",
-                        "group": "The application of the group must match the application of the data flow.",
+                        "application": (
+                            "The application of the data flow must match "
+                            "the application of its group."
+                        ),
+                        "group": (
+                            "The application of the group must match the "
+                            "application of the data flow."
+                        ),
                     }
                 )
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/models/groups.py` & `netbox-data-flows-0.7.0/netbox_data_flows/models/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,16 +117,22 @@
 
         if self.parent and self.parent.application != self.application:
             if not self.application:
                 self.application = self.parent.application
             else:
                 raise ValidationError(
                     {
-                        "application": "The application of the data flow must match the application of its parent.",
-                        "parent": "The application of the parent must match the application of the data flow.",
+                        "application": (
+                            "The application of the data flow must match "
+                            "the application of its parent."
+                        ),
+                        "parent": (
+                            "The application of the parent must match the "
+                            "application of the data flow."
+                        ),
                     }
                 )
 
         # update all our descendants' application
         if self.pk:
             self.get_descendants().update(application_id=self.application)
 
@@ -136,12 +142,15 @@
             if groups.filter(
                 name=self.name,
                 application=self.application,
                 parent__isnull=True,
             ).exists():
                 raise ValidationError(
                     {
-                        "name": "A data flow with this name already exists for this application."
+                        "name": (
+                            "A data flow with this name already exists for "
+                            "this application."
+                        )
                     }
                 )
 
         super().validate_unique(exclude=exclude)
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/models/objectaliases.py` & `netbox-data-flows-0.7.0/netbox_data_flows/models/objectaliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import math
-
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
-from django.contrib.postgres.fields import ArrayField
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.urls import reverse
 
 from netbox.models import NetBoxModel
 from utilities.querysets import RestrictedQuerySet
 
@@ -55,15 +52,15 @@
                 query |= models.Q(target_type=ct, target_id=t.pk)
             else:
                 try:
                     ip_addresses = get_device_ipaddresses(t)
                 except Exception as e:
                     raise Exception(
                         f"Cannot test if {self.__class__} contains {t}"
-                    )
+                    ) from e
 
                 if ip_addresses:
                     ip_ct = ContentType.objects.get_for_model(
                         ip_addresses[0].__class__
                     )
 
                     for ip in ip_addresses:
@@ -86,15 +83,15 @@
     def get_or_create(cls, target):
         """Return an existing instance for this target or create one"""
         instance = cls.objects.contains(target).first()
         if not instance:
             ct = ContentType.objects.get_for_model(target.__class__)
             type = (ct.app_label, ct.model)
 
-            if not type in OBJECTALIAS_ASSIGNMENT_MODELS:
+            if type not in OBJECTALIAS_ASSIGNMENT_MODELS:
                 raise TypeError(
                     f"Unsupported type {':'.join(type)} for ObjectAliasTarget"
                 )
 
             instance = cls(target=target)
 
         return instance
@@ -131,15 +128,14 @@
     @property
     def type_verbose_name(self):
         return self.target._meta.verbose_name
 
     @property
     def name(self):
         if self._model == "ipaddress":
-            address = str(self.target).split("/")[0]
             if self.parent:
                 return f"{self.target} ({self.parent})"
             else:
                 return str(self.target)
         else:
             return str(self.target)
 
@@ -158,27 +154,28 @@
         else:
             return None
 
     @property
     def family(self):
         try:
             return self.target.family
-        except:
+        except AttributeError:
             return None
 
     @property
     def _model(self):
         return self.target_type.model
 
     def __contains__(self, other: "ObjectAliasTarget"):
         """Return True if other is fully contained in this ObjectAliasTarget"""
 
         if not isinstance(other, self.__class__):
             raise TypeError(
-                f"{self.__class__} can only be compared to other {self.__class__}, not {type(other)}"
+                f"{self.__class__} can only be compared to other "
+                f"{self.__class__}, not {type(other)}"
             )
 
         attr_mapping = {
             "ipaddress": "address",
             "iprange": "range",
             "prefix": "prefix",
         }
@@ -203,15 +200,15 @@
             )
 
         return other_value in own_value
 
     def save(self, *args, **kwargs):
         if self.target_type:
             type = (self.target_type.app_label, self.target_type.model)
-            if not type in OBJECTALIAS_ASSIGNMENT_MODELS:
+            if type not in OBJECTALIAS_ASSIGNMENT_MODELS:
                 raise ValidationError(
                     f"Unsupported type {':'.join(type)} for ObjectAliasTarget"
                 )
 
         super().save(*args, **kwargs)
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/navigation.py` & `netbox-data-flows-0.7.0/netbox_data_flows/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/search.py` & `netbox-data-flows-0.7.0/netbox_data_flows/search.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/tables/applications.py` & `netbox-data-flows-0.7.0/netbox_data_flows/tables/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import django_tables2 as tables
 
 from netbox.tables import (
-    ChoiceFieldColumn,
     columns,
     NetBoxTable,
 )
 from tenancy.tables import ContactsColumnMixin
 
 from netbox_data_flows.models import Application, ApplicationRole
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/tables/dataflows.py` & `netbox-data-flows-0.7.0/netbox_data_flows/tables/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/tables/groups.py` & `netbox-data-flows-0.7.0/netbox_data_flows/tables/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/tables/objectaliases.py` & `netbox-data-flows-0.7.0/netbox_data_flows/tables/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/application.html` & `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/application.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html` & `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html` & `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html` & `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html` & `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html` & `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
   </div>
   {% endif %}
 
   {% if dataflows_recursive_table %}
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Data Flows (direct and recursive members)</h5>
+        <h5 class="card-header">Data Flows (child groups' members)</h5>
         <div class="card-body table-responsive">
           {% render_table dataflows_recursive_table %}
         </div>
       </div>
     </div>
   </div>
   {% endif %}
```

#### html2text {}

```diff
@@ -14,12 +14,12 @@
 ** Child Groups **
 {% render_table children_table %}
 {% plugin_right_page object %}
 {% if dataflows_table %}
 ** Data Flows (direct members) **
 {% render_table dataflows_table %}
 {% endif %} {% if dataflows_recursive_table %}
-** Data Flows (direct and recursive members) **
+** Data Flows (child groups' members) **
 {% render_table dataflows_recursive_table %}
 {% endif %}
 {% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html` & `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html` & `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/urls.py` & `netbox-data-flows-0.7.0/netbox_data_flows/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from django.urls import include, path
 
-from netbox.views.generic import ObjectChangeLogView, ObjectJournalView
 from utilities.urls import get_model_urls
 
-from . import models, views
+from . import views
 
 
 urlpatterns = tuple()
 
 # Application Roles
 urlpatterns += (
     path(
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/utils/aliases.py` & `netbox-data-flows-0.7.0/netbox_data_flows/utils/aliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import logging
-from copy import deepcopy
 
 from django import forms
 from django.contrib import messages
 from django.db import transaction
 from django.db.models import ProtectedError
 from django.shortcuts import get_object_or_404, render, redirect
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
-from django.views.generic import View
 
 from netbox.views import generic as generic_views
 from extras.signals import clear_webhooks
+from utilities.error_handlers import handle_protectederror
 from utilities.exceptions import AbortRequest, PermissionsViolation
 from utilities.forms import (
     restrict_form_fields,
     ConfirmationForm,
     BootstrapMixin,
 )
 from utilities.permissions import get_permission_for_model
@@ -124,15 +123,16 @@
                     form.pre_save_object(form, obj, aliases)
                     obj.save()
 
                 msg = f"Added {len(aliases)} alias to"
                 logger.info(f"{msg} {obj} (PK: {obj.pk})")
                 if hasattr(obj, "get_absolute_url"):
                     msg = mark_safe(
-                        f'{msg} <a href="{obj.get_absolute_url()}">{escape(obj)}</a>'
+                        f'{msg} <a href="{obj.get_absolute_url()}">'
+                        f"{escape(obj)}</a>"
                     )
                 else:
                     msg = f"{msg} {obj}"
                 messages.success(request, msg)
 
                 if "_addanother" in request.POST:
                     redirect_url = request.path
@@ -229,19 +229,20 @@
                 return redirect(obj.get_absolute_url())
 
             except AbortRequest as e:
                 logger.debug(e.message)
                 messages.error(request, mark_safe(e.message))
                 return redirect(obj.get_absolute_url())
 
-            msg = f"Removed alias from"
+            msg = "Removed alias from"
             logger.info(f"{msg} {obj} (PK: {obj.pk})")
             if hasattr(obj, "get_absolute_url"):
                 msg = mark_safe(
-                    f'{msg} <a href="{obj.get_absolute_url()}">{escape(obj)}</a>'
+                    f'{msg} <a href="{obj.get_absolute_url()}">'
+                    f"{escape(obj)}</a>"
                 )
             else:
                 msg = f"{msg} {obj}"
             messages.success(request, msg)
 
             return_url = self.get_return_url(request, obj)
             return redirect(return_url)
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/utils/helpers.py` & `netbox-data-flows-0.7.0/netbox_data_flows/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,17 @@
     for app_label, model in models:
         qs |= Q(app_label=app_label, model=model)
 
     return Q(qs)
 
 
 def get_device_ipaddresses(*devices):
-    """Return the list of IP addresses of a list of devices or virtual machines"""
+    """
+    Return the list of IP addresses of a list of devices or virtual machines
+    """
 
     interfaces = []
     for dev in devices:
         if hasattr(dev, "vc_interfaces"):
             # Device
             interfaces += [dev.vc_interfaces(if_master=False)]
         else:
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/views/applicationroles.py` & `netbox-data-flows-0.7.0/netbox_data_flows/views/applicationroles.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,27 +15,29 @@
     "ApplicationRoleBulkEditView",
     "ApplicationRoleBulkDeleteView",
 )
 
 
 class ApplicationRoleListView(generic.ObjectListView):
     queryset = models.ApplicationRole.objects.annotate(
-        application_count=Count("applications"),
+        application_count=Count("applications", distinct=True),
     )
     table = tables.ApplicationRoleTable
     filterset = filtersets.ApplicationRoleFilterSet
 
 
 @register_model_view(models.ApplicationRole)
 class ApplicationRoleView(generic.ObjectView):
     queryset = models.ApplicationRole.objects.all()
 
     def get_extra_context(self, request, instance):
         applications_table = tables.ApplicationTable(
-            instance.applications.all()
+            instance.applications.prefetch_related("role").annotate(
+                dataflow_count=Count("dataflows", distinct=True),
+            )
         )
         applications_table.configure(request)
 
         return {
             "applications_table": applications_table,
         }
 
@@ -54,17 +56,21 @@
 class ApplicationRoleBulkImportView(generic.BulkImportView):
     queryset = models.ApplicationRole.objects.all()
     model_form = forms.ApplicationRoleImportForm
     table = tables.ApplicationRoleTable
 
 
 class ApplicationRoleBulkEditView(generic.BulkEditView):
-    queryset = models.ApplicationRole.objects.all()
+    queryset = models.ApplicationRole.objects.annotate(
+        application_count=Count("applications", distinct=True),
+    )
     filterset = filtersets.ApplicationRoleFilterSet
     table = tables.ApplicationRoleTable
     form = forms.ApplicationRoleBulkEditForm
 
 
 class ApplicationRoleBulkDeleteView(generic.BulkDeleteView):
-    queryset = models.ApplicationRole.objects.all()
+    queryset = models.ApplicationRole.objects.annotate(
+        application_count=Count("applications", distinct=True),
+    )
     filterset = filtersets.ApplicationRoleFilterSet
     table = tables.ApplicationRoleTable
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/views/applications.py` & `netbox-data-flows-0.7.0/netbox_data_flows/views/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,36 +17,48 @@
     "ApplicationBulkEditView",
     "ApplicationBulkDeleteView",
 )
 
 
 class ApplicationListView(generic.ObjectListView):
     queryset = models.Application.objects.prefetch_related("role").annotate(
-        dataflow_count=Count("dataflows"),
+        dataflow_count=Count("dataflows", distinct=True),
     )
     table = tables.ApplicationTable
     filterset = filtersets.ApplicationFilterSet
     filterset_form = forms.ApplicationFilterForm
 
 
 @register_model_view(models.Application)
 class ApplicationView(generic.ObjectView):
     queryset = models.Application.objects.prefetch_related(
         "role", "contacts", "dataflows", "dataflow_groups"
     )
 
     def get_extra_context(self, request, instance):
         dataflowgroups_table = tables.DataFlowGroupTable(
-            instance.dataflow_groups.all().annotate(
+            instance.dataflow_groups.prefetch_related(
+                "application",
+                "application__role",
+                "parent",
+            ).annotate(
                 dataflow_count=Count("dataflows", distinct=True),
             )
         )
         dataflowgroups_table.configure(request)
 
-        dataflows_table = tables.DataFlowTable(instance.dataflows.all())
+        dataflows_table = tables.DataFlowTable(
+            instance.dataflows.prefetch_related(
+                "application",
+                "application__role",
+                "group",
+                "sources",
+                "destinations",
+            )
+        )
         dataflows_table.configure(request)
 
         return {
             "dataflowgroups_table": dataflowgroups_table,
             "dataflows_table": dataflows_table,
         }
 
@@ -74,15 +86,15 @@
     )
     filterset = filtersets.ApplicationFilterSet
     table = tables.ApplicationTable
     form = forms.ApplicationBulkEditForm
 
 
 class ApplicationBulkDeleteView(generic.BulkDeleteView):
-    queryset = models.Application.objects.annotate(
+    queryset = models.Application.objects.prefetch_related("role").annotate(
         dataflow_count=Count("dataflows", distinct=True),
     )
     filterset = filtersets.ApplicationFilterSet
     table = tables.ApplicationTable
 
 
 @register_model_view(models.Application, "contacts")
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/views/groups.py` & `netbox-data-flows-0.7.0/netbox_data_flows/views/groups.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,43 +17,60 @@
 )
 
 
 class DataFlowGroupListView(generic.ObjectListView):
     queryset = models.DataFlowGroup.objects.prefetch_related(
         "application",
         "application__role",
-        "parent",
     ).annotate(
-        dataflow_count=Count("dataflows"),
+        dataflow_count=Count("dataflows", distinct=True),
     )
     table = tables.DataFlowGroupTable
     filterset = filtersets.DataFlowGroupFilterSet
     filterset_form = forms.DataFlowGroupFilterForm
 
 
 @register_model_view(models.DataFlowGroup)
 class DataFlowGroupView(generic.ObjectView):
     queryset = models.DataFlowGroup.objects.prefetch_related(
         "application",
-        "application__role",
         "parent",
-        "dataflows",
     )
 
     def get_extra_context(self, request, instance):
         children_table = tables.DataFlowGroupTable(
-            instance.get_descendants(include_self=False)
+            instance.get_descendants(include_self=False).annotate(
+                dataflow_count=Count("dataflows", distinct=True),
+            )
         )
         children_table.configure(request)
 
-        dataflows_table = tables.DataFlowTable(instance.dataflows.all())
+        # our direct dataflows
+        dataflows_table = tables.DataFlowTable(
+            instance.dataflows.prefetch_related(
+                "application",
+                "application__role",
+                "group",
+                "sources",
+                "destinations",
+            )
+        )
         dataflows_table.configure(request)
 
+        # dataflows of our descendants
         dataflows_recursive_table = tables.DataFlowTable(
-            models.DataFlow.objects.part_of_group_recursive(instance)
+            models.DataFlow.objects.part_of_group_recursive(
+                instance, include_direct_children=False
+            ).prefetch_related(
+                "application",
+                "application__role",
+                "group",
+                "sources",
+                "destinations",
+            )
         )
         dataflows_recursive_table.configure(request)
 
         return {
             "children_table": children_table,
             "dataflows_table": dataflows_table,
             "dataflows_recursive_table": dataflows_recursive_table,
@@ -83,24 +100,24 @@
 
 class DataFlowGroupBulkEditView(generic.BulkEditView):
     queryset = models.DataFlowGroup.objects.prefetch_related(
         "application",
         "application__role",
         "parent",
     ).annotate(
-        dataflow_count=Count("dataflows"),
+        dataflow_count=Count("dataflows", distinct=True),
     )
     filterset = filtersets.DataFlowGroupFilterSet
     table = tables.DataFlowGroupTable
     form = forms.DataFlowGroupBulkEditForm
 
 
 class DataFlowGroupBulkDeleteView(generic.BulkDeleteView):
     queryset = models.DataFlowGroup.objects.prefetch_related(
         "application",
         "application__role",
         "parent",
     ).annotate(
-        dataflow_count=Count("dataflows"),
+        dataflow_count=Count("dataflows", distinct=True),
     )
     filterset = filtersets.DataFlowGroupFilterSet
     table = tables.DataFlowGroupTable
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows/views/objectaliases.py` & `netbox-data-flows-0.7.0/netbox_data_flows/views/objectaliases.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from django.db.models import Count
 
 from netbox.views import generic
-from utilities.views import ViewTab, register_model_view
-
-from dcim.models import Device
-from ipam.models import IPAddress, IPRange, Prefix
-from virtualization.models import VirtualMachine
+from utilities.views import register_model_view
 
 from netbox_data_flows import filtersets, forms, models, tables
 from netbox_data_flows.utils.aliases import AddAliasesView, RemoveAliasView
 
 
 __all__ = (
     "ObjectAliasView",
@@ -21,33 +17,30 @@
     "ObjectAliasBulkDeleteView",
     "ObjectAliasAddTargetView",
     "ObjectAliasRemoveTargetView",
 )
 
 
 class ObjectAliasListView(generic.ObjectListView):
-    queryset = models.ObjectAlias.objects.annotate(
-        target_count=Count("targets"),
+    queryset = models.ObjectAlias.objects.all().annotate(
+        target_count=Count("targets", distinct=True),
     )
     table = tables.ObjectAliasTable
     filterset = filtersets.ObjectAliasFilterSet
     filterset_form = forms.ObjectAliasFilterForm
 
 
 @register_model_view(models.ObjectAlias)
 class ObjectAliasView(generic.ObjectView):
-    queryset = models.ObjectAlias.objects.prefetch_related(
-        "targets",
-        "dataflow_sources",
-        "dataflow_destinations",
-    )
+    queryset = models.ObjectAlias.objects.all()
 
     def get_extra_context(self, request, instance):
         targets_table = tables.ObjectAliasTargetTable(
-            instance.targets.all(), extra_context={"objectalias": instance}
+            instance.targets.prefetch_related("target_type", "target"),
+            extra_context={"objectalias": instance},
         )
         targets_table.configure(request)
 
         dataflow_sources_table = tables.DataFlowTable(
             instance.dataflow_sources.all()
         )
         dataflow_sources_table.configure(request)
@@ -78,22 +71,26 @@
 class ObjectAliasBulkImportView(generic.BulkImportView):
     queryset = models.ObjectAlias.objects.all()
     model_form = forms.ObjectAliasImportForm
     table = tables.ObjectAliasTable
 
 
 class ObjectAliasBulkEditView(generic.BulkEditView):
-    queryset = models.ObjectAlias.objects.all()
+    queryset = models.ObjectAlias.objects.annotate(
+        target_count=Count("targets", distinct=True),
+    )
     filterset = filtersets.ObjectAliasFilterSet
     table = tables.ObjectAliasTable
     form = forms.ObjectAliasBulkEditForm
 
 
 class ObjectAliasBulkDeleteView(generic.BulkDeleteView):
-    queryset = models.ObjectAlias.objects.all()
+    queryset = models.ObjectAlias.objects.annotate(
+        target_count=Count("targets", distinct=True),
+    )
     filterset = filtersets.ObjectAliasFilterSet
     table = tables.ObjectAliasTable
 
 
 @register_model_view(models.ObjectAlias, name="addtarget", path="link")
 class ObjectAliasAddTargetView(AddAliasesView):
     """Add ObjectAliasTarget(s) to an ObjectAlias"""
@@ -109,58 +106,7 @@
 )
 class ObjectAliasRemoveTargetView(RemoveAliasView):
     """Remove one ObjectAliasTarget from an ObjectAlias"""
 
     queryset = models.ObjectAlias.objects.all()
     aliases_attribute = "targets"
     template_name = "netbox_data_flows/objectalias_removetarget.html"
-
-
-#
-# As tabs
-#
-
-
-class ObjectAliasListTabViewBase(generic.ObjectChildrenView):
-    queryset = None
-    child_model = models.ObjectAlias
-    table = tables.ObjectAliasTable
-    filterset = filtersets.ObjectAliasFilterSet
-    template_name = "netbox_data_flows/objectalias_tab.html"
-    actions = ("changelog",)
-
-    tab = ViewTab(
-        label="Object Aliases",
-        permission="netbox_data_flows.view_objectalias",
-        badge=lambda obj: models.ObjectAlias.objects.contains(obj).count(),
-        hide_if_empty=True,
-    )
-
-    def get_children(self, request, parent):
-        return models.ObjectAlias.objects.contains(parent).annotate(
-            target_count=Count("targets"),
-        )
-
-
-@register_model_view(Device, name="objectalias-tab", path="aliases")
-class DeviceObjectAliasListTabView(ObjectAliasListTabViewBase):
-    queryset = Device.objects.all()
-
-
-@register_model_view(VirtualMachine, name="objectalias-tab", path="aliases")
-class VirtualMachineObjectAliasListTabView(ObjectAliasListTabViewBase):
-    queryset = VirtualMachine.objects.all()
-
-
-@register_model_view(IPAddress, name="objectalias-tab", path="aliases")
-class VirtualMachineObjectAliasListTabView(ObjectAliasListTabViewBase):
-    queryset = IPAddress.objects.all()
-
-
-@register_model_view(IPRange, name="objectalias-tab", path="aliases")
-class VirtualMachineObjectAliasListTabView(ObjectAliasListTabViewBase):
-    queryset = IPRange.objects.all()
-
-
-@register_model_view(Prefix, name="objectalias-tab", path="aliases")
-class VirtualMachineObjectAliasListTabView(ObjectAliasListTabViewBase):
-    queryset = Prefix.objects.all()
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows.egg-info/PKG-INFO` & `netbox-data-flows-0.7.0/netbox_data_flows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.6.0
+Version: 0.7.0
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `netbox-data-flows-0.6.0/netbox_data_flows.egg-info/SOURCES.txt` & `netbox-data-flows-0.7.0/netbox_data_flows.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,27 +61,25 @@
 netbox_data_flows/tables/applications.py
 netbox_data_flows/tables/dataflows.py
 netbox_data_flows/tables/groups.py
 netbox_data_flows/tables/objectaliases.py
 netbox_data_flows/templates/netbox_data_flows/application.html
 netbox_data_flows/templates/netbox_data_flows/applicationrole.html
 netbox_data_flows/templates/netbox_data_flows/dataflow.html
-netbox_data_flows/templates/netbox_data_flows/dataflow_edit.html
 netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
 netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
 netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
 netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
 netbox_data_flows/templates/netbox_data_flows/objectalias.html
 netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
-netbox_data_flows/templates/netbox_data_flows/objectalias_tab.html
-netbox_data_flows/templates/netbox_data_flows/inc/dataflow_specifications.html
 netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
 netbox_data_flows/utils/__init__.py
 netbox_data_flows/utils/aliases.py
 netbox_data_flows/utils/helpers.py
 netbox_data_flows/utils/tables.py
 netbox_data_flows/views/__init__.py
 netbox_data_flows/views/applicationroles.py
 netbox_data_flows/views/applications.py
 netbox_data_flows/views/dataflows.py
 netbox_data_flows/views/groups.py
+netbox_data_flows/views/model_tabs.py
 netbox_data_flows/views/objectaliases.py
```

### Comparing `netbox-data-flows-0.6.0/pyproject.toml` & `netbox-data-flows-0.7.0/pyproject.toml`

 * *Files identical despite different names*

