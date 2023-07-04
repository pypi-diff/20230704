# Comparing `tmp/cloudshell-networking-juniper-6.0.1.tar.gz` & `tmp/cloudshell-networking-juniper-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudshell-networking-juniper-6.0.1.tar", last modified: Thu Jun 29 15:11:57 2023, max compression
+gzip compressed data, was "cloudshell-networking-juniper-6.0.2.tar", last modified: Tue Jul  4 15:20:29 2023, max compression
```

## Comparing `cloudshell-networking-juniper-6.0.1.tar` & `cloudshell-networking-juniper-6.0.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.307769 cloudshell-networking-juniper-6.0.1/.tox/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/.tox/build/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-29 15:11:48.000000 cloudshell-networking-juniper-6.0.1/.tox/build/.tox-info.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/cloudshell/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/generic/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/generic/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/junos_generic_snmp_autoload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.315769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/HCNUM-TC.json
--rw-r--r--   0 runner    (1001) docker     (123)   657494 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-CHASSIS-DEFINES-MIB.json
--rw-r--r--   0 runner    (1001) docker     (123)    30839 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-IF-MIB.json
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-L2CP-FEATURES-MIB.json
--rw-r--r--   0 runner    (1001) docker     (123)    90661 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-MIB.json
--rw-r--r--   0 runner    (1001) docker     (123)    17568 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-SMI.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.315769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/snmp_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/snmp_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/snmp_tables/mibs_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.315769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_cli_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_command_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_ssh_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_telnet_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.315769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/add_remove_vlan_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/commit_rollback_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/enable_disable_snmp_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/enable_disable_snmp_v3_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/save_restore_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/system_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.315769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/add_remove_vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/commit_rollback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/enable_disable_snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/enable_disable_snmp_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/generic_action_error_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/save_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/system_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/autoload_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/configuration_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/connectivity_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/juniper_enable_disable_snmp_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/juniper_firmware_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/juniper_state_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/helpers/add_remove_vlan_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/helpers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-29 15:11:57.000000 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-29 15:11:57.000000 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:11:57.000000 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-29 15:11:57.000000 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 15:11:57.000000 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/autoload/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/autoload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/test_juniper_ssh_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/test_juniper_telnet_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_add_remove_vlan_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_commit_rollback_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_enable_disable_snmp_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_save_restore_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_system_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/flows/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/flows/test_juniper_enable_disable_snmp_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/helpers/test_add_remove_vlan_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/snmp/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/snmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.666414 cloudshell-networking-juniper-6.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.654414 cloudshell-networking-juniper-6.0.2/.tox/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.658414 cloudshell-networking-juniper-6.0.2/.tox/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-04 15:20:22.000000 cloudshell-networking-juniper-6.0.2/.tox/build/.tox-info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-04 15:20:29.666414 cloudshell-networking-juniper-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.658414 cloudshell-networking-juniper-6.0.2/cloudshell/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.658414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.658414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.658414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.658414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/generic/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/junos_generic_snmp_autoload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.658414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/HCNUM-TC.json
+-rw-r--r--   0 runner    (1001) docker     (123)   657494 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/JUNIPER-CHASSIS-DEFINES-MIB.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30839 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/JUNIPER-IF-MIB.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/JUNIPER-L2CP-FEATURES-MIB.json
+-rw-r--r--   0 runner    (1001) docker     (123)    90661 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/JUNIPER-MIB.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17568 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/JUNIPER-SMI.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.658414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/snmp_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/snmp_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/snmp_tables/mibs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.662414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/cli/juniper_cli_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/cli/juniper_command_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/cli/juniper_ssh_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/cli/juniper_telnet_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.662414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/add_remove_vlan_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/commit_rollback_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/enable_disable_snmp_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/enable_disable_snmp_v3_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/save_restore_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/system_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.662414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/add_remove_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/commit_rollback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/enable_disable_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/enable_disable_snmp_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/generic_action_error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/save_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/system_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.662414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/autoload_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/configuration_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/connectivity_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/juniper_enable_disable_snmp_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/juniper_firmware_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/juniper_state_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.662414 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/helpers/add_remove_vlan_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/helpers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.662414 cloudshell-networking-juniper-6.0.2/cloudshell_networking_juniper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-04 15:20:29.000000 cloudshell-networking-juniper-6.0.2/cloudshell_networking_juniper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-04 15:20:29.000000 cloudshell-networking-juniper-6.0.2/cloudshell_networking_juniper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:20:29.000000 cloudshell-networking-juniper-6.0.2/cloudshell_networking_juniper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 15:20:29.000000 cloudshell-networking-juniper-6.0.2/cloudshell_networking_juniper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:20:29.000000 cloudshell-networking-juniper-6.0.2/cloudshell_networking_juniper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:20:29.666414 cloudshell-networking-juniper-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.662414 cloudshell-networking-juniper-6.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.662414 cloudshell-networking-juniper-6.0.2/tests/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.662414 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.662414 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/autoload/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/autoload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.666414 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/cli/test_juniper_ssh_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/cli/test_juniper_telnet_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.666414 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/test_add_remove_vlan_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/test_commit_rollback_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/test_enable_disable_snmp_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/test_save_restore_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/test_system_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.666414 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.666414 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/flows/test_juniper_enable_disable_snmp_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.666414 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/helpers/test_add_remove_vlan_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:20:29.666414 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/snmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tests/networking/juniper/snmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 15:20:16.000000 cloudshell-networking-juniper-6.0.2/version.txt
```

### Comparing `cloudshell-networking-juniper-6.0.1/.tox/build/.tox-info.json` & `cloudshell-networking-juniper-6.0.2/.tox/build/.tox-info.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/README.md` & `cloudshell-networking-juniper-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/generic/entities.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/generic/entities.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/junos_generic_snmp_autoload.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/junos_generic_snmp_autoload.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/HCNUM-TC.json` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/HCNUM-TC.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-CHASSIS-DEFINES-MIB.json` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/JUNIPER-CHASSIS-DEFINES-MIB.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-IF-MIB.json` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/JUNIPER-IF-MIB.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-L2CP-FEATURES-MIB.json` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/JUNIPER-L2CP-FEATURES-MIB.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-MIB.json` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/JUNIPER-MIB.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-SMI.json` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/mibs/JUNIPER-SMI.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/snmp_tables/mibs_conf.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/autoload/snmp_tables/mibs_conf.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_cli_configurator.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/cli/juniper_cli_configurator.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_command_modes.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/cli/juniper_command_modes.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_ssh_session.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/cli/juniper_ssh_session.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_telnet_session.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/cli/juniper_telnet_session.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/add_remove_vlan_actions.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/add_remove_vlan_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/commit_rollback_actions.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/commit_rollback_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/enable_disable_snmp_actions.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/enable_disable_snmp_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/enable_disable_snmp_v3_actions.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/enable_disable_snmp_v3_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/save_restore_actions.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/save_restore_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/system_actions.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_actions/system_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/add_remove_vlan.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/add_remove_vlan.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/enable_disable_snmp.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/enable_disable_snmp.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/enable_disable_snmp_v3.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/enable_disable_snmp_v3.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/save_restore.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/save_restore.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/system_commands.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/command_templates/system_commands.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/autoload_flow.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/autoload_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/configuration_flow.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/configuration_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,13 +120,13 @@
             password = config_path.password
             config_path.password = None
             try:
                 restore_actions.restore_running(
                     restore_type, str(config_path), password
                 )
                 # wait longer for applying changes
