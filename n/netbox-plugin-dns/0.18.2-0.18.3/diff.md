# Comparing `tmp/netbox_plugin_dns-0.18.2.tar.gz` & `tmp/netbox_plugin_dns-0.18.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_dns-0.18.2.tar", max compression
+gzip compressed data, was "netbox_plugin_dns-0.18.3.tar", max compression
```

## Comparing `netbox_plugin_dns-0.18.2.tar` & `netbox_plugin_dns-0.18.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     1076 2023-05-14 13:07:16.080783 netbox_plugin_dns-0.18.2/LICENSE
--rw-r--r--   0        0        0     3096 2023-05-14 13:07:16.080783 netbox_plugin_dns-0.18.2/README.md
--rw-r--r--   0        0        0      903 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/__init__.py
--rw-r--r--   0        0        0      512 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/admin.py
--rw-r--r--   0        0        0     1951 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/api/nested_serializers.py
--rw-r--r--   0        0        0     4555 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/api/serializers.py
--rw-r--r--   0        0        0      441 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/api/urls.py
--rw-r--r--   0        0        0     3060 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/api/views.py
--rw-r--r--   0        0        0      151 2023-05-14 13:07:16.100784 netbox_plugin_dns-0.18.2/netbox_dns/apps.py
--rw-r--r--   0        0        0       46 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/fields/__init__.py
--rw-r--r--   0        0        0     1530 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/fields/address.py
--rw-r--r--   0        0        0     3023 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/fields/network.py
--rw-r--r--   0        0        0       88 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/filters/__init__.py
--rwxr-xr-x   0        0        0      601 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/filters/nameserver.py
--rwxr-xr-x   0        0        0     1615 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/filters/record.py
--rw-r--r--   0        0        0      577 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/filters/view.py
--rwxr-xr-x   0        0        0     1185 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/filters/zone.py
--rw-r--r--   0        0        0       88 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/forms/__init__.py
--rwxr-xr-x   0        0        0     1308 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/forms/nameserver.py
--rwxr-xr-x   0        0        0     5083 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/forms/record.py
--rw-r--r--   0        0        0      961 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/forms/view.py
--rwxr-xr-x   0        0        0    14198 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/forms/zone.py
--rw-r--r--   0        0        0      604 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/__init__.py
--rw-r--r--   0        0        0      527 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/nameserver.py
--rw-r--r--   0        0        0      487 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/record.py
--rw-r--r--   0        0        0      221 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/schema.py
--rw-r--r--   0        0        0      467 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/view.py
--rw-r--r--   0        0        0      467 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/graphql/zone.py
--rw-r--r--   0        0        0     6035 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/management/commands/cleanup_database.py
--rw-r--r--   0        0        0      661 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/management/commands/update_soa.py
--rw-r--r--   0        0        0     4153 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0001_initial.py
--rw-r--r--   0        0        0    11513 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
--rw-r--r--   0        0        0      437 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0002_zone_default_ttl.py
--rw-r--r--   0        0        0     3716 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0003_soa_managed_records.py
--rw-r--r--   0        0        0     2287 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py
--rw-r--r--   0        0        0     1156 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0005_update_ns_records.py
--rw-r--r--   0        0        0      861 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0006_zone_soa_serial_auto.py
--rw-r--r--   0        0        0      399 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0007_alter_zone_soa_serial_auto.py
--rw-r--r--   0        0        0      527 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0008_zone_status_names.py
--rw-r--r--   0        0        0     2176 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0009_netbox32.py
--rw-r--r--   0        0        0     1543 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0010_update_soa_records.py
--rw-r--r--   0        0        0     2201 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0011_add_view_model.py
--rw-r--r--   0        0        0      402 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0012_adjust_zone_and_record.py
--rw-r--r--   0        0        0      733 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py
--rw-r--r--   0        0        0      428 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0014_add_view_description.py
--rw-r--r--   0        0        0      393 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0015_add_record_status.py
--rw-r--r--   0        0        0     1053 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0016_cleanup_ptr_records.py
--rw-r--r--   0        0        0      405 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0017_alter_record_ttl.py
--rw-r--r--   0        0        0     1553 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0018_zone_arpa_network.py
--rw-r--r--   0        0        0      433 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0019_update_ns_ttl.py
--rw-r--r--   0        0        0     1260 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0020_netbox_3_4.py
--rw-r--r--   0        0        0     3304 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0021_record_ip_address.py
--rw-r--r--   0        0        0      891 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/0022_search.py
--rw-r--r--   0        0        0        0 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/migrations/__init__.py
--rw-r--r--   0        0        0    28247 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/models.py
--rw-r--r--   0        0        0     3158 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/navigation.py
--rw-r--r--   0        0        0       88 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/tables/__init__.py
--rw-r--r--   0        0        0      701 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/tables/nameserver.py
--rw-r--r--   0        0        0     3064 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/tables/record.py
--rw-r--r--   0        0        0      325 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/tables/view.py
--rw-r--r--   0        0        0     1660 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/tables/zone.py
--rw-r--r--   0        0        0     1980 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/template_content.py
--rw-r--r--   0        0        0     1192 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/nameserver.html
--rw-r--r--   0        0        0       89 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/record/managed.html
--rw-r--r--   0        0        0      378 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/record/related.html
--rw-r--r--   0        0        0     4136 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/record.html
--rw-r--r--   0        0        0      919 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/view.html
--rw-r--r--   0        0        0      460 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/base.html
--rw-r--r--   0        0        0     2171 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/child.html
--rw-r--r--   0        0        0      524 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/managed_record.html
--rw-r--r--   0        0        0     2218 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/record.html
--rw-r--r--   0        0        0      215 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/related.html
--rw-r--r--   0        0        0     5480 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone.html
--rw-r--r--   0        0        0        0 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templatetags/__init__.py
--rw-r--r--   0        0        0      271 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/templatetags/view_helpers.py
--rw-r--r--   0        0        0     5202 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/urls.py
--rw-r--r--   0        0        0     1537 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/utilities.py
--rw-r--r--   0        0        0     1969 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/validators.py
--rw-r--r--   0        0        0       88 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/views/__init__.py
--rw-r--r--   0        0        0     2991 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/views/nameserver.py
--rw-r--r--   0        0        0     2554 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/views/record.py
--rw-r--r--   0        0        0     1895 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/views/view.py
--rw-r--r--   0        0        0     3600 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/netbox_dns/views/zone.py
--rw-r--r--   0        0        0      690 2023-05-14 13:07:16.104784 netbox_plugin_dns-0.18.2/pyproject.toml
--rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 netbox_plugin_dns-0.18.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-04 16:05:01.470693 netbox_plugin_dns-0.18.3/LICENSE
+-rw-r--r--   0        0        0     3096 2023-07-04 16:05:01.470693 netbox_plugin_dns-0.18.3/README.md
+-rw-r--r--   0        0        0      919 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/__init__.py
+-rw-r--r--   0        0        0      512 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/admin.py
+-rw-r--r--   0        0        0     1951 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/api/nested_serializers.py
+-rw-r--r--   0        0        0     4555 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/api/serializers.py
+-rw-r--r--   0        0        0      441 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/api/urls.py
+-rw-r--r--   0        0        0     3015 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/api/views.py
+-rw-r--r--   0        0        0      151 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/apps.py
+-rw-r--r--   0        0        0       46 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/fields/__init__.py
+-rw-r--r--   0        0        0     1530 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/fields/address.py
+-rw-r--r--   0        0        0     3023 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/fields/network.py
+-rw-r--r--   0        0        0       88 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/filters/__init__.py
+-rwxr-xr-x   0        0        0      601 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/filters/nameserver.py
+-rwxr-xr-x   0        0        0     1615 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/filters/record.py
+-rw-r--r--   0        0        0      577 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/filters/view.py
+-rwxr-xr-x   0        0        0     1185 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/filters/zone.py
+-rw-r--r--   0        0        0       88 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/forms/__init__.py
+-rwxr-xr-x   0        0        0     1308 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/forms/nameserver.py
+-rwxr-xr-x   0        0        0     5083 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/forms/record.py
+-rw-r--r--   0        0        0      961 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/forms/view.py
+-rwxr-xr-x   0        0        0    14198 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/forms/zone.py
+-rw-r--r--   0        0        0      604 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/graphql/__init__.py
+-rw-r--r--   0        0        0      527 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/graphql/nameserver.py
+-rw-r--r--   0        0        0      487 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/graphql/record.py
+-rw-r--r--   0        0        0      221 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/graphql/schema.py
+-rw-r--r--   0        0        0      467 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/graphql/view.py
+-rw-r--r--   0        0        0      467 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/graphql/zone.py
+-rw-r--r--   0        0        0     6035 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/management/commands/cleanup_database.py
+-rw-r--r--   0        0        0      661 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/management/commands/update_soa.py
+-rw-r--r--   0        0        0     4153 2023-07-04 16:05:01.494694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0001_initial.py
+-rw-r--r--   0        0        0    11513 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
+-rw-r--r--   0        0        0      437 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0002_zone_default_ttl.py
+-rw-r--r--   0        0        0     3716 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0003_soa_managed_records.py
+-rw-r--r--   0        0        0     2287 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py
+-rw-r--r--   0        0        0     1156 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0005_update_ns_records.py
+-rw-r--r--   0        0        0      861 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0006_zone_soa_serial_auto.py
+-rw-r--r--   0        0        0      399 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0007_alter_zone_soa_serial_auto.py
+-rw-r--r--   0        0        0      527 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0008_zone_status_names.py
+-rw-r--r--   0        0        0     2176 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0009_netbox32.py
+-rw-r--r--   0        0        0     1543 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0010_update_soa_records.py
+-rw-r--r--   0        0        0     2201 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0011_add_view_model.py
+-rw-r--r--   0        0        0      402 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0012_adjust_zone_and_record.py
+-rw-r--r--   0        0        0      733 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py
+-rw-r--r--   0        0        0      428 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0014_add_view_description.py
+-rw-r--r--   0        0        0      393 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0015_add_record_status.py
+-rw-r--r--   0        0        0     1053 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0016_cleanup_ptr_records.py
+-rw-r--r--   0        0        0      405 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0017_alter_record_ttl.py
+-rw-r--r--   0        0        0     1553 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0018_zone_arpa_network.py
+-rw-r--r--   0        0        0      433 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0019_update_ns_ttl.py
+-rw-r--r--   0        0        0     1260 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0020_netbox_3_4.py
+-rw-r--r--   0        0        0     3304 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0021_record_ip_address.py
+-rw-r--r--   0        0        0      891 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/0022_search.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/migrations/__init__.py
+-rw-r--r--   0        0        0    28259 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/models.py
+-rw-r--r--   0        0        0     3158 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/navigation.py
+-rw-r--r--   0        0        0       88 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/tables/__init__.py
+-rw-r--r--   0        0        0      701 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/tables/nameserver.py
+-rw-r--r--   0        0        0     3064 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/tables/record.py
+-rw-r--r--   0        0        0      325 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/tables/view.py
+-rw-r--r--   0        0        0     1660 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/tables/zone.py
+-rw-r--r--   0        0        0     1980 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/template_content.py
+-rw-r--r--   0        0        0     1192 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/nameserver.html
+-rw-r--r--   0        0        0       89 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/record/managed.html
+-rw-r--r--   0        0        0      378 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/record/related.html
+-rw-r--r--   0        0        0     4136 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/record.html
+-rw-r--r--   0        0        0      919 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/view.html
+-rw-r--r--   0        0        0      460 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/zone/base.html
+-rw-r--r--   0        0        0     2171 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/zone/child.html
+-rw-r--r--   0        0        0      524 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/zone/managed_record.html
+-rw-r--r--   0        0        0     2218 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/zone/record.html
+-rw-r--r--   0        0        0      215 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/zone/related.html
+-rw-r--r--   0        0        0     5480 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/zone.html
+-rw-r--r--   0        0        0        0 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templatetags/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/templatetags/view_helpers.py
+-rw-r--r--   0        0        0     5202 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/urls.py
+-rw-r--r--   0        0        0     1537 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/utilities.py
+-rw-r--r--   0        0        0     1969 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/validators.py
+-rw-r--r--   0        0        0       88 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/views/__init__.py
+-rw-r--r--   0        0        0     2991 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/views/nameserver.py
+-rw-r--r--   0        0        0     2554 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/views/record.py
+-rw-r--r--   0        0        0     1895 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/views/view.py
+-rw-r--r--   0        0        0     3600 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/netbox_dns/views/zone.py
+-rw-r--r--   0        0        0      690 2023-07-04 16:05:01.498694 netbox_plugin_dns-0.18.3/pyproject.toml
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 netbox_plugin_dns-0.18.3/PKG-INFO
```

### Comparing `netbox_plugin_dns-0.18.2/LICENSE` & `netbox_plugin_dns-0.18.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/README.md` & `netbox_plugin_dns-0.18.3/README.md`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/__init__.py` & `netbox_plugin_dns-0.18.3/netbox_dns/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from extras.plugins import PluginConfig
 
-__version__ = "0.18.2"
+__version__ = "0.18.3"
 
 
 class DNSConfig(PluginConfig):
     name = "netbox_dns"
-    verbose_name = "Netbox DNS"
-    description = "Netbox DNS"
+    verbose_name = "NetBox DNS"
+    description = "NetBox plugin for DNS data"
     min_version = "3.5"
     version = __version__
     author = "Peter Eckel"
     author_email = "pe-netbox-plugin-dns@hindenburgring.com"
     required_settings = []
     default_settings = {
         "zone_default_ttl": 86400,
```

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/admin.py` & `netbox_plugin_dns-0.18.3/netbox_dns/admin.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/api/nested_serializers.py` & `netbox_plugin_dns-0.18.3/netbox_dns/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/api/serializers.py` & `netbox_plugin_dns-0.18.3/netbox_dns/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/api/views.py` & `netbox_plugin_dns-0.18.3/netbox_dns/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,17 @@
     NameServerSerializer,
     RecordSerializer,
 )
 from netbox_dns.filters import ViewFilter, ZoneFilter, NameServerFilter, RecordFilter
 from netbox_dns.models import View, Zone, NameServer, Record
 
 
