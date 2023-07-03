# Comparing `tmp/parsl-2023.6.5.tar.gz` & `tmp/parsl-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2023.6.5.tar", last modified: Mon Jun  5 22:43:11 2023, max compression
+gzip compressed data, was "parsl-2023.7.3.tar", last modified: Mon Jul  3 22:43:00 2023, max compression
```

## Comparing `parsl-2023.6.5.tar` & `parsl-2023.7.3.tar`

### file list

```diff
@@ -1,472 +1,473 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.190580 parsl-2023.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 22:43:01.000000 parsl-2023.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 22:43:01.000000 parsl-2023.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 22:43:11.190580 parsl-2023.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-05 22:43:01.000000 parsl-2023.6.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.122580 parsl-2023.6.5/parsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.130580 parsl-2023.6.5/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/cooley.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/cori.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/exex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.130580 parsl-2023.6.5/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62269 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/executor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/job_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/executors/extreme_scale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/extreme_scale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/extreme_scale/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18710 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/extreme_scale/mpi_worker_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.138580 parsl-2023.6.5/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    33191 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33011 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/status_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/swift_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.138580 parsl-2023.6.5/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    48137 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.138580 parsl-2023.6.5/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29073 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.154580 parsl-2023.6.5/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.158580 parsl-2023.6.5/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/cori.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/exex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/workqueue_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.158580 parsl-2023.6.5/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.158580 parsl-2023.6.5/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_regression_220.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_start_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_task_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_file_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_output_chain_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_memoization_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_viz_colouring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.174580 parsl-2023.6.5/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_providers/test_local_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.178580 parsl-2023.6.5/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_at_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_type5.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_worker_fail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.182580 parsl-2023.6.5/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_69b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_97_parallelism_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.182580 parsl-2023.6.5/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_scaling/test_regression_1621.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_scaling/test_scale_down.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.186580 parsl-2023.6.5/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_https_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.186580 parsl-2023.6.5/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_threads/test_lazy_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.190580 parsl-2023.6.5/parsl/tests/workqueue_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3835 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.190580 parsl-2023.6.5/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-05 22:43:09.000000 parsl-2023.6.5/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.122580 parsl-2023.6.5/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-05 22:43:01.000000 parsl-2023.6.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 22:43:11.190580 parsl-2023.6.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-06-05 22:43:01.000000 parsl-2023.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.767384 parsl-2023.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:42:55.000000 parsl-2023.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-03 22:42:55.000000 parsl-2023.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 22:43:00.767384 parsl-2023.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-03 22:42:55.000000 parsl-2023.7.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.703384 parsl-2023.7.3/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/cooley.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.703384 parsl-2023.7.3/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.707383 parsl-2023.7.3/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62269 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/job_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.707383 parsl-2023.7.3/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.707383 parsl-2023.7.3/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.711384 parsl-2023.7.3/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33191 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33011 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/status_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.711384 parsl-2023.7.3/parsl/executors/taskvine/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48948 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.711384 parsl-2023.7.3/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48130 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28980 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.731384 parsl-2023.7.3/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.735384 parsl-2023.7.3/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/taskvine_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.735384 parsl-2023.7.3/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.735384 parsl-2023.7.3/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.739384 parsl-2023.7.3/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.739384 parsl-2023.7.3/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_regression_220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/scaling_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3751 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/vineex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_start_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.747384 parsl-2023.7.3/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.747384 parsl-2023.7.3/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.747384 parsl-2023.7.3/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_task_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.751384 parsl-2023.7.3/parsl/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_file_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_output_chain_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.751384 parsl-2023.7.3/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_memoization_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_viz_colouring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_providers/test_local_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.759384 parsl-2023.7.3/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_type5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_69b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_97_parallelism_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_scaling/test_regression_1621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_scaling/test_scale_down.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_serialization/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_https_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_threads/test_lazy_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.767384 parsl-2023.7.3/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-03 22:42:59.000000 parsl-2023.7.3/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-03 22:42:55.000000 parsl-2023.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:43:00.767384 parsl-2023.7.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2626 2023-07-03 22:42:55.000000 parsl-2023.7.3/setup.py
```

### Comparing `parsl-2023.6.5/LICENSE` & `parsl-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/PKG-INFO` & `parsl-2023.7.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.6.5
+Version: 2023.7.3
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.06.05.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.07.03.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7.0
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8.0
 Provides-Extra: monitoring
 Provides-Extra: aws
 Provides-Extra: kubernetes
 Provides-Extra: oauth_ssh
 Provides-Extra: docs
 Provides-Extra: google_cloud
 Provides-Extra: gssapi
```

### Comparing `parsl-2023.6.5/README.rst` & `parsl-2023.7.3/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -59,18 +59,14 @@
 .. |NSF-1550528| image:: https://img.shields.io/badge/NSF-1550528-blue.svg
    :target: https://nsf.gov/awardsearch/showAward?AWD_ID=1550528
    :alt: NSF award info
    
 Quickstart
 ==========
 
-Parsl is now available on PyPI, but first make sure you have Python3.7+ ::
-
-    $ python3 --version
-
 Install Parsl using pip::
 
     $ pip3 install parsl
 
 To run the Parsl tutorial notebooks you will need to install Jupyter::
 
     $ pip3 install jupyter
@@ -110,15 +106,15 @@
     $ python3 setup.py install
 
 4. Use Parsl!
 
 Requirements
 ============
 
-Parsl is supported in Python 3.7+. Requirements can be found `here <requirements.txt>`_. Requirements for running tests can be found `here <test-requirements.txt>`_.
+Parsl is supported in Python 3.8+. Requirements can be found `here <requirements.txt>`_. Requirements for running tests can be found `here <test-requirements.txt>`_.
 
 Code of Conduct
 ===============
 
 Parsl seeks to foster an open and welcoming environment - Please see the `Parsl Code of Conduct <https://github.com/Parsl/parsl/blob/master/CoC.md>`_ for more details.
 
 Contributing
```

### Comparing `parsl-2023.6.5/parsl/__init__.py` & `parsl-2023.7.3/parsl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 from parsl.log_utils import set_file_logger
 from parsl.monitoring import MonitoringHub
 
 from parsl.data_provider.files import File
 
 from parsl.dataflow.dflow import DataFlowKernel, DataFlowKernelLoader
 
-import multiprocessing
+import multiprocessing as _multiprocessing
 if platform.system() == 'Darwin':
