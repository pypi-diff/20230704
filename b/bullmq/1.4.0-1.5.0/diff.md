# Comparing `tmp/bullmq-1.4.0.tar.gz` & `tmp/bullmq-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-1.4.0.tar", last modified: Fri Jun 30 22:04:10 2023, max compression
+gzip compressed data, was "bullmq-1.5.0.tar", last modified: Tue Jul  4 17:28:42 2023, max compression
```

## Comparing `bullmq-1.4.0.tar` & `bullmq-1.5.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:10.588881 bullmq-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-30 22:04:10.588881 bullmq-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-30 22:02:38.000000 bullmq-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:10.576881 bullmq-1.4.0/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-30 22:04:08.000000 bullmq-1.4.0/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:10.584881 bullmq-1.4.0/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/addJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/changePriority-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveToActive-10.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveToFinished-13.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/pause-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/promote-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/retryJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:10.584881 bullmq-1.4.0/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:10.576881 bullmq-1.4.0/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-30 22:04:10.000000 bullmq-1.4.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-30 22:04:10.000000 bullmq-1.4.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:04:10.000000 bullmq-1.4.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 22:04:10.000000 bullmq-1.4.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:04:10.000000 bullmq-1.4.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-30 22:04:08.000000 bullmq-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:04:10.588881 bullmq-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-30 22:02:38.000000 bullmq-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:42.833291 bullmq-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-04 17:28:42.833291 bullmq-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-04 17:27:35.000000 bullmq-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:42.825291 bullmq-1.5.0/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-04 17:28:40.000000 bullmq-1.5.0/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:42.829291 bullmq-1.5.0/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/addJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/changePriority-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveToActive-10.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveToFinished-13.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/pause-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/promote-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/retryJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:42.829291 bullmq-1.5.0/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:42.825291 bullmq-1.5.0/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-04 17:28:42.000000 bullmq-1.5.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-04 17:28:42.000000 bullmq-1.5.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:28:42.000000 bullmq-1.5.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 17:28:42.000000 bullmq-1.5.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 17:28:42.000000 bullmq-1.5.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-04 17:28:40.000000 bullmq-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:28:42.833291 bullmq-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 17:27:35.000000 bullmq-1.5.0/setup.py
```

### Comparing `bullmq-1.4.0/PKG-INFO` & `bullmq-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.4.0
+Version: 1.5.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.4.0/README.md` & `bullmq-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/backoffs.py` & `bullmq-1.5.0/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/addJob-9.lua` & `bullmq-1.5.0/bullmq/commands/addJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/changeDelay-3.lua` & `bullmq-1.5.0/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/changePriority-5.lua` & `bullmq-1.5.0/bullmq/commands/changePriority-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-1.5.0/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/drain-4.lua` & `bullmq-1.5.0/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/getCounts-1.lua` & `bullmq-1.5.0/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/getRanges-1.lua` & `bullmq-1.5.0/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/getState-8.lua` & `bullmq-1.5.0/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/getStateV2-8.lua` & `bullmq-1.5.0/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/isFinished-3.lua` & `bullmq-1.5.0/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-1.5.0/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-1.5.0/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/moveToActive-10.lua` & `bullmq-1.5.0/bullmq/commands/moveToActive-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/moveToDelayed-8.lua` & `bullmq-1.5.0/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/moveToFinished-13.lua` & `bullmq-1.5.0/bullmq/commands/moveToFinished-13.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-1.5.0/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/obliterate-2.lua` & `bullmq-1.5.0/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/pause-5.lua` & `bullmq-1.5.0/bullmq/commands/pause-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/promote-7.lua` & `bullmq-1.5.0/bullmq/commands/promote-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/removeJob-1.lua` & `bullmq-1.5.0/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/removeRepeatable-2.lua` & `bullmq-1.5.0/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/reprocessJob-6.lua` & `bullmq-1.5.0/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/retryJob-9.lua` & `bullmq-1.5.0/bullmq/commands/retryJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/commands/retryJobs-6.lua` & `bullmq-1.5.0/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/event_emitter.py` & `bullmq-1.5.0/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/job.py` & `bullmq-1.5.0/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/queue.py` & `bullmq-1.5.0/bullmq/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         """
         return self.scripts.pause(False)
 
     async def isPaused(self):
         """
         Returns true if the queue is currently paused.
         """
-        paused_key_exists = await self.client.hexists(self.opts.get("prefix", f"bull:{self.name}:meta"), "paused")
+        paused_key_exists = await self.client.hexists(f"{self.prefix}:{self.name}:meta", "paused")
         return paused_key_exists == 1
 
     async def obliterate(self, force: bool = False):
         """
         Completely destroys the queue and all of its contents irreversibly.
         This method will the *pause* the queue and requires that there are no
         active jobs. It is possible to bypass this requirement, i.e. not
```

### Comparing `bullmq-1.4.0/bullmq/redis_connection.py` & `bullmq-1.5.0/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/scripts.py` & `bullmq-1.5.0/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/timer.py` & `bullmq-1.5.0/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/types/job_options.py` & `bullmq-1.5.0/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/types/worker_options.py` & `bullmq-1.5.0/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq/worker.py` & `bullmq-1.5.0/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/bullmq.egg-info/PKG-INFO` & `bullmq-1.5.0/bullmq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.4.0
+Version: 1.5.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.4.0/bullmq.egg-info/SOURCES.txt` & `bullmq-1.5.0/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-1.4.0/pyproject.toml` & `bullmq-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "1.4.0"
+version = "1.5.0"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
 classifiers=[
     'Development Status :: 3 - Alpha',
@@ -28,15 +28,15 @@
 
 [project.optional-dependencies]
 dev = [
     "setuptools==63.1.0",
     "pre-commit==3.3.3",
     "build==0.8.0",
     "python-semantic-release==7.28.1",
-    "types-redis==4.5.5.0"
+    "types-redis==4.6.0.1"
 ]
 
 [project.urls]
 "Homepage" = "https://bullmq.io"
 "Bug Tracker" = "https://github.com/taskforcesh/bullmq/issues"
 
 [tool.setuptools.packages.find]
```

