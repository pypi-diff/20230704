# Comparing `tmp/pulumi_proxmoxve-5.7.0.tar.gz` & `tmp/pulumi_proxmoxve-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-5.7.0.tar", last modified: Sun Jun 25 17:20:26 2023, max compression
+gzip compressed data, was "pulumi_proxmoxve-5.8.0.tar", last modified: Tue Jul  4 07:42:46 2023, max compression
```

## Comparing `pulumi_proxmoxve-5.7.0.tar` & `pulumi_proxmoxve-5.8.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/cluster/get_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34964 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (123)    28878 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83149 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/virtual_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:46.084627 pulumi_proxmoxve-5.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-04 07:42:46.084627 pulumi_proxmoxve-5.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:46.076626 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:46.076626 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/cluster/get_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:46.076626 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:46.080626 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:46.080626 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:46.084627 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:46.084627 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:46.084627 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37273 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31126 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85270 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/virtual_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:42:46.076626 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-04 07:42:46.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-04 07:42:46.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:42:46.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:42:46.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 07:42:46.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 07:42:46.000000 pulumi_proxmoxve-5.8.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:42:46.084627 pulumi_proxmoxve-5.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-04 07:42:45.000000 pulumi_proxmoxve-5.8.0/setup.py
```

### Comparing `pulumi_proxmoxve-5.7.0/PKG-INFO` & `pulumi_proxmoxve-5.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 5.7.0
+Version: 5.8.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_proxmoxve-5.7.0/README.md` & `pulumi_proxmoxve-5.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_dns.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_hosts.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_time.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_version.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     'VirtualMachineAgentArgs',
     'VirtualMachineAudioDeviceArgs',
     'VirtualMachineCdromArgs',
     'VirtualMachineCloneArgs',
     'VirtualMachineCpuArgs',
     'VirtualMachineDiskArgs',
     'VirtualMachineDiskSpeedArgs',
+    'VirtualMachineEfiDiskArgs',
     'VirtualMachineHostpciArgs',
     'VirtualMachineInitializationArgs',
     'VirtualMachineInitializationDnsArgs',
     'VirtualMachineInitializationIpConfigArgs',
     'VirtualMachineInitializationIpConfigIpv4Args',
     'VirtualMachineInitializationIpConfigIpv6Args',
     'VirtualMachineInitializationUserAccountArgs',
@@ -221,25 +222,28 @@
 @pulumi.input_type
 class VirtualMachineCpuArgs:
     def __init__(__self__, *,
                  architecture: Optional[pulumi.Input[str]] = None,
                  cores: Optional[pulumi.Input[int]] = None,
                  flags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  hotplugged: Optional[pulumi.Input[int]] = None,
+                 numa: Optional[pulumi.Input[bool]] = None,
                  sockets: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  units: Optional[pulumi.Input[int]] = None):
         if architecture is not None:
             pulumi.set(__self__, "architecture", architecture)
         if cores is not None:
             pulumi.set(__self__, "cores", cores)
         if flags is not None:
             pulumi.set(__self__, "flags", flags)
         if hotplugged is not None:
             pulumi.set(__self__, "hotplugged", hotplugged)
+        if numa is not None:
+            pulumi.set(__self__, "numa", numa)
         if sockets is not None:
             pulumi.set(__self__, "sockets", sockets)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if units is not None:
             pulumi.set(__self__, "units", units)
 
@@ -277,14 +281,23 @@
 
     @hotplugged.setter
     def hotplugged(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "hotplugged", value)
 
     @property
     @pulumi.getter
+    def numa(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "numa")
+
+    @numa.setter
+    def numa(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "numa", value)
+
+    @property
+    @pulumi.getter
     def sockets(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "sockets")
 
     @sockets.setter
     def sockets(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "sockets", value)
 
@@ -469,14 +482,67 @@
 
     @write_burstable.setter
     def write_burstable(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "write_burstable", value)
 
 
 @pulumi.input_type
