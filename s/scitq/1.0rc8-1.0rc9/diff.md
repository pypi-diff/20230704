# Comparing `tmp/scitq-1.0rc8.tar.gz` & `tmp/scitq-1.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scitq-1.0rc8.tar", last modified: Tue Jan 10 20:49:03 2023, max compression
+gzip compressed data, was "scitq-1.0rc9.tar", last modified: Sun Jan 15 12:49:01 2023, max compression
```

## Comparing `scitq-1.0rc8.tar` & `scitq-1.0rc9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.331174 scitq-1.0rc8/
--rw-r--r--   0 lahondes   (501) staff       (20)       21 2022-12-02 12:57:12.000000 scitq-1.0rc8/.gitignore
--rw-r--r--   0 lahondes   (501) staff       (20)    35149 2022-11-03 09:42:58.000000 scitq-1.0rc8/LICENSE
--rw-r--r--   0 lahondes   (501) staff       (20)      114 2022-11-27 14:16:00.000000 scitq-1.0rc8/MANIFEST.in
--rw-r--r--   0 lahondes   (501) staff       (20)    11253 2023-01-10 20:49:03.330329 scitq-1.0rc8/PKG-INFO
--rw-r--r--   0 lahondes   (501) staff       (20)    10623 2022-12-10 11:35:31.000000 scitq-1.0rc8/README.md
--rw-r--r--   0 lahondes   (501) staff       (20)     1255 2023-01-07 14:17:51.000000 scitq-1.0rc8/pyproject.toml
--rw-r--r--   0 lahondes   (501) staff       (20)       38 2023-01-10 20:49:03.331322 scitq-1.0rc8/setup.cfg
--rw-r--r--   0 lahondes   (501) staff       (20)       38 2022-11-27 13:55:47.000000 scitq-1.0rc8/setup.py
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.215533 scitq-1.0rc8/src/
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.239073 scitq-1.0rc8/src/scitq/
--rw-r--r--   0 lahondes   (501) staff       (20)        0 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/__init__.py
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.254343 scitq-1.0rc8/src/scitq/ansible/
--rw-r--r--   0 lahondes   (501) staff       (20)     6148 2022-10-22 13:42:43.000000 scitq-1.0rc8/src/scitq/ansible/.DS_Store
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.255224 scitq-1.0rc8/src/scitq/ansible/.vscode/
--rw-r--r--   0 lahondes   (501) staff       (20)     1537 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/ansible/.vscode/settings.json
--rw-r--r--   0 lahondes   (501) staff       (20)     3563 2022-11-27 14:00:24.000000 scitq-1.0rc8/src/scitq/ansible/README.md
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.256249 scitq-1.0rc8/src/scitq/ansible/etc/
--rw-r--r--   0 lahondes   (501) staff       (20)    38400 2022-11-27 10:10:40.000000 scitq-1.0rc8/src/scitq/ansible/etc/ansible.cfg
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.294495 scitq-1.0rc8/src/scitq/ansible/playbooks/
--rw-r--r--   0 lahondes   (501) staff       (20)       76 2022-11-24 22:02:30.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_docker.j2
--rw-r--r--   0 lahondes   (501) staff       (20)      878 2022-11-24 22:02:30.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_docker.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      119 2022-11-24 22:02:30.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_docker2.j2
--rw-r--r--   0 lahondes   (501) staff       (20)      198 2022-04-06 19:46:46.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_in_etchosts.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      540 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_in_firewall.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      156 2022-04-06 19:47:08.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_in_nfs_exports.j2
--rw-r--r--   0 lahondes   (501) staff       (20)      595 2022-07-05 14:54:21.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_in_nfs_exports.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)       77 2022-07-05 14:54:21.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_in_nfs_exports2.j2
--rw-r--r--   0 lahondes   (501) staff       (20)      798 2022-07-05 14:54:21.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_nfs.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      535 2022-07-05 14:54:21.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_s3authentication.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      188 2022-07-05 14:54:21.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_s3authentication_config.j2
--rw-r--r--   0 lahondes   (501) staff       (20)       91 2022-07-05 14:54:21.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_s3authentication_credentials.j2
--rw-r--r--   0 lahondes   (501) staff       (20)      227 2023-01-06 07:52:11.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_scitq.j2
--rw-r--r--   0 lahondes   (501) staff       (20)     1114 2022-12-01 21:46:13.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_scitq.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      597 2022-07-05 14:54:21.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_scratch.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      995 2022-10-22 21:33:23.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/add_swap.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      195 2023-01-04 16:42:08.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/check_after_reboot.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)     3263 2023-01-04 09:02:45.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/deploy_one_vm.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)     1965 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/deploy_one_vm_manual.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      852 2023-01-09 07:57:17.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/destroy_vm.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      509 2022-07-05 14:54:21.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/destroy_vm_manual.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      124 2022-04-01 10:19:34.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/remove_from_etchosts.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      621 2023-01-09 07:56:22.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/remove_from_firewall.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      308 2022-07-05 14:54:21.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/remove_from_nfs_exports.yaml
--rw-r--r--   0 lahondes   (501) staff       (20)      191 2022-04-01 11:43:42.000000 scitq-1.0rc8/src/scitq/ansible/playbooks/remove_from_static_inventory.yaml
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.298464 scitq-1.0rc8/src/scitq/ansible/scitq/
--rw-r--r--   0 lahondes   (501) staff       (20)      341 2023-01-07 14:21:27.000000 scitq-1.0rc8/src/scitq/ansible/scitq/01-scitq-default
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.302239 scitq-1.0rc8/src/scitq/ansible/scitq/__pycache__/
--rw-r--r--   0 lahondes   (501) staff       (20)     7621 2022-11-28 23:14:49.000000 scitq-1.0rc8/src/scitq/ansible/scitq/__pycache__/sqlite_inventory.cpython-310.pyc
--rw-r--r--   0 lahondes   (501) staff       (20)     7631 2022-11-30 21:07:20.000000 scitq-1.0rc8/src/scitq/ansible/scitq/__pycache__/sqlite_inventory.cpython-38.pyc
--rwxr-xr-x   0 lahondes   (501) staff       (20)     8800 2023-01-04 15:10:32.000000 scitq-1.0rc8/src/scitq/ansible/scitq/sqlite_inventory.py
--rw-r--r--   0 lahondes   (501) staff       (20)    29139 2023-01-04 19:35:30.000000 scitq-1.0rc8/src/scitq/client.py
--rw-r--r--   0 lahondes   (501) staff       (20)      322 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/default_settings.py
--rw-r--r--   0 lahondes   (501) staff       (20)    16756 2023-01-06 17:42:35.000000 scitq-1.0rc8/src/scitq/fetch.py
--rwxr-xr-x   0 lahondes   (501) staff       (20)    10997 2022-11-28 23:19:32.000000 scitq-1.0rc8/src/scitq/launch.py
--rw-r--r--   0 lahondes   (501) staff       (20)    23301 2023-01-10 19:06:29.000000 scitq-1.0rc8/src/scitq/lib.py
--rw-r--r--   0 lahondes   (501) staff       (20)    18731 2023-01-09 07:48:32.000000 scitq-1.0rc8/src/scitq/manage.py
--rw-r--r--   0 lahondes   (501) staff       (20)    72283 2023-01-10 19:37:08.000000 scitq-1.0rc8/src/scitq/server.py
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.304807 scitq-1.0rc8/src/scitq/static/
--rw-r--r--   0 lahondes   (501) staff       (20)     6148 2022-11-24 18:54:18.000000 scitq-1.0rc8/src/scitq/static/.DS_Store
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.305947 scitq-1.0rc8/src/scitq/static/css/
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.308709 scitq-1.0rc8/src/scitq/static/css/bootstrap.v5.0.2/
--rw-r--r--   0 lahondes   (501) staff       (20)   155845 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/css/bootstrap.v5.0.2/bootstrap.min.css
--rw-r--r--   0 lahondes   (501) staff       (20)   431289 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/css/bootstrap.v5.0.2/bootstrap.min.css.map
--rw-r--r--   0 lahondes   (501) staff       (20)     1044 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/css/ui.css
--rw-r--r--   0 lahondes   (501) staff       (20)    48296 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/favicon.png
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.316298 scitq-1.0rc8/src/scitq/static/js/
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.319189 scitq-1.0rc8/src/scitq/static/js/FileSaver.v2.0.4/
--rw-r--r--   0 lahondes   (501) staff       (20)     2737 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/js/FileSaver.v2.0.4/FileSaver.min.js
--rw-r--r--   0 lahondes   (501) staff       (20)    10405 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/js/FileSaver.v2.0.4/FileSaver.min.js.map
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.322023 scitq-1.0rc8/src/scitq/static/js/bootstrap.v5.0.2/
--rw-r--r--   0 lahondes   (501) staff       (20)    60089 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/js/bootstrap.v5.0.2/bootstrap.min.js
--rw-r--r--   0 lahondes   (501) staff       (20)   217084 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/js/bootstrap.v5.0.2/bootstrap.min.js.map
--rw-r--r--   0 lahondes   (501) staff       (20)    89947 2023-01-10 15:58:43.000000 scitq-1.0rc8/src/scitq/static/js/jquery-3.6.3.min.js
--rw-r--r--   0 lahondes   (501) staff       (20)   138465 2023-01-10 15:58:44.000000 scitq-1.0rc8/src/scitq/static/js/jquery-3.6.3.min.map
--rw-r--r--   0 lahondes   (501) staff       (20)    97587 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/js/jszip.min.v3.10.0.js
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.325633 scitq-1.0rc8/src/scitq/static/js/socket.io.v4.0.1/
--rw-r--r--   0 lahondes   (501) staff       (20)   184956 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/js/socket.io.v4.0.1/socket.io.js
--rw-r--r--   0 lahondes   (501) staff       (20)   245074 2022-11-26 15:25:25.000000 scitq-1.0rc8/src/scitq/static/js/socket.io.v4.0.1/socket.io.js.map
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.329236 scitq-1.0rc8/src/scitq/templates/
--rw-r--r--   0 lahondes   (501) staff       (20)    13688 2023-01-10 15:58:44.000000 scitq-1.0rc8/src/scitq/templates/batch.html
--rw-r--r--   0 lahondes   (501) staff       (20)    34504 2023-01-10 15:58:44.000000 scitq-1.0rc8/src/scitq/templates/task.html
--rw-r--r--   0 lahondes   (501) staff       (20)    18293 2023-01-10 15:58:44.000000 scitq-1.0rc8/src/scitq/templates/ui.html
--rw-r--r--   0 lahondes   (501) staff       (20)     5350 2023-01-08 18:12:42.000000 scitq-1.0rc8/src/scitq/util.py
-drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-10 20:49:03.248005 scitq-1.0rc8/src/scitq.egg-info/
--rw-r--r--   0 lahondes   (501) staff       (20)    11253 2023-01-10 20:49:03.000000 scitq-1.0rc8/src/scitq.egg-info/PKG-INFO
--rw-r--r--   0 lahondes   (501) staff       (20)     2785 2023-01-10 20:49:03.000000 scitq-1.0rc8/src/scitq.egg-info/SOURCES.txt
--rw-r--r--   0 lahondes   (501) staff       (20)        1 2023-01-10 20:49:03.000000 scitq-1.0rc8/src/scitq.egg-info/dependency_links.txt
--rw-r--r--   0 lahondes   (501) staff       (20)      155 2023-01-10 20:49:03.000000 scitq-1.0rc8/src/scitq.egg-info/entry_points.txt
--rw-r--r--   0 lahondes   (501) staff       (20)      178 2023-01-10 20:49:03.000000 scitq-1.0rc8/src/scitq.egg-info/requires.txt
--rw-r--r--   0 lahondes   (501) staff       (20)        6 2023-01-10 20:49:03.000000 scitq-1.0rc8/src/scitq.egg-info/top_level.txt
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.574258 scitq-1.0rc9/
+-rw-r--r--   0 lahondes   (501) staff       (20)       21 2022-12-02 12:57:12.000000 scitq-1.0rc9/.gitignore
+-rw-r--r--   0 lahondes   (501) staff       (20)    35149 2022-11-03 09:42:58.000000 scitq-1.0rc9/LICENSE
+-rw-r--r--   0 lahondes   (501) staff       (20)      114 2022-11-27 14:16:00.000000 scitq-1.0rc9/MANIFEST.in
+-rw-r--r--   0 lahondes   (501) staff       (20)    11279 2023-01-15 12:49:01.573419 scitq-1.0rc9/PKG-INFO
+-rw-r--r--   0 lahondes   (501) staff       (20)    10649 2023-01-10 22:10:36.000000 scitq-1.0rc9/README.md
+-rw-r--r--   0 lahondes   (501) staff       (20)     1255 2023-01-12 07:40:35.000000 scitq-1.0rc9/pyproject.toml
+-rw-r--r--   0 lahondes   (501) staff       (20)       38 2023-01-15 12:49:01.574373 scitq-1.0rc9/setup.cfg
+-rw-r--r--   0 lahondes   (501) staff       (20)       38 2022-11-27 13:55:47.000000 scitq-1.0rc9/setup.py
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.398369 scitq-1.0rc9/src/
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.419717 scitq-1.0rc9/src/scitq/
+-rw-r--r--   0 lahondes   (501) staff       (20)        0 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/__init__.py
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.425183 scitq-1.0rc9/src/scitq/ansible/
+-rw-r--r--   0 lahondes   (501) staff       (20)     6148 2022-10-22 13:42:43.000000 scitq-1.0rc9/src/scitq/ansible/.DS_Store
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.426003 scitq-1.0rc9/src/scitq/ansible/.vscode/
+-rw-r--r--   0 lahondes   (501) staff       (20)     1537 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/ansible/.vscode/settings.json
+-rw-r--r--   0 lahondes   (501) staff       (20)     3563 2022-11-27 14:00:24.000000 scitq-1.0rc9/src/scitq/ansible/README.md
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.427029 scitq-1.0rc9/src/scitq/ansible/etc/
+-rw-r--r--   0 lahondes   (501) staff       (20)    38400 2022-11-27 10:10:40.000000 scitq-1.0rc9/src/scitq/ansible/etc/ansible.cfg
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.451404 scitq-1.0rc9/src/scitq/ansible/playbooks/
+-rw-r--r--   0 lahondes   (501) staff       (20)       76 2022-11-24 22:02:30.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_docker.j2
+-rw-r--r--   0 lahondes   (501) staff       (20)      878 2022-11-24 22:02:30.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_docker.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      119 2022-11-24 22:02:30.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_docker2.j2
+-rw-r--r--   0 lahondes   (501) staff       (20)      198 2022-04-06 19:46:46.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_in_etchosts.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      540 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_in_firewall.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      156 2022-04-06 19:47:08.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_in_nfs_exports.j2
+-rw-r--r--   0 lahondes   (501) staff       (20)      595 2022-07-05 14:54:21.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_in_nfs_exports.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)       77 2022-07-05 14:54:21.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_in_nfs_exports2.j2
+-rw-r--r--   0 lahondes   (501) staff       (20)      798 2022-07-05 14:54:21.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_nfs.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      535 2022-07-05 14:54:21.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_s3authentication.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      188 2022-07-05 14:54:21.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_s3authentication_config.j2
+-rw-r--r--   0 lahondes   (501) staff       (20)       91 2022-07-05 14:54:21.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_s3authentication_credentials.j2
+-rw-r--r--   0 lahondes   (501) staff       (20)      227 2023-01-06 07:52:11.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_scitq.j2
+-rw-r--r--   0 lahondes   (501) staff       (20)     1114 2022-12-01 21:46:13.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_scitq.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      597 2022-07-05 14:54:21.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_scratch.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      995 2022-10-22 21:33:23.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/add_swap.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      195 2023-01-04 16:42:08.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/check_after_reboot.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)     3288 2023-01-12 10:21:38.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/deploy_one_vm.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)     1965 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/deploy_one_vm_manual.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      952 2023-01-13 08:19:21.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/destroy_vm.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      509 2022-07-05 14:54:21.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/destroy_vm_manual.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      124 2022-04-01 10:19:34.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/remove_from_etchosts.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      667 2023-01-13 08:03:14.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/remove_from_firewall.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      354 2023-01-13 08:03:23.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/remove_from_nfs_exports.yaml
+-rw-r--r--   0 lahondes   (501) staff       (20)      191 2023-01-13 08:03:31.000000 scitq-1.0rc9/src/scitq/ansible/playbooks/remove_from_static_inventory.yaml
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.453004 scitq-1.0rc9/src/scitq/ansible/scitq/
+-rw-r--r--   0 lahondes   (501) staff       (20)      341 2023-01-10 21:26:01.000000 scitq-1.0rc9/src/scitq/ansible/scitq/01-scitq-default
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.454892 scitq-1.0rc9/src/scitq/ansible/scitq/__pycache__/
+-rw-r--r--   0 lahondes   (501) staff       (20)     7621 2022-11-28 23:14:49.000000 scitq-1.0rc9/src/scitq/ansible/scitq/__pycache__/sqlite_inventory.cpython-310.pyc
+-rw-r--r--   0 lahondes   (501) staff       (20)     7631 2022-11-30 21:07:20.000000 scitq-1.0rc9/src/scitq/ansible/scitq/__pycache__/sqlite_inventory.cpython-38.pyc
+-rwxr-xr-x   0 lahondes   (501) staff       (20)     8800 2023-01-04 15:10:32.000000 scitq-1.0rc9/src/scitq/ansible/scitq/sqlite_inventory.py
+-rw-r--r--   0 lahondes   (501) staff       (20)    30227 2023-01-14 11:02:21.000000 scitq-1.0rc9/src/scitq/client.py
+-rw-r--r--   0 lahondes   (501) staff       (20)      322 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/default_settings.py
+-rw-r--r--   0 lahondes   (501) staff       (20)    16776 2023-01-13 20:53:33.000000 scitq-1.0rc9/src/scitq/fetch.py
+-rwxr-xr-x   0 lahondes   (501) staff       (20)    10997 2022-11-28 23:19:32.000000 scitq-1.0rc9/src/scitq/launch.py
+-rw-r--r--   0 lahondes   (501) staff       (20)    23313 2023-01-12 19:31:53.000000 scitq-1.0rc9/src/scitq/lib.py
+-rw-r--r--   0 lahondes   (501) staff       (20)    18731 2023-01-09 07:48:32.000000 scitq-1.0rc9/src/scitq/manage.py
+-rw-r--r--   0 lahondes   (501) staff       (20)    72480 2023-01-14 11:10:44.000000 scitq-1.0rc9/src/scitq/server.py
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.507681 scitq-1.0rc9/src/scitq/static/
+-rw-r--r--   0 lahondes   (501) staff       (20)     6148 2022-11-24 18:54:18.000000 scitq-1.0rc9/src/scitq/static/.DS_Store
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.509108 scitq-1.0rc9/src/scitq/static/css/
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.511914 scitq-1.0rc9/src/scitq/static/css/bootstrap.v5.0.2/
+-rw-r--r--   0 lahondes   (501) staff       (20)   155845 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/css/bootstrap.v5.0.2/bootstrap.min.css
+-rw-r--r--   0 lahondes   (501) staff       (20)   431289 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/css/bootstrap.v5.0.2/bootstrap.min.css.map
+-rw-r--r--   0 lahondes   (501) staff       (20)     1044 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/css/ui.css
+-rw-r--r--   0 lahondes   (501) staff       (20)    48296 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/favicon.png
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.522591 scitq-1.0rc9/src/scitq/static/js/
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.531922 scitq-1.0rc9/src/scitq/static/js/FileSaver.v2.0.4/
+-rw-r--r--   0 lahondes   (501) staff       (20)     2737 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/js/FileSaver.v2.0.4/FileSaver.min.js
+-rw-r--r--   0 lahondes   (501) staff       (20)    10405 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/js/FileSaver.v2.0.4/FileSaver.min.js.map
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.542050 scitq-1.0rc9/src/scitq/static/js/bootstrap.v5.0.2/
+-rw-r--r--   0 lahondes   (501) staff       (20)    60089 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/js/bootstrap.v5.0.2/bootstrap.min.js
+-rw-r--r--   0 lahondes   (501) staff       (20)   217084 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/js/bootstrap.v5.0.2/bootstrap.min.js.map
+-rw-r--r--   0 lahondes   (501) staff       (20)    89947 2023-01-10 15:58:43.000000 scitq-1.0rc9/src/scitq/static/js/jquery-3.6.3.min.js
+-rw-r--r--   0 lahondes   (501) staff       (20)   138465 2023-01-10 15:58:44.000000 scitq-1.0rc9/src/scitq/static/js/jquery-3.6.3.min.map
+-rw-r--r--   0 lahondes   (501) staff       (20)    97587 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/js/jszip.min.v3.10.0.js
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.554888 scitq-1.0rc9/src/scitq/static/js/socket.io.v4.0.1/
+-rw-r--r--   0 lahondes   (501) staff       (20)   184956 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/js/socket.io.v4.0.1/socket.io.js
+-rw-r--r--   0 lahondes   (501) staff       (20)   245074 2022-11-26 15:25:25.000000 scitq-1.0rc9/src/scitq/static/js/socket.io.v4.0.1/socket.io.js.map
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.570667 scitq-1.0rc9/src/scitq/templates/
+-rw-r--r--   0 lahondes   (501) staff       (20)    13859 2023-01-14 10:55:51.000000 scitq-1.0rc9/src/scitq/templates/batch.html
+-rw-r--r--   0 lahondes   (501) staff       (20)    34716 2023-01-14 11:00:40.000000 scitq-1.0rc9/src/scitq/templates/task.html
+-rw-r--r--   0 lahondes   (501) staff       (20)    18580 2023-01-14 10:46:05.000000 scitq-1.0rc9/src/scitq/templates/ui.html
+-rw-r--r--   0 lahondes   (501) staff       (20)     5350 2023-01-08 18:12:42.000000 scitq-1.0rc9/src/scitq/util.py
+drwxr-xr-x   0 lahondes   (501) staff       (20)        0 2023-01-15 12:49:01.423290 scitq-1.0rc9/src/scitq.egg-info/
+-rw-r--r--   0 lahondes   (501) staff       (20)    11279 2023-01-15 12:49:01.000000 scitq-1.0rc9/src/scitq.egg-info/PKG-INFO
+-rw-r--r--   0 lahondes   (501) staff       (20)     2785 2023-01-15 12:49:01.000000 scitq-1.0rc9/src/scitq.egg-info/SOURCES.txt
+-rw-r--r--   0 lahondes   (501) staff       (20)        1 2023-01-15 12:49:01.000000 scitq-1.0rc9/src/scitq.egg-info/dependency_links.txt
+-rw-r--r--   0 lahondes   (501) staff       (20)      155 2023-01-15 12:49:01.000000 scitq-1.0rc9/src/scitq.egg-info/entry_points.txt
+-rw-r--r--   0 lahondes   (501) staff       (20)      178 2023-01-15 12:49:01.000000 scitq-1.0rc9/src/scitq.egg-info/requires.txt
+-rw-r--r--   0 lahondes   (501) staff       (20)        6 2023-01-15 12:49:01.000000 scitq-1.0rc9/src/scitq.egg-info/top_level.txt
```

### Comparing `scitq-1.0rc8/LICENSE` & `scitq-1.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/PKG-INFO` & `scitq-1.0rc9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitq
-Version: 1.0rc8
+Version: 1.0rc9
 Summary: A (distributed) scientific task queue
 Author: Raynald de Lahondès, Rémi Tan
 Project-URL: Homepage, https://github.com/gmtsciencedev/scitq
 Project-URL: Bug Tracker, https://github.com/gmtsciencedev/scitq/issues
 Project-URL: Documentation, https://scitq.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -198,14 +198,14 @@
 you wish, etc. At least that's what we thought, now with heavier loads, PostgreSQL
 is recommended (concurrency has its limits with sqlite), and is now the default.
 - A simple multiprocess worker (if you read multithread, re-read the sentence), 
 with a clever management of output flow. Asyncio was the solution here (process.poll()
 with stdout.readline() is not performant enough if you have heavy output).
 - A nice UI (like Celery Flower) : now this nice UI must update its display very
 often you do not want to reload the page to refresh (Flower is smart enough for 
-that): I did write a very small game in Python with Flask and I had had a go with
-SocketIO with quite a success, so I tried here and it fits the case. I compared
-with basic jQuery and it performed better so scitq uses SocketIO (and a nice
-Flask package: Flask-SocketIO)
+that): initially we had chosen socket.io for the UI however when we decided to deploy
+scitq in a serious way (with a wsgi server and not Flask development server), we were
+not able not configure socket.io in a multi-worker uwsgi setup, so we went back to 
+jQuery which is sufficient in our case.
 
 For now, UI and server live in the same Flask application which makes deploy
 very easy.