-    multiprocessing.set_start_method('fork', force=True)
+    _multiprocessing.set_start_method('fork', force=True)
 
 __author__ = 'The Parsl Team'
 __version__ = VERSION
 
 AUTO_LOGNAME = -1
 
 __all__ = [
```

### Comparing `parsl-2023.6.5/parsl/addresses.py` & `parsl-2023.7.3/parsl/addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,16 @@
     for interface in net_interfaces:
         try:
             s_addresses.add(address_by_interface(interface))
         except Exception:
             logger.exception("Ignoring failure to fetch address from interface {}".format(interface))
             pass
 
-    resolution_functions = [address_by_hostname, address_by_route, address_by_query]  # type: List[Callable[[], str]]
+    resolution_functions: List[Callable[[], str]]
+    resolution_functions = [address_by_hostname, address_by_route, address_by_query]
     for f in resolution_functions:
         try:
             s_addresses.add(f())
         except Exception:
             logger.exception("Ignoring an address finder exception")
 
     return s_addresses
```

### Comparing `parsl-2023.6.5/parsl/app/app.py` & `parsl-2023.7.3/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/app/bash.py` & `parsl-2023.7.3/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/app/errors.py` & `parsl-2023.7.3/parsl/app/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/app/futures.py` & `parsl-2023.7.3/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/app/python.py` & `parsl-2023.7.3/parsl/app/python.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 import logging
+import threading
 
 import tblib.pickling_support
 tblib.pickling_support.install()
 
 from functools import wraps
 
 from parsl.app.app import AppBase
 from parsl.app.errors import wrap_error
 from parsl.dataflow.dflow import DataFlowKernelLoader
+from parsl.utils import AutoCancelTimer
 
 
 logger = logging.getLogger(__name__)
 
 
-def timeout(f, seconds):
+def timeout(f, seconds: float):
     @wraps(f)
     def wrapper(*args, **kwargs):
-        import threading
         import ctypes
         import parsl.app.errors
 
         def inject_exception(thread):
             ctypes.pythonapi.PyThreadState_SetAsyncExc(
                 ctypes.c_long(thread),
                 ctypes.py_object(parsl.app.errors.AppTimeout)
             )
 
         thread = threading.current_thread().ident
-        timer = threading.Timer(seconds, inject_exception, args=[thread])
-        timer.start()
-        result = f(*args, **kwargs)
-        timer.cancel()
-        return result
+        with AutoCancelTimer(seconds, inject_exception, args=[thread]):
+            return f(*args, **kwargs)
     return wrapper
 
 
 class PythonApp(AppBase):
     """Extends AppBase to cover the Python App."""
 
     def __init__(self, func, data_flow_kernel=None, cache=False, executors='all', ignore_for_cache=[], join=False):
```

### Comparing `parsl-2023.6.5/parsl/benchmark/perf.py` & `parsl-2023.7.3/parsl/benchmark/perf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/channels/base.py` & `parsl-2023.7.3/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/channels/errors.py` & `parsl-2023.7.3/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/channels/local/local.py` & `parsl-2023.7.3/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2023.7.3/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/channels/ssh/ssh.py` & `parsl-2023.7.3/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/channels/ssh_il/ssh_il.py` & `parsl-2023.7.3/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/concurrent/__init__.py` & `parsl-2023.7.3/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/config.py` & `parsl-2023.7.3/parsl/config.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/ASPIRE1.py` & `parsl-2023.7.3/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/Azure.py` & `parsl-2023.7.3/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/ad_hoc.py` & `parsl-2023.7.3/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/bluewaters.py` & `parsl-2023.7.3/parsl/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/bridges.py` & `parsl-2023.7.3/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/cc_in2p3.py` & `parsl-2023.7.3/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/comet.py` & `parsl-2023.7.3/parsl/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/cooley.py` & `parsl-2023.7.3/parsl/configs/cooley.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/cori.py` & `parsl-2023.7.3/parsl/tests/configs/midway.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from parsl.config import Config
 from parsl.providers import SlurmProvider
 from parsl.launchers import SrunLauncher
 from parsl.executors import HighThroughputExecutor
-from parsl.addresses import address_by_interface
 
+from .user_opts import user_opts
 
-config = Config(
-    executors=[
-        HighThroughputExecutor(
-            label='Cori_HTEX_multinode',
-            # This is the network interface on the login node to
-            # which compute nodes can communicate
-            address=address_by_interface('bond0.144'),
-            cores_per_worker=2,
-            provider=SlurmProvider(
-                'regular',  # Partition / QOS
-                nodes_per_block=2,
-                init_blocks=1,
-                # string to prepend to #SBATCH blocks in the submit
-                # script to the scheduler eg: '#SBATCH --constraint=knl,quad,cache'
-                scheduler_options='',
-                # Command to be run before starting a worker, such as:
-                # 'module load Anaconda; source activate parsl_env'.
-                worker_init='',
-                # We request all hyperthreads on a node.
-                launcher=SrunLauncher(overrides='-c 272'),
-                walltime='00:10:00',
-                # Slurm scheduler on Cori can be slow at times,
-                # increase the command timeouts
-                cmd_timeout=120,
-            ),
-        )
-    ]
-)
+
+def fresh_config():
+    config = Config(
+        executors=[
+            HighThroughputExecutor(
+                label='Midway_HTEX_multinode',
+                worker_debug=False,
+                max_workers=1,
+                provider=SlurmProvider(
+                    'broadwl',  # Partition name, e.g 'broadwl'
+                    launcher=SrunLauncher(),
+                    nodes_per_block=2,
+                    init_blocks=1,
+                    min_blocks=1,
+                    max_blocks=1,
+                    # string to prepend to #SBATCH blocks in the submit
+                    # script to the scheduler eg: '#SBATCH --constraint=knl,quad,cache'
+                    scheduler_options='',
+                    # Command to be run before starting a worker, such as:
+                    # 'module load Anaconda; source activate parsl_env'.
+                    worker_init=user_opts['midway']['worker_init'],
+                    walltime='00:30:00',
+                    cmd_timeout=120,
+                ),
+            )
+        ],
+    )
+    return config
+
+
+config = fresh_config()
```

### Comparing `parsl-2023.6.5/parsl/configs/ec2.py` & `parsl-2023.7.3/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/exex_local.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from parsl.providers import LocalProvider
 from parsl.channels import LocalChannel
 from parsl.launchers import SimpleLauncher
 
 from parsl.config import Config
-from parsl.executors.extreme_scale.executor import ExtremeScaleExecutor
+from parsl.executors import HighThroughputExecutor
 
-config = Config(
-    executors=[
-        ExtremeScaleExecutor(
-            label="Extreme_Local",
-            worker_debug=True,
-            ranks_per_node=2,
-            provider=LocalProvider(
-                channel=LocalChannel(),
-                init_blocks=1,
-                max_blocks=1,
-                launcher=SimpleLauncher(),
+
+def fresh_config():
+    return Config(
+        executors=[
+            HighThroughputExecutor(
+                label="htex_local",
+                worker_debug=True,
+                cores_per_worker=1,
+                provider=LocalProvider(
+                    channel=LocalChannel(),
+                    init_blocks=1,
+                    max_blocks=1,
+                    launcher=SimpleLauncher(),
+                ),
             )
-        )
-    ],
-    strategy='none',
-)
+        ],
+        strategy='none',
+    )
```

### Comparing `parsl-2023.6.5/parsl/configs/frontera.py` & `parsl-2023.7.3/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/illinoiscluster.py` & `parsl-2023.7.3/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/kubernetes.py` & `parsl-2023.7.3/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/midway.py` & `parsl-2023.7.3/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/osg.py` & `parsl-2023.7.3/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/polaris.py` & `parsl-2023.7.3/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/stampede2.py` & `parsl-2023.7.3/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/summit.py` & `parsl-2023.7.3/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/theta.py` & `parsl-2023.7.3/parsl/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/toss3_llnl.py` & `parsl-2023.7.3/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/configs/wqex_local.py` & `parsl-2023.7.3/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/data_provider/data_manager.py` & `parsl-2023.7.3/parsl/data_provider/data_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 if TYPE_CHECKING:
     from parsl.dataflow.dflow import DataFlowKernel
 
 logger = logging.getLogger(__name__)
 
 # these will be shared between all executors that do not explicitly
 # override, so should not contain executor-specific state
-default_staging = [NoOpFileStaging(), FTPSeparateTaskStaging(), HTTPSeparateTaskStaging()]  # type: List[Staging]
+default_staging: List[Staging]
+default_staging = [NoOpFileStaging(), FTPSeparateTaskStaging(), HTTPSeparateTaskStaging()]
 
 
 class DataManager:
     """The DataManager is responsible for transferring input and output data.
 
     """
```

### Comparing `parsl-2023.6.5/parsl/data_provider/files.py` & `parsl-2023.7.3/parsl/data_provider/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         """
         self.url = url
         parsed_url = urlparse(self.url)
         self.scheme = parsed_url.scheme if parsed_url.scheme else 'file'
         self.netloc = parsed_url.netloc
         self.path = parsed_url.path
         self.filename = os.path.basename(self.path)
-        self.local_path = None  # type: Optional[str]
+        self.local_path: Optional[str] = None
 
     def cleancopy(self) -> "File":
         """Returns a copy of the file containing only the global immutable state,
            without any mutable site-local local_path information. The returned File
            object will be as the original object was when it was constructed.
         """
         logger.debug("Making clean copy of File object {}".format(repr(self)))
```

### Comparing `parsl-2023.6.5/parsl/data_provider/ftp.py` & `parsl-2023.7.3/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/data_provider/globus.py` & `parsl-2023.7.3/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/data_provider/http.py` & `parsl-2023.7.3/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/data_provider/rsync.py` & `parsl-2023.7.3/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/data_provider/staging.py` & `parsl-2023.7.3/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/dataflow/dflow.py` & `parsl-2023.7.3/parsl/dataflow/dflow.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/dataflow/errors.py` & `parsl-2023.7.3/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/dataflow/futures.py` & `parsl-2023.7.3/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/dataflow/job_error_handler.py` & `parsl-2023.7.3/parsl/dataflow/job_error_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/dataflow/job_status_poller.py` & `parsl-2023.7.3/parsl/dataflow/job_status_poller.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/dataflow/memoization.py` & `parsl-2023.7.3/parsl/dataflow/memoization.py`

 * *Files 8% similar despite different names*

```diff
@@ -172,41 +172,38 @@
         Args:
             - task (dict) : Task dictionary from dfk.tasks
 
         Returns:
             - hash (str) : A unique hash string
         """
 
-        t = []  # type: List[bytes]
+        t: List[bytes] = []
 
         # if kwargs contains an outputs parameter, that parameter is removed
         # and normalised differently - with output_ref set to True.
         # kwargs listed in ignore_for_cache will also be removed
 
         filtered_kw = task['kwargs'].copy()
 
         ignore_list = task['ignore_for_cache']
 
-        logger.debug("Ignoring these kwargs for checkpointing: {}".format(ignore_list))
+        logger.debug("Ignoring these kwargs for checkpointing: %s", ignore_list)
         for k in ignore_list:
-            logger.debug("Ignoring kwarg {}".format(k))
+            logger.debug("Ignoring kwarg %s", k)
             del filtered_kw[k]
 
         if 'outputs' in task['kwargs']:
             outputs = task['kwargs']['outputs']
             del filtered_kw['outputs']
-            t = t + [id_for_memo(outputs, output_ref=True)]   # TODO: use append?
+            t.append(id_for_memo(outputs, output_ref=True))
 
-        t = t + [id_for_memo(filtered_kw)]
-        t = t + [id_for_memo(task['func']),
-                 id_for_memo(task['args'])]
+        t.extend(map(id_for_memo, (filtered_kw, task['func'], task['args'])))
 
         x = b''.join(t)
-        hashedsum = hashlib.md5(x).hexdigest()
-        return hashedsum
+        return hashlib.md5(x).hexdigest()
 
     def check_memo(self, task: TaskRecord) -> Optional[Future[Any]]:
         """Create a hash of the task and its inputs and check the lookup table for this hash.
 
         If present, the results are returned.
 
         Args:
```

### Comparing `parsl-2023.6.5/parsl/dataflow/rundirs.py` & `parsl-2023.7.3/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/dataflow/states.py` & `parsl-2023.7.3/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/dataflow/strategy.py` & `parsl-2023.7.3/parsl/dataflow/strategy.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/dataflow/taskrecord.py` & `parsl-2023.7.3/parsl/dataflow/taskrecord.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/errors.py` & `parsl-2023.7.3/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/base.py` & `parsl-2023.7.3/parsl/executors/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/errors.py` & `parsl-2023.7.3/parsl/executors/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/extreme_scale/mpi_worker_pool.py` & `parsl-2023.7.3/parsl/executors/flux/executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,496 +1,443 @@
-#!/usr/bin/env python3
+"""Defines the FluxExecutor class."""
 
-import argparse
-import logging
+import concurrent.futures as cf
+import functools
 import os
 import sys
-import platform
-# import random
+import uuid
 import threading
-import pickle
-import time
-import datetime
+import itertools
+import shutil
 import queue
-import uuid
+from socket import gethostname
+import collections
+from collections.abc import Mapping, Callable
+from typing import Optional, Any, Dict
+import weakref
+
 import zmq
-import json
 
-from mpi4py import MPI
+from parsl.utils import RepresentationMixin
+from parsl.executors.status_handling import NoStatusHandlingExecutor
+from parsl.executors.flux.execute_parsl_task import __file__ as _WORKER_PATH
+from parsl.executors.flux.flux_instance_manager import __file__ as _MANAGER_PATH
+from parsl.executors.errors import SerializationError, ScalingFailed
+from parsl.providers import LocalProvider
+from parsl.providers.base import ExecutionProvider
+from parsl.serialize import pack_apply_message, deserialize
+from parsl.app.errors import AppException
 
-from parsl.app.errors import RemoteExceptionWrapper
-from parsl.version import VERSION as PARSL_VERSION
-from parsl.serialize import unpack_apply_message, serialize
 
-RESULT_TAG = 10
-TASK_REQUEST_TAG = 11
+_WORKER_PATH = os.path.realpath(_WORKER_PATH)
+_MANAGER_PATH = os.path.realpath(_MANAGER_PATH)
 
-LOOP_SLOWDOWN = 0.0  # in seconds
 
-HEARTBEAT_CODE = (2 ** 32) - 1
+_FluxJobInfo = collections.namedtuple(
+    "_FluxJobInfo", ("future", "task_id", "infile", "outfile", "resource_spec")
+)
 
 
-class Manager:
-    """ Orchestrates the flow of tasks and results to and from the workers
+class FluxFutureWrapper(cf.Future):
+    """Wrapper class around a ``flux.job.FluxExecutorFuture.``
 
-    1. Queue up task requests from workers
-    2. Make batched requests from to the interchange for tasks
-    3. Receive and distribute tasks to workers
-    4. Act as a proxy to the Interchange for results.
+    Forwards methods onto the underlying FluxExecutorFuture.
     """
-    def __init__(self,
-                 comm, rank,
-                 task_q_url="tcp://127.0.0.1:50097",
-                 result_q_url="tcp://127.0.0.1:50098",
-                 max_queue_size=10,
-                 heartbeat_threshold=120,
-                 heartbeat_period=30,
-                 uid=None):
-        """
-        Parameters
-        ----------
-        worker_url : str
-             Worker url on which workers will attempt to connect back
-
-        heartbeat_threshold : int
-             Number of seconds since the last message from the interchange after which the worker
-             assumes that the interchange is lost and the manager shuts down. Default:120
-
-        heartbeat_period : int
-             Number of seconds after which a heartbeat message is sent to the interchange
-
-        """
-        self.uid = uid
-
-        self.context = zmq.Context()
-        self.task_incoming = self.context.socket(zmq.DEALER)
-        self.task_incoming.setsockopt(zmq.IDENTITY, uid.encode('utf-8'))
-        # Linger is set to 0, so that the manager can exit even when there might be
-        # messages in the pipe
-        self.task_incoming.setsockopt(zmq.LINGER, 0)
-        self.task_incoming.connect(task_q_url)
-
-        self.result_outgoing = self.context.socket(zmq.DEALER)
-        self.result_outgoing.setsockopt(zmq.IDENTITY, uid.encode('utf-8'))
-        self.result_outgoing.setsockopt(zmq.LINGER, 0)
-        self.result_outgoing.connect(result_q_url)
-
-        logger.info("Manager connected")
-        self.max_queue_size = max_queue_size + comm.size
-
-        # Creating larger queues to avoid queues blocking
-        # These can be updated after queue limits are better understood
-        self.pending_task_queue = queue.Queue()
-        self.pending_result_queue = queue.Queue()
-        self.ready_worker_queue = queue.Queue()
-
-        self.tasks_per_round = 1
-
-        self.heartbeat_period = heartbeat_period
-        self.heartbeat_threshold = heartbeat_threshold
-        self.comm = comm
-        self.rank = rank
-
-    def create_reg_message(self):
-        """ Creates a registration message to identify the worker to the interchange
-        """
-        msg = {'parsl_v': PARSL_VERSION,
-               'python_v': "{}.{}.{}".format(sys.version_info.major,
-                                             sys.version_info.minor,
-                                             sys.version_info.micro),
-               'os': platform.system(),
-               'hostname': platform.node(),
-               'dir': os.getcwd(),
-               'prefetch_capacity': 0,
-               'worker_count': (self.comm.size - 1),
-               'max_capacity': (self.comm.size - 1) + 0,  # (+prefetch)
-               'reg_time': datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
-        }
-        b_msg = json.dumps(msg).encode('utf-8')
-        return b_msg
 
-    def heartbeat(self):
-        """ Send heartbeat to the incoming task queue
-        """
-        heartbeat = (HEARTBEAT_CODE).to_bytes(4, "little")
-        r = self.task_incoming.send(heartbeat)
-        logger.debug("Return from heartbeat : {}".format(r))
-
-    def recv_result_from_workers(self):
-        """ Receives a results from the MPI worker pool and send it out via zmq
-
-        Returns:
-        --------
-            result: task result from the workers
-        """
-        info = MPI.Status()
-        result = self.comm.recv(source=MPI.ANY_SOURCE, tag=RESULT_TAG, status=info)
-        logger.debug("Received result from workers: {}".format(result))
-        return result
-
-    def recv_task_request_from_workers(self):
-        """ Receives 1 task request from MPI comm
-
-        Returns:
-        --------
-            worker_rank: worker_rank id
-        """
-        info = MPI.Status()
-        comm.recv(source=MPI.ANY_SOURCE, tag=TASK_REQUEST_TAG, status=info)
-        worker_rank = info.Get_source()
-        logger.info("Received task request from worker:{}".format(worker_rank))
-        return worker_rank
-
-    def pull_tasks(self, kill_event):
-        """ Pulls tasks from the incoming tasks zmq pipe onto the internal
-        pending task queue
-
-        Parameters:
-        -----------
-        kill_event : threading.Event
-              Event to let the thread know when it is time to die.
-        """
-        logger.info("[TASK PULL THREAD] starting")
-        poller = zmq.Poller()
-        poller.register(self.task_incoming, zmq.POLLIN)
-
-        # Send a registration message
-        msg = self.create_reg_message()
-        logger.debug("Sending registration message: {}".format(msg))
-        self.task_incoming.send(msg)
-        last_beat = time.time()
-        last_interchange_contact = time.time()
-        task_recv_counter = 0
-
-        poll_timer = 1
-
-        while not kill_event.is_set():
-            time.sleep(LOOP_SLOWDOWN)
-            ready_worker_count = self.ready_worker_queue.qsize()
-            pending_task_count = self.pending_task_queue.qsize()
-
-            logger.debug("[TASK_PULL_THREAD] ready workers:{}, pending tasks:{}".format(ready_worker_count,
-                                                                                        pending_task_count))
-
-            if time.time() > last_beat + self.heartbeat_period:
-                self.heartbeat()
-                last_beat = time.time()
-
-            if pending_task_count < self.max_queue_size and ready_worker_count > 0:
-                logger.debug("[TASK_PULL_THREAD] Requesting tasks: {}".format(ready_worker_count))
-                msg = ((ready_worker_count).to_bytes(4, "little"))
-                self.task_incoming.send(msg)
-
-            socks = dict(poller.poll(timeout=poll_timer))
-
-            if self.task_incoming in socks and socks[self.task_incoming] == zmq.POLLIN:
-                _, pkl_msg = self.task_incoming.recv_multipart()
-                tasks = pickle.loads(pkl_msg)
-                last_interchange_contact = time.time()
-
-                if tasks == 'STOP':
-                    logger.critical("[TASK_PULL_THREAD] Received stop request")
-                    kill_event.set()
-                    break
-
-                elif tasks == HEARTBEAT_CODE:
-                    logger.debug("Got heartbeat from interchange")
-
-                else:
-                    # Reset timer on receiving message
-                    poll_timer = 1
-                    task_recv_counter += len(tasks)
-                    logger.debug("[TASK_PULL_THREAD] Got tasks: {} of {}".format([t['task_id'] for t in tasks],
-                                                                                 task_recv_counter))
-                    for task in tasks:
-                        self.pending_task_queue.put(task)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._flux_future = None
+        self._cancellation_lock = threading.Lock()
+
+    def cancel(self):
+        # potential race condition: executor sets _flux_future after check
+        # that _flux_future is None. Protect the check and cancel() call with a lock.
+        with self._cancellation_lock:
+            if self._flux_future is None:
+                return super().cancel()
+        if self._flux_future.cancelled():
+            # due to a bug, flux futures can only have ``cancel`` called once
+            return True
+        if self._flux_future.cancel():  # cancel underlying future and then self
+            if not super().cancel():
+                raise RuntimeError("Unexpected state")
+            self.set_running_or_notify_cancel()  # also should be called only once
+            return True
+        return False
+
+    cancel.__doc__ = cf.Future.cancel.__doc__
+
+    def running(self):
+        if self._flux_future is None:
+            return False  # no race condition since ``running()`` just advisory
+        return self._flux_future.running()
+
+    running.__doc__ = cf.Future.running.__doc__
+
+
+def _complete_future(
+    expected_file: str, future_wrapper: FluxFutureWrapper, flux_future: Any
+):
+    """Callback triggered when a FluxExecutorFuture completes.
+
+    When the FluxExecutorFuture completes, check for the Parsl task's
+    output file, and assign the result to the FluxWrapperFuture future.
+
+    Parameters
+    ----------
+    expected_file : str
+        The path to the Parsl task's output file, storing the result of the task.
+    future_wrapper : FluxFutureWrapper
+        The user-facing future.
+    flux_future : FluxExecutorFuture
+        The future wrapped by ``future_wrapper``. Also accessible via
+        ``future_wrapper``, but the flux_future must be accepted as an argument
+        due to how ``concurrent.futures.add_done_callback`` works.
+    """
+    if flux_future.cancelled():  # if underlying future was cancelled, return
+        return  # no need to set a result on the wrapper future
+    try:
+        returncode = flux_future.result()
+    except Exception as unknown_err:
+        future_wrapper.set_exception(unknown_err)
+        return
+    if returncode == 0:
+        try:  # look for the output file
+            with open(expected_file, "rb") as file_handle:
+                task_result = deserialize(file_handle.read())
+        except FileNotFoundError:
+            future_wrapper.set_exception(
+                FileNotFoundError(
+                    f"No result found for Parsl task, expected {expected_file}"
+                )
+            )
+        except Exception as unknown_err:
+            future_wrapper.set_exception(unknown_err)
+        else:  # task package deserialized successfully
+            if task_result.exception is not None:
+                future_wrapper.set_exception(task_result.exception)
             else:
-                logger.debug("[TASK_PULL_THREAD] No incoming tasks")
-                # Limit poll duration to heartbeat_period
-                # heartbeat_period is in s vs poll_timer in ms
-                poll_timer = min(self.heartbeat_period * 1000, poll_timer * 2)
-
-                # Only check if no messages were received.
-                if time.time() > last_interchange_contact + self.heartbeat_threshold:
-                    logger.critical("[TASK_PULL_THREAD] Missing contact with interchange beyond heartbeat_threshold")
-                    kill_event.set()
-                    logger.critical("[TASK_PULL_THREAD] Exiting")
-                    break
-
-    def push_results(self, kill_event):
-        """ Listens on the pending_result_queue and sends out results via zmq
-
-        Parameters:
-        -----------
-        kill_event : threading.Event
-              Event to let the thread know when it is time to die.
-        """
-
-        # We set this timeout so that the thread checks the kill_event and does not
-        # block forever on the internal result queue
-        timeout = 0.1
-        # timer = time.time()
-        logger.debug("[RESULT_PUSH_THREAD] Starting thread")
-
-        while not kill_event.is_set():
-            time.sleep(LOOP_SLOWDOWN)
-            try:
-                items = []
-                while not self.pending_result_queue.empty():
-                    r = self.pending_result_queue.get(block=True)
-                    items.append(r)
-                if items:
-                    self.result_outgoing.send_multipart(items)
-
-            except queue.Empty:
-                logger.debug("[RESULT_PUSH_THREAD] No results to send in past {}seconds".format(timeout))
+                future_wrapper.set_result(task_result.returnval)
+    else:  # the job exited abnormally
+        future_wrapper.set_exception(
+            AppException(f"Parsl task exited abnormally: returned {returncode}")
+        )
+
+
+class FluxExecutor(NoStatusHandlingExecutor, RepresentationMixin):
+    """Executor that uses Flux to schedule and run jobs.
+
+    Every callable submitted to the executor is wrapped into a Flux job.
+
+    This executor requires that there be a Flux installation available
+    locally, and that it can be located either in PATH or through the
+    ``flux_path`` argument.
+
+    Flux jobs are fairly heavyweight. As of Flux v0.25, a single Flux
+    instance is (on many systems) capped at 50 jobs per second. As such,
+    this executor is not a good fit for use-cases consisting of large numbers
+    of small, fast jobs.
+
+    However, Flux is great at handling jobs with large resource requirements,
+    and collections of jobs with varying resource requirements.
+
+    Note that due to vendor-specific extensions, on certain Cray machines like
+    ALCF's Theta or LANL's Trinitite/Trinity, Flux cannot run applications
+    that use the default MPI library. Generally the only workaround is to
+    recompile with another MPI library like OpenMPI.
+
+    This executor acts as a sort of wrapper around a ``flux.job.FluxExecutor``,
+    which can be confusing since both wrapped and wrapper classes share the same name.
+    Whenever possible, the underlying executor is referred by its fully qualified name,
+    ``flux.job.FluxExecutor``.
+
+    Parameters
+    ----------
+    working_dir: str
+        Directory in which the executor should place its files, possibly overwriting
+        existing files. If ``None``, generate a unique directory.
+    label: str
+        Label for this executor instance.
+    flux_handle_args: collections.abc.Sequence
+        Positional arguments to ``flux.Flux()`` instance, if any.
+        The first positional argument, ``url``, is provided by this executor.
+    flux_executor_kwargs: collections.abc.Mapping
+        Keyword arguments to pass to the underlying ``flux.job.FluxExecutor()``
+        instance, if any. Note that the ``handle_args`` keyword
+        argument is provided by this executor,
+        in order to supply the URL of a remote Flux instance.
+    flux_path: str
+        Path to flux installation to use, or None to search PATH for flux.
+    launch_cmd: str
+        The command to use when launching the executor's backend. The default
+        command is available as the ``DEFAULT_LAUNCH_COMMAND`` attribute. The
+        default command starts a new Flux instance, which may not be desirable
+        if a Flux instance will already be provisioned (this is not likely).
+    """
 
-            except Exception as e:
-                logger.exception("[RESULT_PUSH_THREAD] Got an exception : {}".format(e))
+    DEFAULT_LAUNCH_CMD = "{flux} start {python} {manager} {protocol} {hostname} {port}"
 
-        logger.critical("[RESULT_PUSH_THREAD] Exiting")
+    def __init__(
+        self,
+        provider: Optional[ExecutionProvider] = None,
+        working_dir: Optional[str] = None,
+        label: str = "FluxExecutor",
+        flux_executor_kwargs: Mapping = {},
+        flux_path: Optional[str] = None,
+        launch_cmd: Optional[str] = None,
+    ):
+        super().__init__()
+        if provider is None:
+            provider = LocalProvider()
+        self._provider = provider
+        self.label = label
+        if working_dir is None:
+            working_dir = self.label + "_" + str(uuid.uuid4())
+        self.working_dir = os.path.abspath(working_dir)
+        # check that flux_path is an executable, or look for flux in PATH
+        if flux_path is None:
+            flux_path = shutil.which("flux")
+            if flux_path is None:
+                raise EnvironmentError("Cannot find Flux installation in PATH")
+        self.flux_path = os.path.abspath(flux_path)
+        self._task_id_counter = itertools.count()
+        self._socket = zmq.Context().socket(zmq.REP)
+        # Assumes a launch command cannot be None or empty
+        self.launch_cmd = launch_cmd or self.DEFAULT_LAUNCH_CMD
+        self._submission_queue: queue.Queue = queue.Queue()
+        self._stop_event = threading.Event()
+        # lock to protect self._task_id_counter and also submission/shutdown race
+        self._submission_lock = threading.Lock()
+        self.flux_executor_kwargs = flux_executor_kwargs
+        self._submission_thread = threading.Thread(
+            target=_submit_wrapper,
+            args=(
+                self._submission_queue,
+                self._stop_event,
+                self._socket,
+                self.working_dir,
+                self.flux_executor_kwargs,
+                self.provider,
+                self,
+                self.flux_path,
+                self.launch_cmd,
+            ),
+            daemon=True,
+        )
+        # add a ``weakref.finalize()`` function for joining the executor thread
+        weakref.finalize(
+            self,
+            lambda x, y: x.set() or y.join(),
+            self._stop_event,
+            self._submission_thread,
+        )
 
     def start(self):
-        """ Start the Manager process.
-
-        The worker loops on this:
+        """Called when DFK starts the executor when the config is loaded."""
+        os.makedirs(self.working_dir, exist_ok=True)
+        self._submission_thread.start()
 
-        1. If the last message sent was older than heartbeat period we send a heartbeat
-        2.
+    def shutdown(self, wait=True):
+        """Shut down the executor, causing further calls to ``submit`` to fail.
 
-
-        TODO: Move task receiving to a thread
+        Parameters
+        ----------
+        wait
+            If ``True``, do not return until all submitted Futures are done.
         """
+        with self._submission_lock:
+            self._stop_event.set()
+        if wait:
+            self._submission_thread.join()
+
+    def submit(
+        self,
+        func: Callable,
+        resource_specification: Dict[str, Any],
+        *args: Any,
+        **kwargs: Any,
+    ):
+        """Wrap a callable in a Flux job and submit it to Flux.
+
+        :param func: The callable to submit as a job to Flux
+
+        :param resource_specification: A mapping defining the resources to allocate to the Flux job.
+
+            Only the following keys are checked for:
+
+            -  num_tasks: the number of tasks to launch (MPI ranks for an MPI job), default 1
+            -  cores_per_task: cores per task, default 1
+            -  gpus_per_task: gpus per task, default 1
+            -  num_nodes: if > 0, evenly distribute the allocated cores/gpus
+               across the given number of nodes. Does *not* give the job exclusive
+               access to those nodes; this option only affects distribution.
 
-        self.comm.Barrier()
-        logger.debug("Manager synced with workers")
-
-        self._kill_event = threading.Event()
-        self._task_puller_thread = threading.Thread(target=self.pull_tasks,
-                                                    args=(self._kill_event,))
-        self._result_pusher_thread = threading.Thread(target=self.push_results,
-                                                      args=(self._kill_event,))
-        self._task_puller_thread.start()
-        self._result_pusher_thread.start()
-
-        start = None
-
-        result_counter = 0
-        task_recv_counter = 0
-        task_sent_counter = 0
-
-        logger.info("Loop start")
-        while not self._kill_event.is_set():
-            time.sleep(LOOP_SLOWDOWN)
-
-            # In this block we attempt to probe MPI for a set amount of time,
-            # and if we have exhausted all available MPI events, we move on
-            # to the next block. The timer and counter trigger balance
-            # fairness and responsiveness.
-            timer = time.time() + 0.05
-            counter = min(10, comm.size)
-            while time.time() < timer:
-                info = MPI.Status()
-
-                if counter > 10:
-                    logger.debug("Hit max mpi events per round")
-                    break
-
-                if not self.comm.Iprobe(status=info):
-                    logger.debug("Timer expired, processed {} mpi events".format(counter))
-                    break
-                else:
-                    tag = info.Get_tag()
-                    logger.info("Message with tag {} received".format(tag))
-
-                    counter += 1
-                    if tag == RESULT_TAG:
-                        result = self.recv_result_from_workers()
-                        self.pending_result_queue.put(result)
-                        result_counter += 1
-
-                    elif tag == TASK_REQUEST_TAG:
-                        worker_rank = self.recv_task_request_from_workers()
-                        self.ready_worker_queue.put(worker_rank)
-
-                    else:
-                        logger.error("Unknown tag {} - ignoring this message and continuing".format(tag))
-
-            available_worker_cnt = self.ready_worker_queue.qsize()
-            available_task_cnt = self.pending_task_queue.qsize()
-            logger.debug("[MAIN] Ready workers: {} Ready tasks: {}".format(available_worker_cnt,
-                                                                           available_task_cnt))
-            this_round = min(available_worker_cnt, available_task_cnt)
-            for i in range(this_round):
-                worker_rank = self.ready_worker_queue.get()
-                task = self.pending_task_queue.get()
-                comm.send(task, dest=worker_rank, tag=worker_rank)
-                task_sent_counter += 1
-                logger.debug("Assigning worker:{} task:{}".format(worker_rank, task['task_id']))
-
-            if not start:
-                start = time.time()
-
-            logger.debug("Tasks recvd:{} Tasks dispatched:{} Results recvd:{}".format(
-                task_recv_counter, task_sent_counter, result_counter))
-            # print("[{}] Received: {}".format(self.identity, msg))
-            # time.sleep(random.randint(4,10)/10)
-
-        self._task_puller_thread.join()
-        self._result_pusher_thread.join()
-
-        self.task_incoming.close()
-        self.result_outgoing.close()
-        self.context.term()
-
-        delta = time.time() - start
-        logger.info("mpi_worker_pool ran for {} seconds".format(delta))
+        :param args: positional arguments for the callable
 
+        :param kwargs: keyword arguments for the callable
+        """
+        # protect self._task_id_counter and shutdown/submit race
+        with self._submission_lock:
+            if self._stop_event.is_set():
+                raise RuntimeError("`shutdown()` already called")
+            task_id = str(next(self._task_id_counter))
+            infile = os.path.join(self.working_dir, f"{task_id}_in{os.extsep}pkl")
+            outfile = os.path.join(self.working_dir, f"{task_id}_out{os.extsep}pkl")
+            try:
+                fn_buf = pack_apply_message(
+                    func, args, kwargs, buffer_threshold=1024 * 1024
+                )
+            except TypeError:
+                raise SerializationError(func.__name__)
+            with open(infile, "wb") as infile_handle:
+                infile_handle.write(fn_buf)
+            future = FluxFutureWrapper()
+            self._submission_queue.put(
+                _FluxJobInfo(future, task_id, infile, outfile, resource_specification)
+            )
+            return future
+
+    def scale_in(self, *args, **kwargs):
+        pass
+
+    def scale_out(self):
+        pass
+
+
+def _submit_wrapper(
+    submission_queue: queue.Queue, stop_event: threading.Event, *args, **kwargs
+):
+    """Wrap the ``_submit_flux_jobs`` function in a try/except.
 
-def execute_task(bufs):
-    """Deserialize the buffer and execute the task.
-
-    Returns the serialized result or exception.
+    If an exception is thrown, error out all submitted tasks.
     """
-    user_ns = locals()
-    user_ns.update({'__builtins__': __builtins__})
-
-    f, args, kwargs = unpack_apply_message(bufs, user_ns, copy=False)
-
-    fname = getattr(f, '__name__', 'f')
-    prefix = "parsl_"
-    fname = prefix + "f"
-    argname = prefix + "args"
-    kwargname = prefix + "kwargs"
-    resultname = prefix + "result"
-
-    user_ns.update({fname: f,
-                    argname: args,
-                    kwargname: kwargs,
-                    resultname: resultname})
-
-    code = "{0} = {1}(*{2}, **{3})".format(resultname, fname,
-                                           argname, kwargname)
-
     try:
-        logger.debug("[RUNNER] Executing: {0}".format(code))
-        exec(code, user_ns, user_ns)
+        _submit_flux_jobs(submission_queue, stop_event, *args, **kwargs)
+    except Exception as exc:
+        _error_out_jobs(submission_queue, stop_event, exc)
+        raise
 
-    except Exception as e:
-        logger.warning("Caught exception; will raise it: {}".format(e))
-        raise e
-
-    else:
-        logger.debug("[RUNNER] Result: {0}".format(user_ns.get(resultname)))
-        return user_ns.get(resultname)
-
-
-def worker(comm, rank):
-    logger.info("Worker started")
-
-    # Sync worker with master
-    comm.Barrier()
-    logger.debug("Synced")
-
-    task_request = b'TREQ'
-
-    while True:
-        comm.send(task_request, dest=0, tag=TASK_REQUEST_TAG)
-        # The worker will receive {'task_id':<tid>, 'buffer':<buf>}
-        req = comm.recv(source=0, tag=rank)
-        logger.debug("Got req: {}".format(req))
-        tid = req['task_id']
-        logger.debug("Got task: {}".format(tid))
 
+def _error_out_jobs(
+    submission_queue: queue.Queue, stop_event: threading.Event, exc: Exception
+):
+    """Clear out ``submission_queue``, setting errors on all futures."""
+    while not stop_event.is_set() or not submission_queue.empty():
         try:
-            result = execute_task(req['buffer'])
-        except Exception as e:
-            result_package = {'type': 'result', 'task_id': tid, 'exception': serialize(RemoteExceptionWrapper(*sys.exc_info()))}
-            logger.debug("No result due to exception: {} with result package {}".format(e, result_package))
+            jobinfo = submission_queue.get(timeout=0.05)
+        except queue.Empty:
+            pass
         else:
-            result_package = {'type': 'result', 'task_id': tid, 'result': serialize(result)}
-            logger.debug("Result: {}".format(result))
-
-        pkl_package = pickle.dumps(result_package)
-        comm.send(pkl_package, dest=0, tag=RESULT_TAG)
+            jobinfo.future.set_exception(exc)
 
 
-def start_file_logger(filename, rank, name='parsl', level=logging.DEBUG, format_string=None):
-    """Add a stream log handler.
+def _submit_flux_jobs(
+    submission_queue: queue.Queue,
+    stop_event: threading.Event,
+    socket: zmq.Socket,
+    working_dir: str,
+    flux_executor_kwargs: Mapping,
+    provider: ExecutionProvider,
+    executor: FluxExecutor,
+    flux_path: str,
+    launch_cmd: str,
+):
+    """Function to be run in a separate thread by executor.
 
-    Args:
-        - filename (string): Name of the file to write logs to
-        - name (string): Logger name
-        - level (logging.LEVEL): Set the logging level.
-        - format_string (string): Set the format string
-
-    Returns:
-       -  None
+    Pull ``_FluxJobInfo`` job packages from a queue and submit them to Flux.
     """
-    if format_string is None:
-        format_string = "%(asctime)s.%(msecs)03d %(name)s:%(lineno)d Rank:{0} [%(levelname)s]  %(message)s".format(rank)
-
-    global logger
-    logger = logging.getLogger(name)
-    logger.setLevel(logging.DEBUG)
-    handler = logging.FileHandler(filename)
-    handler.setLevel(level)
-    formatter = logging.Formatter(format_string, datefmt='%Y-%m-%d %H:%M:%S')
-    handler.setFormatter(formatter)
-    logger.addHandler(handler)
-
-
-if __name__ == "__main__":
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    parser.add_argument("-l", "--logdir", default="parsl_worker_logs",
-                        help="Parsl worker log directory")
-    parser.add_argument("-u", "--uid", default=str(uuid.uuid4()).split('-')[-1],
-                        help="Unique identifier string for Manager")
-    parser.add_argument("-t", "--task_url", required=True,
-                        help="REQUIRED: ZMQ url for receiving tasks")
-    parser.add_argument("--hb_period", default=30,
-                        help="Heartbeat period in seconds. Uses manager default unless set")
-    parser.add_argument("--hb_threshold", default=120,
-                        help="Heartbeat threshold in seconds. Uses manager default unless set")
-    parser.add_argument("-r", "--result_url", required=True,
-                        help="REQUIRED: ZMQ url for posting results")
-
-    args = parser.parse_args()
-
-    comm = MPI.COMM_WORLD
-    rank = comm.Get_rank()
-    print("Starting rank: {}".format(rank))
+    provider.script_dir = working_dir
+    job_id = provider.submit(
+        launch_cmd.format(
+            port=socket.bind_to_random_port("tcp://*"),
+            protocol="tcp",
+            hostname=gethostname(),
+            python=sys.executable,
+            flux=flux_path,
+            manager=_MANAGER_PATH,
+        ),
+        1,
+    )
+    if not job_id:
+        raise ScalingFailed(
+            executor, "Attempt to provision nodes via provider has failed",
+        )
+    # wait for the flux package path to be sent
+    _check_provider_job(socket, provider, job_id)
+    # receive path to the ``flux`` package from the ZMQ socket
+    flux_pkg_path = socket.recv().decode()
+    # load the package. Unfortunately the only good way to do this is to
+    # modify sys.path
+    if flux_pkg_path not in sys.path:
+        sys.path.append(flux_pkg_path)
+    import flux.job
+
+    socket.send(b"ack")  # dummy message
+    # receive the URI of the Flux instance launched by provider
+    _check_provider_job(socket, provider, job_id)
+    flux_instance_uri = socket.recv()
+    # create a ``flux.job.FluxExecutor`` connected to remote Flux instance
+    with flux.job.FluxExecutor(
+        handle_args=(flux_instance_uri,), **flux_executor_kwargs
+    ) as flux_executor:
+        # need to ensure that no jobs submitted after stop_event set
+        # exit loop when event is set and queue is drained
+        while not stop_event.is_set() or not submission_queue.empty():
+            try:
+                jobinfo = submission_queue.get(timeout=0.05)
+            except queue.Empty:
+                pass
+            else:
+                _submit_single_job(flux_executor, working_dir, jobinfo)
+    socket.send(b"shutdown")
 
-    os.makedirs(args.logdir, exist_ok=True)
 
-    try:
-        if rank == 0:
-            start_file_logger('{}/manager.mpi_rank_{}.log'.format(args.logdir, rank),
-                              rank,
-                              level=logging.DEBUG if args.debug is True else logging.INFO)
-
-            logger.info("Python version: {}".format(sys.version))
-
-            manager = Manager(comm, rank,
-                              task_q_url=args.task_url,
-                              result_q_url=args.result_url,
-                              uid=args.uid,
-                              heartbeat_threshold=int(args.hb_threshold),
-                              heartbeat_period=int(args.hb_period))
-            manager.start()
-            logger.debug("Finalizing MPI Comm")
-            comm.Abort()
-        else:
-            start_file_logger('{}/worker.mpi_rank_{}.log'.format(args.logdir, rank),
-                              rank,
-                              level=logging.DEBUG if args.debug is True else logging.INFO)
-            worker(comm, rank)
-    except Exception as e:
-        logger.critical("mpi_worker_pool exiting from an exception")
-        logger.exception("Caught error: {}".format(e))
-        raise
-    else:
-        logger.info("mpi_worker_pool exiting")
-        print("MPI_WORKER_POOL exiting.")
+def _check_provider_job(socket: zmq.Socket, provider: ExecutionProvider, job_id: Any):
+    """Poll for messages, checking that the provider's allocation is alive."""
+    while not socket.poll(1000, zmq.POLLIN):
+        if provider.status([job_id])[0].terminal:
+            raise RuntimeError("Provider job has terminated")
+
+
+def _submit_single_job(flux_executor: Any, working_dir: str, jobinfo: _FluxJobInfo):
+    """Submit a single job to Flux. Link the Flux future with a user-facing future."""
+    import flux.job
+
+    jobspec = flux.job.JobspecV1.from_command(
+        command=[
+            sys.executable,
+            _WORKER_PATH,
+            "-i",
+            jobinfo.infile,
+            "-o",
+            jobinfo.outfile,
+        ],
+        num_tasks=jobinfo.resource_spec.get("num_tasks", 1),
+        num_nodes=jobinfo.resource_spec.get("num_nodes"),
+        cores_per_task=jobinfo.resource_spec.get("cores_per_task", 1),
+        gpus_per_task=jobinfo.resource_spec.get("gpus_per_task"),
+    )
+    jobspec.cwd = os.getcwd()
+    jobspec.environment = dict(os.environ)
+    jobspec.stdout = os.path.abspath(
+        os.path.join(working_dir, f"{jobinfo.task_id}_stdout{os.extsep}txt")
+    )
+    jobspec.stderr = os.path.abspath(
+        os.path.join(working_dir, f"{jobinfo.task_id}_stderr{os.extsep}txt")
+    )
+    # need to shield user future from cancellation while setting its underlying future
+    with jobinfo.future._cancellation_lock:
+        if jobinfo.future.cancelled():
+            return
+        try:
+            # flux_executor.submit() raises if the executor is broken for any reason
+            # most importantly, it raises if the remote flux instance dies
+            flux_future = flux_executor.submit(jobspec)
+        except Exception as exc:
+            jobinfo.future.set_exception(exc)
+            return
+        jobinfo.future._flux_future = flux_future
+    # Trigger the user-facing wrapper future to complete when the
+    # wrapped ``flux.job.FluxExecutor`` future completes.
+    flux_future.add_done_callback(
+        functools.partial(_complete_future, jobinfo.outfile, jobinfo.future)
+    )
```

### Comparing `parsl-2023.6.5/parsl/executors/flux/execute_parsl_task.py` & `parsl-2023.7.3/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/flux/flux_instance_manager.py` & `parsl-2023.7.3/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/high_throughput/executor.py` & `parsl-2023.7.3/parsl/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/high_throughput/interchange.py` & `parsl-2023.7.3/parsl/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/high_throughput/probe.py` & `parsl-2023.7.3/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2023.7.3/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2023.7.3/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/status_handling.py` & `parsl-2023.7.3/parsl/executors/status_handling.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/swift_t.py` & `parsl-2023.7.3/parsl/providers/lsf/lsf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,360 +1,284 @@
-"""Sample Executor for integration with SwiftT.
-
-This follows the model used by `EMEWS <http://www.mcs.anl.gov/~wozniak/papers/Cancer2_2016.pdf>`_
-to some extent.
-
-"""
-from concurrent.futures import Future
+import os
+import time
 import logging
-import uuid
-import threading
-import queue
-import multiprocessing as mp
-
-from parsl.serialize import serialize, deserialize
-from parsl.serialize import pack_apply_message, unpack_apply_message
-from parsl.executors.status_handling import NoStatusHandlingExecutor
-
-logger = logging.getLogger(__name__)
-
-
-BUFFER_THRESHOLD = 1024 * 1024
-
-
-def runner(incoming_q, outgoing_q):
-    """This is a function that mocks the Swift-T side.
-
-    It listens on the the incoming_q for tasks and posts returns on the outgoing_q.
-
-    Args:
-         - incoming_q (Queue object) : The queue to listen on
-         - outgoing_q (Queue object) : Queue to post results on
-
-    The messages posted on the incoming_q will be of the form :
-
-    .. code:: python
-
-       {
-          "task_id" : <uuid.uuid4 string>,
-          "buffer"  : serialized buffer containing the fn, args and kwargs
-       }
+import math
 
-    If ``None`` is received, the runner will exit.
+from parsl.channels import LocalChannel
+from parsl.launchers import SingleNodeLauncher
+from parsl.providers.cluster_provider import ClusterProvider
+from parsl.providers.lsf.template import template_string
+from parsl.providers.base import JobState, JobStatus
+from parsl.utils import RepresentationMixin, wtime_to_minutes
 
-    Response messages should be of the form:
-
-    .. code:: python
-
-       {
-          "task_id" : <uuid.uuid4 string>,
-          "result"  : serialized buffer containing result
-          "exception" : serialized exception object
-       }
-
-    On exiting the runner will post ``None`` to the outgoing_q
+logger = logging.getLogger(__name__)
 
+translate_table = {
+    'PEND': JobState.PENDING,
+    'RUN': JobState.RUNNING,
+    'DONE': JobState.COMPLETED,
+    'EXIT': JobState.FAILED,  # (failed),
+    'PSUSP': JobState.CANCELLED,
+    'USUSP': JobState.CANCELLED,
+    'SSUSP': JobState.CANCELLED,
+}
+
+
+class LSFProvider(ClusterProvider, RepresentationMixin):
+    """LSF Execution Provider
+
+    This provider uses bsub to submit, bjobs for status and bkill to cancel
+    jobs. The bsub script to be used is created from a template file in this
+    same module.
+
+    Parameters
+    ----------
+    channel : Channel
+        Channel for accessing this provider. Possible channels include
+        :class:`~parsl.channels.LocalChannel` (the default),
+        :class:`~parsl.channels.SSHChannel`, or
+        :class:`~parsl.channels.SSHInteractiveLoginChannel`.
+    nodes_per_block : int
+        Nodes to provision per block.
+        When request_by_nodes is False, it is computed by cores_per_block / cores_per_node.
+    cores_per_block : int
+        Cores to provision per block. Enabled only when request_by_nodes is False.
+    cores_per_node: int
+        Cores to provision per node. Enabled only when request_by_nodes is False.
+    init_blocks : int
+        Number of blocks to request at the start of the run.
+    min_blocks : int
+        Minimum number of blocks to maintain.
+    max_blocks : int
+        Maximum number of blocks to maintain.
+    parallelism : float
+        Ratio of provisioned task slots to active tasks. A parallelism value of 1 represents aggressive
+        scaling where as many resources as possible are used; parallelism close to 0 represents
+        the opposite situation in which as few resources as possible (i.e., min_blocks) are used.
+    walltime : str
+        Walltime requested per block in HH:MM:SS.
+    project : str
+        Project to which the resources must be charged
+    queue : str
+        Queue to which to submit the job request
+    scheduler_options : str
+        String to prepend to the #BSUB blocks in the submit script to the scheduler.
+    worker_init : str
+        Command to be run before starting a worker, such as 'module load Anaconda; source activate env'.
+    cmd_timeout : int
+        Seconds after which requests to the scheduler will timeout. Default: 120s
+    launcher : Launcher
+        Launcher for this provider. Possible launchers include
+        :class:`~parsl.launchers.SingleNodeLauncher` (the default),
+        :class:`~parsl.launchers.SrunLauncher`, or
+        :class:`~parsl.launchers.AprunLauncher`
+    move_files : Optional[Bool]: should files be moved? by default, Parsl will try to move files.
+    bsub_redirection: Bool
+        Should a redirection symbol "<" be included when submitting jobs, i.e., Bsub < job_script.
+    request_by_nodes: Bool
+        Request by nodes or request by cores per block.
+        When this is set to false, nodes_per_block is computed by cores_per_block / cores_per_node.
+        Default is True.
     """
-    logger.debug("[RUNNER] Starting")
-
-    def execute_task(bufs):
-        """Deserialize the buffer and execute the task.
-
-        Returns the serialized result or exception.
-        """
-        user_ns = locals()
-        user_ns.update({'__builtins__': __builtins__})
-
-        f, args, kwargs = unpack_apply_message(bufs, user_ns, copy=False)
-
-        fname = getattr(f, '__name__', 'f')
-        prefix = "parsl_"
-        fname = prefix + "f"
-        argname = prefix + "args"
-        kwargname = prefix + "kwargs"
-        resultname = prefix + "result"
-
-        user_ns.update({fname: f,
-                        argname: args,
-                        kwargname: kwargs,
-                        resultname: resultname})
-
-        code = "{0} = {1}(*{2}, **{3})".format(resultname, fname,
-                                               argname, kwargname)
-
-        try:
-            logger.debug("[RUNNER] Executing: {0}".format(code))
-            exec(code, user_ns, user_ns)
-
-        except Exception as e:
-            logger.warning("Caught exception; will raise it: {}".format(e))
-            raise e
-
-        else:
-            logger.debug("[RUNNER] Result: {0}".format(user_ns.get(resultname)))
-            return user_ns.get(resultname)
-
-    while True:
-        try:
-            # Blocking wait on the queue
-            msg = incoming_q.get(block=True, timeout=10)
-
-        except queue.Empty:
-            # Handle case where no items were in the queue
-            logger.debug("[RUNNER] Queue is empty")
-
-        except IOError as e:
-            logger.debug("[RUNNER] Broken pipe: {}".format(e))
-            try:
-                # Attempt to send a stop notification to the management thread
-                outgoing_q.put(None)
-
-            except Exception:
-                pass
-
-            break
-
-        except Exception as e:
-            logger.debug("[RUNNER] Caught unknown exception: {}".format(e))
 
+    def __init__(self,
+                 channel=LocalChannel(),
+                 nodes_per_block=1,
+                 cores_per_block=None,
+                 cores_per_node=None,
+                 init_blocks=1,
+                 min_blocks=0,
+                 max_blocks=1,
+                 parallelism=1,
+                 walltime="00:10:00",
+                 scheduler_options='',
+                 worker_init='',
+                 project=None,
+                 queue=None,
+                 cmd_timeout=120,
+                 move_files=True,
+                 bsub_redirection=False,
+                 request_by_nodes=True,
+                 launcher=SingleNodeLauncher()):
+        label = 'LSF'
+        super().__init__(label,
+                         channel,
+                         nodes_per_block,
+                         init_blocks,
+                         min_blocks,
+                         max_blocks,
+                         parallelism,
+                         walltime,
+                         cmd_timeout=cmd_timeout,
+                         launcher=launcher)
+
+        self.project = project
+        self.queue = queue
+        self.cores_per_block = cores_per_block
+        self.cores_per_node = cores_per_node
+        self.move_files = move_files
+        self.bsub_redirection = bsub_redirection
+        self.request_by_nodes = request_by_nodes
+
+        # Update scheduler options
+        self.scheduler_options = scheduler_options + "\n"
+        if project:
+            self.scheduler_options += "#BSUB -P {}\n".format(project)
+        if queue:
+            self.scheduler_options += "#BSUB -q {}\n".format(queue)
+        if request_by_nodes:
+            self.scheduler_options += "#BSUB -nnodes {}\n".format(nodes_per_block)
         else:
-            # Handle received message
-            if not msg:
-                # Empty message is a die request
-                logger.debug("[RUNNER] Received exit request")
-                outgoing_q.put(None)
-                break
-            else:
-                # Received a valid message, handle it
-                logger.debug("[RUNNER] Got a valid task with ID {}".format(msg["task_id"]))
-                try:
-                    response_obj = execute_task(msg['buffer'])
-                    response = {"task_id": msg["task_id"],
-                                "result": serialize(response_obj)}
-
-                    logger.debug("[RUNNER] Returing result: {}".format(
-                                   deserialize(response["result"])))
-
-                except Exception as e:
-                    logger.debug("[RUNNER] Caught task exception: {}".format(e))
-                    response = {"task_id": msg["task_id"],
-                                "exception": serialize(e)}
-
-                outgoing_q.put(response)
-
-    logger.debug("[RUNNER] Terminating")
-
-
-class TurbineExecutor(NoStatusHandlingExecutor):
-    """The Turbine executor.
-
-    Bypass the Swift/T language and run on top off the Turbine engines
-    in an MPI environment.
-
-    Here is a diagram
-
-    .. code:: python
-
-                        |  Data   |  Executor   |   IPC      | External Process(es)
-                        |  Flow   |             |            |
-                   Task | Kernel  |             |            |
-                 +----->|-------->|------------>|outgoing_q -|-> Worker_Process
-                 |      |         |             |            |    |         |
-           Parsl<---Fut-|         |             |            |  result   exception
-                     ^  |         |             |            |    |         |
-                     |  |         |   Q_mngmnt  |            |    V         V
-                     |  |         |    Thread<--|incoming_q<-|--- +---------+
-                     |  |         |      |      |            |
-                     |  |         |      |      |            |
-                     +----update_fut-----+
+            assert cores_per_block is not None and cores_per_node is not None, \
+                       "Requesting resources by the number of cores. " \
+                       "Need to specify cores_per_block and cores_per_node in the LSF provider."
 
-    """
+            self.scheduler_options += "#BSUB -n {}\n".format(cores_per_block)
+            self.scheduler_options += '#BSUB -R "span[ptile={}]"\n'.format(cores_per_node)
 
-    def __init__(self, label='turbine', storage_access=None, working_dir=None):
-        """Initialize the thread pool.
-
-        Trying to implement the emews model.
-
-        """
-        NoStatusHandlingExecutor.__init__(self)
-        logger.debug("Initializing TurbineExecutor")
-        self.label = label
-        self.storage_access = storage_access
-        self.working_dir = working_dir
-
-    def start(self):
-        self.mp_manager = mp.Manager()
-        self.outgoing_q = self.mp_manager.Queue()
-        self.incoming_q = self.mp_manager.Queue()
-        self.is_alive = True
-
-        self._queue_management_thread = None
-        self._start_queue_management_thread()
-        logger.debug("Created management thread : %s", self._queue_management_thread)
-
-        self.worker = mp.Process(target=runner, args=(self.outgoing_q, self.incoming_q))
-        self.worker.start()
-        logger.debug("Created worker : %s", self.worker)
-
-    def _queue_management_worker(self):
-        """Listen to the queue for task status messages and handle them.
-
-        Depending on the message, tasks will be updated with results, exceptions,
-        or updates. It expects the following messages:
-
-        .. code:: python
-
-            {
-               "task_id" : <task_id>
-               "result"  : serialized result object, if task succeeded
-               ... more tags could be added later
-            }
-
-            {
-               "task_id" : <task_id>
-               "exception" : serialized exception object, on failure
-            }
-
-        We do not support these yet, but they could be added easily.
-
-        .. code:: python
-
-            {
-               "task_id" : <task_id>
-               "cpu_stat" : <>
-               "mem_stat" : <>
-               "io_stat"  : <>
-               "started"  : tstamp
-            }
+            # Set nodes_per_block manually for Parsl strategy
+            assert cores_per_node != 0, "Need to specify a non-zero cores_per_node."
+            self.nodes_per_block = int(math.ceil(cores_per_block / cores_per_node))
 
-        The `None` message is a die request.
-        """
-        while True:
-            logger.debug("[MTHREAD] Management thread active")
-            try:
-                msg = self.incoming_q.get(block=True, timeout=1)
-
-            except queue.Empty:
-                # Timed out.
-                pass
-
-            except IOError as e:
-                logger.debug("[MTHREAD] Caught broken queue with exception code {}: {}".format(e.errno, e))
-                return
-
-            except Exception as e:
-                logger.debug("[MTHREAD] Caught unknown exception: {}".format(e))
-
-            else:
-
-                if msg is None:
-                    logger.debug("[MTHREAD] Got None")
-                    return
-
-                else:
-                    logger.debug("[MTHREAD] Received message: {}".format(msg))
-                    task_fut = self.tasks[msg['task_id']]
-                    if 'result' in msg:
-                        result, _ = deserialize(msg['result'])
-                        task_fut.set_result(result)
-
-                    elif 'exception' in msg:
-                        exception, _ = deserialize(msg['exception'])
-                        task_fut.set_exception(exception)
-
-            if not self.is_alive:
-                break
-
-    # When the executor gets lost, the weakref callback will wake up
-    # the queue management thread.
-    def weakref_cb(self, q=None):
-        """We do not use this yet."""
-        q.put(None)
-
-    def _start_queue_management_thread(self):
-        """Method to start the management thread as a daemon.
-
-        Checks if a thread already exists, then starts it.
-        Could be used later as a restart if the management thread dies.
-        """
-        logging.debug("In _start %s", "*" * 40)
-        if self._queue_management_thread is None:
-            logging.debug("Starting management thread ")
-            self._queue_management_thread = threading.Thread(target=self._queue_management_worker)
-            self._queue_management_thread.daemon = True
-            self._queue_management_thread.start()
-
-        else:
-            logging.debug("Management thread already exists, returning")
+        self.worker_init = worker_init
 
-    def shutdown(self):
-        """Shutdown method, to kill the threads and workers."""
-        self.is_alive = False
-        logging.debug("Waking management thread")
-        self.incoming_q.put(None)  # Wake up the thread
-        self._queue_management_thread.join()  # Force join
-        logging.debug("Exiting thread")
-        self.worker.join()
-        return True
-
-    def submit(self, func, *args, **kwargs):
-        """Submits work to the the outgoing_q.
-
-        The outgoing_q is an external process listens on this
-        queue for new work. This method is simply pass through and behaves like a
-        submit call as described here `Python docs: <https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor>`_
+    def _status(self):
+        '''Returns the status list for a list of job_ids
 
         Args:
-            - func (callable) : Callable function
-            - args (list) : List of arbitrary positional arguments.
-
-        Kwargs:
-            - kwargs (dict) : A dictionary of arbitrary keyword args for func.
+              self
 
         Returns:
-              Future
+              [status...] : Status list of all jobs
+        '''
+        logger.debug(f"Resources: {self.resources}")
+        job_id_list = [jid for jid, job in self.resources.items() if not job['status'].terminal]
+        if not job_id_list:
+            logger.debug('No active jobs, skipping status update')
+            return
+        logger.debug(f"job_id_list: {job_id_list}")
+        # only request the JOBID and STAT columns from LSF
+        cmd = f"bjobs -noheader -o 'jobid stat' {' '.join(job_id_list)}"
+        logger.debug(f"Executing command: {cmd}")
+        retcode, stdout, stderr = self.execute_wait(cmd)
+        logger.debug(f"bjobs returned:\nstdout=\n{stdout}stderr=\n{stderr}")
+        # Execute_wait failed. Do no update
+        if retcode != 0:
+            logger.warning(f"bjobs failed with non-zero exit code: {retcode}")
+            return
+
+        jobs_missing = set(job_id_list)
+        bjobs_lines = stdout.rstrip('\n').split('\n')
+
+        for line in bjobs_lines:
+            line_list = line.split()
+            if len(line_list) != 2:
+                logger.debug(f"{line_list} length not equal to 2, skipping")
+                continue
+            job_id, lsf_state = line_list
+            if job_id not in job_id_list:
+                logger.debug(f"job_id {job_id} not in job_id_list, skipping")
+                continue
+            if lsf_state not in translate_table:
+                logger.warning(f"LSF status {lsf_state} is not recognized")
+            state = translate_table.get(lsf_state, JobState.UNKNOWN)
+            logger.debug(f"Updating job {job_id} with LSF status {lsf_state} "
+                         f"to parsl state {state}")
+            self.resources[job_id]['status'] = JobStatus(state)
+            jobs_missing.remove(job_id)
+
+        # bjobs does not report on jobs that are not running. So we are filling in the
+        # blanks for missing jobs, we might lose some information about why the jobs failed.
+        for missing_job in jobs_missing:
+            logger.debug(f"Updating missing job {missing_job} to completed status")
+            self.resources[missing_job]['status'] = JobStatus(JobState.COMPLETED)
+
+    def submit(self, command, tasks_per_node, job_name="parsl.lsf"):
+        """Submit the command as an LSF job.
+
+        Parameters
+        ----------
+        command : str
+            Command to be made on the remote side.
+        tasks_per_node : int
+            Command invocations to be launched per node
+        job_name : str
+            Name for the job (must be unique).
+        Returns
+        -------
+        None or str
+            If at capacity, returns None; otherwise, a string identifier for the job
         """
-        task_id = uuid.uuid4()
-
-        logger.debug("Pushing function {} to queue with args {}".format(func, args))
-
-        self.tasks[task_id] = Future()
 
-        fn_buf = pack_apply_message(func, args, kwargs,
-                                    buffer_threshold=1024 * 1024)
+        job_name = "{0}.{1}".format(job_name, time.time())
 
-        msg = {"task_id": task_id,
-               "buffer": fn_buf}
+        script_path = "{0}/{1}.submit".format(self.script_dir, job_name)
+        script_path = os.path.abspath(script_path)
 
-        # Post task to the the outgoing queue
-        self.outgoing_q.put(msg)
+        logger.debug("Requesting one block with {} nodes".format(self.nodes_per_block))
 
-        # Return the future
-        return self.tasks[task_id]
-
-    def scale_out(self, blocks=1):
-        """Scales out the number of active workers by 1.
-
-        This method is not implemented for threads and will raise the error if called.
-        This would be nice to have, and can be done
+        job_config = {}
+        job_config["submit_script_dir"] = self.channel.script_dir
+        job_config["nodes"] = self.nodes_per_block
+        job_config["tasks_per_node"] = tasks_per_node
+        job_config["walltime"] = wtime_to_minutes(self.walltime)
+        job_config["scheduler_options"] = self.scheduler_options
+        job_config["worker_init"] = self.worker_init
+        job_config["user_script"] = command
+
+        # Wrap the command
+        job_config["user_script"] = self.launcher(command,
+                                                  tasks_per_node,
+                                                  self.nodes_per_block)
+
+        logger.debug("Writing submit script")
+        self._write_submit_script(template_string, script_path, job_name, job_config)
+
+        if self.move_files:
+            logger.debug("moving files")
+            channel_script_path = self.channel.push_file(script_path, self.channel.script_dir)
+        else:
+            logger.debug("not moving files")
+            channel_script_path = script_path
 
-        Raises:
-             NotImplementedError
-        """
-        raise NotImplementedError
+        if self.bsub_redirection:
+            cmd = "bsub < {0}".format(channel_script_path)
+        else:
+            cmd = "bsub {0}".format(channel_script_path)
+        retcode, stdout, stderr = super().execute_wait(cmd)
 
-    def scale_in(self, blocks):
-        """Scale in the number of active blocks by specified amount.
+        job_id = None
+        if retcode == 0:
+            for line in stdout.split('\n'):
+                if line.lower().startswith("job") and "is submitted to" in line.lower():
+                    job_id = line.split()[1].strip('<>')
+                    self.resources[job_id] = {'job_id': job_id, 'status': JobStatus(JobState.PENDING)}
+        else:
+            logger.warning("Submit command failed")
+            logger.error("Retcode:%s STDOUT:%s STDERR:%s", retcode, stdout.strip(), stderr.strip())
+        return job_id
 
-        This method is not implemented for turbine and will raise an error if called.
+    def cancel(self, job_ids):
+        ''' Cancels the jobs specified by a list of job ids
 
-        Raises:
-             NotImplementedError
-        """
-        raise NotImplementedError
+        Args:
+        job_ids : [<job_id> ...]
 
+        Returns :
+        [True/False...] : If the cancel operation fails the entire list will be False.
+        '''
+
+        job_id_list = ' '.join(job_ids)
+        retcode, stdout, stderr = self.execute_wait("bkill {0}".format(job_id_list))
+        rets = None
+        if retcode == 0:
+            for jid in job_ids:
+                self.resources[jid]['status'] = JobStatus(JobState.CANCELLED)  # Setting state to cancelled
+            rets = [True for i in job_ids]
+        else:
+            rets = [False for i in job_ids]
 
-if __name__ == "__main__":
+        return rets
 
-    print("Start")
-    turb_x = TurbineExecutor()
-    print("Done")
+    @property
+    def status_polling_interval(self):
+        return 60
```

### Comparing `parsl-2023.6.5/parsl/executors/threads.py` & `parsl-2023.7.3/parsl/executors/threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2023.7.3/parsl/executors/taskvine/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/workqueue/executor.py` & `parsl-2023.7.3/parsl/executors/workqueue/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,15 @@
             TCP port on Parsl submission machine for Work Queue workers
             to connect to. Workers will connect to Parsl using this port.
 
             If 0, Work Queue will allocate a port number automatically.
             In this case, environment variables can be used to influence the
             choice of port, documented here:
             https://ccl.cse.nd.edu/software/manuals/api/html/work__queue_8h.html#a21714a10bcdfcf5c3bd44a96f5dcbda6
-
-            Default: 0.
+            Default: WORK_QUEUE_DEFAULT_PORT.
 
         env: dict{str}
             Dictionary that contains the environmental variables that
             need to be set on the Work Queue worker machine.
 
         shared_fs: bool
             Define if working in a shared file system or not. If Parsl
@@ -175,15 +174,15 @@
             resources spent collecting stats.
 
         autocategory: bool
             Place each app in its own category by default. If all
             invocations of an app have similar performance characteristics,
             this will provide a reasonable set of categories automatically.
 
-        max_retries: Optional[int]
+        max_retries: int
             Set the number of retries that Work Queue will make when a task
             fails. This is distinct from Parsl level retries configured in
             parsl.config.Config. Set to None to allow Work Queue to retry
             tasks forever. By default, this is set to 1, so that all retries
             will be managed by Parsl.
 
         init_command: str
@@ -230,15 +229,15 @@
                  use_cache: bool = False,
                  source: bool = False,
                  pack: bool = False,
                  extra_pkgs: Optional[List[str]] = None,
                  autolabel: bool = False,
                  autolabel_window: int = 1,
                  autocategory: bool = True,
-                 max_retries: Optional[int] = 1,
+                 max_retries: int = 1,
                  init_command: str = "",
                  worker_options: str = "",
                  full_debug: bool = True,
                  worker_executable: str = 'work_queue_worker',
                  function_dir: Optional[str] = None,
                  coprocess: bool = False):
         BlockProviderExecutor.__init__(self, provider=provider,
@@ -257,15 +256,15 @@
         self.project_password_file = project_password_file
         self.env = env
         self.init_command = init_command
         self.shared_fs = shared_fs
         self.storage_access = storage_access
         self.use_cache = use_cache
         self.working_dir = working_dir
-        self.registered_files = set()  # type: Set[str]
+        self.registered_files: Set[str] = set()
         self.full_debug = full_debug
         self.source = True if pack else source
         self.pack = pack
         self.extra_pkgs = extra_pkgs or []
         self.autolabel = autolabel
         self.autolabel_window = autolabel_window
         self.autocategory = autocategory
```

### Comparing `parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/launchers/__init__.py` & `parsl-2023.7.3/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/launchers/launchers.py` & `parsl-2023.7.3/parsl/launchers/launchers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,14 @@
-from abc import ABCMeta, abstractmethod
 import logging
 
-from parsl.utils import RepresentationMixin
+from parsl.launchers.base import Launcher
 
 logger = logging.getLogger(__name__)
 
 
-class Launcher(RepresentationMixin, metaclass=ABCMeta):
-    """Launchers are basically wrappers for user submitted scripts as they
-    are submitted to a specific execution resource.
-    """
-    def __init__(self, debug: bool = True):
-        self.debug = debug
-
-    @abstractmethod
-    def __call__(self, command: str, tasks_per_node: int, nodes_per_block: int) -> str:
-        """ Wraps the command with the Launcher calls.
-        """
-        pass
-
-
 class SimpleLauncher(Launcher):
     """ Does no wrapping. Just returns the command as-is
     """
     def __init_(self, debug: bool = True) -> None:
         super().__init__(debug=debug)
 
     def __call__(self, command: str, tasks_per_node: int, nodes_per_block: int) -> str:
```

### Comparing `parsl-2023.6.5/parsl/log_utils.py` & `parsl-2023.7.3/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/db_manager.py` & `parsl-2023.7.3/parsl/monitoring/db_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/monitoring.py` & `parsl-2023.7.3/parsl/monitoring/monitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         # Any is used to disable typechecking on uses of _dfk_channel,
         # because it is used in the code as if it points to a channel, but
         # the static type is that it can also be None. The code relies on
         # .start() being called and initialising this to a real channel.
         self._dfk_channel = None  # type: Any
 
         if _db_manager_excepts:
-            raise(_db_manager_excepts)
+            raise _db_manager_excepts
 
         self.client_address = client_address
         self.client_port_range = client_port_range
 
         self.hub_address = hub_address
         self.hub_port = hub_port
         self.hub_port_range = hub_port_range
@@ -166,20 +166,31 @@
         os.makedirs(self.logdir, exist_ok=True)
 
         # Initialize the ZMQ pipe to the Parsl Client
 
         self.logger.debug("Initializing ZMQ Pipes to client")
         self.monitoring_hub_active = True
 
-        comm_q = SizedQueue(maxsize=10)  # type: Queue[Union[Tuple[int, int], str]]
-        self.exception_q = SizedQueue(maxsize=10)  # type: Queue[Tuple[str, str]]
-        self.priority_msgs = SizedQueue()  # type: Queue[Tuple[Any, int]]
-        self.resource_msgs = SizedQueue()  # type: Queue[AddressedMonitoringMessage]
-        self.node_msgs = SizedQueue()  # type: Queue[AddressedMonitoringMessage]
-        self.block_msgs = SizedQueue()  # type:  Queue[AddressedMonitoringMessage]
+        comm_q: Queue[Union[Tuple[int, int], str]]
+        comm_q = SizedQueue(maxsize=10)
+
+        self.exception_q: Queue[Tuple[str, str]]
+        self.exception_q = SizedQueue(maxsize=10)
+
+        self.priority_msgs: Queue[Tuple[Any, int]]
+        self.priority_msgs = SizedQueue()
+
+        self.resource_msgs: Queue[AddressedMonitoringMessage]
+        self.resource_msgs = SizedQueue()
+
+        self.node_msgs: Queue[AddressedMonitoringMessage]
+        self.node_msgs = SizedQueue()
+
+        self.block_msgs: Queue[AddressedMonitoringMessage]
+        self.block_msgs = SizedQueue()
 
         self.router_proc = ForkProcess(target=router_starter,
                                        args=(comm_q, self.exception_q, self.priority_msgs, self.node_msgs, self.block_msgs, self.resource_msgs),
                                        kwargs={"hub_address": self.hub_address,
                                                "hub_port": self.hub_port,
                                                "hub_port_range": self.hub_port_range,
                                                "logdir": self.logdir,
@@ -324,15 +335,15 @@
         for filename in os.listdir(new_dir):
             try:
                 logger.info(f"Processing filesystem radio file {filename}")
                 full_path_filename = f"{new_dir}/{filename}"
                 with open(full_path_filename, "rb") as f:
                     message = deserialize(f.read())
                 logger.info(f"Message received is: {message}")
-                assert(isinstance(message, tuple))
+                assert isinstance(message, tuple)
                 q.put(cast(AddressedMonitoringMessage, message))
                 os.remove(full_path_filename)
             except Exception:
                 logger.exception(f"Exception processing {filename} - probably will be retried next iteration")
 
         time.sleep(1)  # whats a good time for this poll?
```

### Comparing `parsl-2023.6.5/parsl/monitoring/queries/pandas.py` & `parsl-2023.7.3/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/radios.py` & `parsl-2023.7.3/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/remote.py` & `parsl-2023.7.3/parsl/monitoring/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import time
 import logging
 import datetime
 from functools import wraps
 
 from parsl.multiprocessing import ForkProcess
-from multiprocessing import Event, Process
+from multiprocessing import Event
 from parsl.process_loggers import wrap_with_logs
 
 from parsl.monitoring.message_type import MessageType
 from parsl.monitoring.radios import MonitoringRadio, UDPRadio, HTEXRadio, FilesystemRadio
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Callable, Dict, List, Sequence, Tuple
 
 logger = logging.getLogger(__name__)
 
 monitoring_wrapper_cache: Dict
 monitoring_wrapper_cache = {}
 
 
@@ -53,28 +53,28 @@
             send_first_message(try_id,
                                task_id,
                                monitoring_hub_url,
                                run_id,
                                radio_mode,
                                run_dir)
 
-            p: Optional[Process]
             if monitor_resources:
                 # create the monitor process and start
                 pp = ForkProcess(target=monitor,
                                  args=(os.getpid(),
                                        try_id,
                                        task_id,
                                        monitoring_hub_url,
                                        run_id,
                                        radio_mode,
                                        logging_level,
                                        sleep_dur,
                                        run_dir,
                                        terminate_event),
+                                 daemon=True,
                                  name="Monitor-Wrapper-{}".format(task_id))
                 pp.start()
                 p = pp
                 #  TODO: awkwardness because ForkProcess is not directly a constructor
                 # and type-checking is expecting p to be optional and cannot
                 # narrow down the type of p in this block.
 
@@ -185,14 +185,18 @@
     In some circumstances, it might be useful to hack in a handler so the
     logger calls remain in place.
     """
     import logging
     import platform
     import psutil
 
+    from parsl.utils import setproctitle
+
+    setproctitle("parsl: task resource monitor")
+
     radio: MonitoringRadio
     if radio_mode == "udp":
         radio = UDPRadio(monitoring_hub_url,
                          source_id=task_id)
     elif radio_mode == "htex":
         radio = HTEXRadio(monitoring_hub_url,
                           source_id=task_id)
```

### Comparing `parsl-2023.6.5/parsl/monitoring/types.py` & `parsl-2023.7.3/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/app.py` & `parsl-2023.7.3/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/models.py` & `parsl-2023.7.3/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2023.7.3/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2023.7.3/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/templates/app.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/templates/dag.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/templates/layout.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/templates/task.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/monitoring/visualization/views.py` & `parsl-2023.7.3/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/multiprocessing.py` & `parsl-2023.7.3/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/process_loggers.py` & `parsl-2023.7.3/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/__init__.py` & `parsl-2023.7.3/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2023.7.3/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/aws/aws.py` & `parsl-2023.7.3/parsl/providers/aws/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,35 +61,33 @@
     init_blocks : int
         Number of blocks to provision at the start of the run. Default is 1.
     min_blocks : int
         Minimum number of blocks to maintain. Default is 0.
     max_blocks : int
         Maximum number of blocks to maintain. Default is 10.
     instance_type : str
-        EC2 instance type. Instance types comprise varying combinations of CPU, memory,  .
-        storage, and networking capacity For more information on possible instance types,.
-        see `here <https://aws.amazon.com/ec2/instance-types/>`_ Default is 't2.small'.
+        EC2 instance type. Instance types comprise varying combinations of CPU, memory,
+        storage, and networking capacity For more information on possible instance types,
+        see `here <https://aws.amazon.com/ec2/instance-types/>`_. Default is 't2.small'.
     region : str
         Amazon Web Service (AWS) region to launch machines. Default is 'us-east-2'.
     key_name : str
         Name of the AWS private key (.pem file) that is usually generated on the console
         to allow SSH access to the EC2 instances. This is mostly used for debugging.
     spot_max_bid : float
         Maximum bid price (if requesting spot market machines).
     iam_instance_profile_arn : str
         Launch instance with a specific role.
     state_file : str
         Path to the state file from a previous run to re-use.
     walltime : str
         Walltime requested per block in HH:MM:SS. This option is not currently honored by this provider.
     launcher : Launcher
-        Launcher for this provider. Possible launchers include
-        :class:`~parsl.launchers.SingleNodeLauncher` (the default),
-        :class:`~parsl.launchers.SrunLauncher`, or
-        :class:`~parsl.launchers.AprunLauncher`
+        Launcher for this provider. With AWS, usually the default
+        :class:`~parsl.launchers.SingleNodeLauncher` will be appropriate.
     linger : Bool
         When set to True, the workers will not ``halt``. The user is responsible for shutting
         down the node.
     """
 
     def __init__(self,
                  image_id,
```

### Comparing `parsl-2023.6.5/parsl/providers/azure/azure.py` & `parsl-2023.7.3/parsl/providers/azure/azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/base.py` & `parsl-2023.7.3/parsl/providers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/cluster_provider.py` & `parsl-2023.7.3/parsl/providers/cluster_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,17 +63,15 @@
         self.min_blocks = min_blocks
         self.max_blocks = max_blocks
         self.parallelism = parallelism
         self.launcher = launcher
         self.walltime = walltime
         self.cmd_timeout = cmd_timeout
         if not callable(self.launcher):
-            raise(BadLauncher(self.launcher,
-                              "Launcher for executor: {} is of type: {}. Expects a parsl.launcher.launcher.Launcher or callable".format(
-                                  label, type(self.launcher))))
+            raise BadLauncher(self.launcher)
 
         self.script_dir = None
 
         # Dictionary that keeps track of jobs, keyed on job_id
         self.resources = {}
 
     def execute_wait(self, cmd, timeout=None):
```

### Comparing `parsl-2023.6.5/parsl/providers/cobalt/cobalt.py` & `parsl-2023.7.3/parsl/providers/cobalt/cobalt.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/condor/condor.py` & `parsl-2023.7.3/parsl/providers/condor/condor.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import time
 import typeguard
 
 from parsl.channels import LocalChannel
 from parsl.providers.base import JobState, JobStatus
 from parsl.utils import RepresentationMixin
 from parsl.launchers import SingleNodeLauncher
+from parsl.launchers.base import Launcher
 from parsl.providers.condor.template import template_string
 from parsl.providers.cluster_provider import ClusterProvider
 from parsl.providers.errors import ScaleOutFailed
 
 logger = logging.getLogger(__name__)
 
 from typing import Dict, List, Optional
 from parsl.channels.base import Channel
-from parsl.launchers.launchers import Launcher
 
 # See http://pages.cs.wisc.edu/~adesmet/status.html
 translate_table = {
     '1': JobState.PENDING,
     '2': JobState.RUNNING,
     '3': JobState.CANCELLED,
     '4': JobState.COMPLETED,
```

### Comparing `parsl-2023.6.5/parsl/providers/condor/template.py` & `parsl-2023.7.3/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/errors.py` & `parsl-2023.7.3/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/googlecloud/googlecloud.py` & `parsl-2023.7.3/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/grid_engine/grid_engine.py` & `parsl-2023.7.3/parsl/providers/grid_engine/grid_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,15 @@
         job_config["user_script"] = self.launcher(command,
                                                   tasks_per_node,
                                                   self.nodes_per_block)
         return job_config
 
     def submit(self, command, tasks_per_node, job_name="parsl.sge"):
         ''' The submit method takes the command string to be executed upon
-        instantiation of a resource most often to start a pilot (such as IPP engine
-        or even Swift-T engines).
+        instantiation of a resource most often to start a pilot.
 
         Args :
              - command (str) : The bash command string to be executed.
              - tasks_per_node (int) : command invocations to be launched per node
 
         KWargs:
              - job_name (str) : Human friendly name to be assigned to the job request
```

### Comparing `parsl-2023.6.5/parsl/providers/kubernetes/kube.py` & `parsl-2023.7.3/parsl/providers/kubernetes/kube.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,16 @@
         self.group_id = group_id
         self.run_as_non_root = run_as_non_root
         self.persistent_volumes = persistent_volumes
 
         self.kube_client = client.CoreV1Api()
 
         # Dictionary that keeps track of jobs, keyed on job_id
-        self.resources = {}  # type: Dict[object, Dict[str, Any]]
+        self.resources: Dict[object, Dict[str, Any]]
+        self.resources = {}
 
     def submit(self, cmd_string, tasks_per_node, job_name="parsl"):
         """ Submit a job
         Args:
              - cmd_string  :(String) - Name of the container to initiate
              - tasks_per_node (int) : command invocations to be launched per node
```

### Comparing `parsl-2023.6.5/parsl/providers/local/local.py` & `parsl-2023.7.3/parsl/providers/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/lsf/lsf.py` & `parsl-2023.7.3/parsl/providers/slurm/slurm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,216 +1,231 @@
 import os
+import math
 import time
 import logging
-import math
+import re
+import typeguard
+
+from typing import Optional
 
 from parsl.channels import LocalChannel
+from parsl.channels.base import Channel
 from parsl.launchers import SingleNodeLauncher
+from parsl.launchers.base import Launcher
 from parsl.providers.cluster_provider import ClusterProvider
-from parsl.providers.lsf.template import template_string
 from parsl.providers.base import JobState, JobStatus
+from parsl.providers.slurm.template import template_string
 from parsl.utils import RepresentationMixin, wtime_to_minutes
 
 logger = logging.getLogger(__name__)
 
 translate_table = {
-    'PEND': JobState.PENDING,
-    'RUN': JobState.RUNNING,
-    'DONE': JobState.COMPLETED,
-    'EXIT': JobState.FAILED,  # (failed),
-    'PSUSP': JobState.CANCELLED,
-    'USUSP': JobState.CANCELLED,
-    'SSUSP': JobState.CANCELLED,
+    'PD': JobState.PENDING,
+    'R': JobState.RUNNING,
+    'CA': JobState.CANCELLED,
+    'CF': JobState.PENDING,  # (configuring),
+    'CG': JobState.RUNNING,  # (completing),
+    'CD': JobState.COMPLETED,
+    'F': JobState.FAILED,  # (failed),
+    'TO': JobState.TIMEOUT,  # (timeout),
+    'NF': JobState.FAILED,  # (node failure),
+    'RV': JobState.FAILED,  # (revoked) and
+    'SE': JobState.FAILED   # (special exit state)
 }
 
 
-class LSFProvider(ClusterProvider, RepresentationMixin):
-    """LSF Execution Provider
+class SlurmProvider(ClusterProvider, RepresentationMixin):
+    """Slurm Execution Provider
 
     This provider uses sbatch to submit, squeue for status and scancel to cancel
     jobs. The sbatch script to be used is created from a template file in this
     same module.
 
     Parameters
     ----------
+    partition : str
+        Slurm partition to request blocks from. If unspecified or ``None``, no partition slurm directive will be specified.
+    account : str
+        Slurm account to which to charge resources used by the job. If unspecified or ``None``, the job will use the
+        user's default account.
     channel : Channel
         Channel for accessing this provider. Possible channels include
         :class:`~parsl.channels.LocalChannel` (the default),
         :class:`~parsl.channels.SSHChannel`, or
         :class:`~parsl.channels.SSHInteractiveLoginChannel`.
     nodes_per_block : int
         Nodes to provision per block.
-        When request_by_nodes is False, it is computed by cores_per_block / cores_per_node.
-    cores_per_block : int
-        Cores to provision per block. Enabled only when request_by_nodes is False.
-    cores_per_node: int
-        Cores to provision per node. Enabled only when request_by_nodes is False.
-    init_blocks : int
-        Number of blocks to request at the start of the run.
+    cores_per_node : int
+        Specify the number of cores to provision per node. If set to None, executors
+        will assume all cores on the node are available for computation. Default is None.
+    mem_per_node : int
+        Specify the real memory to provision per node in GB. If set to None, no
+        explicit request to the scheduler will be made. Default is None.
     min_blocks : int
         Minimum number of blocks to maintain.
     max_blocks : int
         Maximum number of blocks to maintain.
     parallelism : float
         Ratio of provisioned task slots to active tasks. A parallelism value of 1 represents aggressive
         scaling where as many resources as possible are used; parallelism close to 0 represents
         the opposite situation in which as few resources as possible (i.e., min_blocks) are used.
     walltime : str
         Walltime requested per block in HH:MM:SS.
-    project : str
-        Project to which the resources must be charged
-    queue : str
-        Queue to which to submit the job request
     scheduler_options : str
         String to prepend to the #SBATCH blocks in the submit script to the scheduler.
+    regex_job_id : str
+        The regular expression used to extract the job ID from the ``sbatch`` standard output.
+        The default is ``r"Submitted batch job (?P<id>\\S*)"``, where ``id`` is the regular expression
+        symbolic group for the job ID.
     worker_init : str
         Command to be run before starting a worker, such as 'module load Anaconda; source activate env'.
-    cmd_timeout : int
-        Seconds after which requests to the scheduler will timeout. Default: 120s
+    exclusive : bool (Default = True)
+        Requests nodes which are not shared with other running jobs.
     launcher : Launcher
         Launcher for this provider. Possible launchers include
         :class:`~parsl.launchers.SingleNodeLauncher` (the default),
         :class:`~parsl.launchers.SrunLauncher`, or
         :class:`~parsl.launchers.AprunLauncher`
     move_files : Optional[Bool]: should files be moved? by default, Parsl will try to move files.
-    bsub_redirection: Bool
-        Should a redirection symbol "<" be included when submitting jobs, i.e., Bsub < job_script.
-    request_by_nodes: Bool
-        Request by nodes or request by cores per block.
-        When this is set to false, nodes_per_block is computed by cores_per_block / cores_per_node.
-        Default is True.
     """
 
+    @typeguard.typechecked
     def __init__(self,
-                 channel=LocalChannel(),
-                 nodes_per_block=1,
-                 cores_per_block=None,
-                 cores_per_node=None,
-                 init_blocks=1,
-                 min_blocks=0,
-                 max_blocks=1,
-                 parallelism=1,
-                 walltime="00:10:00",
-                 scheduler_options='',
-                 worker_init='',
-                 project=None,
-                 queue=None,
-                 cmd_timeout=120,
-                 move_files=True,
-                 bsub_redirection=False,
-                 request_by_nodes=True,
-                 launcher=SingleNodeLauncher()):
-        label = 'LSF'
+                 partition: Optional[str] = None,
+                 account: Optional[str] = None,
+                 channel: Channel = LocalChannel(),
+                 nodes_per_block: int = 1,
+                 cores_per_node: Optional[int] = None,
+                 mem_per_node: Optional[int] = None,
+                 init_blocks: int = 1,
+                 min_blocks: int = 0,
+                 max_blocks: int = 1,
+                 parallelism: float = 1,
+                 walltime: str = "00:10:00",
+                 scheduler_options: str = '',
+                 regex_job_id: str = r"Submitted batch job (?P<id>\S*)",
+                 worker_init: str = '',
+                 cmd_timeout: int = 10,
+                 exclusive: bool = True,
+                 move_files: bool = True,
+                 launcher: Launcher = SingleNodeLauncher()):
+        label = 'slurm'
         super().__init__(label,
                          channel,
                          nodes_per_block,
                          init_blocks,
                          min_blocks,
                          max_blocks,
                          parallelism,
                          walltime,
                          cmd_timeout=cmd_timeout,
                          launcher=launcher)
 
-        self.project = project
-        self.queue = queue
-        self.cores_per_block = cores_per_block
+        self.partition = partition
         self.cores_per_node = cores_per_node
+        self.mem_per_node = mem_per_node
+        self.exclusive = exclusive
         self.move_files = move_files
-        self.bsub_redirection = bsub_redirection
-        self.request_by_nodes = request_by_nodes
-
-        # Update scheduler options
-        self.scheduler_options = scheduler_options + "\n"
-        if project:
-            self.scheduler_options += "#BSUB -P {}\n".format(project)
-        if queue:
-            self.scheduler_options += "#BSUB -q {}\n".format(queue)
-        if request_by_nodes:
-            self.scheduler_options += "#BSUB -nnodes {}\n".format(nodes_per_block)
-        else:
-            assert cores_per_block is not None and cores_per_node is not None, \
-                       "Requesting resources by the number of cores. " \
-                       "Need to specify cores_per_block and cores_per_node in the LSF provider."
-
-            self.scheduler_options += "#BSUB -n {}\n".format(cores_per_block)
-            self.scheduler_options += '#BSUB -R "span[ptile={}]"\n'.format(cores_per_node)
-
-            # Set nodes_per_block manually for Parsl strategy
-            assert cores_per_node != 0, "Need to specify a non-zero cores_per_node."
-            self.nodes_per_block = int(math.ceil(cores_per_block / cores_per_node))
-
-        self.worker_init = worker_init
+        self.account = account
+        self.scheduler_options = scheduler_options + '\n'
+        if exclusive:
+            self.scheduler_options += "#SBATCH --exclusive\n"
+        if partition:
+            self.scheduler_options += "#SBATCH --partition={}\n".format(partition)
+        if account:
+            self.scheduler_options += "#SBATCH --account={}\n".format(account)
+        self.regex_job_id = regex_job_id
+        self.worker_init = worker_init + '\n'
 
     def _status(self):
         '''Returns the status list for a list of job_ids
 
         Args:
               self
 
         Returns:
               [status...] : Status list of all jobs
         '''
-        job_id_list = ','.join(self.resources.keys())
-        cmd = "bjobs {0}".format(job_id_list)
+        job_id_list = ','.join(
+            [jid for jid, job in self.resources.items() if not job['status'].terminal]
+        )
+        if not job_id_list:
+            logger.debug('No active jobs, skipping status update')
+            return
+
+        cmd = "squeue --noheader --format='%i %t' --job '{0}'".format(job_id_list)
+        logger.debug("Executing %s", cmd)
+        retcode, stdout, stderr = self.execute_wait(cmd)
+        logger.debug("squeue returned %s %s", stdout, stderr)
 
-        retcode, stdout, stderr = super().execute_wait(cmd)
         # Execute_wait failed. Do no update
         if retcode != 0:
-            logger.debug("Updating job status from {} failed with return code {}".format(self.label,
-                                                                                         retcode))
+            logger.warning("squeue failed with non-zero exit code {}".format(retcode))
             return
 
-        jobs_missing = list(self.resources.keys())
+        jobs_missing = set(self.resources.keys())
         for line in stdout.split('\n'):
-            parts = line.split()
-            if parts and parts[0] != 'JOBID':
-                job_id = parts[0]
-                # the line can be uncompleted. len > 2 ensures safe indexing.
-                if len(parts) > 2:
-                    state = translate_table.get(parts[2], JobState.UNKNOWN)
-                    self.resources[job_id]['status'] = JobStatus(state)
-                    jobs_missing.remove(job_id)
+            if not line:
+                # Blank line
+                continue
+            job_id, slurm_state = line.split()
+            if slurm_state not in translate_table:
+                logger.warning(f"Slurm status {slurm_state} is not recognized")
+            status = translate_table.get(slurm_state, JobState.UNKNOWN)
+            logger.debug("Updating job {} with slurm status {} to parsl state {!s}".format(job_id, slurm_state, status))
+            self.resources[job_id]['status'] = JobStatus(status)
+            jobs_missing.remove(job_id)
 
         # squeue does not report on jobs that are not running. So we are filling in the
         # blanks for missing jobs, we might lose some information about why the jobs failed.
         for missing_job in jobs_missing:
+            logger.debug("Updating missing job {} to completed status".format(missing_job))
             self.resources[missing_job]['status'] = JobStatus(JobState.COMPLETED)
 
-    def submit(self, command, tasks_per_node, job_name="parsl.lsf"):
-        """Submit the command as an LSF job.
+    def submit(self, command, tasks_per_node, job_name="parsl.slurm"):
+        """Submit the command as a slurm job.
 
         Parameters
         ----------
         command : str
             Command to be made on the remote side.
         tasks_per_node : int
             Command invocations to be launched per node
         job_name : str
-            Name for the job (must be unique).
+            Name for the job
         Returns
         -------
         None or str
             If at capacity, returns None; otherwise, a string identifier for the job
         """
 
+        scheduler_options = self.scheduler_options
+        worker_init = self.worker_init
+        if self.mem_per_node is not None:
+            scheduler_options += '#SBATCH --mem={}g\n'.format(self.mem_per_node)
+            worker_init += 'export PARSL_MEMORY_GB={}\n'.format(self.mem_per_node)
+        if self.cores_per_node is not None:
+            cpus_per_task = math.floor(self.cores_per_node / tasks_per_node)
+            scheduler_options += '#SBATCH --cpus-per-task={}'.format(cpus_per_task)
+            worker_init += 'export PARSL_CORES={}\n'.format(cpus_per_task)
+
         job_name = "{0}.{1}".format(job_name, time.time())
 
         script_path = "{0}/{1}.submit".format(self.script_dir, job_name)
         script_path = os.path.abspath(script_path)
 
         logger.debug("Requesting one block with {} nodes".format(self.nodes_per_block))
 
         job_config = {}
         job_config["submit_script_dir"] = self.channel.script_dir
         job_config["nodes"] = self.nodes_per_block
         job_config["tasks_per_node"] = tasks_per_node
         job_config["walltime"] = wtime_to_minutes(self.walltime)
-        job_config["scheduler_options"] = self.scheduler_options
-        job_config["worker_init"] = self.worker_init
+        job_config["scheduler_options"] = scheduler_options
+        job_config["worker_init"] = worker_init
         job_config["user_script"] = command
 
         # Wrap the command
         job_config["user_script"] = self.launcher(command,
                                                   tasks_per_node,
                                                   self.nodes_per_block)
 
@@ -220,47 +235,48 @@
         if self.move_files:
             logger.debug("moving files")
             channel_script_path = self.channel.push_file(script_path, self.channel.script_dir)
         else:
             logger.debug("not moving files")
             channel_script_path = script_path
 
-        if self.bsub_redirection:
-            cmd = "bsub < {0}".format(channel_script_path)
-        else:
-            cmd = "bsub {0}".format(channel_script_path)
-        retcode, stdout, stderr = super().execute_wait(cmd)
+        retcode, stdout, stderr = self.execute_wait("sbatch {0}".format(channel_script_path))
 
         job_id = None
         if retcode == 0:
             for line in stdout.split('\n'):
-                if line.lower().startswith("job") and "is submitted to" in line.lower():
-                    job_id = line.split()[1].strip('<>')
+                match = re.match(self.regex_job_id, line)
+                if match:
+                    job_id = match.group("id")
                     self.resources[job_id] = {'job_id': job_id, 'status': JobStatus(JobState.PENDING)}
+                    break
+            else:
+                logger.error("Could not read job ID from sumbit command standard output.")
+                logger.error("Retcode:%s STDOUT:%s STDERR:%s", retcode, stdout.strip(), stderr.strip())
         else:
-            logger.warning("Submit command failed")
+            logger.error("Submit command failed")
             logger.error("Retcode:%s STDOUT:%s STDERR:%s", retcode, stdout.strip(), stderr.strip())
         return job_id
 
     def cancel(self, job_ids):
         ''' Cancels the jobs specified by a list of job ids
 
         Args:
         job_ids : [<job_id> ...]
 
         Returns :
         [True/False...] : If the cancel operation fails the entire list will be False.
         '''
 
         job_id_list = ' '.join(job_ids)
-        retcode, stdout, stderr = super().execute_wait("bkill {0}".format(job_id_list))
+        retcode, stdout, stderr = self.execute_wait("scancel {0}".format(job_id_list))
         rets = None
         if retcode == 0:
             for jid in job_ids:
-                self.resources[jid]['status'] = translate_table['USUSP']  # Job suspended by user/admin
+                self.resources[jid]['status'] = JobStatus(JobState.CANCELLED)  # Setting state to cancelled
             rets = [True for i in job_ids]
         else:
             rets = [False for i in job_ids]
 
         return rets
 
     @property
```

### Comparing `parsl-2023.6.5/parsl/providers/pbspro/pbspro.py` & `parsl-2023.7.3/parsl/providers/pbspro/pbspro.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/providers/slurm/slurm.py` & `parsl-2023.7.3/parsl/providers/torque/torque.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,282 +1,242 @@
+import logging
 import os
-import math
 import time
-import logging
-import re
-import typeguard
-
-from typing import Optional
 
 from parsl.channels import LocalChannel
-from parsl.channels.base import Channel
-from parsl.launchers import SingleNodeLauncher
-from parsl.launchers.launchers import Launcher
-from parsl.providers.cluster_provider import ClusterProvider
+from parsl.launchers import AprunLauncher
 from parsl.providers.base import JobState, JobStatus
-from parsl.providers.slurm.template import template_string
-from parsl.utils import RepresentationMixin, wtime_to_minutes
+from parsl.providers.torque.template import template_string
+from parsl.providers.cluster_provider import ClusterProvider
+from parsl.utils import RepresentationMixin
 
 logger = logging.getLogger(__name__)
 
+# From the man pages for qstat for PBS/Torque systems
 translate_table = {
-    'PD': JobState.PENDING,
+    'B': JobState.RUNNING,  # This state is returned for running array jobs
     'R': JobState.RUNNING,
-    'CA': JobState.CANCELLED,
-    'CF': JobState.PENDING,  # (configuring),
-    'CG': JobState.RUNNING,  # (completing),
-    'CD': JobState.COMPLETED,
-    'F': JobState.FAILED,  # (failed),
-    'TO': JobState.TIMEOUT,  # (timeout),
-    'NF': JobState.FAILED,  # (node failure),
-    'RV': JobState.FAILED,  # (revoked) and
-    'SE': JobState.FAILED   # (special exit state)
+    'C': JobState.COMPLETED,  # Completed after having run
+    'E': JobState.COMPLETED,  # Exiting after having run
+    'H': JobState.HELD,  # Held
+    'Q': JobState.PENDING,  # Queued, and eligible to run
+    'W': JobState.PENDING,  # Job is waiting for it's execution time (-a option) to be reached
+    'S': JobState.HELD  # Suspended
 }
 
 
-class SlurmProvider(ClusterProvider, RepresentationMixin):
-    """Slurm Execution Provider
+class TorqueProvider(ClusterProvider, RepresentationMixin):
+    """Torque Execution Provider
 
-    This provider uses sbatch to submit, squeue for status and scancel to cancel
-    jobs. The sbatch script to be used is created from a template file in this
+    This provider uses qsub to submit, qstat for status, and qdel to cancel
+    jobs. The qsub script to be used is created from a template file in this
     same module.
 
     Parameters
     ----------
-    partition : str
-        Slurm partition to request blocks from. If unspecified or ``None``, no partition slurm directive will be specified.
-    account : str
-        Slurm account to which to charge resources used by the job. If unspecified or ``None``, the job will use the
-        user's default account.
     channel : Channel
         Channel for accessing this provider. Possible channels include
         :class:`~parsl.channels.LocalChannel` (the default),
         :class:`~parsl.channels.SSHChannel`, or
         :class:`~parsl.channels.SSHInteractiveLoginChannel`.
+    account : str
+        Account the job will be charged against.
+    queue : str
+        Torque queue to request blocks from.
     nodes_per_block : int
         Nodes to provision per block.
-    cores_per_node : int
-        Specify the number of cores to provision per node. If set to None, executors
-        will assume all cores on the node are available for computation. Default is None.
-    mem_per_node : int
-        Specify the real memory to provision per node in GB. If set to None, no
-        explicit request to the scheduler will be made. Default is None.
+    init_blocks : int
+        Number of blocks to provision at the start of the run. Default is 1.
     min_blocks : int
-        Minimum number of blocks to maintain.
+        Minimum number of blocks to maintain. Default is 0.
     max_blocks : int
         Maximum number of blocks to maintain.
     parallelism : float
         Ratio of provisioned task slots to active tasks. A parallelism value of 1 represents aggressive
         scaling where as many resources as possible are used; parallelism close to 0 represents
         the opposite situation in which as few resources as possible (i.e., min_blocks) are used.
     walltime : str
         Walltime requested per block in HH:MM:SS.
     scheduler_options : str
-        String to prepend to the #SBATCH blocks in the submit script to the scheduler.
-    regex_job_id : str
-        The regular expression used to extract the job ID from the ``sbatch`` standard output.
-        The default is ``r"Submitted batch job (?P<id>\\S*)"``, where ``id`` is the regular expression
-        symbolic group for the job ID.
+        String to prepend to the #PBS blocks in the submit script to the scheduler.
+        WARNING: scheduler_options should only be given #PBS strings, and should not have trailing newlines.
     worker_init : str
         Command to be run before starting a worker, such as 'module load Anaconda; source activate env'.
-    exclusive : bool (Default = True)
-        Requests nodes which are not shared with other running jobs.
     launcher : Launcher
         Launcher for this provider. Possible launchers include
-        :class:`~parsl.launchers.SingleNodeLauncher` (the default),
-        :class:`~parsl.launchers.SrunLauncher`, or
-        :class:`~parsl.launchers.AprunLauncher`
-    move_files : Optional[Bool]: should files be moved? by default, Parsl will try to move files.
-    """
+        :class:`~parsl.launchers.AprunLauncher` (the default), or
+        :class:`~parsl.launchers.SingleNodeLauncher`,
 
-    @typeguard.typechecked
+    """
     def __init__(self,
-                 partition: Optional[str] = None,
-                 account: Optional[str] = None,
-                 channel: Channel = LocalChannel(),
-                 nodes_per_block: int = 1,
-                 cores_per_node: Optional[int] = None,
-                 mem_per_node: Optional[int] = None,
-                 init_blocks: int = 1,
-                 min_blocks: int = 0,
-                 max_blocks: int = 1,
-                 parallelism: float = 1,
-                 walltime: str = "00:10:00",
-                 scheduler_options: str = '',
-                 regex_job_id: str = r"Submitted batch job (?P<id>\S*)",
-                 worker_init: str = '',
-                 cmd_timeout: int = 10,
-                 exclusive: bool = True,
-                 move_files: bool = True,
-                 launcher: Launcher = SingleNodeLauncher()):
-        label = 'slurm'
+                 channel=LocalChannel(),
+                 account=None,
+                 queue=None,
+                 scheduler_options='',
+                 worker_init='',
+                 nodes_per_block=1,
+                 init_blocks=1,
+                 min_blocks=0,
+                 max_blocks=1,
+                 parallelism=1,
+                 launcher=AprunLauncher(),
+                 walltime="00:20:00",
+                 cmd_timeout=120):
+        label = 'torque'
         super().__init__(label,
                          channel,
                          nodes_per_block,
                          init_blocks,
                          min_blocks,
                          max_blocks,
                          parallelism,
                          walltime,
-                         cmd_timeout=cmd_timeout,
-                         launcher=launcher)
+                         launcher,
+                         cmd_timeout=cmd_timeout)
 
-        self.partition = partition
-        self.cores_per_node = cores_per_node
-        self.mem_per_node = mem_per_node
-        self.exclusive = exclusive
-        self.move_files = move_files
         self.account = account
-        self.scheduler_options = scheduler_options + '\n'
-        if exclusive:
-            self.scheduler_options += "#SBATCH --exclusive\n"
-        if partition:
-            self.scheduler_options += "#SBATCH --partition={}\n".format(partition)
-        if account:
-            self.scheduler_options += "#SBATCH --account={}\n".format(account)
-        self.regex_job_id = regex_job_id
-        self.worker_init = worker_init + '\n'
+        self.queue = queue
+        self.scheduler_options = scheduler_options
+        self.worker_init = worker_init
+        self.template_string = template_string
+
+        # Dictionary that keeps track of jobs, keyed on job_id
+        self.resources = {}
 
     def _status(self):
         '''Returns the status list for a list of job_ids
 
         Args:
               self
 
         Returns:
               [status...] : Status list of all jobs
         '''
-        job_id_list = ','.join(
-            [jid for jid, job in self.resources.items() if not job['status'].terminal]
-        )
-        if not job_id_list:
-            logger.debug('No active jobs, skipping status update')
-            return
-
-        cmd = "squeue --noheader --format='%i %t' --job '{0}'".format(job_id_list)
-        logger.debug("Executing %s", cmd)
-        retcode, stdout, stderr = self.execute_wait(cmd)
-        logger.debug("squeue returned %s %s", stdout, stderr)
-
-        # Execute_wait failed. Do no update
-        if retcode != 0:
-            logger.warning("squeue failed with non-zero exit code {}".format(retcode))
-            return
 
-        jobs_missing = set(self.resources.keys())
+        job_ids = list(self.resources.keys())
+        job_id_list = ' '.join(self.resources.keys())
+
+        jobs_missing = list(self.resources.keys())
+
+        retcode, stdout, stderr = self.execute_wait("qstat {0}".format(job_id_list))
         for line in stdout.split('\n'):
-            if not line:
-                # Blank line
+            parts = line.split()
+            if not parts or parts[0].upper().startswith('JOB') or parts[0].startswith('---'):
                 continue
-            job_id, slurm_state = line.split()
-            if slurm_state not in translate_table:
-                logger.warning(f"Slurm status {slurm_state} is not recognized")
-            status = translate_table.get(slurm_state, JobState.UNKNOWN)
-            logger.debug("Updating job {} with slurm status {} to parsl state {!s}".format(job_id, slurm_state, status))
-            self.resources[job_id]['status'] = JobStatus(status)
+            job_id = parts[0]  # likely truncated
+            for long_job_id in job_ids:
+                if long_job_id.startswith(job_id):
+                    logger.debug('coerced job_id %s -> %s', job_id, long_job_id)
+                    job_id = long_job_id
+                    break
+            state = translate_table.get(parts[4], JobState.UNKNOWN)
+            self.resources[job_id]['status'] = JobStatus(state)
             jobs_missing.remove(job_id)
 
         # squeue does not report on jobs that are not running. So we are filling in the
         # blanks for missing jobs, we might lose some information about why the jobs failed.
         for missing_job in jobs_missing:
-            logger.debug("Updating missing job {} to completed status".format(missing_job))
             self.resources[missing_job]['status'] = JobStatus(JobState.COMPLETED)
 
-    def submit(self, command, tasks_per_node, job_name="parsl.slurm"):
-        """Submit the command as a slurm job.
+    def submit(self, command, tasks_per_node, job_name="parsl.torque"):
+        ''' Submits the command onto an Local Resource Manager job.
+        Submit returns an ID that corresponds to the task that was just submitted.
 
-        Parameters
-        ----------
-        command : str
-            Command to be made on the remote side.
-        tasks_per_node : int
-            Command invocations to be launched per node
-        job_name : str
-            Name for the job
-        Returns
-        -------
-        None or str
-            If at capacity, returns None; otherwise, a string identifier for the job
-        """
-
-        scheduler_options = self.scheduler_options
-        worker_init = self.worker_init
-        if self.mem_per_node is not None:
-            scheduler_options += '#SBATCH --mem={}g\n'.format(self.mem_per_node)
-            worker_init += 'export PARSL_MEMORY_GB={}\n'.format(self.mem_per_node)
-        if self.cores_per_node is not None:
-            cpus_per_task = math.floor(self.cores_per_node / tasks_per_node)
-            scheduler_options += '#SBATCH --cpus-per-task={}'.format(cpus_per_task)
-            worker_init += 'export PARSL_CORES={}\n'.format(cpus_per_task)
+        If tasks_per_node <  1 : ! This is illegal. tasks_per_node should be integer
 
-        job_name = "{0}.{1}".format(job_name, time.time())
+        If tasks_per_node == 1:
+             A single node is provisioned
 
+        If tasks_per_node >  1 :
+             tasks_per_node number of nodes are provisioned.
+
+        Args:
+             - command  :(String) Commandline invocation to be made on the remote side.
+             - tasks_per_node (int) : command invocations to be launched per node
+
+        Kwargs:
+             - job_name (String): Name for job, must be unique
+
+        Returns:
+             - None: At capacity, cannot provision more
+             - job_id: (string) Identifier for the job
+
+        '''
+
+        # Set job name
+        job_name = "parsl.{0}.{1}".format(job_name, time.time())
+
+        # Set script path
         script_path = "{0}/{1}.submit".format(self.script_dir, job_name)
         script_path = os.path.abspath(script_path)
 
-        logger.debug("Requesting one block with {} nodes".format(self.nodes_per_block))
+        logger.debug("Requesting nodes_per_block:%s tasks_per_node:%s", self.nodes_per_block,
+                     tasks_per_node)
 
         job_config = {}
+        # TODO : script_path might need to change to accommodate script dir set via channels
         job_config["submit_script_dir"] = self.channel.script_dir
         job_config["nodes"] = self.nodes_per_block
+        job_config["task_blocks"] = self.nodes_per_block * tasks_per_node
+        job_config["nodes_per_block"] = self.nodes_per_block
         job_config["tasks_per_node"] = tasks_per_node
-        job_config["walltime"] = wtime_to_minutes(self.walltime)
-        job_config["scheduler_options"] = scheduler_options
-        job_config["worker_init"] = worker_init
+        job_config["walltime"] = self.walltime
+        job_config["scheduler_options"] = self.scheduler_options
+        job_config["worker_init"] = self.worker_init
         job_config["user_script"] = command
 
         # Wrap the command
         job_config["user_script"] = self.launcher(command,
                                                   tasks_per_node,
                                                   self.nodes_per_block)
 
         logger.debug("Writing submit script")
-        self._write_submit_script(template_string, script_path, job_name, job_config)
+        self._write_submit_script(self.template_string, script_path, job_name, job_config)
 
-        if self.move_files:
-            logger.debug("moving files")
-            channel_script_path = self.channel.push_file(script_path, self.channel.script_dir)
-        else:
-            logger.debug("not moving files")
-            channel_script_path = script_path
+        channel_script_path = self.channel.push_file(script_path, self.channel.script_dir)
 
-        retcode, stdout, stderr = self.execute_wait("sbatch {0}".format(channel_script_path))
+        submit_options = ''
+        if self.queue is not None:
+            submit_options = '{0} -q {1}'.format(submit_options, self.queue)
+        if self.account is not None:
+            submit_options = '{0} -A {1}'.format(submit_options, self.account)
+
+        launch_cmd = "qsub {0} {1}".format(submit_options, channel_script_path)
+        retcode, stdout, stderr = self.execute_wait(launch_cmd)
 
         job_id = None
         if retcode == 0:
             for line in stdout.split('\n'):
-                match = re.match(self.regex_job_id, line)
-                if match:
-                    job_id = match.group("id")
+                if line.strip():
+                    job_id = line.strip()
                     self.resources[job_id] = {'job_id': job_id, 'status': JobStatus(JobState.PENDING)}
-                    break
-            else:
-                logger.error("Could not read job ID from sumbit command standard output.")
-                logger.error("Retcode:%s STDOUT:%s STDERR:%s", retcode, stdout.strip(), stderr.strip())
         else:
-            logger.error("Submit command failed")
-            logger.error("Retcode:%s STDOUT:%s STDERR:%s", retcode, stdout.strip(), stderr.strip())
+            message = "Command '{}' failed with return code {}".format(launch_cmd, retcode)
+            if (stdout is not None) and (stderr is not None):
+                message += "\nstderr:{}\nstdout{}".format(stderr.strip(), stdout.strip())
+            logger.error(message)
+
         return job_id
 
     def cancel(self, job_ids):
         ''' Cancels the jobs specified by a list of job ids
 
         Args:
         job_ids : [<job_id> ...]
 
         Returns :
         [True/False...] : If the cancel operation fails the entire list will be False.
         '''
 
         job_id_list = ' '.join(job_ids)
-        retcode, stdout, stderr = self.execute_wait("scancel {0}".format(job_id_list))
+        retcode, stdout, stderr = self.execute_wait("qdel {0}".format(job_id_list))
         rets = None
         if retcode == 0:
             for jid in job_ids:
-                self.resources[jid]['status'] = JobStatus(JobState.CANCELLED)  # Setting state to cancelled
+                self.resources[jid]['status'] = JobStatus(JobState.COMPLETED)  # Setting state to exiting
             rets = [True for i in job_ids]
         else:
             rets = [False for i in job_ids]
 
         return rets
 
     @property
```

### Comparing `parsl-2023.6.5/parsl/serialize/base.py` & `parsl-2023.7.3/parsl/serialize/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
         """ This forces all child classes to register themselves as
         methods for serializing code or data
         """
         super().__init_subclass__(**kwargs)
 
-        assert len(cls._identifier) == 3
-
         if cls._for_code:
             METHODS_MAP_CODE[cls._identifier] = cls
         if cls._for_data:
             METHODS_MAP_DATA[cls._identifier] = cls
 
     _identifier: bytes
     _for_code: bool
@@ -38,27 +36,14 @@
 
         Returns
         -------
         identifier : str
         """
         return self._identifier
 
-    def chomp(self, payload: bytes) -> bytes:
-        """ If the payload starts with the identifier, return the remaining block
-
-        Parameters
-        ----------
-        payload : str
-            Payload blob
-        """
-        s_id, payload = payload.split(b'\n', 1)
-        if (s_id + b'\n') != self.identifier:
-            raise TypeError("Buffer does not start with parsl.serialize identifier:{!r}".format(self.identifier))
-        return payload
-
     def enable_caching(self, maxsize: int = 128) -> None:
         """ Add functools.lru_cache onto the serialize, deserialize methods
         """
 
         # ignore types here because mypy at the moment is not fond of monkeypatching
         self.serialize = functools.lru_cache(maxsize=maxsize)(self.serialize)  # type: ignore[method-assign]
         self.deserialize = functools.lru_cache(maxsize=maxsize)(self.deserialize)  # type: ignore[method-assign]
```

### Comparing `parsl-2023.6.5/parsl/serialize/concretes.py` & `parsl-2023.7.3/parsl/serialize/concretes.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,45 +13,39 @@
 
     * functions defined in a interpreter/notebook
     * classes defined in local context and not importable using a fully qualified name
     * closures, generators and coroutines
     * [sometimes] issues with wrapped/decorated functions
     """
 
-    _identifier = b'01\n'
+    _identifier = b'01'
     _for_code = True
     _for_data = True
 
     def serialize(self, data: Any) -> bytes:
-        x = pickle.dumps(data)
-        return self.identifier + x
+        return pickle.dumps(data)
 
-    def deserialize(self, payload: bytes) -> Any:
-        chomped = self.chomp(payload)
-        data = pickle.loads(chomped)
-        return data
+    def deserialize(self, body: bytes) -> Any:
+        return pickle.loads(body)
 
 
 class DillSerializer(SerializerBase):
     """ Dill serialization works on a superset of object including the ones covered by pickle.
     However for most cases pickle is faster. For most callable objects the additional overhead
     of dill can be amortized with an lru_cache. Here's items that dill handles that pickle
     doesn't:
 
     * functions defined in a interpreter/notebook
     * classes defined in local context and not importable using a fully qualified name
     * functions that are wrapped/decorated by other functions/classes
     * closures
     """
 
-    _identifier = b'02\n'
+    _identifier = b'02'
     _for_code = True
     _for_data = True
 
     def serialize(self, data: Any) -> bytes:
-        x = dill.dumps(data)
-        return self.identifier + x
+        return dill.dumps(data)
 
-    def deserialize(self, payload: bytes) -> Any:
-        chomped = self.chomp(payload)
-        data = dill.loads(chomped)
-        return data
+    def deserialize(self, body: bytes) -> Any:
+        return dill.loads(body)
```

### Comparing `parsl-2023.6.5/parsl/serialize/facade.py` & `parsl-2023.7.3/parsl/serialize/facade.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 from typing import Any, Dict, List, Tuple, Union
 
 logger = logging.getLogger(__name__)
 
 
 """ Instantiate the appropriate classes
 """
-headers = list(METHODS_MAP_CODE.keys()) + list(METHODS_MAP_DATA.keys())
-header_size = len(headers[0])
-
 methods_for_code = {}
 methods_for_data = {}
 
 for key in METHODS_MAP_CODE:
     methods_for_code[key] = METHODS_MAP_CODE[key]()
     methods_for_code[key].enable_caching(maxsize=128)
 
@@ -66,24 +63,24 @@
     Individual serialization methods might raise a TypeError (eg. if objects are non serializable)
     This method will raise the exception from the last method that was tried, if all methods fail.
     """
     result: Union[bytes, Exception]
     if callable(obj):
         for method in methods_for_code.values():
             try:
-                result = method.serialize(obj)
+                result = method._identifier + b'\n' + method.serialize(obj)
             except Exception as e:
                 result = e
                 continue
             else:
                 break
     else:
         for method in methods_for_data.values():
             try:
-                result = method.serialize(obj)
+                result = method._identifier + b'\n' + method.serialize(obj)
             except Exception as e:
                 result = e
                 continue
             else:
                 break
 
     if isinstance(result, BaseException):
@@ -98,19 +95,20 @@
     """
     Parameters
     ----------
     payload : str
        Payload object to be deserialized
 
     """
-    header = payload[0:header_size]
+    header, body = payload.split(b'\n', 1)
+
     if header in methods_for_code:
-        result = methods_for_code[header].deserialize(payload)
+        result = methods_for_code[header].deserialize(body)
     elif header in methods_for_data:
-        result = methods_for_data[header].deserialize(payload)
+        result = methods_for_data[header].deserialize(body)
     else:
         raise TypeError("Invalid header: {!r} in data payload. Buffer is either corrupt or not created by ParslSerializer".format(header))
 
     return result
 
 
 def pack_buffers(buffers: List[bytes]) -> bytes:
```

### Comparing `parsl-2023.6.5/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2023.7.3/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/azure_single_node.py` & `parsl-2023.7.3/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/bluewaters.py` & `parsl-2023.7.3/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/bridges.py` & `parsl-2023.7.3/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/cc_in2p3.py` & `parsl-2023.7.3/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/comet.py` & `parsl-2023.7.3/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/cooley_htex.py` & `parsl-2023.7.3/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/cori.py` & `parsl-2023.7.3/parsl/tests/configs/summit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 from parsl.config import Config
-from parsl.providers import SlurmProvider
-from parsl.launchers import SrunLauncher
 from parsl.executors import HighThroughputExecutor
-from parsl.addresses import address_by_interface
+from parsl.launchers import JsrunLauncher
+from parsl.providers import LSFProvider
+
 from .user_opts import user_opts
+""" This config assumes that it is used to launch parsl tasks from the login nodes
+of Frontera at TACC. Each job submitted to the scheduler will request 2 nodes for 10 minutes.
+"""
 
 
 def fresh_config():
     return Config(
         executors=[
             HighThroughputExecutor(
-                label='Cori_HTEX_multinode',
-                # This is the network interface on the login node to
-                # which compute nodes can communicate
-                # address=address_by_interface('bond0.144'),
+                label='Summit_HTEX',
+                # On Summit ensure that the working dir is writeable from the compute nodes,
+                # for eg. paths below /gpfs/alpine/world-shared/
+                # working_dir='',
+
+                # address=address_by_interface('ib0'),  # This assumes Parsl is running on login node
+                worker_port_range=(50000, 55000),
                 max_workers=1,
-                address=address_by_interface('bond0.144'),
-                provider=SlurmProvider(
-                    'debug',  # Partition / QOS
+                provider=LSFProvider(
+                    launcher=JsrunLauncher(),
+                    walltime="00:10:00",
                     nodes_per_block=2,
                     init_blocks=1,
-                    # string to prepend to #SBATCH blocks in the submit
-                    # script to the scheduler eg: '#SBATCH --constraint=knl,quad,cache'
-                    scheduler_options=user_opts['cori']['scheduler_options'],
-
-                    # Command to be run before starting a worker, such as:
-                    # 'module load Anaconda; source activate parsl_env'.
-                    worker_init=user_opts['cori']['worker_init'],
-
-                    # We request all hyperthreads on a node.
-                    launcher=SrunLauncher(overrides='-c 272'),
-                    walltime='00:10:00',
-                    # Slurm scheduler on Cori can be slow at times,
-                    # increase the command timeouts
-                    cmd_timeout=120,
+                    max_blocks=1,
+                    worker_init=user_opts['summit']['worker_init'],
+                    project=user_opts['summit']['project'],
+                    cmd_timeout=60
                 ),
             )
-        ]
+        ],
     )
```

### Comparing `parsl-2023.6.5/parsl/tests/configs/ec2_single_node.py` & `parsl-2023.7.3/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/ec2_spot.py` & `parsl-2023.7.3/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/frontera.py` & `parsl-2023.7.3/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2023.7.3/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/htex_local.py` & `parsl-2023.7.3/parsl/tests/configs/nscc_singapore.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,42 @@
-from parsl.providers import LocalProvider
-from parsl.channels import LocalChannel
-from parsl.launchers import SimpleLauncher
-
-from parsl.config import Config
+from parsl.providers import PBSProProvider
 from parsl.executors import HighThroughputExecutor
+from parsl.launchers import MpiRunLauncher
+from parsl.addresses import address_by_interface
+from parsl.config import Config
+
+from .user_opts import user_opts
 
 
 def fresh_config():
     return Config(
         executors=[
             HighThroughputExecutor(
-                label="htex_local",
-                worker_debug=True,
-                cores_per_worker=1,
-                provider=LocalProvider(
-                    channel=LocalChannel(),
-                    init_blocks=1,
+                label="htex",
+                heartbeat_period=15,
+                heartbeat_threshold=120,
+                worker_debug=False,
+                max_workers=1,
+                address=address_by_interface('ib0'),
+                provider=PBSProProvider(
+                    launcher=MpiRunLauncher(),
+                    # string to prepend to #PBS blocks in the submit
+                    # script to the scheduler
+                    # E.g., project name
+                    scheduler_options=user_opts['nscc']['scheduler_options'],
+                    # Command to be run before starting a worker, such as:
+                    # 'module load Anaconda; source activate parsl_env'.
+                    worker_init=user_opts['nscc']['worker_init'],
+                    nodes_per_block=2,
+                    min_blocks=1,
                     max_blocks=1,
-                    launcher=SimpleLauncher(),
+                    cpus_per_node=24,
+                    walltime="00:20:00",
+                    cmd_timeout=300,
                 ),
-            )
+            ),
         ],
-        strategy='none',
+        strategy='simple',
     )
+
+
+config = fresh_config()
```

### Comparing `parsl-2023.6.5/parsl/tests/configs/htex_local_alternate.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/local_threads_globus.py` & `parsl-2023.7.3/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/midway.py` & `parsl-2023.7.3/parsl/tests/configs/osg_htex.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 from parsl.config import Config
-from parsl.providers import SlurmProvider
-from parsl.launchers import SrunLauncher
+from parsl.providers import CondorProvider
 from parsl.executors import HighThroughputExecutor
 
+# If you are a developer running tests, make sure to update parsl/tests/configs/user_opts.py
+# If you are a user copying-and-pasting this as an example, make sure to either
+#       1) create a local `user_opts.py`, or
+#       2) delete the user_opts import below and replace all appearances of `user_opts` with the literal value
+#          (i.e., user_opts['swan']['username'] -> 'your_username')
 from .user_opts import user_opts
 
-
-def fresh_config():
-    config = Config(
-        executors=[
-            HighThroughputExecutor(
-                label='Midway_HTEX_multinode',
-                worker_debug=False,
-                max_workers=1,
-                provider=SlurmProvider(
-                    'broadwl',  # Partition name, e.g 'broadwl'
-                    launcher=SrunLauncher(),
-                    nodes_per_block=2,
-                    init_blocks=1,
-                    min_blocks=1,
-                    max_blocks=1,
-                    # string to prepend to #SBATCH blocks in the submit
-                    # script to the scheduler eg: '#SBATCH --constraint=knl,quad,cache'
-                    scheduler_options='',
-                    # Command to be run before starting a worker, such as:
-                    # 'module load Anaconda; source activate parsl_env'.
-                    worker_init=user_opts['midway']['worker_init'],
-                    walltime='00:30:00',
-                    cmd_timeout=120,
-                ),
-            )
-        ],
-    )
-    return config
-
-
-config = fresh_config()
+config = Config(
+    executors=[
+        HighThroughputExecutor(
+            label='OSG_HTEX',
+            max_workers=1,
+            provider=CondorProvider(
+                nodes_per_block=1,
+                init_blocks=4,
+                max_blocks=4,
+                # This scheduler option string ensures that the compute nodes provisioned
+                # will have modules
+                scheduler_options='Requirements = OSGVO_OS_STRING == "RHEL 6" && Arch == "X86_64" &&  HAS_MODULES == True',
+                # Command to be run before starting a worker, such as:
+                # 'module load Anaconda; source activate parsl_env'.
+                worker_init=user_opts['osg']['worker_init'],
+                walltime="00:20:00",
+            ),
+        )
+    ]
+)
```

### Comparing `parsl-2023.6.5/parsl/tests/configs/petrelkube.py` & `parsl-2023.7.3/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/swan_htex.py` & `parsl-2023.7.3/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/theta.py` & `parsl-2023.7.3/parsl/tests/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/configs/user_opts.py` & `parsl-2023.7.3/parsl/tests/configs/user_opts.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,14 @@
     },
     'nscc': {
         'worker_init': 'source ~/setup_parsl_test_env.sh;',
     },
     'theta': {
         'worker_init': 'source ~/setup_parsl_test_env.sh;',
     },
-    'cori': {
-        'worker_init': 'source ~/setup_parsl_test_env.sh;',
-    },
     'summit': {
         'worker_init': 'source ~/setup_parsl_test_env.sh;',
     },
     'bluewaters': {
         'worker_init': 'source ~/setup_parsl_test_env.sh;',
     },
     'midway': {
@@ -59,21 +56,14 @@
     # },
     # 'osg': {
     #     'username': OSG_USERNAME,
     #     'script_dir': '/home/{}/parsl_scripts'.format(OSG_USERNAME),
     #     'scheduler_options': "",
     #     'worker_init' : 'module load python/3.5.2; python3 -m venv parsl_env; source parsl_env/bin/activate; python3 -m pip install parsl==0.5.2'
     # },
-    # 'cori': {
-    #     'username': CORI_USERNAME,
-    #     'script_dir': "/global/homes/y/{}/parsl_scripts".format(CORI_USERNAME),
-    #     'scheduler_options': "#SBATCH --constraint=haswell",
-    #     "worker_init": """module load python/3.6-anaconda-4.4 ;
-    #     source activate parsl_env_3.6"""
-    # },
     # 'swan': {
     #     'username': SWAN_USERNAME,
     #     'script_dir' : "/home/users/{}/parsl_scripts".format(SWAN_USERNAME),
     #     'scheduler_options': "",
     #     'worker_init': "module load cray-python/3.6.1.1; source parsl_env/bin/activate"
     # },
     # 'cooley': {
```

### Comparing `parsl-2023.6.5/parsl/tests/conftest.py` & `parsl-2023.7.3/parsl/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         elif hasattr(module, 'fresh_config'):
             dfk = parsl.load(module.fresh_config())
         else:
             raise RuntimeError("Config module does not define config or fresh_config")
 
         yield
 
-        if(parsl.dfk() != dfk):
+        if parsl.dfk() != dfk:
             raise RuntimeError("DFK changed unexpectedly during test")
         dfk.cleanup()
         parsl.clear()
     else:
         yield
 
 
@@ -154,24 +154,24 @@
 
         if local_config:
             assert callable(local_config)
             c = local_config()
             assert isinstance(c, parsl.Config)
             dfk = parsl.load(c)
 
-        if(callable(local_setup)):
+        if callable(local_setup):
             local_setup()
 
         yield
 
-        if(callable(local_teardown)):
+        if callable(local_teardown):
             local_teardown()
 
-        if(local_config):
-            if(parsl.dfk() != dfk):
+        if local_config:
+            if parsl.dfk() != dfk:
                 raise RuntimeError("DFK changed unexpectedly during test")
             dfk.cleanup()
             parsl.clear()
 
     else:
         yield
 
@@ -207,24 +207,24 @@
             else:
                 pytest.skip(m.args[0])
     else:  # is not marked as local
         if config == 'local':
             pytest.skip('intended for explicit config')
 
 
-@pytest.fixture()
-def setup_data():
-    import os
-    if not os.path.isdir('data'):
-        os.mkdir('data')
+@pytest.fixture
+def setup_data(tmp_path):
+    data_dir = tmp_path / "data"
+    data_dir.mkdir()
 
-    with open("data/test1.txt", 'w') as f:
+    with open(data_dir / "test1.txt", "w") as f:
         f.write("1\n")
-    with open("data/test2.txt", 'w') as f:
+    with open(data_dir / "test2.txt", "w") as f:
         f.write("2\n")
+    return data_dir
 
 
 @pytest.fixture(autouse=True, scope='function')
 def wait_for_task_completion(pytestconfig):
     """If we're in a config-file based mode, wait for task completion between
        each test. This will detect early on (by hanging) if particular test
        tasks are not finishing, rather than silently falling off the end of
@@ -267,11 +267,11 @@
 
 
 def pytest_ignore_collect(path):
     if 'integration' in path.strpath:
         return True
     elif 'manual_tests' in path.strpath:
         return True
-    elif 'workqueue_tests/test_scale' in path.strpath:
+    elif 'scaling_tests/test_scale' in path.strpath:
         return True
     else:
         return False
```

### Comparing `parsl-2023.6.5/parsl/tests/integration/latency.py` & `parsl-2023.7.3/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,18 +28,14 @@
         'midway': {
             'url': 'midway.rcc.uchicago.edu',
             'uname': 'yadunand'
         },
         'swift': {
             'url': 'swift.rcc.uchicago.edu',
             'uname': 'yadunand'
-        },
-        'cori': {
-            'url': 'cori.nersc.gov',
-            'uname': 'yadunand'
         }
     }
 
     for site in sites.values():
         out = connect_and_list(site['url'], site['uname'])
         print("Sitename :{0}  hostname:{1}".format(site['url'], out))
```

### Comparing `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,19 +31,10 @@
     '''
     url = 'login.osgconnect.net'
     uname = 'yadunand'
     out = connect_and_list(url, uname)
     print("Sitename :{0}  hostname:{1}".format(url, out))
 
 
-def test_cori():
-    ''' Test ssh connectivity to cori
-    '''
-    url = 'cori.nersc.gov'
-    uname = 'yadunand'
-    out = connect_and_list(url, uname)
-    print("Sitename :{0}  hostname:{1}".format(url, out))
-
-
 if __name__ == "__main__":
 
     pass
```

### Comparing `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/manual_tests/htex_local.py` & `parsl-2023.7.3/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/manual_tests/test_basic.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,29 +21,22 @@
 
 # Tested. Confirmed. ssh X Torque X AprunLauncher
 # from parsl.tests.configs.swan_ipp import config
 
 # Tested. Confirmed. ssh X Torque X AprunLauncher
 # from parsl.tests.configs.swan_ipp_multinode import config
 
-# Tested. Confirmed. ssh X Slurm X SingleNodeLauncher
-# from parsl.tests.configs.cori_ipp_single_node import config
-
-# Tested. Confirmed. ssh X Slurm X srun
-# from parsl.tests.configs.cori_ipp_multinode import config
-
 # from parsl.tests.configs.cooley_ssh_il_single_node import config
 
 # Tested. Confirmed. local X GridEngine X singleNode
 # from parsl.tests.configs.cc_in2p3_local_single_node import config
 
 # from parsl.tests.configs.comet_ipp_multinode import config
 
 # from parsl.tests.configs.htex_local import config
-# from parsl.tests.configs.exex_local import config
 parsl.set_stream_logger()
 
 # from htex_midway import config
 # from htex_swan import config
 
 
 from parsl.app.app import python_app  # , bash_app
```

### Comparing `parsl-2023.6.5/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/manual_tests/test_regression_220.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/site_tests/site_config_selector.py` & `parsl-2023.7.3/parsl/tests/site_tests/site_config_selector.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,14 @@
         config = fresh_config()
 
     elif 'summit' in socket.getfqdn():
         print("Loading Frontera config")
         from parsl.tests.configs.summit import fresh_config
         config = fresh_config()
 
-    elif 'cori' in hostname:
-        print("Loading Cori config")
-        from parsl.tests.configs.cori import fresh_config
-        config = fresh_config()
-
     elif 'comet' in hostname:
         print("Loading Comet config")
         from parsl.tests.configs.comet import fresh_config
         config = fresh_config()
 
     elif 'midway' in hostname:
         print("Loading Midway config")
```

### Comparing `parsl-2023.6.5/parsl/tests/site_tests/test_provider.py` & `parsl-2023.7.3/parsl/tests/site_tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/site_tests/test_site.py` & `parsl-2023.7.3/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/sites/test_affinity.py` & `parsl-2023.7.3/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/sites/test_concurrent.py` & `parsl-2023.7.3/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2023.7.3/parsl/tests/sites/test_dynamic_executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/sites/test_ec2.py` & `parsl-2023.7.3/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/sites/test_local_adhoc.py` & `parsl-2023.7.3/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/sites/test_start_method.py` & `parsl-2023.7.3/parsl/tests/sites/test_start_method.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/sites/test_worker_info.py` & `parsl-2023.7.3/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_aalst_patterns.py` & `parsl-2023.7.3/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_bash_apps/test_kwarg_storage.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_kwarg_storage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_bash_apps/test_multiline.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_multiline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_bash_apps/test_pipeline.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,25 +48,25 @@
     open("test0.txt", 'w').write('0\n')
 
     # Create the first entry in the dictionary holding the futures
     prev = File("test0.txt")
     futs = {}
     for i in range(1, depth):
         print("Launching {0} with {1}".format(i, prev))
-        assert(isinstance(prev, DataFuture) or isinstance(prev, File))
+        assert isinstance(prev, DataFuture) or isinstance(prev, File)
         output = File("test{0}.txt".format(i))
         fu = increment(inputs=[prev],  # Depend on the future from previous call
                        # Name the file to be created here
                        outputs=[output],
                        stdout="incr{0}.out".format(i),
                        stderr="incr{0}.err".format(i))
         [prev] = fu.outputs
         futs[i] = prev
         print(prev.filepath)
-        assert(isinstance(prev, DataFuture))
+        assert isinstance(prev, DataFuture)
 
     for key in futs:
         if key > 0:
             fu = futs[key]
             file = fu.result()
             filename = file.filepath
```

### Comparing `parsl-2023.6.5/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_callables.py` & `parsl-2023.7.3/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_channels/test_large_output.py` & `parsl-2023.7.3/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_data/test_file.py` & `parsl-2023.7.3/parsl/tests/test_data/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_data/test_file_staging.py` & `parsl-2023.7.3/parsl/tests/test_data/test_file_apps.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,60 @@
-import os
 import pytest
+
 from parsl.app.app import bash_app
 from parsl.data_provider.files import File
 
 
 @bash_app
-def cat(inputs=[], outputs=[], stdout=None, stderr=None):
-    infiles = ' '.join([i.filepath for i in inputs])
-    return """echo {i}
-    cat {i} &> {o}
-    """.format(i=infiles, o=outputs[0])
-
-
-@pytest.mark.usefixtures('setup_data')
-@pytest.mark.issue363
-def test_files():
-
-    if os.path.exists('cat_out.txt'):
-        os.remove('cat_out.txt')
-
-    fs = [File('data/' + f) for f in os.listdir('data')]
-    x = cat(inputs=fs, outputs=[File('cat_out.txt')],
-            stdout='f_app.out', stderr='f_app.err')
+def cat(inputs=(), outputs=(), stdout=None, stderr=None):
+    infiles = " ".join(i.filepath for i in inputs)
+    return f"cat {infiles} &> {outputs[0]}"
+
+
+@pytest.mark.staging_required
+def test_files(setup_data):
+    fs = sorted(str(setup_data / f) for f in setup_data.iterdir())
+    fs = list(map(File, fs))
+    x = cat(
+        inputs=fs,
+        outputs=[File(str(setup_data / "cat_out.txt"))],
+        stdout=str(setup_data / "f_app.out"),
+        stderr=str(setup_data / "f_app.err"),
+    )
+    x.result()
     d_x = x.outputs[0]
-    print(x.result())
-    print(d_x, type(d_x))
+    data = open(d_x.filepath).read().strip()
+    assert "1\n2" == data, "Per setup_data fixture"
 
 
 @bash_app
-def increment(inputs=[], outputs=[], stdout=None, stderr=None):
+def increment(inputs=(), outputs=(), stdout=None, stderr=None):
     # Place double braces to avoid python complaining about missing keys for {item = $1}
     return """
     x=$(cat {i})
     echo $(($x+1)) > {o}
     """.format(i=inputs[0], o=outputs[0])
 
 
 @pytest.mark.staging_required
-def test_regression_200():
-    """Regression test for #200. Pickleablility of Files"""
-
-    if os.path.exists('test_output.txt'):
-        os.remove('test_output.txt')
-
-    with open("test.txt", 'w') as f:
-        f.write("Hello World")
-
-    fu = cat(inputs=[File("test.txt")],
-             outputs=[File("test_output.txt")])
-    fu.result()
-
-    fi = fu.outputs[0].result()
-    print("type of fi: {}".format(type(fi)))
-    with open(str(fi), 'r') as f:
-        data = f.readlines()
-        assert "Hello World" in data, "Missed data"
-
-
-@pytest.mark.staging_required
-def test_increment(depth=5):
+def test_increment(tmp_path, depth=5):
     """Test simple pipeline A->B...->N
     """
-    # Create the first file
-    open("test0.txt", 'w').write('0\n')
+    # Test setup
+    first_fpath = tmp_path / "test0.txt"
+    first_fpath.write_text("0\n")
 
-    # Create the first entry in the dictionary holding the futures
-    prev = File("test0.txt")
-    futs = {}
+    prev = [File(str(first_fpath))]
+    futs = []
     for i in range(1, depth):
-        if os.path.exists('test{0}.txt'.format(i)):
-            os.remove('test{0}.txt'.format(i))
-        print("Launching {0} with {1}".format(i, prev))
-        fu = increment(inputs=[prev],  # Depend on the future from previous call
-                       # Name the file to be created here
-                       outputs=[File("test{0}.txt".format(i))],
-                       stdout="incr{0}.out".format(i),
-                       stderr="incr{0}.err".format(i))
-        [prev] = fu.outputs
-        futs[i] = prev
-        print(prev.filepath)
-
-    for key in futs:
-        if key > 0:
-            fu = futs[key]
-            data = open(fu.result().filepath, 'r').read().strip()
-            assert data == str(
-                key), "[TEST] incr failed for key:{0} got:{1}".format(key, data)
+        f = increment(
+            inputs=prev,
+            outputs=[File(str(tmp_path / f"test{i}.txt"))],
+            stdout=str(tmp_path / f"incr{i}.out"),
+            stderr=str(tmp_path / f"incr{i}.err"),
+        )
+        prev = f.outputs
+        futs.append((i, prev[0]))
+
+    for i, f in futs:
+        data = open(f.result().filepath).read().strip()
+        assert data == str(i)
```

### Comparing `parsl-2023.6.5/parsl/tests/test_data/test_output_chain_filenames.py` & `parsl-2023.7.3/parsl/tests/test_data/test_output_chain_filenames.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_docs/test_from_slides.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_docs/test_workflow1.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_docs/test_workflow2.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_docs/test_workflow3.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_docs/test_workflow4.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_missing_worker.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_worker_failure.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_worker_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_error_handling/test_retries.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,8 +57,8 @@
     except OSError:
         pass
     fu = succeed_on_retry(fname, success_on=5)
 
     with pytest.raises(parsl.app.errors.BashExitFailure):
         fu.result()
 
-    assert(fu.exception().exitcode == 5)
+    assert fu.exception().exitcode == 5
```

### Comparing `parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_flux.py` & `parsl-2023.7.3/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_monitoring/test_basic.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_monitoring/test_viz_colouring.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_viz_colouring.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_providers/test_local_provider.py` & `parsl-2023.7.3/parsl/tests/test_providers/test_local_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_fail.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_futures.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_futures.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,125 +7,81 @@
 
 Same applies to datafutures, and we need to know the behavior wrt.
 
 1. result() called on 1, vs 2
 2. done() called on 1, vs 2
 
 """
-import argparse
-import os
 import pytest
+from os.path import basename
 
-import parsl
 from parsl.app.app import python_app
 from parsl.data_provider.files import File
-from parsl.tests.configs.local_threads import config
 
 
 @python_app
-def delay_incr(x, delay=0, outputs=[]):
+def delay_incr(x, delay=0.0, outputs=()):
     import time
     if outputs:
         with open(outputs[0].filepath, 'w') as outs:
             outs.write(str(x + 1))
     time.sleep(delay)
     return x + 1
 
 
 def get_contents(filename):
-    c = None
     with open(filename, 'r') as f:
-        c = f.read()
-    return c
+        return f.read()
 
 
 def test_fut_case_1():
     """Testing the behavior of AppFutures where there are no dependencies
     """
 
-    app_fu = delay_incr(1, delay=0.5)
-
-    status = app_fu.done()
-    result = app_fu.result()
-
-    print("Status : ", status)
-    print("Result : ", result)
-
-    assert result == 2, 'Output does not match expected 2, goot: "{0}"'.format(
-        result)
-    return True
+    app_fu = delay_incr(1, delay=0.01)
+    assert app_fu.result() == 2
 
 
 @pytest.mark.staging_required
-def test_fut_case_2():
+def test_fut_case_2(tmp_path):
     """Testing the behavior of DataFutures where there are no dependencies
     """
-    output_f = 'test_fut_case_2.txt'
-    app_fu = delay_incr(1, delay=10, outputs=[File(output_f)])
+    output_f = tmp_path / 'test_fut_case_2.txt'
+    app_fu = delay_incr(1, delay=0.01, outputs=[File(str(output_f))])
     data_fu = app_fu.outputs[0]
 
-    data_fu.done()
     result = data_fu.result().filepath
-    print("App_fu  : ", app_fu)
-    print("Data_fu : ", data_fu)
-
-    assert os.path.basename(result) == output_f, \
-        "DataFuture did not return the filename, got : {0}".format(result)
-    print("Status : ", data_fu.done())
-    print("Result : ", result)
+    assert basename(result) == output_f.name, "DataFuture did not return filename"
 
     contents = get_contents(result)
-    assert contents == '2', 'Output does not match expected "2", got: "{0}"'.format(
-        contents)
-    return True
+    assert contents == '2'
 
 
 def test_fut_case_3():
     """Testing the behavior of AppFutures where there are dependencies
 
-    The first call has a delay of 0.5s, and the second call depends on the first
+    The first call has a delay, and the second call depends on the first
     """
 
-    app_1 = delay_incr(1, delay=0.5)
+    app_1 = delay_incr(1, delay=0.01)
     app_2 = delay_incr(app_1)
 
-    status = app_2.done()
-    result = app_2.result()
-
-    print("Status : ", status)
-    print("Result : ", result)
-
-    assert result == 3, 'Output does not match expected 2, goot: "{0}"'.format(
-        result)
-    return True
+    assert app_2.result() == 3
 
 
 @pytest.mark.staging_required
-def test_fut_case_4():
+def test_fut_case_4(tmp_path):
     """Testing the behavior of DataFutures where there are dependencies
 
-    The first call has a delay of 0.5s, and the second call depends on the first
-    """
-    """Testing the behavior of DataFutures where there are no dependencies
+    The first call has a delay, and the second call depends on the first
     """
-    output_f1 = 'test_fut_case_4_f1.txt'
-    output_f2 = 'test_fut_case_4_f2.txt'
-    app_1 = delay_incr(1, delay=0.5, outputs=[File(output_f1)])
-    app_1.outputs[0]
-    app_2 = delay_incr(app_1, delay=0.5, outputs=[File(output_f2)])
+    output_f1 = tmp_path / 'test_fut_case_4_f1.txt'
+    output_f2 = tmp_path / 'test_fut_case_4_f2.txt'
+    app_1 = delay_incr(1, delay=0.01, outputs=[File(str(output_f1))])
+    app_2 = delay_incr(app_1, delay=0.01, outputs=[File(str(output_f2))])
     data_2 = app_2.outputs[0]
 
-    status = data_2.done()
     result = data_2.result().filepath
-    print("App_fu  : ", app_2)
-    print("Data_fu : ", data_2)
-
-    print("Status : ", status)
-    print("Result : ", result)
-
-    assert os.path.basename(result) == output_f2, \
-        "DataFuture did not return the filename, got : {0}".format(result)
+    assert basename(result) == output_f2.name, "DataFuture did not return the filename"
 
     contents = get_contents(result)
-    assert contents == '3', 'Output does not match expected "3", got: "{0}"'.format(
-        result)
-    return True
+    assert contents == '3'
```

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_join.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_join.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_mapred.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_mapred.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_outputs.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_outputs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_overview.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_overview.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_python_apps/test_simple.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_regression/test_1480.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_regression/test_1653.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_regression/test_221.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_regression/test_226.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_regression/test_2652.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_2652.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_regression/test_69a.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_regression/test_69b.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_69b.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_regression/test_854.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_regression/test_97_parallelism_0.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_97_parallelism_0.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_scaling/test_regression_1621.py` & `parsl-2023.7.3/parsl/tests/test_scaling/test_regression_1621.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2023.7.3/parsl/tests/test_scaling/test_scale_down.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_staging/staging_provider.py` & `parsl-2023.7.3/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_staging/test_1316.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_staging/test_docs_1.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_staging/test_staging_https.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_staging/test_staging_https_in_task.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_https_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_summary.py` & `parsl-2023.7.3/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_thread_parallelism.py` & `parsl-2023.7.3/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_threads/test_configs.py` & `parsl-2023.7.3/parsl/tests/test_threads/test_configs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2023.7.3/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/workqueue_tests/htex_local.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/workqueue_tests/test_scale.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/test_scale.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 import argparse
 import time
 
 import parsl
 
 # from parsl.tests.configs.htex_local import config
 # from htex_local import config
-# from exex_local import config
 # from parsl.configs.local_threads import config
 # from parsl.configs.local_ipp import config
-# from parsl.tests.configs.exex_local import config
 
 # parsl.set_stream_logger()
 # config.executors[0].provider.tasks_per_node = 4
 # parsl.load(config)
 from parsl.app.app import python_app  # , bash_app
```

### Comparing `parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_condor.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_local.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/usage_tracking/usage.py` & `parsl-2023.7.3/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/parsl/utils.py` & `parsl-2023.7.3/parsl/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import inspect
 import logging
 import os
 import shlex
 import subprocess
 import threading
 import time
+from types import TracebackType
+
 import typeguard
 from contextlib import contextmanager
 from typing import Any, Callable, List, Tuple, Union, Generator, IO, AnyStr, Dict, Optional
 
+from typing_extensions import Type
+
 import parsl
 from parsl.version import VERSION
 
 
 try:
     import setproctitle as setproctitle_module
 except ImportError:
@@ -51,15 +55,15 @@
        - rundir(str) : Path to the runinfo directory
 
     Returns:
        - a list suitable for the checkpoint_files parameter of `Config`
 
     """
 
-    if(not os.path.isdir(rundir)):
+    if not os.path.isdir(rundir):
         return []
 
     dirs = sorted(os.listdir(rundir))
 
     checkpoints = []
 
     for runid in dirs:
@@ -95,15 +99,15 @@
 
     if len(dirs) == 0:
         return []
 
     last_runid = dirs[-1]
     last_checkpoint = os.path.abspath(f'{rundir}/{last_runid}/checkpoint')
 
-    if(not(os.path.isdir(last_checkpoint))):
+    if not os.path.isdir(last_checkpoint):
         return []
 
     return [last_checkpoint]
 
 
 @typeguard.typechecked
 def get_std_fname_mode(fdname: str, stdfspec: Union[str, Tuple[str, str]]) -> Tuple[str, str]:
@@ -343,7 +347,32 @@
             logger.error("Callback threw an exception - logging and proceeding anyway", exc_info=True)
 
     def close(self) -> None:
         """Merge the threads and terminate.
         """
         self._kill_event.set()
         self._thread.join()
+
+
+class AutoCancelTimer(threading.Timer):
+    """
+    Extend threading.Timer for use as a context manager
+
+    Example:
+
+        with AutoCancelTimer(delay, your_callback):
+            some_func()
+
+    If `some_func()` returns before the delay is up, the timer will
+    be cancelled.
+    """
+    def __enter__(self) -> "AutoCancelTimer":
+        self.start()
+        return self
+
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        exc_tb: Optional[TracebackType]
+    ) -> None:
+        self.cancel()
```

### Comparing `parsl-2023.6.5/parsl.egg-info/PKG-INFO` & `parsl-2023.7.3/parsl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.6.5
+Version: 2023.7.3
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.06.05.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.07.03.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7.0
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8.0
 Provides-Extra: monitoring
 Provides-Extra: aws
 Provides-Extra: kubernetes
 Provides-Extra: oauth_ssh
 Provides-Extra: docs
 Provides-Extra: google_cloud
 Provides-Extra: gssapi
