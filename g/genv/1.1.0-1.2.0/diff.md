# Comparing `tmp/genv-1.1.0.tar.gz` & `tmp/genv-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genv-1.1.0.tar", last modified: Wed Jun 21 18:07:06 2023, max compression
+gzip compressed data, was "genv-1.2.0.tar", last modified: Tue Jul  4 15:57:16 2023, max compression
```

## Comparing `genv-1.1.0.tar` & `genv-1.2.0.tar`

### file list

```diff
@@ -1,121 +1,126 @@
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.518116 genv-1.1.0/
--rw-r--r--   0 raz       (1001) raz       (1001)    34523 2022-12-27 17:45:39.000000 genv-1.1.0/LICENSE
--rw-r--r--   0 raz       (1001) raz       (1001)     4446 2023-06-21 18:07:06.517116 genv-1.1.0/PKG-INFO
--rw-r--r--   0 raz       (1001) raz       (1001)     3780 2023-06-21 18:04:45.000000 genv-1.1.0/README.md
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.246113 genv-1.1.0/genv/
--rw-r--r--   0 raz       (1001) raz       (1001)      306 2023-06-12 07:39:27.000000 genv-1.1.0/genv/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.253113 genv-1.1.0/genv/cli/
--rw-r--r--   0 raz       (1001) raz       (1001)        0 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5007 2023-06-21 18:04:45.000000 genv-1.1.0/genv/cli/__main__.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     2755 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/activate.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     1358 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/attach.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     2295 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/config.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)      738 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/deactivate.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)      465 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/detach.py
--rw-r--r--   0 raz       (1001) raz       (1001)    10817 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3227 2023-06-21 17:25:32.000000 genv-1.1.0/genv/cli/enforce.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     9382 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/envs.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)      656 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/home.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)      610 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/lock.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     1945 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/monitor.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)    16105 2023-06-21 18:04:45.000000 genv-1.1.0/genv/cli/remote.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5133 2023-06-21 18:04:45.000000 genv-1.1.0/genv/cli/shell.py
--rw-r--r--   0 raz       (1001) raz       (1001)      892 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/status.py
--rwxr-xr-x   0 raz       (1001) raz       (1001)     1986 2023-06-12 07:39:27.000000 genv-1.1.0/genv/cli/usage.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.255113 genv-1.1.0/genv/core/
--rw-r--r--   0 raz       (1001) raz       (1001)      116 2023-06-12 07:39:27.000000 genv-1.1.0/genv/core/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5677 2023-06-12 07:39:27.000000 genv-1.1.0/genv/core/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3703 2023-06-12 07:39:27.000000 genv-1.1.0/genv/core/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      894 2023-06-12 07:39:27.000000 genv-1.1.0/genv/core/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      379 2023-06-12 07:39:27.000000 genv-1.1.0/genv/core/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1424 2023-06-12 07:39:27.000000 genv-1.1.0/genv/core/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.257113 genv-1.1.0/genv/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       49 2023-06-12 07:39:27.000000 genv-1.1.0/genv/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1288 2023-06-12 07:39:27.000000 genv-1.1.0/genv/enforce/execute.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.266113 genv-1.1.0/genv/enforce/rules/
--rw-r--r--   0 raz       (1001) raz       (1001)      176 2023-06-12 07:39:27.000000 genv-1.1.0/genv/enforce/rules/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      864 2023-06-12 07:39:27.000000 genv-1.1.0/genv/enforce/rules/env_devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1394 2023-06-12 07:39:27.000000 genv-1.1.0/genv/enforce/rules/env_memory.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1449 2023-06-21 17:59:41.000000 genv-1.1.0/genv/enforce/rules/max_devices_per_user.py
--rw-r--r--   0 raz       (1001) raz       (1001)      642 2023-06-12 07:39:27.000000 genv-1.1.0/genv/enforce/rules/non_env_processes.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.266113 genv-1.1.0/genv/entities/
--rw-r--r--   0 raz       (1001) raz       (1001)      111 2023-06-12 07:39:27.000000 genv-1.1.0/genv/entities/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.280113 genv-1.1.0/genv/entities/core/
--rw-r--r--   0 raz       (1001) raz       (1001)      138 2023-06-12 07:39:27.000000 genv-1.1.0/genv/entities/core/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     7231 2023-06-12 07:39:27.000000 genv-1.1.0/genv/entities/core/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5875 2023-06-12 07:39:27.000000 genv-1.1.0/genv/entities/core/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3484 2023-06-12 07:39:27.000000 genv-1.1.0/genv/entities/core/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      982 2023-06-12 07:39:27.000000 genv-1.1.0/genv/entities/core/snapshot.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.281113 genv-1.1.0/genv/entities/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       54 2023-06-12 07:39:27.000000 genv-1.1.0/genv/entities/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      270 2023-06-12 07:39:27.000000 genv-1.1.0/genv/entities/enforce/report.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1126 2023-06-12 07:39:27.000000 genv-1.1.0/genv/entities/enforce/survey.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.284113 genv-1.1.0/genv/metrics/
--rw-r--r--   0 raz       (1001) raz       (1001)      184 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3074 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/collection.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.243113 genv-1.1.0/genv/metrics/export/
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.285113 genv-1.1.0/genv/metrics/export/grafana/
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.285113 genv-1.1.0/genv/metrics/export/grafana/dashboards/
--rw-r--r--   0 raz       (1001) raz       (1001)     9965 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/export/grafana/dashboards/overview.json
--rw-r--r--   0 raz       (1001) raz       (1001)      182 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/export/grafana/grafana.ini
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.243113 genv-1.1.0/genv/metrics/export/grafana/provisioning/
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.289113 genv-1.1.0/genv/metrics/export/grafana/provisioning/dashboards/
--rw-r--r--   0 raz       (1001) raz       (1001)      114 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/export/grafana/provisioning/dashboards/default.yml
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.290113 genv-1.1.0/genv/metrics/export/grafana/provisioning/datasources/
--rw-r--r--   0 raz       (1001) raz       (1001)      134 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/export/grafana/provisioning/datasources/default.yml
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.290113 genv-1.1.0/genv/metrics/export/prometheus/
--rw-r--r--   0 raz       (1001) raz       (1001)      155 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/export/prometheus/prometheus.yml
--rw-r--r--   0 raz       (1001) raz       (1001)     1786 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/metric.py
--rw-r--r--   0 raz       (1001) raz       (1001)     2663 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/publisher.py
--rw-r--r--   0 raz       (1001) raz       (1001)      431 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/spec.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3593 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/specs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      157 2023-06-12 07:39:27.000000 genv-1.1.0/genv/metrics/type.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.291113 genv-1.1.0/genv/remote/
--rw-r--r--   0 raz       (1001) raz       (1001)       87 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/__init__.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.302114 genv-1.1.0/genv/remote/core/
--rw-r--r--   0 raz       (1001) raz       (1001)       96 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/core/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      381 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/core/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)      377 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/core/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      387 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/core/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      834 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/core/snapshot.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.418115 genv-1.1.0/genv/remote/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       29 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      637 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/enforce/execute.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.507116 genv-1.1.0/genv/remote/metrics/
--rw-r--r--   0 raz       (1001) raz       (1001)       35 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/metrics/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1683 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/metrics/collection.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.508116 genv-1.1.0/genv/remote/utils/
--rw-r--r--   0 raz       (1001) raz       (1001)       40 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/utils/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3110 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/utils/ssh.py
--rw-r--r--   0 raz       (1001) raz       (1001)      515 2023-06-12 07:39:27.000000 genv-1.1.0/genv/remote/utils/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.513116 genv-1.1.0/genv/sdk/
--rw-r--r--   0 raz       (1001) raz       (1001)      272 2023-06-12 07:39:27.000000 genv-1.1.0/genv/sdk/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4132 2023-06-21 18:04:45.000000 genv-1.1.0/genv/sdk/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4280 2023-06-21 18:04:45.000000 genv-1.1.0/genv/sdk/env.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1300 2023-06-21 18:04:45.000000 genv-1.1.0/genv/sdk/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.513116 genv-1.1.0/genv/serialization/
--rw-r--r--   0 raz       (1001) raz       (1001)       44 2023-06-12 07:39:27.000000 genv-1.1.0/genv/serialization/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1803 2023-06-12 07:39:27.000000 genv-1.1.0/genv/serialization/json_.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.514116 genv-1.1.0/genv/shims/
--rwxr-xr-x   0 raz       (1001) raz       (1001)     2750 2023-06-10 15:50:03.000000 genv-1.1.0/genv/shims/docker
--rwxr-xr-x   0 raz       (1001) raz       (1001)     7030 2023-05-07 09:36:08.000000 genv-1.1.0/genv/shims/nvidia-smi
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.515116 genv-1.1.0/genv/utils/
--rw-r--r--   0 raz       (1001) raz       (1001)      107 2023-06-12 07:39:27.000000 genv-1.1.0/genv/utils/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1393 2023-06-12 07:39:27.000000 genv-1.1.0/genv/utils/nvidia_smi.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3144 2023-06-21 18:04:45.000000 genv-1.1.0/genv/utils/os_.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1253 2023-06-12 07:39:27.000000 genv-1.1.0/genv/utils/poll.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.516116 genv-1.1.0/genv/utils/runners/
--rw-r--r--   0 raz       (1001) raz       (1001)       93 2023-06-12 07:39:27.000000 genv-1.1.0/genv/utils/runners/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      688 2023-06-12 07:39:27.000000 genv-1.1.0/genv/utils/runners/local.py
--rw-r--r--   0 raz       (1001) raz       (1001)     2046 2023-06-12 07:39:27.000000 genv-1.1.0/genv/utils/runners/runner.py
--rw-r--r--   0 raz       (1001) raz       (1001)     2113 2023-06-12 07:39:27.000000 genv-1.1.0/genv/utils/runners/ssh.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3446 2023-06-12 07:39:27.000000 genv-1.1.0/genv/utils/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-21 18:07:06.248113 genv-1.1.0/genv.egg-info/
--rw-r--r--   0 raz       (1001) raz       (1001)     4446 2023-06-21 18:07:03.000000 genv-1.1.0/genv.egg-info/PKG-INFO
--rw-r--r--   0 raz       (1001) raz       (1001)     2373 2023-06-21 18:07:05.000000 genv-1.1.0/genv.egg-info/SOURCES.txt
--rw-r--r--   0 raz       (1001) raz       (1001)        1 2023-06-21 18:07:03.000000 genv-1.1.0/genv.egg-info/dependency_links.txt
--rw-r--r--   0 raz       (1001) raz       (1001)       48 2023-06-21 18:07:04.000000 genv-1.1.0/genv.egg-info/entry_points.txt
--rw-r--r--   0 raz       (1001) raz       (1001)       29 2023-06-21 18:07:04.000000 genv-1.1.0/genv.egg-info/requires.txt
--rw-r--r--   0 raz       (1001) raz       (1001)        5 2023-06-21 18:07:04.000000 genv-1.1.0/genv.egg-info/top_level.txt
--rw-r--r--   0 raz       (1001) raz       (1001)       38 2023-06-21 18:07:06.518116 genv-1.1.0/setup.cfg
--rw-r--r--   0 raz       (1001) raz       (1001)     1079 2023-06-21 18:06:25.000000 genv-1.1.0/setup.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.112110 genv-1.2.0/
+-rw-r--r--   0 raz       (1001) raz       (1001)    34523 2022-12-27 17:45:39.000000 genv-1.2.0/LICENSE
+-rw-r--r--   0 raz       (1001) raz       (1001)     4742 2023-07-04 15:57:16.112110 genv-1.2.0/PKG-INFO
+-rw-r--r--   0 raz       (1001) raz       (1001)     4036 2023-07-04 15:54:23.000000 genv-1.2.0/README.md
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.104110 genv-1.2.0/genv/
+-rw-r--r--   0 raz       (1001) raz       (1001)      306 2023-06-12 07:39:27.000000 genv-1.2.0/genv/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.105110 genv-1.2.0/genv/_ray/
+-rw-r--r--   0 raz       (1001) raz       (1001)       27 2023-07-04 15:54:42.000000 genv-1.2.0/genv/_ray/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1737 2023-07-04 15:54:42.000000 genv-1.2.0/genv/_ray/remote.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.106110 genv-1.2.0/genv/cli/
+-rw-r--r--   0 raz       (1001) raz       (1001)        0 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5007 2023-07-04 15:54:23.000000 genv-1.2.0/genv/cli/__main__.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     2755 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/activate.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     1358 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/attach.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     2295 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/config.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)      738 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/deactivate.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)      465 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/detach.py
+-rw-r--r--   0 raz       (1001) raz       (1001)    10817 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3227 2023-06-21 17:25:32.000000 genv-1.2.0/genv/cli/enforce.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     9382 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/envs.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)      656 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/home.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)      610 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/lock.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     1945 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/monitor.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)    16105 2023-07-04 15:54:23.000000 genv-1.2.0/genv/cli/remote.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5133 2023-07-04 15:54:23.000000 genv-1.2.0/genv/cli/shell.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      892 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/status.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     1986 2023-06-12 07:39:27.000000 genv-1.2.0/genv/cli/usage.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.107110 genv-1.2.0/genv/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)      116 2023-06-12 07:39:27.000000 genv-1.2.0/genv/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5677 2023-06-12 07:39:27.000000 genv-1.2.0/genv/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3703 2023-06-12 07:39:27.000000 genv-1.2.0/genv/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      894 2023-06-12 07:39:27.000000 genv-1.2.0/genv/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      379 2023-06-12 07:39:27.000000 genv-1.2.0/genv/core/snapshot.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1424 2023-06-12 07:39:27.000000 genv-1.2.0/genv/core/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.107110 genv-1.2.0/genv/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       49 2023-06-12 07:39:27.000000 genv-1.2.0/genv/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1288 2023-06-12 07:39:27.000000 genv-1.2.0/genv/enforce/execute.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.107110 genv-1.2.0/genv/enforce/rules/
+-rw-r--r--   0 raz       (1001) raz       (1001)      176 2023-06-12 07:39:27.000000 genv-1.2.0/genv/enforce/rules/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      864 2023-06-12 07:39:27.000000 genv-1.2.0/genv/enforce/rules/env_devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1394 2023-06-12 07:39:27.000000 genv-1.2.0/genv/enforce/rules/env_memory.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1449 2023-06-21 17:59:41.000000 genv-1.2.0/genv/enforce/rules/max_devices_per_user.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      642 2023-06-12 07:39:27.000000 genv-1.2.0/genv/enforce/rules/non_env_processes.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.107110 genv-1.2.0/genv/entities/
+-rw-r--r--   0 raz       (1001) raz       (1001)      111 2023-06-12 07:39:27.000000 genv-1.2.0/genv/entities/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.108110 genv-1.2.0/genv/entities/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)      138 2023-06-12 07:39:27.000000 genv-1.2.0/genv/entities/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     7231 2023-06-12 07:39:27.000000 genv-1.2.0/genv/entities/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5875 2023-06-12 07:39:27.000000 genv-1.2.0/genv/entities/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3484 2023-06-12 07:39:27.000000 genv-1.2.0/genv/entities/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      982 2023-06-12 07:39:27.000000 genv-1.2.0/genv/entities/core/snapshot.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.108110 genv-1.2.0/genv/entities/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       54 2023-06-12 07:39:27.000000 genv-1.2.0/genv/entities/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      270 2023-06-12 07:39:27.000000 genv-1.2.0/genv/entities/enforce/report.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1126 2023-06-12 07:39:27.000000 genv-1.2.0/genv/entities/enforce/survey.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.109110 genv-1.2.0/genv/metrics/
+-rw-r--r--   0 raz       (1001) raz       (1001)      184 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3074 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/collection.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.103110 genv-1.2.0/genv/metrics/export/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.109110 genv-1.2.0/genv/metrics/export/grafana/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.109110 genv-1.2.0/genv/metrics/export/grafana/dashboards/
+-rw-r--r--   0 raz       (1001) raz       (1001)     9965 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/export/grafana/dashboards/overview.json
+-rw-r--r--   0 raz       (1001) raz       (1001)      182 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/export/grafana/grafana.ini
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.103110 genv-1.2.0/genv/metrics/export/grafana/provisioning/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.109110 genv-1.2.0/genv/metrics/export/grafana/provisioning/dashboards/
+-rw-r--r--   0 raz       (1001) raz       (1001)      114 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/export/grafana/provisioning/dashboards/default.yml
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.109110 genv-1.2.0/genv/metrics/export/grafana/provisioning/datasources/
+-rw-r--r--   0 raz       (1001) raz       (1001)      134 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/export/grafana/provisioning/datasources/default.yml
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.109110 genv-1.2.0/genv/metrics/export/prometheus/
+-rw-r--r--   0 raz       (1001) raz       (1001)      155 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/export/prometheus/prometheus.yml
+-rw-r--r--   0 raz       (1001) raz       (1001)     1786 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/metric.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2663 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/publisher.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      431 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/spec.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3593 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/specs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      157 2023-06-12 07:39:27.000000 genv-1.2.0/genv/metrics/type.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.109110 genv-1.2.0/genv/ray/
+-rw-r--r--   0 raz       (1001) raz       (1001)       21 2023-07-04 15:54:42.000000 genv-1.2.0/genv/ray/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.109110 genv-1.2.0/genv/remote/
+-rw-r--r--   0 raz       (1001) raz       (1001)       87 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.110110 genv-1.2.0/genv/remote/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)       96 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      381 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      377 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      387 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      834 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/core/snapshot.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.110110 genv-1.2.0/genv/remote/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       29 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      637 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/enforce/execute.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.110110 genv-1.2.0/genv/remote/metrics/
+-rw-r--r--   0 raz       (1001) raz       (1001)       35 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/metrics/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1683 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/metrics/collection.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.110110 genv-1.2.0/genv/remote/utils/
+-rw-r--r--   0 raz       (1001) raz       (1001)       40 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/utils/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3110 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/utils/ssh.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      515 2023-06-12 07:39:27.000000 genv-1.2.0/genv/remote/utils/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.110110 genv-1.2.0/genv/sdk/
+-rw-r--r--   0 raz       (1001) raz       (1001)      272 2023-06-12 07:39:27.000000 genv-1.2.0/genv/sdk/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4132 2023-07-04 15:54:23.000000 genv-1.2.0/genv/sdk/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4280 2023-07-04 15:54:23.000000 genv-1.2.0/genv/sdk/env.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1300 2023-07-04 15:54:23.000000 genv-1.2.0/genv/sdk/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.111110 genv-1.2.0/genv/serialization/
+-rw-r--r--   0 raz       (1001) raz       (1001)       44 2023-06-12 07:39:27.000000 genv-1.2.0/genv/serialization/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1803 2023-06-12 07:39:27.000000 genv-1.2.0/genv/serialization/json_.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.111110 genv-1.2.0/genv/shims/
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     2750 2023-06-10 15:50:03.000000 genv-1.2.0/genv/shims/docker
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     7030 2023-05-07 09:36:08.000000 genv-1.2.0/genv/shims/nvidia-smi
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.111110 genv-1.2.0/genv/utils/
+-rw-r--r--   0 raz       (1001) raz       (1001)      107 2023-06-12 07:39:27.000000 genv-1.2.0/genv/utils/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1393 2023-06-12 07:39:27.000000 genv-1.2.0/genv/utils/nvidia_smi.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3144 2023-07-04 15:54:23.000000 genv-1.2.0/genv/utils/os_.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1253 2023-06-12 07:39:27.000000 genv-1.2.0/genv/utils/poll.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.112110 genv-1.2.0/genv/utils/runners/
+-rw-r--r--   0 raz       (1001) raz       (1001)       93 2023-06-12 07:39:27.000000 genv-1.2.0/genv/utils/runners/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      688 2023-06-12 07:39:27.000000 genv-1.2.0/genv/utils/runners/local.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2046 2023-06-12 07:39:27.000000 genv-1.2.0/genv/utils/runners/runner.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2113 2023-06-12 07:39:27.000000 genv-1.2.0/genv/utils/runners/ssh.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3446 2023-06-12 07:39:27.000000 genv-1.2.0/genv/utils/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-07-04 15:57:16.105110 genv-1.2.0/genv.egg-info/
+-rw-r--r--   0 raz       (1001) raz       (1001)     4742 2023-07-04 15:57:15.000000 genv-1.2.0/genv.egg-info/PKG-INFO
+-rw-r--r--   0 raz       (1001) raz       (1001)     2436 2023-07-04 15:57:16.000000 genv-1.2.0/genv.egg-info/SOURCES.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)        1 2023-07-04 15:57:15.000000 genv-1.2.0/genv.egg-info/dependency_links.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)       48 2023-07-04 15:57:15.000000 genv-1.2.0/genv.egg-info/entry_points.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)       60 2023-07-04 15:57:15.000000 genv-1.2.0/genv.egg-info/requires.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)        5 2023-07-04 15:57:16.000000 genv-1.2.0/genv.egg-info/top_level.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)       38 2023-07-04 15:57:16.112110 genv-1.2.0/setup.cfg
+-rw-r--r--   0 raz       (1001) raz       (1001)     1154 2023-07-04 15:55:49.000000 genv-1.2.0/setup.py
```

### Comparing `genv-1.1.0/LICENSE` & `genv-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/PKG-INFO` & `genv-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: genv
-Version: 1.1.0
+Version: 1.2.0
 Summary: GPU environment and cluster management
 Home-page: https://github.com/run-ai/genv
 Author: Run.ai
 Author-email: pypi@run.ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Terminals
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: monitor
+Provides-Extra: ray
 License-File: LICENSE
 
 <p align="center">
   <img src="images/genv blade landscape black@4x.png#gh-light-mode-only" width="600" alt="genv"/>
   <img src="images/genv blade landscape white@4x.png#gh-dark-mode-only" width="600" alt="genv"/>
 </p>
 
 # Genv - GPU Environment and Cluster Management