```

### Comparing `scitq-1.0rc8/README.md` & `scitq-1.0rc9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,14 @@
 you wish, etc. At least that's what we thought, now with heavier loads, PostgreSQL
 is recommended (concurrency has its limits with sqlite), and is now the default.
 - A simple multiprocess worker (if you read multithread, re-read the sentence), 
 with a clever management of output flow. Asyncio was the solution here (process.poll()
 with stdout.readline() is not performant enough if you have heavy output).
 - A nice UI (like Celery Flower) : now this nice UI must update its display very
 often you do not want to reload the page to refresh (Flower is smart enough for 
-that): I did write a very small game in Python with Flask and I had had a go with
-SocketIO with quite a success, so I tried here and it fits the case. I compared
-with basic jQuery and it performed better so scitq uses SocketIO (and a nice
-Flask package: Flask-SocketIO)
+that): initially we had chosen socket.io for the UI however when we decided to deploy
+scitq in a serious way (with a wsgi server and not Flask development server), we were
+not able not configure socket.io in a multi-worker uwsgi setup, so we went back to 
+jQuery which is sufficient in our case.
 
 For now, UI and server live in the same Flask application which makes deploy
 very easy.
```

### Comparing `scitq-1.0rc8/pyproject.toml` & `scitq-1.0rc9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scitq"
-version = "1.0rc8"
+version = "1.0rc9"
 authors = [
   { name="Raynald de Lahondès" },
   { name="Rémi Tan" }
 ]
 description = "A (distributed) scientific task queue"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `scitq-1.0rc8/src/scitq/ansible/.DS_Store` & `scitq-1.0rc9/src/scitq/ansible/.DS_Store`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/.vscode/settings.json` & `scitq-1.0rc9/src/scitq/ansible/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/README.md` & `scitq-1.0rc9/src/scitq/ansible/README.md`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/etc/ansible.cfg` & `scitq-1.0rc9/src/scitq/ansible/etc/ansible.cfg`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/add_docker.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/add_docker.yaml`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/add_in_firewall.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/add_in_firewall.yaml`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/add_in_nfs_exports.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/add_in_nfs_exports.yaml`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/add_nfs.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/add_nfs.yaml`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/add_s3authentication.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/add_s3authentication.yaml`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/add_scitq.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/add_scitq.yaml`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/add_scratch.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/add_scratch.yaml`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/add_swap.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/add_swap.yaml`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/deploy_one_vm.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/deploy_one_vm.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -67,18 +67,18 @@
   tasks:
           - name: Wait for ssh
             wait_for_connection:
               timeout: 300
           - name: Gather facts
             setup:
           - name: Copy scitq source