```

### Comparing `parsl-2023.6.5/parsl.egg-info/SOURCES.txt` & `parsl-2023.7.3/parsl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,29 +44,28 @@
 parsl/configs/__init__.py
 parsl/configs/ad_hoc.py
 parsl/configs/bluewaters.py
 parsl/configs/bridges.py
 parsl/configs/cc_in2p3.py
 parsl/configs/comet.py
 parsl/configs/cooley.py
-parsl/configs/cori.py
 parsl/configs/ec2.py
-parsl/configs/exex_local.py
 parsl/configs/frontera.py
 parsl/configs/htex_local.py
 parsl/configs/illinoiscluster.py
 parsl/configs/kubernetes.py
 parsl/configs/local_threads.py
 parsl/configs/midway.py
 parsl/configs/osg.py
 parsl/configs/polaris.py
 parsl/configs/stampede2.py
 parsl/configs/summit.py
 parsl/configs/theta.py
 parsl/configs/toss3_llnl.py
+parsl/configs/vineex_local.py
 parsl/configs/wqex_local.py
 parsl/data_provider/__init__.py
 parsl/data_provider/data_manager.py
 parsl/data_provider/file_noop.py
 parsl/data_provider/files.py
 parsl/data_provider/ftp.py
 parsl/data_provider/globus.py