+[![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT)
 [![Docs](https://img.shields.io/badge/docs-genv-blue)](https://docs.genv.dev/)
 [![PyPI](https://img.shields.io/pypi/v/genv)](https://pypi.org/project/genv/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/genv?style=plastic)](https://pypi.org/project/genv/)
-[![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/genv?label=pypi%20downloads)](https://pypi.org/project/genv/)
+[![Conda](https://img.shields.io/conda/v/conda-forge/genv?label=conda)](https://anaconda.org/conda-forge/genv)
+[![Conda - Downloads](https://img.shields.io/conda/dn/conda-forge/genv?label=conda%20downloads)](https://anaconda.org/conda-forge/genv)
 
 Genv is an open-source environment and cluster management system for GPUs.
 
 Genv lets you easily control, configure, monitor and enforce the GPU resources that you are using in a GPU machine or cluster.
 
 It is intendend to ease up the process of GPU allocation for data scientists without code changes 💪🏻
```

### Comparing `genv-1.1.0/README.md` & `genv-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 <p align="center">
   <img src="images/genv blade landscape black@4x.png#gh-light-mode-only" width="600" alt="genv"/>
   <img src="images/genv blade landscape white@4x.png#gh-dark-mode-only" width="600" alt="genv"/>
 </p>
 
 # Genv - GPU Environment and Cluster Management
+[![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT)
 [![Docs](https://img.shields.io/badge/docs-genv-blue)](https://docs.genv.dev/)
 [![PyPI](https://img.shields.io/pypi/v/genv)](https://pypi.org/project/genv/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/genv?style=plastic)](https://pypi.org/project/genv/)
-[![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/genv?label=pypi%20downloads)](https://pypi.org/project/genv/)
+[![Conda](https://img.shields.io/conda/v/conda-forge/genv?label=conda)](https://anaconda.org/conda-forge/genv)
+[![Conda - Downloads](https://img.shields.io/conda/dn/conda-forge/genv?label=conda%20downloads)](https://anaconda.org/conda-forge/genv)
 
 Genv is an open-source environment and cluster management system for GPUs.
 
 Genv lets you easily control, configure, monitor and enforce the GPU resources that you are using in a GPU machine or cluster.
 
 It is intendend to ease up the process of GPU allocation for data scientists without code changes 💪🏻
```

### Comparing `genv-1.1.0/genv/cli/__main__.py` & `genv-1.2.0/genv/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/activate.py` & `genv-1.2.0/genv/cli/activate.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/attach.py` & `genv-1.2.0/genv/cli/attach.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/config.py` & `genv-1.2.0/genv/cli/config.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/deactivate.py` & `genv-1.2.0/genv/cli/deactivate.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/devices.py` & `genv-1.2.0/genv/cli/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/enforce.py` & `genv-1.2.0/genv/cli/enforce.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/envs.py` & `genv-1.2.0/genv/cli/envs.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/home.py` & `genv-1.2.0/genv/cli/home.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/lock.py` & `genv-1.2.0/genv/cli/lock.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/monitor.py` & `genv-1.2.0/genv/cli/monitor.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/remote.py` & `genv-1.2.0/genv/cli/remote.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/shell.py` & `genv-1.2.0/genv/cli/shell.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/status.py` & `genv-1.2.0/genv/cli/status.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/cli/usage.py` & `genv-1.2.0/genv/cli/usage.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/core/devices.py` & `genv-1.2.0/genv/core/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/core/envs.py` & `genv-1.2.0/genv/core/envs.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/core/processes.py` & `genv-1.2.0/genv/core/processes.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/core/utils.py` & `genv-1.2.0/genv/core/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/enforce/execute.py` & `genv-1.2.0/genv/enforce/execute.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/enforce/rules/env_devices.py` & `genv-1.2.0/genv/enforce/rules/env_devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/enforce/rules/env_memory.py` & `genv-1.2.0/genv/enforce/rules/env_memory.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/enforce/rules/max_devices_per_user.py` & `genv-1.2.0/genv/enforce/rules/max_devices_per_user.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/enforce/rules/non_env_processes.py` & `genv-1.2.0/genv/enforce/rules/non_env_processes.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/entities/core/devices.py` & `genv-1.2.0/genv/entities/core/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/entities/core/envs.py` & `genv-1.2.0/genv/entities/core/envs.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/entities/core/processes.py` & `genv-1.2.0/genv/entities/core/processes.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/entities/core/snapshot.py` & `genv-1.2.0/genv/entities/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/entities/enforce/survey.py` & `genv-1.2.0/genv/entities/enforce/survey.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/metrics/collection.py` & `genv-1.2.0/genv/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/metrics/export/grafana/dashboards/overview.json` & `genv-1.2.0/genv/metrics/export/grafana/dashboards/overview.json`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/metrics/metric.py` & `genv-1.2.0/genv/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/metrics/publisher.py` & `genv-1.2.0/genv/metrics/publisher.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/metrics/specs.py` & `genv-1.2.0/genv/metrics/specs.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/remote/core/snapshot.py` & `genv-1.2.0/genv/remote/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/remote/enforce/execute.py` & `genv-1.2.0/genv/remote/enforce/execute.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/remote/metrics/collection.py` & `genv-1.2.0/genv/remote/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/remote/utils/ssh.py` & `genv-1.2.0/genv/remote/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/remote/utils/utils.py` & `genv-1.2.0/genv/remote/utils/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/sdk/devices.py` & `genv-1.2.0/genv/sdk/devices.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/sdk/env.py` & `genv-1.2.0/genv/sdk/env.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/sdk/utils.py` & `genv-1.2.0/genv/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/serialization/json_.py` & `genv-1.2.0/genv/serialization/json_.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/shims/docker` & `genv-1.2.0/genv/shims/docker`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/shims/nvidia-smi` & `genv-1.2.0/genv/shims/nvidia-smi`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/utils/nvidia_smi.py` & `genv-1.2.0/genv/utils/nvidia_smi.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/utils/os_.py` & `genv-1.2.0/genv/utils/os_.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/utils/poll.py` & `genv-1.2.0/genv/utils/poll.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/utils/runners/local.py` & `genv-1.2.0/genv/utils/runners/local.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/utils/runners/runner.py` & `genv-1.2.0/genv/utils/runners/runner.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/utils/runners/ssh.py` & `genv-1.2.0/genv/utils/runners/ssh.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv/utils/utils.py` & `genv-1.2.0/genv/utils/utils.py`

 * *Files identical despite different names*

### Comparing `genv-1.1.0/genv.egg-info/PKG-INFO` & `genv-1.2.0/genv.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: genv
-Version: 1.1.0
+Version: 1.2.0
 Summary: GPU environment and cluster management
 Home-page: https://github.com/run-ai/genv
 Author: Run.ai
 Author-email: pypi@run.ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Terminals
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: monitor
+Provides-Extra: ray
 License-File: LICENSE
 
 <p align="center">
   <img src="images/genv blade landscape black@4x.png#gh-light-mode-only" width="600" alt="genv"/>
   <img src="images/genv blade landscape white@4x.png#gh-dark-mode-only" width="600" alt="genv"/>
 </p>
 
 # Genv - GPU Environment and Cluster Management
+[![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT)
 [![Docs](https://img.shields.io/badge/docs-genv-blue)](https://docs.genv.dev/)
 [![PyPI](https://img.shields.io/pypi/v/genv)](https://pypi.org/project/genv/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/genv?style=plastic)](https://pypi.org/project/genv/)
-[![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/genv?label=pypi%20downloads)](https://pypi.org/project/genv/)
+[![Conda](https://img.shields.io/conda/v/conda-forge/genv?label=conda)](https://anaconda.org/conda-forge/genv)
+[![Conda - Downloads](https://img.shields.io/conda/dn/conda-forge/genv?label=conda%20downloads)](https://anaconda.org/conda-forge/genv)
 
 Genv is an open-source environment and cluster management system for GPUs.
 
 Genv lets you easily control, configure, monitor and enforce the GPU resources that you are using in a GPU machine or cluster.
 
 It is intendend to ease up the process of GPU allocation for data scientists without code changes 💪🏻
```

### Comparing `genv-1.1.0/genv.egg-info/SOURCES.txt` & `genv-1.2.0/genv.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 genv/__init__.py
 genv.egg-info/PKG-INFO
 genv.egg-info/SOURCES.txt
 genv.egg-info/dependency_links.txt
 genv.egg-info/entry_points.txt
 genv.egg-info/requires.txt
 genv.egg-info/top_level.txt
+genv/_ray/__init__.py
+genv/_ray/remote.py
 genv/cli/__init__.py
 genv/cli/__main__.py
 genv/cli/activate.py
 genv/cli/attach.py
 genv/cli/config.py
 genv/cli/deactivate.py
 genv/cli/detach.py
@@ -55,14 +57,15 @@
 genv/metrics/specs.py
 genv/metrics/type.py
 genv/metrics/export/grafana/grafana.ini
 genv/metrics/export/grafana/dashboards/overview.json
 genv/metrics/export/grafana/provisioning/dashboards/default.yml
 genv/metrics/export/grafana/provisioning/datasources/default.yml
 genv/metrics/export/prometheus/prometheus.yml
+genv/ray/__init__.py
 genv/remote/__init__.py
 genv/remote/core/__init__.py
 genv/remote/core/devices.py
 genv/remote/core/envs.py
 genv/remote/core/processes.py
 genv/remote/core/snapshot.py
 genv/remote/enforce/__init__.py
```

### Comparing `genv-1.1.0/setup.py` & `genv-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="genv",
-    version="1.1.0",
+    version="1.2.0",
     author="Run.ai",
     author_email="pypi@run.ai",
     description="GPU environment and cluster management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/run-ai/genv",
     packages=setuptools.find_packages(),
@@ -26,9 +26,13 @@
     ],
     entry_points={
         "console_scripts": [
             "genv = genv.cli.__main__:main",
         ]
     },
     python_requires=">=3.7",
-    extras_require={"monitor": ["prometheus_client"]},
+    extras_require={
+        "dev": ["black"],
+        "monitor": ["prometheus_client"],
+        "ray": ["ray", "pynvml"],
+    },
 )
```