-            copy:
-              remote_src: no
+            ansible.posix.synchronize:
               src: "{{ scitq_src }}/"
               dest: /opt/scitq
+              use_ssh_args: true
             become: true
             when: scitq_src is defined
           - include_tasks: add_docker.yaml
           - include_tasks: add_nfs.yaml
           - include_tasks: add_scratch.yaml
           - include_tasks: add_s3authentication.yaml
           - name: Add swap
```

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/deploy_one_vm_manual.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/deploy_one_vm_manual.yaml`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/playbooks/remove_from_firewall.yaml` & `scitq-1.0rc9/src/scitq/ansible/playbooks/remove_from_firewall.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,24 @@
     source: "{{ hostvars[nodename].ipv4 }}"
     jump: ACCEPT
     protocol: all
     action: insert
     comment: "scitq : {{ nodename }}"
     state: absent
   become: true
+  async: 60
+  poll: 10
   when: hostvars[nodename].ipv4 is defined
 - name: Update the firewall with node IPv6
   ansible.builtin.iptables:
     chain: INPUT
     source: "{{ hostvars[nodename].ipv6 }}"
     jump: ACCEPT
     protocol: all
     action: insert
     comment: "scitq : {{ nodename }}"
     ip_version: ipv6
     state: absent
   become: true