@@ -85,39 +84,40 @@
 parsl/dataflow/states.py
 parsl/dataflow/strategy.py
 parsl/dataflow/taskrecord.py
 parsl/executors/__init__.py
 parsl/executors/base.py
 parsl/executors/errors.py
 parsl/executors/status_handling.py
-parsl/executors/swift_t.py
 parsl/executors/threads.py
-parsl/executors/extreme_scale/__init__.py
-parsl/executors/extreme_scale/executor.py
-parsl/executors/extreme_scale/mpi_worker_pool.py
 parsl/executors/flux/__init__.py
 parsl/executors/flux/execute_parsl_task.py
 parsl/executors/flux/executor.py
 parsl/executors/flux/flux_instance_manager.py
 parsl/executors/high_throughput/__init__.py
 parsl/executors/high_throughput/errors.py
 parsl/executors/high_throughput/executor.py
 parsl/executors/high_throughput/interchange.py
 parsl/executors/high_throughput/manager_record.py
 parsl/executors/high_throughput/monitoring_info.py
 parsl/executors/high_throughput/probe.py
 parsl/executors/high_throughput/process_worker_pool.py
 parsl/executors/high_throughput/zmq_pipes.py
+parsl/executors/taskvine/__init__.py
+parsl/executors/taskvine/errors.py
+parsl/executors/taskvine/exec_parsl_function.py
+parsl/executors/taskvine/executor.py
 parsl/executors/workqueue/__init__.py
 parsl/executors/workqueue/errors.py
 parsl/executors/workqueue/exec_parsl_function.py
 parsl/executors/workqueue/executor.py
 parsl/executors/workqueue/parsl_coprocess.py
 parsl/executors/workqueue/parsl_coprocess_stub.py
 parsl/launchers/__init__.py