-                commit_rollback_actions.commit(timeout=120)
+                commit_rollback_actions.commit(timeout=5 * 60)
             except CommandExecutionException:
                 commit_rollback_actions.rollback()
                 raise
             finally:
                 config_path.password = password
```

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/connectivity_flow.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/connectivity_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/juniper_enable_disable_snmp_flow.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/juniper_enable_disable_snmp_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/juniper_firmware_flow.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/flows/juniper_firmware_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/helpers/add_remove_vlan_helper.py` & `cloudshell-networking-juniper-6.0.2/cloudshell/networking/juniper/helpers/add_remove_vlan_helper.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/SOURCES.txt` & `cloudshell-networking-juniper-6.0.2/cloudshell_networking_juniper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/setup.py` & `cloudshell-networking-juniper-6.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/test_juniper_ssh_session.py` & `cloudshell-networking-juniper-6.0.2/tests/networking/juniper/cli/test_juniper_ssh_session.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/test_juniper_telnet_session.py` & `cloudshell-networking-juniper-6.0.2/tests/networking/juniper/cli/test_juniper_telnet_session.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_add_remove_vlan_actions.py` & `cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/test_add_remove_vlan_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_commit_rollback_actions.py` & `cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/test_commit_rollback_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_enable_disable_snmp_actions.py` & `cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/test_enable_disable_snmp_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_save_restore_actions.py` & `cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/test_save_restore_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_system_actions.py` & `cloudshell-networking-juniper-6.0.2/tests/networking/juniper/command_actions/test_system_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/flows/test_juniper_enable_disable_snmp_flow.py` & `cloudshell-networking-juniper-6.0.2/tests/networking/juniper/flows/test_juniper_enable_disable_snmp_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/helpers/test_add_remove_vlan_helper.py` & `cloudshell-networking-juniper-6.0.2/tests/networking/juniper/helpers/test_add_remove_vlan_helper.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.1/tox.ini` & `cloudshell-networking-juniper-6.0.2/tox.ini`

 * *Files identical despite different names*