+  async: 60
+  poll: 10
   when: hostvars[nodename].ipv6 is defined
```

### Comparing `scitq-1.0rc8/src/scitq/ansible/scitq/__pycache__/sqlite_inventory.cpython-310.pyc` & `scitq-1.0rc9/src/scitq/ansible/scitq/__pycache__/sqlite_inventory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/scitq/__pycache__/sqlite_inventory.cpython-38.pyc` & `scitq-1.0rc9/src/scitq/ansible/scitq/__pycache__/sqlite_inventory.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/ansible/scitq/sqlite_inventory.py` & `scitq-1.0rc9/src/scitq/ansible/scitq/sqlite_inventory.py`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/client.py` & `scitq-1.0rc9/src/scitq/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,17 @@
     server.
     It performs now preparation tasks and post operation tasks."""
 
     def __init__(self, server, execution_id, task_id, command, input, output, 
                 container, container_options, execution_started, execution_queue,
                 cpu, resource_dir, resource, resources_db, run_slots, run_slots_semaphore,
                 worker_id, status):
+        log.warning(f'Starting executor for {execution_id}')
         self.s = Server(server, style='object')
+        self.s.execution_update(execution_id, status='accepted')
         self.worker_id = worker_id
         self.execution_id = execution_id
         self.task_id = task_id
         self.command = command
         self.input = input
         if output and not output.endswith('/'):
             output+='/'
@@ -224,30 +226,46 @@
                 if time()-now>self.dynamic_read_timeout:
                     break
             except asyncio.TimeoutError:
                 break
             except Exception as e:
                 error.append(f'During stdout collection this error occured: {traceback.format_exc()}\n' )
                 break
-        self.s.execution_output_write(execution_id, ''.join(output))
+        
+        retry = 2
+        while retry > 0:
+            try:
+                self.s.execution_output_write(execution_id, ''.join(output))
+                break
+            except:
+                log.exception(f'Could not write output for {execution_id}:{output}')
+                retry -= 1                
 
         now = time()
         while True:
             try:
                 error.append(
                     (await asyncio.wait_for(self.process.stderr.readline(), self.dynamic_read_timeout)).decode('utf-8')
                 )
                 if time()-now>self.dynamic_read_timeout:
                     break
             except asyncio.TimeoutError:
                 break
             except Exception as e:
                 error.append(f'During stderr collection this error occured: {traceback.format_exc()}\n' )
                 break
-        self.s.execution_error_write(execution_id,''.join(error))
+        
+        retry = 2
+        while retry > 0:
+            try:
+                self.s.execution_error_write(execution_id,''.join(error))
+                break
+            except:
+                log.exception(f'Could not write error for {execution_id}:{error}')
+                retry -= 1
 
         qsize = self.s.queue_size()
         if qsize > QUEUE_SIZE_THRESHOLD:
             self.dynamic_read_timeout += READ_TIMEOUT
         elif qsize == 0 and self.dynamic_read_timeout > READ_TIMEOUT:
             self.dynamic_read_timeout -= READ_TIMEOUT
 
@@ -526,16 +544,14 @@
                                     'resource': task.resource,
                                     'resources_db': self.resources_db,
                                     'run_slots': self.run_slots,
                                     'run_slots_semaphore': self.run_slots_semaphore,
                                     'worker_id': self.w.worker_id,
                                     'status': self.executions_status[execution.execution_id]
                                 })
-                            # force synchronous call to make it blocking
-                            self.s.execution_update(execution.execution_id, status='accepted', asynchronous=False)
                             p.start()
                             self.executions[execution.execution_id]=(p,execution_queue)
                             self.has_worked = True
                             self.idle_time = None
                             log.info('Waiting for execution to start')
                             execution_started.acquire()
                             log.info('Execution started')
@@ -560,24 +576,35 @@
                     running_executions = [ execution_id 
                             for execution_id, execution_status in self.executions_status.items()
                             if execution_status.value==STATUS_RUNNING ]
                     log.warning(f'Status are { {execution_id:STATUS_TXT[execution_status.value] for execution_id, execution_status in self.executions_status.items()} }')
                     if self.concurrency-len(running_executions)!=self.run_slots.value:
                         log.warning(f'Race condition detected on process number')
                         # ok time to look what is really going on
+                        
                         running = waiting = 0
                         for execution in self.s.worker_executions(self.w.worker_id):
+                            if execution.status in ['failed','succeeded','pending']:
+                                continue
+                            if execution.execution_id not in self.executions_status:
+                                log.error('Execution {execution.execution_id} seems to have gone away...')
+                                self.s.execution_update(execution.execution_id, status='failed')
+                                continue
+
+                            status = self.executions_status[execution.execution_id].value
                             if execution.status=='running':
-                                if execution.execution_id not in running_executions:
-                                    log.warning(f'Execution {execution.execution_id} is supposed to be running and is not.')
-                                running += 1
+                                if status != STATUS_RUNNING:
+                                    log.warning(f'Execution {execution.execution_id} is supposed to be running and is not ({STATUS_TXT[status]}).')
+                                else:
+                                    running += 1
                             elif execution.status=='accepted':
-                                if execution.execution_id in running_executions:
-                                    log.warning(f'Execution {execution.execution_id} is not supposed to be running but is running.')
-                                waiting += 1
+                                if status not in [STATUS_WAITING, STATUS_LAUNCHING]:
+                                    log.warning(f'Execution {execution.execution_id} is supposed to be running and is not ({STATUS_TXT[status]}).')
+                                else:
+                                    waiting += 1
                         log.warning(f'We are supposed to have {self.concurrency} running processes and we have {running}')
                         log.warning(f'We are supposed to have {self.prefetch} waiting processes and we have {waiting}')    
                         log.warning(f'Overall we should have at max {self.concurrency+self.prefetch} processes and we have {len(self.executions)}')
                         if self.run_slots.value != self.concurrency - running:
                             log.warning(f'Run slot derived, reseting from {self.run_slots.value} to {self.concurrency-running}')
                             self.run_slots.value = self.concurrency - running
                     self.run_slots_semaphore.release()
```

### Comparing `scitq-1.0rc8/src/scitq/fetch.py` & `scitq-1.0rc9/src/scitq/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     subprocess.run(['pigz','-d',filepath], check=True)
     
 def untar(filepath):
     """Untar the tar archive locally where it is and delete the archive.
     (so it behaves like gunzip, and not like tar usually)"""
     path, basename = os.path.split(filepath)
     if basename.endswith('gz'):
-        subprocess.run(['tar','xzf',basename], cwd=path, check=True)
+        subprocess.run(f'pigz -dc "{basename}"|tar x', cwd=path, shell=True, check=True)
     else:
         subprocess.run(['tar','xf',basename], cwd=path, check=True)
     os.remove(filepath)
 
 # AWS S3 
 
 S3_REGEXP=re.compile(r'^s3://(?P<bucket>[^/]*)/(?P<path>.*)$')
```

### Comparing `scitq-1.0rc8/src/scitq/launch.py` & `scitq-1.0rc9/src/scitq/launch.py`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/lib.py` & `scitq-1.0rc9/src/scitq/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
         tasks = None
         dynamic_sleep_time = True
         sleep_time = JOIN_DYNAMIC_SLEEP_TIME_INCREMENT
         failed_tasks = []
         while not all_task_done:
             all_task_done = True
             old_tasks = tasks
-            tasks = {'assigned':0,'failed':0, 'running':0, 'accepted':0, 'pending':0,'succeeded':0}
+            tasks = {'assigned':0,'failed':0, 'running':0, 'accepted':0, 'pending':0,'succeeded':0, 'paused':0}
             for task in self.tasks():
                 if type(task)==dict:
                     task = Namespace(**task)
                 if task.task_id in task_ids:
                     if task.status=='failed':
                         if task_retries[task.task_id]<retry:
                             print(f'Retrying task {task.name or task.task_id} [{task_retries[task.task_id]+1}/{retry}]...')
```

### Comparing `scitq-1.0rc8/src/scitq/manage.py` & `scitq-1.0rc9/src/scitq/manage.py`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/server.py` & `scitq-1.0rc9/src/scitq/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,21 @@
 #app.config.from_pyfile("scitq.cfg", silent=True)
 #app.config.from_prefixed_env()
 if SQLALCHEMY_POOL_SIZE is not None:
     db = SQLAlchemy(app, engine_options={'pool_size': int(SQLALCHEMY_POOL_SIZE)})
 else:
     db = SQLAlchemy(app)
 