+parsl/launchers/base.py
 parsl/launchers/errors.py
 parsl/launchers/launchers.py
 parsl/monitoring/__init__.py
 parsl/monitoring/db_manager.py
 parsl/monitoring/message_type.py
 parsl/monitoring/monitoring.py
 parsl/monitoring/radios.py
@@ -193,29 +193,26 @@
 parsl/tests/__init__.py
 parsl/tests/callables_helper.py
 parsl/tests/conftest.py
 parsl/tests/test_aalst_patterns.py
 parsl/tests/test_callables.py
 parsl/tests/test_flux.py
 parsl/tests/test_summary.py
-parsl/tests/test_swift.py
 parsl/tests/test_thread_parallelism.py
 parsl/tests/utils.py
 parsl/tests/configs/__init__.py
 parsl/tests/configs/ad_hoc_cluster_htex.py
 parsl/tests/configs/azure_single_node.py
 parsl/tests/configs/bluewaters.py
 parsl/tests/configs/bridges.py
 parsl/tests/configs/cc_in2p3.py
 parsl/tests/configs/comet.py
 parsl/tests/configs/cooley_htex.py
-parsl/tests/configs/cori.py
 parsl/tests/configs/ec2_single_node.py
 parsl/tests/configs/ec2_spot.py
-parsl/tests/configs/exex_local.py
 parsl/tests/configs/frontera.py
 parsl/tests/configs/htex_ad_hoc_cluster.py
 parsl/tests/configs/htex_local.py
 parsl/tests/configs/htex_local_alternate.py
 parsl/tests/configs/htex_local_intask_staging.py
 parsl/tests/configs/htex_local_rsync_staging.py
 parsl/tests/configs/local_adhoc.py