+class VirtualMachineEfiDiskArgs:
+    def __init__(__self__, *,
+                 datastore_id: Optional[pulumi.Input[str]] = None,
+                 file_format: Optional[pulumi.Input[str]] = None,
+                 pre_enrolled_keys: Optional[pulumi.Input[bool]] = None,
+                 type: Optional[pulumi.Input[str]] = None):
+        if datastore_id is not None:
+            pulumi.set(__self__, "datastore_id", datastore_id)
+        if file_format is not None:
+            pulumi.set(__self__, "file_format", file_format)
+        if pre_enrolled_keys is not None:
+            pulumi.set(__self__, "pre_enrolled_keys", pre_enrolled_keys)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter(name="datastoreId")
+    def datastore_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "datastore_id")
+
+    @datastore_id.setter
+    def datastore_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "datastore_id", value)
+
+    @property
+    @pulumi.getter(name="fileFormat")
+    def file_format(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "file_format")
+
+    @file_format.setter
+    def file_format(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "file_format", value)
+
+    @property
+    @pulumi.getter(name="preEnrolledKeys")
+    def pre_enrolled_keys(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "pre_enrolled_keys")
+
+    @pre_enrolled_keys.setter
+    def pre_enrolled_keys(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "pre_enrolled_keys", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
+
+@pulumi.input_type
 class VirtualMachineHostpciArgs:
     def __init__(__self__, *,
                  device: pulumi.Input[str],
                  id: pulumi.Input[str],
                  mdev: Optional[pulumi.Input[str]] = None,
                  pcie: Optional[pulumi.Input[bool]] = None,
                  rom_file: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     'VirtualMachineAgent',
     'VirtualMachineAudioDevice',
     'VirtualMachineCdrom',
     'VirtualMachineClone',
     'VirtualMachineCpu',
     'VirtualMachineDisk',
     'VirtualMachineDiskSpeed',
+    'VirtualMachineEfiDisk',
     'VirtualMachineHostpci',
     'VirtualMachineInitialization',
     'VirtualMachineInitializationDns',
     'VirtualMachineInitializationIpConfig',
     'VirtualMachineInitializationIpConfigIpv4',
     'VirtualMachineInitializationIpConfigIpv6',
     'VirtualMachineInitializationUserAccount',
@@ -205,25 +206,28 @@
 @pulumi.output_type
 class VirtualMachineCpu(dict):
     def __init__(__self__, *,
                  architecture: Optional[str] = None,
                  cores: Optional[int] = None,
                  flags: Optional[Sequence[str]] = None,
                  hotplugged: Optional[int] = None,
+                 numa: Optional[bool] = None,
                  sockets: Optional[int] = None,
                  type: Optional[str] = None,
                  units: Optional[int] = None):
         if architecture is not None:
             pulumi.set(__self__, "architecture", architecture)
         if cores is not None:
             pulumi.set(__self__, "cores", cores)
         if flags is not None:
             pulumi.set(__self__, "flags", flags)
         if hotplugged is not None:
             pulumi.set(__self__, "hotplugged", hotplugged)
+        if numa is not None:
+            pulumi.set(__self__, "numa", numa)
         if sockets is not None:
             pulumi.set(__self__, "sockets", sockets)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if units is not None:
             pulumi.set(__self__, "units", units)
 
@@ -245,14 +249,19 @@
     @property
     @pulumi.getter
     def hotplugged(self) -> Optional[int]:
         return pulumi.get(self, "hotplugged")
 
     @property
     @pulumi.getter
+    def numa(self) -> Optional[bool]:
+        return pulumi.get(self, "numa")
+
+    @property
+    @pulumi.getter
     def sockets(self) -> Optional[int]:
         return pulumi.get(self, "sockets")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         return pulumi.get(self, "type")
@@ -413,14 +422,72 @@
     @property
     @pulumi.getter(name="writeBurstable")
     def write_burstable(self) -> Optional[int]:
         return pulumi.get(self, "write_burstable")
 
 
 @pulumi.output_type
+class VirtualMachineEfiDisk(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "datastoreId":
+            suggest = "datastore_id"
+        elif key == "fileFormat":
+            suggest = "file_format"
+        elif key == "preEnrolledKeys":
+            suggest = "pre_enrolled_keys"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in VirtualMachineEfiDisk. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        VirtualMachineEfiDisk.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        VirtualMachineEfiDisk.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 datastore_id: Optional[str] = None,
+                 file_format: Optional[str] = None,
+                 pre_enrolled_keys: Optional[bool] = None,
+                 type: Optional[str] = None):
+        if datastore_id is not None:
+            pulumi.set(__self__, "datastore_id", datastore_id)
+        if file_format is not None:
+            pulumi.set(__self__, "file_format", file_format)
+        if pre_enrolled_keys is not None:
+            pulumi.set(__self__, "pre_enrolled_keys", pre_enrolled_keys)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter(name="datastoreId")
+    def datastore_id(self) -> Optional[str]:
+        return pulumi.get(self, "datastore_id")
+
+    @property
+    @pulumi.getter(name="fileFormat")
+    def file_format(self) -> Optional[str]:
+        return pulumi.get(self, "file_format")
+
+    @property
+    @pulumi.getter(name="preEnrolledKeys")
+    def pre_enrolled_keys(self) -> Optional[bool]:
+        return pulumi.get(self, "pre_enrolled_keys")
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[str]:
+        return pulumi.get(self, "type")
+
+
+@pulumi.output_type
 class VirtualMachineHostpci(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "romFile":
             suggest = "rom_file"
```

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
                  bios: Optional[pulumi.Input[str]] = None,
                  boot_orders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cdrom: Optional[pulumi.Input['VirtualMachineCdromArgs']] = None,
                  clone: Optional[pulumi.Input['VirtualMachineCloneArgs']] = None,
                  cpu: Optional[pulumi.Input['VirtualMachineCpuArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disks: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]]] = None,
+                 efi_disk: Optional[pulumi.Input['VirtualMachineEfiDiskArgs']] = None,
                  hostpcis: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]]] = None,
                  initialization: Optional[pulumi.Input['VirtualMachineInitializationArgs']] = None,
                  keyboard_layout: Optional[pulumi.Input[str]] = None,
                  kvm_arguments: Optional[pulumi.Input[str]] = None,
                  machine: Optional[pulumi.Input[str]] = None,
                  memory: Optional[pulumi.Input['VirtualMachineMemoryArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
@@ -62,14 +63,15 @@
         :param pulumi.Input[str] bios: The BIOS implementation
         :param pulumi.Input[Sequence[pulumi.Input[str]]] boot_orders: The guest will attempt to boot from devices in the order they appear here
         :param pulumi.Input['VirtualMachineCdromArgs'] cdrom: The CDROM drive
         :param pulumi.Input['VirtualMachineCloneArgs'] clone: The cloning configuration
         :param pulumi.Input['VirtualMachineCpuArgs'] cpu: The CPU allocation
         :param pulumi.Input[str] description: The description
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]] disks: The disk devices
+        :param pulumi.Input['VirtualMachineEfiDiskArgs'] efi_disk: The efidisk device
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]] hostpcis: The Host PCI devices mapped to the VM
         :param pulumi.Input['VirtualMachineInitializationArgs'] initialization: The cloud-init configuration
         :param pulumi.Input[str] keyboard_layout: The keyboard layout
         :param pulumi.Input[str] kvm_arguments: The args implementation
         :param pulumi.Input[str] machine: The VM machine type, either default i440fx or q35
         :param pulumi.Input['VirtualMachineMemoryArgs'] memory: The memory allocation
         :param pulumi.Input[str] name: The name
@@ -110,14 +112,16 @@
             pulumi.set(__self__, "clone", clone)
         if cpu is not None:
             pulumi.set(__self__, "cpu", cpu)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if disks is not None:
             pulumi.set(__self__, "disks", disks)
+        if efi_disk is not None:
+            pulumi.set(__self__, "efi_disk", efi_disk)
         if hostpcis is not None:
             pulumi.set(__self__, "hostpcis", hostpcis)
         if initialization is not None:
             pulumi.set(__self__, "initialization", initialization)
         if keyboard_layout is not None:
             pulumi.set(__self__, "keyboard_layout", keyboard_layout)
         if kvm_arguments is not None:
@@ -296,14 +300,26 @@
         return pulumi.get(self, "disks")
 
     @disks.setter
     def disks(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]]]):
         pulumi.set(self, "disks", value)
 
     @property
+    @pulumi.getter(name="efiDisk")
+    def efi_disk(self) -> Optional[pulumi.Input['VirtualMachineEfiDiskArgs']]:
+        """
+        The efidisk device
+        """
+        return pulumi.get(self, "efi_disk")
+
+    @efi_disk.setter
+    def efi_disk(self, value: Optional[pulumi.Input['VirtualMachineEfiDiskArgs']]):
+        pulumi.set(self, "efi_disk", value)
+
+    @property
     @pulumi.getter
     def hostpcis(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]]]:
         """
         The Host PCI devices mapped to the VM
         """
         return pulumi.get(self, "hostpcis")
 
@@ -621,14 +637,15 @@
                  bios: Optional[pulumi.Input[str]] = None,
                  boot_orders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cdrom: Optional[pulumi.Input['VirtualMachineCdromArgs']] = None,
                  clone: Optional[pulumi.Input['VirtualMachineCloneArgs']] = None,
                  cpu: Optional[pulumi.Input['VirtualMachineCpuArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disks: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]]] = None,
+                 efi_disk: Optional[pulumi.Input['VirtualMachineEfiDiskArgs']] = None,
                  hostpcis: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]]] = None,
                  initialization: Optional[pulumi.Input['VirtualMachineInitializationArgs']] = None,
                  ipv4_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]]] = None,
                  ipv6_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]]] = None,
                  keyboard_layout: Optional[pulumi.Input[str]] = None,
                  kvm_arguments: Optional[pulumi.Input[str]] = None,
                  mac_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
@@ -664,14 +681,15 @@
         :param pulumi.Input[str] bios: The BIOS implementation
         :param pulumi.Input[Sequence[pulumi.Input[str]]] boot_orders: The guest will attempt to boot from devices in the order they appear here
         :param pulumi.Input['VirtualMachineCdromArgs'] cdrom: The CDROM drive
         :param pulumi.Input['VirtualMachineCloneArgs'] clone: The cloning configuration
         :param pulumi.Input['VirtualMachineCpuArgs'] cpu: The CPU allocation
         :param pulumi.Input[str] description: The description
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]] disks: The disk devices
+        :param pulumi.Input['VirtualMachineEfiDiskArgs'] efi_disk: The efidisk device
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]] hostpcis: The Host PCI devices mapped to the VM
         :param pulumi.Input['VirtualMachineInitializationArgs'] initialization: The cloud-init configuration
         :param pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]] ipv4_addresses: The IPv4 addresses published by the QEMU agent
         :param pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]] ipv6_addresses: The IPv6 addresses published by the QEMU agent
         :param pulumi.Input[str] keyboard_layout: The keyboard layout
         :param pulumi.Input[str] kvm_arguments: The args implementation
         :param pulumi.Input[Sequence[pulumi.Input[str]]] mac_addresses: The MAC addresses for the network interfaces
@@ -716,14 +734,16 @@
             pulumi.set(__self__, "clone", clone)
         if cpu is not None:
             pulumi.set(__self__, "cpu", cpu)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if disks is not None:
             pulumi.set(__self__, "disks", disks)
+        if efi_disk is not None:
+            pulumi.set(__self__, "efi_disk", efi_disk)
         if hostpcis is not None:
             pulumi.set(__self__, "hostpcis", hostpcis)
         if initialization is not None:
             pulumi.set(__self__, "initialization", initialization)
         if ipv4_addresses is not None:
             pulumi.set(__self__, "ipv4_addresses", ipv4_addresses)
         if ipv6_addresses is not None:
@@ -900,14 +920,26 @@
         return pulumi.get(self, "disks")
 
     @disks.setter
     def disks(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]]]):
         pulumi.set(self, "disks", value)
 
     @property
+    @pulumi.getter(name="efiDisk")
+    def efi_disk(self) -> Optional[pulumi.Input['VirtualMachineEfiDiskArgs']]:
+        """
+        The efidisk device
+        """
+        return pulumi.get(self, "efi_disk")
+
+    @efi_disk.setter
+    def efi_disk(self, value: Optional[pulumi.Input['VirtualMachineEfiDiskArgs']]):
+        pulumi.set(self, "efi_disk", value)
+
+    @property
     @pulumi.getter
     def hostpcis(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineHostpciArgs']]]]:
         """
         The Host PCI devices mapped to the VM
         """
         return pulumi.get(self, "hostpcis")
 
@@ -1287,14 +1319,15 @@
                  bios: Optional[pulumi.Input[str]] = None,
                  boot_orders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cdrom: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCdromArgs']]] = None,
                  clone: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCloneArgs']]] = None,
                  cpu: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCpuArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]]] = None,
+                 efi_disk: Optional[pulumi.Input[pulumi.InputType['VirtualMachineEfiDiskArgs']]] = None,
                  hostpcis: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]]] = None,
                  initialization: Optional[pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']]] = None,
                  keyboard_layout: Optional[pulumi.Input[str]] = None,
                  kvm_arguments: Optional[pulumi.Input[str]] = None,
                  machine: Optional[pulumi.Input[str]] = None,
                  memory: Optional[pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
@@ -1329,14 +1362,15 @@
         :param pulumi.Input[str] bios: The BIOS implementation
         :param pulumi.Input[Sequence[pulumi.Input[str]]] boot_orders: The guest will attempt to boot from devices in the order they appear here
         :param pulumi.Input[pulumi.InputType['VirtualMachineCdromArgs']] cdrom: The CDROM drive
         :param pulumi.Input[pulumi.InputType['VirtualMachineCloneArgs']] clone: The cloning configuration
         :param pulumi.Input[pulumi.InputType['VirtualMachineCpuArgs']] cpu: The CPU allocation
         :param pulumi.Input[str] description: The description
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]] disks: The disk devices
+        :param pulumi.Input[pulumi.InputType['VirtualMachineEfiDiskArgs']] efi_disk: The efidisk device
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]] hostpcis: The Host PCI devices mapped to the VM
         :param pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']] initialization: The cloud-init configuration
         :param pulumi.Input[str] keyboard_layout: The keyboard layout
         :param pulumi.Input[str] kvm_arguments: The args implementation
         :param pulumi.Input[str] machine: The VM machine type, either default i440fx or q35
         :param pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']] memory: The memory allocation
         :param pulumi.Input[str] name: The name
@@ -1390,14 +1424,15 @@
                  bios: Optional[pulumi.Input[str]] = None,
                  boot_orders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cdrom: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCdromArgs']]] = None,
                  clone: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCloneArgs']]] = None,
                  cpu: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCpuArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]]] = None,
+                 efi_disk: Optional[pulumi.Input[pulumi.InputType['VirtualMachineEfiDiskArgs']]] = None,
                  hostpcis: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]]] = None,
                  initialization: Optional[pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']]] = None,
                  keyboard_layout: Optional[pulumi.Input[str]] = None,
                  kvm_arguments: Optional[pulumi.Input[str]] = None,
                  machine: Optional[pulumi.Input[str]] = None,
                  memory: Optional[pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
@@ -1436,14 +1471,15 @@
             __props__.__dict__["bios"] = bios
             __props__.__dict__["boot_orders"] = boot_orders
             __props__.__dict__["cdrom"] = cdrom
             __props__.__dict__["clone"] = clone
             __props__.__dict__["cpu"] = cpu
             __props__.__dict__["description"] = description
             __props__.__dict__["disks"] = disks
+            __props__.__dict__["efi_disk"] = efi_disk
             __props__.__dict__["hostpcis"] = hostpcis
             __props__.__dict__["initialization"] = initialization
             __props__.__dict__["keyboard_layout"] = keyboard_layout
             __props__.__dict__["kvm_arguments"] = kvm_arguments
             __props__.__dict__["machine"] = machine
             __props__.__dict__["memory"] = memory
             __props__.__dict__["name"] = name
@@ -1489,14 +1525,15 @@
             bios: Optional[pulumi.Input[str]] = None,
             boot_orders: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             cdrom: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCdromArgs']]] = None,
             clone: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCloneArgs']]] = None,
             cpu: Optional[pulumi.Input[pulumi.InputType['VirtualMachineCpuArgs']]] = None,
             description: Optional[pulumi.Input[str]] = None,
             disks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]]] = None,
+            efi_disk: Optional[pulumi.Input[pulumi.InputType['VirtualMachineEfiDiskArgs']]] = None,
             hostpcis: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]]] = None,
             initialization: Optional[pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']]] = None,
             ipv4_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]]] = None,
             ipv6_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]]] = None,
             keyboard_layout: Optional[pulumi.Input[str]] = None,
             kvm_arguments: Optional[pulumi.Input[str]] = None,
             mac_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
@@ -1537,14 +1574,15 @@
         :param pulumi.Input[str] bios: The BIOS implementation
         :param pulumi.Input[Sequence[pulumi.Input[str]]] boot_orders: The guest will attempt to boot from devices in the order they appear here
         :param pulumi.Input[pulumi.InputType['VirtualMachineCdromArgs']] cdrom: The CDROM drive
         :param pulumi.Input[pulumi.InputType['VirtualMachineCloneArgs']] clone: The cloning configuration
         :param pulumi.Input[pulumi.InputType['VirtualMachineCpuArgs']] cpu: The CPU allocation
         :param pulumi.Input[str] description: The description
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]] disks: The disk devices
+        :param pulumi.Input[pulumi.InputType['VirtualMachineEfiDiskArgs']] efi_disk: The efidisk device
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineHostpciArgs']]]] hostpcis: The Host PCI devices mapped to the VM
         :param pulumi.Input[pulumi.InputType['VirtualMachineInitializationArgs']] initialization: The cloud-init configuration
         :param pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]] ipv4_addresses: The IPv4 addresses published by the QEMU agent
         :param pulumi.Input[Sequence[pulumi.Input[Sequence[pulumi.Input[str]]]]] ipv6_addresses: The IPv6 addresses published by the QEMU agent
         :param pulumi.Input[str] keyboard_layout: The keyboard layout
         :param pulumi.Input[str] kvm_arguments: The args implementation
         :param pulumi.Input[Sequence[pulumi.Input[str]]] mac_addresses: The MAC addresses for the network interfaces
@@ -1583,14 +1621,15 @@
         __props__.__dict__["bios"] = bios
         __props__.__dict__["boot_orders"] = boot_orders
         __props__.__dict__["cdrom"] = cdrom
         __props__.__dict__["clone"] = clone
         __props__.__dict__["cpu"] = cpu
         __props__.__dict__["description"] = description
         __props__.__dict__["disks"] = disks
+        __props__.__dict__["efi_disk"] = efi_disk
         __props__.__dict__["hostpcis"] = hostpcis
         __props__.__dict__["initialization"] = initialization
         __props__.__dict__["ipv4_addresses"] = ipv4_addresses
         __props__.__dict__["ipv6_addresses"] = ipv6_addresses
         __props__.__dict__["keyboard_layout"] = keyboard_layout
         __props__.__dict__["kvm_arguments"] = kvm_arguments
         __props__.__dict__["mac_addresses"] = mac_addresses
@@ -1697,14 +1736,22 @@
     def disks(self) -> pulumi.Output[Optional[Sequence['outputs.VirtualMachineDisk']]]:
         """
         The disk devices
         """
         return pulumi.get(self, "disks")
 
     @property
+    @pulumi.getter(name="efiDisk")
+    def efi_disk(self) -> pulumi.Output[Optional['outputs.VirtualMachineEfiDisk']]:
+        """
+        The efidisk device
+        """
+        return pulumi.get(self, "efi_disk")
+
+    @property
     @pulumi.getter
     def hostpcis(self) -> pulumi.Output[Optional[Sequence['outputs.VirtualMachineHostpci']]]:
         """
         The Host PCI devices mapped to the VM
         """
         return pulumi.get(self, "hostpcis")
```

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 5.7.0
+Version: 5.8.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-5.8.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.7.0/setup.py` & `pulumi_proxmoxve-5.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.7.0"
-PLUGIN_VERSION = "5.7.0"
+VERSION = "5.8.0"
+PLUGIN_VERSION = "5.8.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'proxmoxve', PLUGIN_VERSION, '--server', 'github://api.github.com/muhlba91/pulumi-proxmoxve'])
         except OSError as error:
```