+# with uwsgi, the master worker is forking to create the workers which receive a 
+# non-working connection (because it comes from another process), it must be discarded
+# so that workers re-open the connection properly
+# idea from https://stackoverflow.com/questions/39562838/how-to-configure-pyramid-uwsgi-sqlalchemy
 try:
+    # import uwsgi is only working in uwsgi context. It is normal that is fails
+    # to import in VisualStudioCode or manually
     import uwsgi
 
     def postfork():
         db.engine.dispose()
     uwsgi.post_fork_hook = postfork
 except ImportError:
     pass
@@ -185,31 +191,15 @@
         self.status = status
         self.creation_date = datetime.utcnow()
         self.modification_date = self.creation_date
         self.hostname = hostname
         self.batch = batch
         self.idle_callback = idle_callback
     
-    def destroy(self):
-        """Destroy self (stop in provider renting)"""
-        log.warning(f'Worker {self.name} is to be destroyed.')
-
-        for i in range(WORKER_DESTROY_RETRY):
-            try:
-                run([self.idle_callback.format(**(self.__dict__))],shell=True,check=True)
-            except Exception as e:
-                log.exception(e)
-
-            worker_check = json.loads(scitq_inventory(host=self.hostname))
-
-            if not worker_check:
-                log.warning(f'Worker {self.name} was destroyed.')
-                break
-            else:
-                log.exception(f'Worker {self.name} was not properly destroyed (f{worker_check}), retrying.')
+
 class Execution(db.Model):
     __tablename__ = "execution"
     execution_id = db.Column(db.Integer, primary_key=True)
     worker_id = db.Column(db.Integer, db.ForeignKey("worker.worker_id"), nullable=True)
     worker = db.relationship(
         Worker,
         backref=db.backref('executions',
@@ -631,19 +621,18 @@
                     Execution.worker_id==worker.worker_id).count()>0:
                 log.warning(f'Worker {worker.name} called idle callback but some tasks are still running, refusing...')
                 return {'result':'still have running tasks'}
             if db.session.query(Task).filter(and_(Task.status.in_(['pending']),
                                     Task.batch==worker.batch)).count()>0:
                 log.warning(f'Worker {worker.name} called idle but some tasks are still due...')
                 return {'result':'still some work to do, lazy one!'}
-            log.warning(f'Worker {worker.name} called idle callback, launching: '+worker.idle_callback.format(**(worker.__dict__)))
+            log.warning(f'Worker {worker.name} ({worker.worker_id}) called idle callback, launching: '+worker.idle_callback.format(**(worker.__dict__)))
             #worker.destroy()
             create_worker_destroy_job(worker, db.session, commit=False)
-
-            db.session.delete(worker)
+            #db.session.delete(worker)
             db.session.commit()
             return {'result':'ok'}
         else:
             log.warning(f'Worker {worker.name} called idle callback but has no idle command')
             return {'result':'nothing to do'}
 
 deploy_parser = api.parser()
@@ -1576,15 +1565,15 @@
                                 worker.idle_callback,
                                 stdout = PIPE,
                                 stderr = PIPE,
                                 shell = True,
                                 encoding = 'utf-8'
                             )
                         job.status='running'
-                        worker_process_queue[('destroy',job.target)]=(worker, worker_delete_process,job.job_id)
+                        worker_process_queue[('destroy',job.target)]=(worker, worker_delete_process, job.job_id)
                         log.warning(f'Worker {job.target} destruction process has been launched')
                 
                 if job.action == 'worker_create':
                     change = True
                     worker = create_worker_object(db_session=session,
                         **job.args)
                     job.action = 'worker_deploy'
@@ -1638,22 +1627,28 @@
                     del(worker_process_queue[(action,worker_name)])
                     if returncode == 0:
                         log.warning(f'Process {action} succeeded for worker {worker.name}.')
                         job.log = worker_process.stdout.read()
                         job.status = 'succeeded'
 
                         if action=='destroy':
-                            log.warning(f'Deleting worker ')
                             #session.execute(Worker.__table__.delete().where(
                             #    Worker.__table__.c.worker_id==worker.worker_id))
-                            worker_dao.delete(worker.worker_id, is_destroyed=True)
+                            log.warning(f'Deleting worker {worker.name} ({worker.worker_id})')
+                            real_worker = session.query(Worker).get(worker.worker_id)
+                            if real_worker is not None:
+                                session.delete(real_worker)
+                            else:
+                                log.error(f'Could not find a worker with worker_id {worker.worker_id}')
+                            #worker_dao.delete(worker.worker_id, is_destroyed=True)
                     else:
                         stderr = worker_process.stderr.read()
                         log.warning(f'Process {action} failed for worker {worker.name}: {stderr}')
                         job.log = worker_process.stdout.read() + stderr
+                        log.warning(f'Job output is {job.log}')
                         if job.retry > 0:
                             job.retry -= 1
                             job.status = 'pending'
                         else:
                             job.status = 'failed'
                             if action=='create':
                                 worker = session.query(Worker).get(job.args['worker_id'])
@@ -1691,14 +1686,13 @@
         sleep(MAIN_THREAD_SLEEP)
 
 if not os.environ.get('SCITQ_PRODUCTION'):
     Thread(target=background).start()
 
 
 def main():
-    #app.run(debug=False)
-    socketio.run(app)
+    app.run(debug=True)
 
 if __name__ == "__main__":
     #raise RuntimeError('Do not launch directly, launch with "FLASK=scitq.server flask run"')
     #main()
     pass
```

### Comparing `scitq-1.0rc8/src/scitq/static/.DS_Store` & `scitq-1.0rc9/src/scitq/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/css/bootstrap.v5.0.2/bootstrap.min.css` & `scitq-1.0rc9/src/scitq/static/css/bootstrap.v5.0.2/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/css/bootstrap.v5.0.2/bootstrap.min.css.map` & `scitq-1.0rc9/src/scitq/static/css/bootstrap.v5.0.2/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/css/ui.css` & `scitq-1.0rc9/src/scitq/static/css/ui.css`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/favicon.png` & `scitq-1.0rc9/src/scitq/static/favicon.png`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/js/FileSaver.v2.0.4/FileSaver.min.js` & `scitq-1.0rc9/src/scitq/static/js/FileSaver.v2.0.4/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/js/FileSaver.v2.0.4/FileSaver.min.js.map` & `scitq-1.0rc9/src/scitq/static/js/FileSaver.v2.0.4/FileSaver.min.js.map`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/js/bootstrap.v5.0.2/bootstrap.min.js` & `scitq-1.0rc9/src/scitq/static/js/bootstrap.v5.0.2/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/js/bootstrap.v5.0.2/bootstrap.min.js.map` & `scitq-1.0rc9/src/scitq/static/js/bootstrap.v5.0.2/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/js/jquery-3.6.3.min.js` & `scitq-1.0rc9/src/scitq/static/js/jquery-3.6.3.min.js`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/js/jquery-3.6.3.min.map` & `scitq-1.0rc9/src/scitq/static/js/jquery-3.6.3.min.map`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/js/jszip.min.v3.10.0.js` & `scitq-1.0rc9/src/scitq/static/js/jszip.min.v3.10.0.js`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/js/socket.io.v4.0.1/socket.io.js` & `scitq-1.0rc9/src/scitq/static/js/socket.io.v4.0.1/socket.io.js`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/static/js/socket.io.v4.0.1/socket.io.js.map` & `scitq-1.0rc9/src/scitq/static/js/socket.io.v4.0.1/socket.io.js.map`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq/templates/batch.html` & `scitq-1.0rc9/src/scitq/templates/batch.html`

 * *Files 3% similar despite different names*

```diff
@@ -7,33 +7,47 @@
   <script src={{ url_for("static", filename="js/FileSaver.v2.0.4/FileSaver.min.js") }}></script>
   <script src={{ url_for("static", filename="js/jszip.min.v3.10.0.js") }}></script>
   <!-- <script src={{ url_for("static", filename="js/socket.io.v4.0.1/socket.io.js") }}></script> -->
   <script src="{{ url_for('static', filename='js/jquery-3.6.3.min.js') }}"></script>
   <script type="text/javascript" charset="utf-8">
     // All the class come from the Bootstrap v5 documentation and icon also come from bootstrap
    //const delay = ms => new Promise(res => setTimeout(res, ms));
-    function sleep (time) {
-        return new Promise((resolve) => setTimeout(resolve, time));
-      }
-    pause=false;
+    //function sleep (time) {
+    //    return new Promise((resolve) => setTimeout(resolve, time));
+    //  }
+    //pause=false;
     //var socket = io();
     //socket.on('connect', function() {
     //    console.log('connecting');
     //    socket.emit('get', {object: 'batch'});
     //    });
         