@@ -231,17 +228,17 @@
 parsl/tests/configs/local_threads_no_cache.py
 parsl/tests/configs/midway.py
 parsl/tests/configs/nscc_singapore.py
 parsl/tests/configs/osg_htex.py
 parsl/tests/configs/petrelkube.py
 parsl/tests/configs/summit.py
 parsl/tests/configs/swan_htex.py
+parsl/tests/configs/taskvine_ex.py
 parsl/tests/configs/theta.py
 parsl/tests/configs/user_opts.py
-parsl/tests/configs/workqueue_blocks.py
 parsl/tests/configs/workqueue_ex.py
 parsl/tests/integration/__init__.py
 parsl/tests/integration/latency.py
 parsl/tests/integration/test_parsl_load_default_config.py
 parsl/tests/integration/test_apps/__init__.py
 parsl/tests/integration/test_channels/__init__.py
 parsl/tests/integration/test_channels/test_channels.py
@@ -261,14 +258,22 @@
 parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
 parsl/tests/manual_tests/test_log_filter.py
 parsl/tests/manual_tests/test_memory_limits.py
 parsl/tests/manual_tests/test_oauth_ssh.py
 parsl/tests/manual_tests/test_regression_220.py
 parsl/tests/manual_tests/test_udp_simple.py
 parsl/tests/manual_tests/test_worker_count.py