-class NetboxDNSRootView(APIRootView):
-    """
-    NetboxDNS API root view
-    """
-
+class NetBoxDNSRootView(APIRootView):
     def get_view_name(self):
-        return "NetboxDNS"
+        return "NetBoxDNS"
 
 
 class ViewViewSet(NetBoxModelViewSet):
     queryset = View.objects.all()
     serializer_class = ViewSerializer
     filterset_class = ViewFilter
```

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/fields/address.py` & `netbox_plugin_dns-0.18.3/netbox_dns/fields/address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/fields/network.py` & `netbox_plugin_dns-0.18.3/netbox_dns/fields/network.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/filters/nameserver.py` & `netbox_plugin_dns-0.18.3/netbox_dns/filters/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/filters/record.py` & `netbox_plugin_dns-0.18.3/netbox_dns/filters/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/filters/view.py` & `netbox_plugin_dns-0.18.3/netbox_dns/filters/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/filters/zone.py` & `netbox_plugin_dns-0.18.3/netbox_dns/filters/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/forms/nameserver.py` & `netbox_plugin_dns-0.18.3/netbox_dns/forms/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/forms/record.py` & `netbox_plugin_dns-0.18.3/netbox_dns/forms/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/forms/view.py` & `netbox_plugin_dns-0.18.3/netbox_dns/forms/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/forms/zone.py` & `netbox_plugin_dns-0.18.3/netbox_dns/forms/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/graphql/__init__.py` & `netbox_plugin_dns-0.18.3/netbox_dns/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/graphql/nameserver.py` & `netbox_plugin_dns-0.18.3/netbox_dns/graphql/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/management/commands/cleanup_database.py` & `netbox_plugin_dns-0.18.3/netbox_dns/management/commands/cleanup_database.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/management/commands/update_soa.py` & `netbox_plugin_dns-0.18.3/netbox_dns/management/commands/update_soa.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0001_initial.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0003_soa_managed_records.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0003_soa_managed_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0005_update_ns_records.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0005_update_ns_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0006_zone_soa_serial_auto.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0006_zone_soa_serial_auto.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0008_zone_status_names.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0008_zone_status_names.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0009_netbox32.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0009_netbox32.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0010_update_soa_records.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0010_update_soa_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0011_add_view_model.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0011_add_view_model.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0016_cleanup_ptr_records.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0016_cleanup_ptr_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0018_zone_arpa_network.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0018_zone_arpa_network.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0020_netbox_3_4.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0020_netbox_3_4.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0021_record_ip_address.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0021_record_ip_address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/migrations/0022_search.py` & `netbox_plugin_dns-0.18.3/netbox_dns/migrations/0022_search.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/models.py` & `netbox_plugin_dns-0.18.3/netbox_dns/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,15 +447,15 @@
     def network_from_name(self):
         return arpa_to_prefix(self.name)
 
     def check_name_conflict(self):
         if self.view is None:
             if (
                 Zone.objects.exclude(pk=self.pk)
-                .filter(name=self.name, view__isnull=True)
+                .filter(name=self.name.rstrip("."), view__isnull=True)
                 .exists()
             ):
                 raise ValidationError(
                     {
                         "name": f"A zone with name {self.name} and no view already exists."
                     }
                 )
```

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/navigation.py` & `netbox_plugin_dns-0.18.3/netbox_dns/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/tables/nameserver.py` & `netbox_plugin_dns-0.18.3/netbox_dns/tables/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/tables/record.py` & `netbox_plugin_dns-0.18.3/netbox_dns/tables/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/tables/zone.py` & `netbox_plugin_dns-0.18.3/netbox_dns/tables/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/template_content.py` & `netbox_plugin_dns-0.18.3/netbox_dns/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/nameserver.html` & `netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/nameserver.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/record.html` & `netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/view.html` & `netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/view.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/child.html` & `netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/zone/child.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/managed_record.html` & `netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/zone/managed_record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone/record.html` & `netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/zone/record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/templates/netbox_dns/zone.html` & `netbox_plugin_dns-0.18.3/netbox_dns/templates/netbox_dns/zone.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/urls.py` & `netbox_plugin_dns-0.18.3/netbox_dns/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/utilities.py` & `netbox_plugin_dns-0.18.3/netbox_dns/utilities.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/validators.py` & `netbox_plugin_dns-0.18.3/netbox_dns/validators.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/views/nameserver.py` & `netbox_plugin_dns-0.18.3/netbox_dns/views/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/views/record.py` & `netbox_plugin_dns-0.18.3/netbox_dns/views/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/views/view.py` & `netbox_plugin_dns-0.18.3/netbox_dns/views/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/netbox_dns/views/zone.py` & `netbox_plugin_dns-0.18.3/netbox_dns/views/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.2/pyproject.toml` & `netbox_plugin_dns-0.18.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "netbox-plugin-dns"
-version = "0.18.2"
-description = "Netbox DNS is a NetBox plugin for managing DNS data."
+version = "0.18.3"
+description = "NetBox DNS is a NetBox plugin for managing DNS data."
 authors = ["Peter Eckel <pe-netbox-dns@hindenburgring.com>"]
 homepage = "https://github.com/peteeckel/netbox-plugin-dns"
 repository = "https://github.com/peteeckel/netbox-plugin-dns"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "netbox_dns"}]
 exclude = ["netbox_dns/tests/*"]
```

### Comparing `netbox_plugin_dns-0.18.2/PKG-INFO` & `netbox_plugin_dns-0.18.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-dns
-Version: 0.18.2
-Summary: Netbox DNS is a NetBox plugin for managing DNS data.
+Version: 0.18.3
+Summary: NetBox DNS is a NetBox plugin for managing DNS data.
 Home-page: https://github.com/peteeckel/netbox-plugin-dns
 License: MIT
 Keywords: netbox,netbox-plugin,dns
 Author: Peter Eckel
 Author-email: pe-netbox-dns@hindenburgring.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-plugin-dns Version: 0.18.2 Summary: Netbox
+Metadata-Version: 2.1 Name: netbox-plugin-dns Version: 0.18.3 Summary: NetBox
 DNS is a NetBox plugin for managing DNS data. Home-page: https://github.com/
 peteeckel/netbox-plugin-dns License: MIT Keywords: netbox,netbox-plugin,dns
 Author: Peter Eckel Author-email: pe-netbox-dns@hindenburgring.com Requires-
 Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