+var intervalID = null;
+function pause() { 
+    if (intervalID) {
+        clearInterval(intervalID);
+        intervalID = null;
+    }
+}
+
+function unpause() {
+    if (intervalID) {
+        clearInterval(intervalID);
+    }
+    intervalID = setInterval(get_batch, 5000);
+}
+    
+
 function get_batch() {
   $.getJSON('/ui/get/', {
     object: 'batch'
-  }, async function(data) {
+  }, function(data) {
   //  socket.on('batch', async function(data){
       //some action such as modify a action needs time to be done so the update of the page can be set on true 
-      while(pause){
-        await sleep(5000);
-      }
+
         batches= data.batches;
         workers=data.workers;
         console.log('Received batches', batches);
         console.log('Received workers', workers);
         batch_table ='<table class="table table-responsive table-hover table-striped text-center "><thead class="text-center table-secondary"><tr><th>#</th><th>Name</th><th>Workers</th><th>Progress</th><th>pending</th><th>running</th><th>successes</th><th>failed</th><th>total</th><th>Average duration [min - max] </th><th>Actions</th></tr></thead>\n<tbody id="table">\n';
         list_batch=[];
         workers_by_batch =new Map();
@@ -101,36 +115,35 @@
                     +'<div id="batch-modal-'+current_batch+'" class="modal"></div>'
                     +'</td></tr>\n';
           
           i--;
         }
         batch_table +='</tbody>\n</table>\n';
         document.getElementById("batches").innerHTML=batch_table; 
-        await sleep(5000);
-        get_batch();
+        unpause();
         //socket.emit('get', {object:'batch'});
     });
   }
 
   function displayModal(current_batch,type,status_paused=0) {
         //Status is only used with type = go.
         console.log(document.getElementById('batch-modal-'+current_batch));
         if(type==='pause'||type==='go'){
           document.getElementById('batch-modal-'+current_batch).innerHTML='<div class="modal-dialog modal-dialog-centered"><form class="modal-content"><div class="container"><h3>'+type+'</h3><p> Do you want to '+(type==='go'?'start/restart the batch ' : type +' the batch' ) +' '+current_batch+' '+(type==='go'?'and resume the tasks in pause ('+status_paused+') ?':'and the tasks in progress ?')+'</p>'
-                                                                +'<div class="clearfix"><button type="button" class="btn btn-danger" onclick="document.getElementById(\'batch-modal-'+current_batch+'\').style.display=\''+'none'+'\'; pause = false" >Cancel</button>'
-                                                                +'<button type="button" class="btn btn-warning" onclick="action_batch(\''+current_batch+'\',\''+type+'\');document.getElementById(\'batch-modal-'+current_batch+'\').style.display=\''+'none'+'\'; pause = false">Both</button>'
-                                                                +'<button type="button" class="btn btn-primary" onclick="action_batch(\''+current_batch+'\',\'simple '+type+'\');document.getElementById(\'batch-modal-'+current_batch+'\').style.display=\''+'none'+'\'; pause = false">Only Batch</button></div></div></form>';
+                                                                +'<div class="clearfix"><button type="button" class="btn btn-danger" onclick="document.getElementById(\'batch-modal-'+current_batch+'\').style.display=\''+'none'+'\'; unpause()" >Cancel</button>'
+                                                                +'<button type="button" class="btn btn-warning" onclick="action_batch(\''+current_batch+'\',\''+type+'\');document.getElementById(\'batch-modal-'+current_batch+'\').style.display=\''+'none'+'\'; unpause()">Both</button>'
+                                                                +'<button type="button" class="btn btn-primary" onclick="action_batch(\''+current_batch+'\',\'simple '+type+'\');document.getElementById(\'batch-modal-'+current_batch+'\').style.display=\''+'none'+'\'; unpause()">Only Batch</button></div></div></form>';
         }
         else{
         document.getElementById('batch-modal-'+current_batch).innerHTML='<div class="modal-dialog modal-dialog-centered"><form class="modal-content"><div class="container"><h3>'+type+'</h3><p>Are you sure you want to '+type+' '+current_batch+' ?</p>'
-                                                                +'<div class="clearfix"><button type="button" class="btn btn-danger" onclick="document.getElementById(\'batch-modal-'+current_batch+'\').style.display=\''+'none'+'\'; pause = false" >Cancel</button>'
-                                                                +'<button type="button" class="btn btn-primary" onclick="action_batch(\''+current_batch+'\',\''+type+'\');document.getElementById(\'batch-modal-'+current_batch+'\').style.display=\''+'none'+'\'; pause = false">Confirm</button></div></div></form>';
+                                                                +'<div class="clearfix"><button type="button" class="btn btn-danger" onclick="document.getElementById(\'batch-modal-'+current_batch+'\').style.display=\''+'none'+'\'; unpause()" >Cancel</button>'
+                                                                +'<button type="button" class="btn btn-primary" onclick="action_batch(\''+current_batch+'\',\''+type+'\');document.getElementById(\'batch-modal-'+current_batch+'\').style.display=\''+'none'+'\'; unpause()">Confirm</button></div></div></form>';
         }
         document.getElementById('batch-modal-'+current_batch).style.display = "block";
-        pause=true;
+        pause();
     }
 
   function getAvg(diff_in_second){
     if (diff_in_second>3600*24) {
         return [(diff_in_second/(3600*24)).toFixed(1),'d'];
     }
     else if(diff_in_second>3600){
```

### Comparing `scitq-1.0rc8/src/scitq/templates/task.html` & `scitq-1.0rc9/src/scitq/templates/task.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,36 @@
 <script src={{ url_for("static", filename="js/jszip.min.v3.10.0.js") }}></script>
 <!-- <script src={{ url_for("static", filename="js/socket.io.v4.0.1/socket.io.js") }}></script> -->
 <script src="{{ url_for('static', filename='js/jquery-3.6.3.min.js') }}"></script>
 <script type="text/javascript" charset="utf-8">
     // All the class come from the Bootstrap v5 documentation and icon also come from bootstrap
     MAX_CARACTERE_DIPLAYED_IN_CONTENT=1000;
     MAX_DISPLAYED_ROW = 500;
-    //const delay = ms => new Promise(res => setTimeout(res, ms));
-    function sleep (time) {
-        return new Promise((resolve) => setTimeout(resolve, time));
-      }
-    pause = false;
+      
+    var intervalID = null;
+    var current_parameters = {};
+
+    function pause() { 
+        if (intervalID) {
+            clearInterval(intervalID);
+            intervalID = null;
+            return true;
+        } {return false;} ;
+    }
+      
+    function unpause(parameters) {
+        if (intervalID) {
+            clearInterval(intervalID);
+        };
+        if (parameters !== undefined) {
+          current_parameters = parameters;
+        };
+        intervalID = setInterval(get_tasks, 5000, current_parameters);
+    }
+      
     
     //var socket = io();
     //getting param for the filter
     url = new URL(window.location.href); 
     var filter = new Map();
     var windows_open=new Map();
     var paused_task=new Map();
@@ -66,18 +83,18 @@
     //    });
     
 function get_tasks(parameters) {
     //socket.on('task', async function(data){
     
     //some action such as modifying a action needs time to be done so the update of the page can be set on true 
     parameters.object='tasks';
-    $.getJSON('/ui/get/', parameters, async function(data) {
-        while(pause){
-            await sleep(5000);
-        };    
+    $.getJSON('/ui/get/', parameters, function(data) {
+        //while(pause){
+        //    await sleep(5000);
+        //};    
         //create a table in a similar way of ui
         tasks= data.tasks;
         console.log('Received tasks', tasks);
         task_table ='<table class="table table-responsive table-hover table-striped"><thead id="task_head" class="text-center table-'+color_table+'"><tr><th>#</th><th>Name</th><th>Command</th><th><div onclick="">Worker</div></th><th>Batch</th><th>Status</th><th>Start</th><th>Runtime</th><th>Output</th><th>Error</th><th>Actions</th></tr></thead></tr></thead>\n<tbody id="table">\n';
         select_worker ='<div> <label class="form-label" for="filter_by_worker">Worker:</label><select id="filter_by_worker" name="worker" class="form-select col-md-3">\n<option value="" '+(filter.get('worker')!=''?'':'')+'>-</option>\n';
         select_batch ='<div> <label class="form-label" for="filter_by_batch">Batch:</label><select id="filter_by_batch" name="batch" class="form-select" col-md-3>\n<option value="" '+(filter.get('batch')!=''?'':'selected')+'>Default</option>\n';
         sort_by='<label for="sortby" class="form-label">Sort by:</label>'
@@ -137,17 +154,17 @@
         document.getElementById("filter_by_worker").innerHTML=select_worker;
         document.getElementById("filter_by_batch").innerHTML=select_batch;
         document.getElementById("sortby").innerHTML=sort_by;
         // Due to the uptade of the page every 5second, This maintain the output to the bottom.
         for(element of document.getElementsByName('scroll')){
             element.scrollTop=999999;
         }
-        await sleep(5000);
+        //await sleep(5000);
         console.log('detailed_tasks: '+detailed_tasks);
-        get_tasks({order_by: order_by, filter_by: filter.get('show'), detailed_tasks: detailed_tasks});
+        unpause({order_by: order_by, filter_by: filter.get('show'), detailed_tasks: detailed_tasks});
         //    socket.emit('get', {object: 'task', order_by: order_by, filter_by: filter.get('show'), detailed_tasks: detailed_tasks});
         //    });
         //);
     });
 }
 
 function remove_from_array(arr, value){
@@ -292,18 +309,18 @@
 return table;
 }
 
 function displayModal(i,type) {
     console.log(document.getElementById('task-modal-'+tasks[i][6]));
     document.getElementById('task-modal-'+tasks[i][6]).innerHTML='<div class="modal-dialog modal-dialog-centered"><form class="modal-content"><div class="container"><h3>'+type+'</h3>'
                                                     +'<p>Are you sure you want to '+type+' task_'+tasks[i][0]+''+(type==='delete'?' ':' execution_'+tasks[i][6])+' ?</p>'
-                                                    +'<div class="clearfix"><button type="button" class="btn btn-danger" onclick="document.getElementById(\'task-modal-'+tasks[i][6]+'\').style.display=\''+'none'+'\'; pause = false" >Cancel</button>'
-                                                    +'<button type="button" class="btn btn-primary" onclick="action_task(\''+tasks[i][0]+'\',\''+type+'\');document.getElementById(\'task-modal-'+tasks[i][6]+'\').style.display=\''+'none'+'\'; pause = false">Confirm</button></div></div></form>';
+                                                    +'<div class="clearfix"><button type="button" class="btn btn-danger" onclick="document.getElementById(\'task-modal-'+tasks[i][6]+'\').style.display=\''+'none'+'\'; unpause()" >Cancel</button>'
+                                                    +'<button type="button" class="btn btn-primary" onclick="action_task(\''+tasks[i][0]+'\',\''+type+'\');document.getElementById(\'task-modal-'+tasks[i][6]+'\').style.display=\''+'none'+'\'; unpause()">Confirm</button></div></div></form>';
     document.getElementById('task-modal-'+tasks[i][6]).style.display = "block";
-    pause=true;
+    pause();
 }
 
 function download(id_task,i) {
     var element = document.createElement('a');
     // I used this code https://www.delftstack.com/fr/howto/javascript/javascript-download/ with some modifications
     if (tasks[i][7] !== '' && task[i][7] !== null){
         element.setAttribute('href', 'data:text/plain;charset=utf-8,' + encodeURIComponent(tasks[i][7]));
@@ -394,40 +411,35 @@
     }
     console.log('Sending action');
 }
 
 //Open a textarea to modify a command.
 function modify_command(id_execution,i){
     content = document.getElementById("command-content-"+id_execution);
-    if(pause==false){
+    if(pause()){
     content.innerHTML='<form><textarea id="textarea-'+id_execution+'"class="form-control" rows="4">'+tasks[i][9]+'</textarea>';
     content.innerHTML+='<button type="button" onclick="modify_command('+id_execution+','+i+')" class="btn btn-danger" style="--bs-btn-padding-y: .10rem; --bs-btn-padding-x: .3rem; --bs-btn-font-size: .75rem;" >Cancel</button><button type="button" class="btn btn-primary" style="--bs-btn-padding-y: .10rem; --bs-btn-padding-x: .3rem; --bs-btn-font-size: .75rem;" onclick="submit_command('+id_execution+','+i+');modify_command('+id_execution+','+i+')">Submit</button></form>';
-    pause=true;
     }
     else{
-    pause=false;
+    unpause();
     content.innerHTML='<div class="d-flex"><div class="p-2 w-100">'+tasks[i][9]+'</div><div class="p-2 flex-shrink-1"><button type="button" tiltle="modify" onclick="modify_command('+tasks[i][6]+','+i+')" class="btn btn-dark " style="--bs-btn-padding-y: .10rem; --bs-btn-padding-x: .3rem; --bs-btn-font-size: .75rem;">modify</button></div>';
     }
 }
 
 //the function required to be set after the texte area so it can get the value of it
 function submit_command(id_execution,i){
     return action_task(tasks[i][0],'modify',document.getElementById('textarea-'+id_execution).value);
 }
 
 function pause_page(){
-    switch(pause){
-        case true:
-            pause=false;
-            document.getElementById('pause').innerHTML='Pause';
-            break;
-        case false:
-            pause=true;
-            document.getElementById('pause').innerHTML='Resume';
-            break;
+    if (pause()) {
+        document.getElementById('pause').innerHTML='Pause';
+    } {
+        unpause();
+        document.getElementById('pause').innerHTML='Resume';
     }
 }
 
 $(document).ready( get_tasks( {} ) );
 </script>
 </head>
 <body>
```

### Comparing `scitq-1.0rc8/src/scitq/templates/ui.html` & `scitq-1.0rc9/src/scitq/templates/ui.html`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 <script src={{ url_for("static", filename="js/bootstrap.v5.0.2/bootstrap.min.js") }}></script>
 <script src={{ url_for("static", filename="js/FileSaver.v2.0.4/FileSaver.min.js") }}></script>
 <script src={{ url_for("static", filename="js/jszip.min.v3.10.0.js") }}></script>
 <!-- <script src={{ url_for("static", filename="js/socket.io.v4.0.1/socket.io.js") }}></script> -->
 <script type="text/javascript" charset="utf-8">
 // All the class come from the Bootstrap v5 documentation and icon also come from bootstrap
 //const delay = ms => new Promise(res => setTimeout(res, ms));
-function sleep (time) {
-    return new Promise((resolve) => setTimeout(resolve, time));
-    }
+//function sleep (time) {
+//    return new Promise((resolve) => setTimeout(resolve, time));
+//    }
 function worker_concurrency_change(worker_id, change) {
     //socket.emit('concurrency_change', {object: 'worker', id: worker_id, change:change})
     $.ajax({url: '/ui/concurrency_change', data: {object: 'worker', id: worker_id, change:change} });
 }
 function worker_prefetch_change(worker_id, change) {
     //socket.emit('prefetch_change', {object: 'worker', id: worker_id, change:change})
     $.ajax({url: '/ui/prefetch_change', data: {object: 'worker', id: worker_id, change:change} });
@@ -33,25 +33,42 @@
         flavor: flavor, region: region, batch:batch, number: number} });
 }
 /* var socket = io();
 socket.on('connect', function() {
     console.log('connecting');
     socket.emit('get', {object: 'workers'});
 }); */
-pause=false;
+//pause=false;
 //socket.on('workers', async function(data) {
+
+var intervalID = null;
+function pause() { 
+    if (intervalID) {
+        clearInterval(intervalID);
+        intervalID = null;
+    }
+}
+
+function unpause() {
+    if (intervalID) {
+        clearInterval(intervalID);
+    }
+    intervalID = setInterval(get_workers, 5000);
+}
+
+
 function get_workers() {
     console.log('Fetching workers...')
     $.getJSON('/ui/get/', {
                 object: 'workers'
-            }, async function(data) {
+            }, function(data) {
         //some action such as modify an action needs time to be done so the update of the page can be set on true 
-        while(pause){
-            await sleep(5000);
-        }
+        //while(pause){
+        //    await sleep(5000);
+        //}
         workers = data.workers;
         totals = data.totals;
         console.log('Received workers ',workers);
         console.log('Received totals ',totals);
         total_div = "<div class=\"container total-div\" style='margin-top:0.5em'><a target='_blank' href='/ui/task/?sortby=&worker=&batch=&show=pending'>Pending: "+totals.pending
             +"</a><a href='#'>Assigned: "+totals.assigned
             +"</a><a target='_blank' href='/ui/task/?sortby=&worker=&batch=&show=running'>Running: "+totals.running
@@ -75,15 +92,15 @@
                     break;
                 case 'running':
                     var worker_status = 'primary';
                     break;
                 }    
 
             worker_table += '<tr class="" ><td><a type="button" class="btn btn-outline-dark border-0" target="_blank" href="/ui/task/?sortby=&worker='+workers[i].worker_id+'&batch="">'+workers[i].name
-                    +'</a></td><td class="" id="batch-name-'+workers[i].worker_id+'" style="padding:0"><a target="_blank" href="/ui/task/?sortby=&worker=&batch='+(workers[i].batch==null?'':workers[i].batch).replace(' ','+')+'" type="button" class="btn btn-outline-dark border-0">'+(workers[i].batch==null?'':workers[i].batch)+'</a><button type="button" onclick="ChangeBatch(\''+workers[i].worker_id+'\','+i+'); pause=true" class="btn btn-sm" style="margin-top:0.5em;"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-pencil-square" viewBox="0 0 16 16"><path d="M15.502 1.94a.5.5 0 0 1 0 .706L14.459 3.69l-2-2L13.502.646a.5.5 0 0 1 .707 0l1.293 1.293zm-1.75 2.456-2-2L4.939 9.21a.5.5 0 0 0-.121.196l-.805 2.414a.25.25 0 0 0 .316.316l2.414-.805a.5.5 0 0 0 .196-.12l6.813-6.814z"/><path fill-rule="evenodd" d="M1 13.5A1.5 1.5 0 0 0 2.5 15h11a1.5 1.5 0 0 0 1.5-1.5v-6a.5.5 0 0 0-1 0v6a.5.5 0 0 1-.5.5h-11a.5.5 0 0 1-.5-.5v-11a.5.5 0 0 1 .5-.5H9a.5.5 0 0 0 0-1H2.5A1.5 1.5 0 0 0 1 2.5v11z"/></button>'
+                    +'</a></td><td class="" id="batch-name-'+workers[i].worker_id+'" style="padding:0"><a target="_blank" href="/ui/task/?sortby=&worker=&batch='+(workers[i].batch==null?'':workers[i].batch).replace(' ','+')+'" type="button" class="btn btn-outline-dark border-0">'+(workers[i].batch==null?'':workers[i].batch)+'</a><button type="button" onclick="ChangeBatch(\''+workers[i].worker_id+'\','+i+'); pause()" class="btn btn-sm" style="margin-top:0.5em;"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-pencil-square" viewBox="0 0 16 16"><path d="M15.502 1.94a.5.5 0 0 1 0 .706L14.459 3.69l-2-2L13.502.646a.5.5 0 0 1 .707 0l1.293 1.293zm-1.75 2.456-2-2L4.939 9.21a.5.5 0 0 0-.121.196l-.805 2.414a.25.25 0 0 0 .316.316l2.414-.805a.5.5 0 0 0 .196-.12l6.813-6.814z"/><path fill-rule="evenodd" d="M1 13.5A1.5 1.5 0 0 0 2.5 15h11a1.5 1.5 0 0 0 1.5-1.5v-6a.5.5 0 0 0-1 0v6a.5.5 0 0 1-.5.5h-11a.5.5 0 0 1-.5-.5v-11a.5.5 0 0 1 .5-.5H9a.5.5 0 0 0 0-1H2.5A1.5 1.5 0 0 0 1 2.5v11z"/></button>'
                     +'</td><td class="text-center text-'+worker_status+'" title ="'+workers[i].status+'"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"class="bi bi-circle-fill " viewBox="0 0 16 16"><circle cx="8" cy="8" r="8"/></svg>'
                     +'</td><td>'+workers[i].concurrency
                         +'<div class ="btn-group"><button class="btn btn-outline-dark btn-sm" onClick="worker_concurrency_change('
                         +workers[i].worker_id
                         +',1)">+</button><button class="btn btn-outline-dark btn-sm" onClick="worker_concurrency_change('
                         +workers[i].worker_id
                         +',-1)"">-</button></div>'
@@ -104,16 +121,15 @@
                     +'<td><button type="button" title="delete" onclick="DeleteWorker('+workers[i].worker_id+')" class="btn btn-outline-dark btn-sm"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-trash3-fill" viewBox="0 0 16 16"><path d="M11 1.5v1h3.5a.5.5 0 0 1 0 1h-.538l-.853 10.66A2 2 0 0 1 11.115 16h-6.23a2 2 0 0 1-1.994-1.84L2.038 3.5H1.5a.5.5 0 0 1 0-1H5v-1A1.5 1.5 0 0 1 6.5 0h3A1.5 1.5 0 0 1 11 1.5Zm-5 0v1h4v-1a.5.5 0 0 0-.5-.5h-3a.5.5 0 0 0-.5.5ZM4.5 5.029l.5 8.5a.5.5 0 1 0 .998-.06l-.5-8.5a.5.5 0 1 0-.998.06Zm6.53-.528a.5.5 0 0 0-.528.47l-.5 8.5a.5.5 0 0 0 .998.058l.5-8.5a.5.5 0 0 0-.47-.528ZM8 4.5a.5.5 0 0 0-.5.5v8.5a.5.5 0 0 0 1 0V5a.5.5 0 0 0-.5-.5Z"/></svg></button>'
                     +'</td></tr>\n';
         }
 
         worker_table += '</tbody>\n</table>\n';
         document.getElementById("workers").innerHTML = total_div +'<br/>' + worker_table;
         get_jobs();
-        await sleep(5000);
-        get_workers();
+        unpause();
     });
 };
 //socket.on('worker_created', function(data) {
 //    document.getElementById("addworker-result").innerHTML = data;
 //    document.getElementById("awf-button").style.visibility = "visible";
 //});
 //send an order to server to delete in db the worker
@@ -134,29 +150,31 @@
     document.getElementById('batch-name-input-'+id_worker).addEventListener("keypress",function(event){
         if (event.key==='Enter'){
             event.preventDefault();
             //socket.emit('change_batch',{batch_name : document.getElementById('batch-name-input-'+id_worker).value,worker_id:id_worker});
             $.ajax({url: '/ui/change_batch', 
                 data: {batch_name : document.getElementById('batch-name-input-'+id_worker).value,worker_id:id_worker} });
             document.getElementById('batch-name-'+id_worker).innerHTML='<a type="button" class="btn btn-outline-dark border-0">Loading..</a>';
-            pause=false;
+            //pause=false;
+            unpause();
         }
     })
 }
 function HideChangeBatch(id_worker,i){
-    document.getElementById('batch-name-'+id_worker).innerHTML='<a type="button" class="btn btn-outline-dark border-0">'+(workers[i][2]==null?'':workers[i][2])+'</a><button type="button" onclick="ChangeBatch(\''+workers[i][0]+'\','+i+'); pause=true" class="btn btn-outline-dark btn-sm"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-pencil-square" viewBox="0 0 16 16"><path d="M15.502 1.94a.5.5 0 0 1 0 .706L14.459 3.69l-2-2L13.502.646a.5.5 0 0 1 .707 0l1.293 1.293zm-1.75 2.456-2-2L4.939 9.21a.5.5 0 0 0-.121.196l-.805 2.414a.25.25 0 0 0 .316.316l2.414-.805a.5.5 0 0 0 .196-.12l6.813-6.814z"/><path fill-rule="evenodd" d="M1 13.5A1.5 1.5 0 0 0 2.5 15h11a1.5 1.5 0 0 0 1.5-1.5v-6a.5.5 0 0 0-1 0v6a.5.5 0 0 1-.5.5h-11a.5.5 0 0 1-.5-.5v-11a.5.5 0 0 1 .5-.5H9a.5.5 0 0 0 0-1H2.5A1.5 1.5 0 0 0 1 2.5v11z"/></button>';
-    pause=false;
+    document.getElementById('batch-name-'+id_worker).innerHTML='<a type="button" class="btn btn-outline-dark border-0">'+(workers[i][2]==null?'':workers[i][2])+'</a><button type="button" onclick="ChangeBatch(\''+workers[i][0]+'\','+i+'); pause()" class="btn btn-outline-dark btn-sm"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-pencil-square" viewBox="0 0 16 16"><path d="M15.502 1.94a.5.5 0 0 1 0 .706L14.459 3.69l-2-2L13.502.646a.5.5 0 0 1 .707 0l1.293 1.293zm-1.75 2.456-2-2L4.939 9.21a.5.5 0 0 0-.121.196l-.805 2.414a.25.25 0 0 0 .316.316l2.414-.805a.5.5 0 0 0 .196-.12l6.813-6.814z"/><path fill-rule="evenodd" d="M1 13.5A1.5 1.5 0 0 0 2.5 15h11a1.5 1.5 0 0 0 1.5-1.5v-6a.5.5 0 0 0-1 0v6a.5.5 0 0 1-.5.5h-11a.5.5 0 0 1-.5-.5v-11a.5.5 0 0 1 .5-.5H9a.5.5 0 0 0 0-1H2.5A1.5 1.5 0 0 0 1 2.5v11z"/></button>';
+    //pause=false;
+    unpause();
 }
 
 //socket.on('jobs', function(data) {
 function get_jobs() {
-    $.getJSON('/ui/jobs', {}, async function(data) {
-        while(pause){
-            await sleep(5000);
-        }    
+    $.getJSON('/ui/jobs', {}, function(data) {
+        //while(pause){
+        //    await sleep(5000);
+        //}    
         console.log('jobs received', data);
         var action_pretify = {
             worker_create: "Create worker",
             worker_deploy: "Deploy worker",
             worker_destroy: "Destroy worker"
         } ;
         var table='';
```

### Comparing `scitq-1.0rc8/src/scitq/util.py` & `scitq-1.0rc9/src/scitq/util.py`

 * *Files identical despite different names*

### Comparing `scitq-1.0rc8/src/scitq.egg-info/PKG-INFO` & `scitq-1.0rc9/src/scitq.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitq
-Version: 1.0rc8
+Version: 1.0rc9
 Summary: A (distributed) scientific task queue
 Author: Raynald de Lahondès, Rémi Tan
 Project-URL: Homepage, https://github.com/gmtsciencedev/scitq
 Project-URL: Bug Tracker, https://github.com/gmtsciencedev/scitq/issues
 Project-URL: Documentation, https://scitq.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -198,14 +198,14 @@
 you wish, etc. At least that's what we thought, now with heavier loads, PostgreSQL
 is recommended (concurrency has its limits with sqlite), and is now the default.
 - A simple multiprocess worker (if you read multithread, re-read the sentence), 
 with a clever management of output flow. Asyncio was the solution here (process.poll()
 with stdout.readline() is not performant enough if you have heavy output).
 - A nice UI (like Celery Flower) : now this nice UI must update its display very
 often you do not want to reload the page to refresh (Flower is smart enough for 
-that): I did write a very small game in Python with Flask and I had had a go with
-SocketIO with quite a success, so I tried here and it fits the case. I compared
-with basic jQuery and it performed better so scitq uses SocketIO (and a nice
-Flask package: Flask-SocketIO)
+that): initially we had chosen socket.io for the UI however when we decided to deploy
+scitq in a serious way (with a wsgi server and not Flask development server), we were
+not able not configure socket.io in a multi-worker uwsgi setup, so we went back to 
+jQuery which is sufficient in our case.
 
 For now, UI and server live in the same Flask application which makes deploy
 very easy.
```

### Comparing `scitq-1.0rc8/src/scitq.egg-info/SOURCES.txt` & `scitq-1.0rc9/src/scitq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