+parsl/tests/scaling_tests/__init__.py
+parsl/tests/scaling_tests/htex_local.py
+parsl/tests/scaling_tests/local_threads.py
+parsl/tests/scaling_tests/test_scale.py
+parsl/tests/scaling_tests/vineex_condor.py
+parsl/tests/scaling_tests/vineex_local.py
+parsl/tests/scaling_tests/wqex_condor.py
+parsl/tests/scaling_tests/wqex_local.py
 parsl/tests/site_tests/__init__.py
 parsl/tests/site_tests/site_config_selector.py
 parsl/tests/site_tests/test_provider.py
 parsl/tests/site_tests/test_site.py
 parsl/tests/sites/__init__.py
 parsl/tests/sites/test_affinity.py
 parsl/tests/sites/test_concurrent.py
@@ -334,15 +339,14 @@
 parsl/tests/test_monitoring/test_fuzz_zmq.py
 parsl/tests/test_monitoring/test_memoization_representation.py
 parsl/tests/test_monitoring/test_viz_colouring.py
 parsl/tests/test_providers/__init__.py
 parsl/tests/test_providers/test_local_provider.py
 parsl/tests/test_python_apps/__init__.py
 parsl/tests/test_python_apps/test_arg_input_types.py
-parsl/tests/test_python_apps/test_at_scale.py
 parsl/tests/test_python_apps/test_basic.py
 parsl/tests/test_python_apps/test_dep_standard_futures.py
 parsl/tests/test_python_apps/test_dependencies.py
 parsl/tests/test_python_apps/test_depfail_propagation.py
 parsl/tests/test_python_apps/test_fail.py
 parsl/tests/test_python_apps/test_fibonacci_iterative.py
 parsl/tests/test_python_apps/test_fibonacci_recursive.py
@@ -357,16 +361,16 @@
 parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
 parsl/tests/test_python_apps/test_memoize_ignore_args.py
 parsl/tests/test_python_apps/test_memoize_joinapp.py
 parsl/tests/test_python_apps/test_outputs.py
 parsl/tests/test_python_apps/test_overview.py
 parsl/tests/test_python_apps/test_pipeline.py
 parsl/tests/test_python_apps/test_simple.py
+parsl/tests/test_python_apps/test_timeout.py
 parsl/tests/test_python_apps/test_type5.py
-parsl/tests/test_python_apps/test_worker_fail.py
 parsl/tests/test_regression/__init__.py
 parsl/tests/test_regression/test_1480.py
 parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
 parsl/tests/test_regression/test_1653.py
 parsl/tests/test_regression/test_221.py
 parsl/tests/test_regression/test_226.py
 parsl/tests/test_regression/test_2652.py
@@ -374,29 +378,25 @@
 parsl/tests/test_regression/test_69b.py
 parsl/tests/test_regression/test_854.py
 parsl/tests/test_regression/test_97_parallelism_0.py
 parsl/tests/test_regression/test_98.py
 parsl/tests/test_scaling/__init__.py
 parsl/tests/test_scaling/test_regression_1621.py
 parsl/tests/test_scaling/test_scale_down.py
+parsl/tests/test_serialization/__init__.py
+parsl/tests/test_serialization/test_basic.py
 parsl/tests/test_staging/__init__.py
 parsl/tests/test_staging/staging_provider.py
 parsl/tests/test_staging/test_1316.py
 parsl/tests/test_staging/test_docs_1.py
 parsl/tests/test_staging/test_docs_2.py
 parsl/tests/test_staging/test_elaborate_noop_file.py
 parsl/tests/test_staging/test_staging_ftp.py
 parsl/tests/test_staging/test_staging_ftp_in_task.py
 parsl/tests/test_staging/test_staging_globus.py
 parsl/tests/test_staging/test_staging_https.py
 parsl/tests/test_staging/test_staging_https_in_task.py
 parsl/tests/test_threads/__init__.py
 parsl/tests/test_threads/test_configs.py
 parsl/tests/test_threads/test_lazy_errors.py
-parsl/tests/workqueue_tests/__init__.py
-parsl/tests/workqueue_tests/htex_local.py
-parsl/tests/workqueue_tests/local_threads.py
-parsl/tests/workqueue_tests/test_scale.py
-parsl/tests/workqueue_tests/wqex_condor.py
-parsl/tests/workqueue_tests/wqex_local.py
 parsl/usage_tracking/__init__.py
 parsl/usage_tracking/usage.py
```

### Comparing `parsl-2023.6.5/parsl.egg-info/requires.txt` & `parsl-2023.7.3/parsl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.5/setup.py` & `parsl-2023.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     author='The Parsl Team',
     author_email='parsl@googlegroups.com',
     license='Apache 2.0',
     download_url='https://github.com/Parsl/parsl/archive/{}.tar.gz'.format(VERSION),
     include_package_data=True,
     package_data={'parsl': ['py.typed']},
     packages=find_packages(),
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     install_requires=install_requires,
     scripts = ['parsl/executors/high_throughput/process_worker_pool.py',
                'parsl/executors/workqueue/exec_parsl_function.py',
                'parsl/executors/workqueue/parsl_coprocess.py',
     ],
 
     extras_require=extras_require,
@@ -56,18 +56,18 @@
         # Maturity
         'Development Status :: 5 - Production/Stable',
         # Intended audience
         'Intended Audience :: Developers',
         # Licence, must match with licence above
         'License :: OSI Approved :: Apache Software License',
         # Python versions supported
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords=['Workflows', 'Scientific computing'],
     entry_points={'console_scripts':
       [
        'parsl-globus-auth=parsl.data_provider.globus:cli_run',
        'parsl-visualize=parsl.monitoring.visualization.app:cli_run',
        'parsl-perf=parsl.benchmark.perf:cli_run',
```

