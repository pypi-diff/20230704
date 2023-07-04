# Comparing `tmp/yojenkins-0.0.85.tar.gz` & `tmp/yojenkins-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yojenkins-0.0.85.tar", last modified: Mon Mar  6 23:47:01 2023, max compression
+gzip compressed data, was "yojenkins-0.0.86.tar", last modified: Tue Jul  4 04:33:50 2023, max compression
```

## Comparing `yojenkins-0.0.85.tar` & `yojenkins-0.0.86.tar`

### file list

```diff
@@ -1,107 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.928755 yojenkins-0.0.85/
--rw-r--r--   0 runner    (1001) docker     (123)    35144 2023-03-06 23:46:38.000000 yojenkins-0.0.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-06 23:46:38.000000 yojenkins-0.0.85/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-03-06 23:47:01.928755 yojenkins-0.0.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-06 23:46:38.000000 yojenkins-0.0.85/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    89388 2023-03-06 23:46:38.000000 yojenkins-0.0.85/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-06 23:46:38.000000 yojenkins-0.0.85/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-06 23:46:38.000000 yojenkins-0.0.85/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 23:47:01.928755 yojenkins-0.0.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-03-06 23:46:38.000000 yojenkins-0.0.85/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.920755 yojenkins-0.0.85/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-06 23:46:38.000000 yojenkins-0.0.85/tests/test_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.920755 yojenkins-0.0.85/yojenkins/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.920755 yojenkins-0.0.85/yojenkins/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/cli_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli/logger_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.924755 yojenkins-0.0.85/yojenkins/cli_sub_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/cli_sub_commands/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.924755 yojenkins-0.0.85/yojenkins/docker_container/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/docker_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/docker_container/docker_jenkins_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.924755 yojenkins-0.0.85/yojenkins/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23914 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/monitor/build_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/monitor/folder_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/monitor/job_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/monitor/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/monitor/monitor_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.916755 yojenkins-0.0.85/yojenkins/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.924755 yojenkins-0.0.85/yojenkins/resources/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2542 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/scripts/node_prepare_amazonlinux2.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.924755 yojenkins-0.0.85/yojenkins/resources/server_docker_settings/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/server_docker_settings/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/server_docker_settings/config_as_code.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/server_docker_settings/dummy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/server_docker_settings/plugins.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.924755 yojenkins-0.0.85/yojenkins/resources/sound/
--rw-r--r--   0 runner    (1001) docker     (123)   144342 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/sound/negative_alert_wooden_mallet_fast_negative_error_two_tone.wav
--rw-r--r--   0 runner    (1001) docker     (123)   158062 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/sound/negative_notification_mallet_wooden_short_alert.wav
--rw-r--r--   0 runner    (1001) docker     (123)   305062 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/sound/negative_ui_ping_chime_mallet_like.wav
--rw-r--r--   0 runner    (1001) docker     (123)   361114 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/sound/negative_ui_ping_chime_mallet_like_error.wav
--rw-r--r--   0 runner    (1001) docker     (123)   274166 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/sound/positive_alert_mallet_wood_simple_musical_003.wav
--rw-r--r--   0 runner    (1001) docker     (123)   299558 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/resources/sound/positive_alert_notification_musical_short_marimba_process_finished.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.928755 yojenkins-0.0.85/yojenkins/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/tools/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/tools/shared_library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.928755 yojenkins-0.0.85/yojenkins/utility/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46910 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/utility/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.928755 yojenkins-0.0.85/yojenkins/yo_jenkins/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    32431 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    32608 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    21044 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.928755 yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/user_create.groovy
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/user_delete.groovy
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/user_list.groovy
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/user_permission_add_remove.groovy
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/user_permission_list.groovy
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/jenkins_item_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/jenkins_item_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/jenkins_item_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    30233 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-03-06 23:46:38.000000 yojenkins-0.0.85/yojenkins/yo_jenkins/yojenkins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 23:47:01.920755 yojenkins-0.0.85/yojenkins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-03-06 23:47:01.000000 yojenkins-0.0.85/yojenkins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-03-06 23:47:01.000000 yojenkins-0.0.85/yojenkins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 23:47:01.000000 yojenkins-0.0.85/yojenkins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-06 23:47:01.000000 yojenkins-0.0.85/yojenkins.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-06 23:47:01.000000 yojenkins-0.0.85/yojenkins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-06 23:47:01.000000 yojenkins-0.0.85/yojenkins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.286600 yojenkins-0.0.86/
+-rw-r--r--   0 runner    (1001) docker     (123)    35144 2023-07-04 04:33:23.000000 yojenkins-0.0.86/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-04 04:33:23.000000 yojenkins-0.0.86/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-04 04:33:50.286600 yojenkins-0.0.86/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-04 04:33:23.000000 yojenkins-0.0.86/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    87211 2023-07-04 04:33:23.000000 yojenkins-0.0.86/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 04:33:23.000000 yojenkins-0.0.86/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-04 04:33:23.000000 yojenkins-0.0.86/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 04:33:50.286600 yojenkins-0.0.86/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-04 04:33:23.000000 yojenkins-0.0.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.274600 yojenkins-0.0.86/yojenkins/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.278600 yojenkins-0.0.86/yojenkins/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/cli_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli/logger_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.278600 yojenkins-0.0.86/yojenkins/cli_sub_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/cli_sub_commands/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.278600 yojenkins-0.0.86/yojenkins/docker_container/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/docker_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/docker_container/docker_jenkins_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.282600 yojenkins-0.0.86/yojenkins/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23914 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/monitor/build_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/monitor/folder_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/monitor/job_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/monitor/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/monitor/monitor_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.274600 yojenkins-0.0.86/yojenkins/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.282600 yojenkins-0.0.86/yojenkins/resources/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2542 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/scripts/node_prepare_amazonlinux2.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.282600 yojenkins-0.0.86/yojenkins/resources/server_docker_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/server_docker_settings/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/server_docker_settings/config_as_code.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/server_docker_settings/dummy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/server_docker_settings/plugins.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.282600 yojenkins-0.0.86/yojenkins/resources/sound/
+-rw-r--r--   0 runner    (1001) docker     (123)   144342 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/sound/negative_alert_wooden_mallet_fast_negative_error_two_tone.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   158062 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/sound/negative_notification_mallet_wooden_short_alert.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   305062 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/sound/negative_ui_ping_chime_mallet_like.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   361114 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/sound/negative_ui_ping_chime_mallet_like_error.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   274166 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/sound/positive_alert_mallet_wood_simple_musical_003.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   299558 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/resources/sound/positive_alert_notification_musical_short_marimba_process_finished.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.282600 yojenkins-0.0.86/yojenkins/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/tools/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/tools/shared_library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.286600 yojenkins-0.0.86/yojenkins/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47022 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/utility/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.286600 yojenkins-0.0.86/yojenkins/yo_jenkins/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32431 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32608 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21044 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.286600 yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/user_create.groovy
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/user_delete.groovy
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/user_list.groovy
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/user_permission_add_remove.groovy
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/user_permission_list.groovy
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/jenkins_item_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/jenkins_item_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/jenkins_item_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30233 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-04 04:33:23.000000 yojenkins-0.0.86/yojenkins/yo_jenkins/yojenkins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:33:50.278600 yojenkins-0.0.86/yojenkins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-04 04:33:50.000000 yojenkins-0.0.86/yojenkins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-04 04:33:50.000000 yojenkins-0.0.86/yojenkins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:33:50.000000 yojenkins-0.0.86/yojenkins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-04 04:33:50.000000 yojenkins-0.0.86/yojenkins.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 04:33:50.000000 yojenkins-0.0.86/yojenkins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 04:33:50.000000 yojenkins-0.0.86/yojenkins.egg-info/top_level.txt
```

### Comparing `yojenkins-0.0.85/LICENSE` & `yojenkins-0.0.86/LICENSE`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/PKG-INFO` & `yojenkins-0.0.86/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yojenkins
-Version: 0.0.85
+Version: 0.0.86
 Summary: A CLI tool to manage and have fun with Jenkins server
 Home-page: https://github.com/ismet55555/yojenkins
 Author: Ismet Handzic
 Author-email: ismet.handzic@gmail.com
 Maintainer: Ismet Handzic
 Keywords: jenkins monitor manage job build fun
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yojenkins Version: 0.0.85 Summary: A CLI tool to
+Metadata-Version: 2.1 Name: yojenkins Version: 0.0.86 Summary: A CLI tool to
 manage and have fun with Jenkins server Home-page: https://github.com/
 ismet55555/yojenkins Author: Ismet Handzic Author-email:
 ismet.handzic@gmail.com Maintainer: Ismet Handzic Keywords: jenkins monitor
 manage job build fun Classifier: Development Status :: 3 - Alpha Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Intended Audience :: System Administrators Classifier:
 Intended Audience :: Developers Classifier: Topic :: Utilities Classifier:
```

### Comparing `yojenkins-0.0.85/Pipfile` & `yojenkins-0.0.86/Pipfile`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 pre-commit = "*"
 pyinstaller = "*"
 pylint = "*"
 pytest = "*"
 setuptools = "*"
 twine = "*"
 wheel = "*"
+yamllint = "*"
 yapf = "*"
 yojenkins = {editable = true, path = "."}
 
 [packages]
 click = "*"
 click-help-colors = "*"
 coloredlogs = "*"
```

### Comparing `yojenkins-0.0.85/Pipfile.lock` & `yojenkins-0.0.86/Pipfile.lock`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9529100529100528%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'10001318587fe4f14ae0e252c8d845f6a89cab9dbb25f1e077e4a90af062533b'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7', "*

 * *              "'sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716'], "*

 * *              "'version': '==2023.5.7'}, 'charset-normalizer': {'hashes': "*

 * *              "['sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6',  […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "4147848aa6495b0558b313fb1bc46b8e0afd878a295fec28acfd954ea68e29ee"
+            "sha256": "10001318587fe4f14ae0e252c8d845f6a89cab9dbb25f1e077e4a90af062533b"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3"
         },
         "sources": [
             {
@@ -14,113 +14,100 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_full_version >= '3.6.0'",
-            "version": "==3.0.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
@@ -156,19 +143,19 @@
                 "sha256:a352e7e428770286cc899e2542b6cdaedb2b4953ff269a210103ec58f6198a61"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.7.1"
         },
         "docker": {
             "hashes": [
-                "sha256:896c4282e5c7af5c45e8b683b0b0c33932974fe6e50fc6906a0a83616ab3da97",
-                "sha256:dbcb3bd2fa80dca0788ed908218bf43972772009b881ed1e20dfc29a65e49782"
+                "sha256:aa6d17830045ba5ef0168d5eaa34d37beeb113948c413affe1d5991fc11f9a20",
+                "sha256:aecd2277b8bf8e506e484f6ab7aec39abe0038e29fa4a6d3ba86c3fe01844ed9"
             ],
             "index": "pypi",
-            "version": "==6.0.1"
+            "version": "==6.1.3"
         },
         "humanfriendly": {
             "hashes": [
                 "sha256:1697e1a8a8f550fd43c2865cd84542fc175a61dcb779b6fee18cf6b6ccba1477",
                 "sha256:6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -197,19 +184,19 @@
                 "sha256:deebdec17aa30a1c432cb3f437e81f8621e1c0542a0c0617a74f71e232e9939e",
                 "sha256:fb67a532d7361a66820aa1e8fe6c0c939f4c34a3a09a3e8db199ce7b77c4fb78"
             ],
             "version": "==2.0.3"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pbr": {
             "hashes": [
                 "sha256:567f09558bae2b3ab53cb3c1e2e33e726ff3338e7bae3db5dc954b3a44eef12b",
                 "sha256:aefc51675b0b533d56bb5fd1c8c6c0522fe31896679882e1c4c63d5e4a0fccb3"
             ],
             "markers": "python_version >= '2.6'",
@@ -230,40 +217,40 @@
                 "sha256:b0efb6516fd4fb07b45949053826a62fa4cb353db5be2bbb4a7aa1fdd1e345fb"
             ],
             "markers": "python_version >= '3.8' and sys_platform == 'win32'",
             "version": "==3.4.1"
         },
         "python-jenkins": {
             "hashes": [
-                "sha256:8f6baed1f6e160447863e8182c90f4536616db4ad853e521fa2af9041be47b77",
-                "sha256:fd7614a31923569545f05da11823ffef657cb2aa40b7e8e182c9bfbdbebc11dc"
+                "sha256:0180a5463f68e2e0110f382b4248d2284bc68481db4a16fcbf61f4f55801c31f",
+                "sha256:f40f54505da1be96160ef571363903c8d2d1eae8fa706dbe701211833f440b80"
             ],
             "index": "pypi",
-            "version": "==1.8.0.0a0"
+            "version": "==1.8.0"
         },
         "pywin32": {
             "hashes": [
-                "sha256:109f98980bfb27e78f4df8a51a8198e10b0f347257d1e265bb1a32993d0c973d",
-                "sha256:13362cc5aa93c2beaf489c9c9017c793722aeb56d3e5166dadd5ef82da021fe1",
-                "sha256:19ca459cd2e66c0e2cc9a09d589f71d827f26d47fe4a9d09175f6aa0256b51c2",
-                "sha256:326f42ab4cfff56e77e3e595aeaf6c216712bbdd91e464d167c6434b28d65990",
-                "sha256:421f6cd86e84bbb696d54563c48014b12a23ef95a14e0bdba526be756d89f116",
-                "sha256:48d8b1659284f3c17b68587af047d110d8c44837736b8932c034091683e05863",
-                "sha256:4ecd404b2c6eceaca52f8b2e3e91b2187850a1ad3f8b746d0796a98b4cea04db",
-                "sha256:50768c6b7c3f0b38b7fb14dd4104da93ebced5f1a50dc0e834594bff6fbe1271",
-                "sha256:56d7a9c6e1a6835f521788f53b5af7912090674bb84ef5611663ee1595860fc7",
-                "sha256:73e819c6bed89f44ff1d690498c0a811948f73777e5f97c494c152b850fad478",
-                "sha256:742eb905ce2187133a29365b428e6c3b9001d79accdc30aa8969afba1d8470f4",
-                "sha256:9d968c677ac4d5cbdaa62fd3014ab241718e619d8e36ef8e11fb930515a1e918",
-                "sha256:9dd98384da775afa009bc04863426cb30596fd78c6f8e4e2e5bbf4edf8029504",
-                "sha256:a55db448124d1c1484df22fa8bbcbc45c64da5e6eae74ab095b9ea62e6d00496"
+                "sha256:06d3420a5155ba65f0b72f2699b5bacf3109f36acbe8923765c22938a69dfc8d",
+                "sha256:1c73ea9a0d2283d889001998059f5eaaba3b6238f767c9cf2833b13e6a685f65",
+                "sha256:37257794c1ad39ee9be652da0462dc2e394c8159dfd913a8a4e8eb6fd346da0e",
+                "sha256:383229d515657f4e3ed1343da8be101000562bf514591ff383ae940cad65458b",
+                "sha256:39b61c15272833b5c329a2989999dcae836b1eed650252ab1b7bfbe1d59f30f4",
+                "sha256:5821ec52f6d321aa59e2db7e0a35b997de60c201943557d108af9d4ae1ec7040",
+                "sha256:70dba0c913d19f942a2db25217d9a1b726c278f483a919f1abfed79c9cf64d3a",
+                "sha256:72c5f621542d7bdd4fdb716227be0dd3f8565c11b280be6315b06ace35487d36",
+                "sha256:84f4471dbca1887ea3803d8848a1616429ac94a4a8d05f4bc9c5dcfd42ca99c8",
+                "sha256:a7639f51c184c0272e93f244eb24dafca9b1855707d94c192d4a0b4c01e1100e",
+                "sha256:e25fd5b485b55ac9c057f67d94bc203f3f6595078d1fb3b458c9c28b7153a802",
+                "sha256:e4c092e2589b5cf0d365849e73e02c391c1349958c5ac3e9d5ccb9a28e017b3a",
+                "sha256:e65028133d15b64d2ed8f06dd9fbc268352478d4f9289e69c190ecd6818b6407",
+                "sha256:e8ac1ae3601bee6ca9f7cb4b5363bf1c0badb935ef243c4733ff9a393b1690c0"
             ],
             "index": "pypi",
             "markers": "sys_platform == 'win32' or platform_system == 'Windows' or os_name == 'nt'",
-            "version": "==305"
+            "version": "==306"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -305,43 +292,51 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "index": "pypi",
             "version": "==6.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "requests-futures": {
             "hashes": [
-                "sha256:35547502bf1958044716a03a2f47092a89efe8f9789ab0c4c528d9c9c30bc148",
-                "sha256:633804c773b960cef009efe2a5585483443c6eac3c39cc64beba2884013bcdd9"
+                "sha256:4a2f5472e9911a79532137d156aa937cd9cd90fec55677f71b2976d1f7a66d38",
+                "sha256:f55a4ef80070e2858e7d1e73123d2bfaeaf25b93fd34384d8ddf148e2b676373"
             ],
             "index": "pypi",
-            "version": "==1.0.0"
+            "version": "==1.0.1"
+        },
+        "setuptools": {
+            "hashes": [
+                "sha256:4d3c92fac8f1118bb77a22181355e29c239cabfe2b9effdaa665c66b711136d7",
+                "sha256:8ab4f1dbf2b4a65f7eec5ad0c620e84c34111a68d3349833494b9088212214dd"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==65.7.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "termcolor": {
             "hashes": [
-                "sha256:91ddd848e7251200eac969846cbae2dacd7d71c2871e92733289e7e3666f48e7",
-                "sha256:dfc8ac3f350788f23b2947b3e6cfa5a53b630b612e6cd8965a015a776020b99a"
+                "sha256:3afb05607b89aed0ffe25202399ee0867ad4d3cb4180d98aaf8eefa6a5f7d475",
+                "sha256:b5b08f68937f138fe92f6c089b99f1e2da0ae56c52b78bf7075fd95420fd9a5a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
+            "version": "==2.3.0"
         },
         "toml": {
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
@@ -353,19 +348,19 @@
                 "sha256:c083dd0dce68dbfbe1129d5271cb90f9447dea7d52097c6e0126120c521ddea8"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.13"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:3f09e6d8230892547132177f575a4e3e73cfdf06526e20cc02aa1c3b47184d40",
-                "sha256:cdf5877568b7e83aa7cf2244ab56a3213de587bbe0ce9d8b9600fc77b455d89e"
+                "sha256:c951af98631d24f8df89ab1019fc365f2227c0892f12fd150e935607c79dd0dd",
+                "sha256:f1f9f2ad5291f0225a49efad77abf9e700b6fef553900623060dad6e26503b9d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.1"
+            "version": "==1.6.1"
         },
         "windows-curses": {
             "hashes": [
                 "sha256:25e7ff3d77aed6c747456b06fbc1528d67fc59d1ef3be9ca244774e65e6bdbb2",
                 "sha256:2644f4547ae5124ce5129b66faa59ee0995b7b7205ed5e3920f6ecfef2e46275",
                 "sha256:395656bfe88d6f60cb18604605d423e0f2d1c3a8f550507dca5877a9d0b3a0f3",
                 "sha256:59856b41676c4b3eb527eb6b1478803d4dc92413b2e63aea762407807ffcd3ac",
@@ -413,35 +408,27 @@
                 "sha256:ad33358114df7c9416cdb8fa1eaa5852166c505118717021c6a8c7c7abbd03dd",
                 "sha256:c8ac1ca6772207179ed8003ce7687757c04b0b71536f81e2ac5755c6226458fe"
             ],
             "version": "==0.17.3"
         },
         "astroid": {
             "hashes": [
-                "sha256:86b0a340a512c65abf4368b80252754cda17c02cdbbd3f587dddf98112233e7b",
-                "sha256:bb24615c77f4837c707669d16907331374ae8a964650a66999da3f5ca68dc946"
-            ],
-            "markers": "python_full_version >= '3.6.2'",
-            "version": "==2.11.7"
-        },
-        "attrs": {
-            "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
+                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
+                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
+            "markers": "python_full_version >= '3.7.2'",
+            "version": "==2.15.5"
         },
         "babel": {
             "hashes": [
-                "sha256:1ad3eca1c885218f6dce2ab67291178944f810a10a9b5f3cb8382a5a232b64fe",
-                "sha256:5ef4b3226b0180dedded4229651c8b0e1a3a6a2837d45a073272f313e4cf97f6"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.11.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.12.1"
         },
         "bleach": {
             "hashes": [
                 "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
@@ -453,121 +440,108 @@
                 "sha256:762cb2bfad61f4ec8e2bdf452c7c267416f8c70dd9ecb1653fd0bbb01fa936e6"
             ],
             "index": "pypi",
             "version": "==1.0.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cfgv": {
             "hashes": [
                 "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
             "version": "==3.3.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_full_version >= '3.6.0'",
-            "version": "==3.0.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
@@ -606,55 +580,55 @@
             "version": "==0.7.1"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
         "docker": {
             "hashes": [
-                "sha256:896c4282e5c7af5c45e8b683b0b0c33932974fe6e50fc6906a0a83616ab3da97",
-                "sha256:dbcb3bd2fa80dca0788ed908218bf43972772009b881ed1e20dfc29a65e49782"
+                "sha256:aa6d17830045ba5ef0168d5eaa34d37beeb113948c413affe1d5991fc11f9a20",
+                "sha256:aecd2277b8bf8e506e484f6ab7aec39abe0038e29fa4a6d3ba86c3fe01844ed9"
             ],
             "index": "pypi",
-            "version": "==6.0.1"
+            "version": "==6.1.3"
         },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "version": "==0.20.1"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e",
-                "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"
+                "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5",
+                "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.0"
+            "version": "==1.1.2"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
+            "version": "==3.12.2"
         },
         "ghp-import": {
             "hashes": [
                 "sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619",
                 "sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343"
             ],
             "version": "==2.1.0"
@@ -665,19 +639,19 @@
                 "sha256:6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==10.0"
         },
         "identify": {
             "hashes": [
-                "sha256:89e144fa560cc4cffb6ef2ab5e9fb18ed9f9b3cb054384bab4b95c12f6c309fe",
-                "sha256:93aac7ecf2f6abf879b8f29a8002d3c6de7086b8c28d88e1ad15045a15ab63f9"
+                "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
+                "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.18"
+            "version": "==2.5.24"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -689,19 +663,19 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
-                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
+                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
+                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==6.0.0"
+            "version": "==6.7.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -737,19 +711,19 @@
                 "sha256:db92ec08ae418d27587c36d76e4eadec2f4f268a21aad6aae667d7fc60ee5c36"
             ],
             "index": "pypi",
             "version": "==3.21.0"
         },
         "keyring": {
             "hashes": [
-                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
-                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
+                "sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6",
+                "sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.13.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==24.2.0"
         },
         "lazy-object-proxy": {
             "hashes": [
                 "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
                 "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
                 "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
                 "sha256:18b78ec83edbbeb69efdc0e9c1cb41a3b1b1ed11ddd8ded602464c3fc6020494",
@@ -803,91 +777,91 @@
                 "sha256:f5da449a6e1c989a4cea2631aa8ee67caa5a2ef855d551c88f9e309f4634c621"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.3.7"
         },
         "markdown-it-py": {
             "hashes": [
-                "sha256:93de681e5c021a432c63147656fe21790bc01231e0cd2da73626f1aa3ac0fe27",
-                "sha256:cf7e59fed14b5ae17c0006eff14a2d9a00ed5f3a846148153899a0224e2c07da"
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.1.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
-                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
-                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
-                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
-                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
-                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
-                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
-                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
-                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
-                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
-                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
-                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
-                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
-                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
-                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
-                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
-                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
-                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
-                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
-                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
-                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
-                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
-                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
-                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
-                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
-                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
-                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
-                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
-                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
-                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
-                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
-                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
-                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
-                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
-                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
-                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
-                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
-                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
-                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
-                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
-                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
-                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
-                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
-                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
-                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
-                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
-                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
-                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
-                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
-                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.2"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
         "mdit-py-plugins": {
             "hashes": [
-                "sha256:36d08a29def19ec43acdcd8ba471d3ebab132e7879d442760d963f19913e04b9",
-                "sha256:5cfd7e7ac582a594e23ba6546a2f406e94e42eb33ae596d0734781261c251260"
+                "sha256:b51b3bb70691f57f974e257e367107857a93b36f322a9e6d44ca5bf28ec2def9",
+                "sha256:d8ab27e9aed6c38aa716819fedfde15ca275715955f8a185a8e1cf90fb1d2c1b"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.3.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==0.4.0"
         },
         "mdurl": {
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
@@ -899,60 +873,68 @@
                 "sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.3.4"
         },
         "mkdocs": {
             "hashes": [
-                "sha256:8947af423a6d0facf41ea1195b8e1e8c85ad94ac95ae307fe11232e0424b11c5",
-                "sha256:c8856a832c1e56702577023cd64cc5f84948280c1c0fcc6af4cd39006ea6aa8c"
+                "sha256:5955093bbd4dd2e9403c5afaf57324ad8b04f16886512a3ee6ef828956481c57",
+                "sha256:6ee46d309bda331aac915cd24aab882c179a933bd9e77b80ce7d2eaaa3f689dd"
             ],
             "index": "pypi",
-            "version": "==1.4.2"
+            "version": "==1.4.3"
         },
         "more-itertools": {
             "hashes": [
-                "sha256:250e83d7e81d0c87ca6bd942e6aeab8cc9daa6096d12c5308f3f92fa5e5c1f41",
-                "sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab"
+                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
+                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==9.0.0"
+            "version": "==9.1.0"
         },
         "multi-key-dict": {
             "hashes": [
                 "sha256:3a1e1fc705a30a7de1a153ec2992b3ca3655ccd9225d2e427fe6525c8f160d6d",
                 "sha256:cb1e00aa9d8192496cc0cc040f6d9602f35e4cf099e866248be06b04fd45b42b",
                 "sha256:deebdec17aa30a1c432cb3f437e81f8621e1c0542a0c0617a74f71e232e9939e",
                 "sha256:fb67a532d7361a66820aa1e8fe6c0c939f4c34a3a09a3e8db199ce7b77c4fb78"
             ],
             "version": "==2.0.3"
         },
         "myst-parser": {
             "hashes": [
-                "sha256:61b275b85d9f58aa327f370913ae1bec26ebad372cc99f3ab85c8ec3ee8d9fb8",
-                "sha256:79317f4bb2c13053dd6e64f9da1ba1da6cd9c40c8a430c447a7b146a594c246d"
+                "sha256:7c36344ae39c8e740dad7fdabf5aa6fc4897a813083c6cc9990044eb93656b14",
+                "sha256:ea929a67a6a0b1683cdbe19b8d2e724cd7643f8aa3e7bb18dd65beac3483bead"
             ],
             "index": "pypi",
-            "version": "==0.18.1"
+            "version": "==2.0.0"
         },
         "nodeenv": {
             "hashes": [
-                "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e",
-                "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
+                "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
+                "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
-            "version": "==1.7.0"
+            "version": "==1.8.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1"
+        },
+        "pathspec": {
+            "hashes": [
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==0.11.1"
         },
         "pbr": {
             "hashes": [
                 "sha256:567f09558bae2b3ab53cb3c1e2e33e726ff3338e7bae3db5dc954b3a44eef12b",
                 "sha256:aefc51675b0b533d56bb5fd1c8c6c0522fe31896679882e1c4c63d5e4a0fccb3"
             ],
             "markers": "python_version >= '2.6'",
@@ -972,77 +954,77 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:8a1228abb1ef82d788f74139988b137e78692984ec7b08eaa6c65f1723af28f9",
-                "sha256:b1d5eb14f221506f50d6604a561f4c5786d9e80355219694a1b244bcd96f4567"
+                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
+                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.0.0"
+            "version": "==3.8.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.2.0"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:9e3255edb0c9e7fe9b4f328cb3dc86069f8fdc38026f1bf521018a05eaf4d67b",
-                "sha256:bc4687478d55578c4ac37272fe96df66f73d9b5cf81be6f28627d4e712e752d5"
+                "sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb",
+                "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"
             ],
             "index": "pypi",
-            "version": "==3.0.4"
+            "version": "==3.3.3"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pyinstaller": {
             "hashes": [
-                "sha256:314fb883caf3cbf06adbea2b77671bb73c3481568e994af0467ea7e47eb64755",
-                "sha256:3b74f50a57b1413047042e47033480b7324b091f23dff790a4494af32b377d94",
-                "sha256:4f4d818588e2d8de4bf24ed018056c3de0c95898ad25719e12d68626161b4933",
-                "sha256:502a2166165a8e8c3d99c19272e923d2548bac2132424d78910ef9dd8bb11705",
-                "sha256:5c9632a20faecd6d79f0124afb31e6557414d19be271e572765b474f860f8d76",
-                "sha256:8d004699c5d71c704c14a5f81eec233faa4f87a3bf0ae68e222b87d63f5dd17e",
-                "sha256:a62ee598b137202ef2e99d8dbaee6bc7379a6565c3ddf0331decb41b98eff1a2",
-                "sha256:bacf236b5c2f8f674723a39daca399646dceb470881f842f52e393b9a67ff2f8",
-                "sha256:bf1f7b7e88b467d7aefcdb2bc9cbd2e856ca88c5ab232c0efe0848f146d3bd5f",
-                "sha256:ded780f0d3642d7bfc21d97b98d4ec4b41d2fe70c3f5c5d243868612f536e011",
-                "sha256:e68bcadf32edc1171ccb06117699a6a4f8e924b7c2c8812cfa00fd0186ade4ee",
-                "sha256:f9361eff44c7108c2312f39d85ed768c4ada7e0aa729046bbcef3ef3c1577d18"
+                "sha256:0df43697c4914285ecd333be968d2cd042ab9b2670124879ee87931d2344eaf5",
+                "sha256:1fde4381155f21d6354dc450dcaa338cd8a40aaacf6bd22b987b0f3e1f96f3ee",
+                "sha256:24009eba63cfdbcde6d2634e9c87f545eb67249ddf3b514e0cd3b2cdaa595828",
+                "sha256:28d9742c37e9fb518444b12f8c8ab3cb4ba212d752693c34475c08009aa21ccf",
+                "sha256:2d03419904d1c25c8968b0ad21da0e0f33d8d65716e29481b5bd83f7f342b0c5",
+                "sha256:3a331951f9744bc2379ea5d65d36f3c828eaefe2785f15039592cdc08560b262",
+                "sha256:5e446df41255e815017d96318e39f65a3eb807e74a796c7e7ff7f13b6366a2e9",
+                "sha256:78975043edeb628e23a73fb3ef0a273cda50e765f1716f75212ea3e91b09dede",
+                "sha256:7fdd319828de679f9c5e381eff998ee9b4164bf4457e7fca56946701cf002c3f",
+                "sha256:9fc27c5a853b14a90d39c252707673c7a0efec921cd817169aff3af0fca8c127",
+                "sha256:cd7d5c06f2847195a23d72ede17c60857d6f495d6f0727dc6c9bc1235f2eb79c",
+                "sha256:e5fb17de6c325d3b2b4ceaeb55130ad7100a79096490e4c5b890224406fa42f4"
             ],
             "index": "pypi",
-            "version": "==5.8.0"
+            "version": "==5.13.0"
         },
         "pyinstaller-hooks-contrib": {
             "hashes": [
-                "sha256:29d052eb73e0ab8f137f11df8e73d464c1c6d4c3044d9dc8df2af44639d8bfbf",
-                "sha256:bd578781cd6a33ef713584bf3726f7cd60a3e656ec08a6cc7971e39990808cc0"
+                "sha256:9c11197653de9605a81975325a60b9369e9cdc37c009b6aeb0221a57211f9388",
+                "sha256:fc9892e46fa19d05725205413fb21a764f2f6ff1e70ba95322fb02420a665a45"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2023.0"
+            "version": "==2023.4"
         },
         "pylint": {
             "hashes": [
-                "sha256:15bc7b37f2022720765247eec24c49b93dcae6c81418adc3c36621b13d946f6d",
-                "sha256:add6bc6380143af0f7a1ab15b5b5f54a8d9d25afc99fc7e2d86fd66f6c3e1ad9"
+                "sha256:eb035800b371862e783f27067b3fc00c6b726880cacfed101b619f366bb813f6",
+                "sha256:f0b0857f6fba90527a30f39937a9f66858b59c5dcbb8c062821ad665637bb742"
             ],
             "index": "pypi",
-            "version": "==3.0.0a5"
+            "version": "==3.0.0a6"
         },
         "pypiwin32": {
             "hashes": [
                 "sha256:67adf399debc1d5d14dffc1ab5acacb800da569754fafdc576b2a039485aa775",
                 "sha256:71be40c1fbd28594214ecaecb58e7aa8b708eabfa0125c8a109ebd51edbd776a"
             ],
             "index": "pypi",
@@ -1055,71 +1037,64 @@
                 "sha256:b0efb6516fd4fb07b45949053826a62fa4cb353db5be2bbb4a7aa1fdd1e345fb"
             ],
             "markers": "python_version >= '3.8' and sys_platform == 'win32'",
             "version": "==3.4.1"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
-            "version": "==7.2.1"
+            "version": "==7.4.0"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "python-jenkins": {
             "hashes": [
-                "sha256:8f6baed1f6e160447863e8182c90f4536616db4ad853e521fa2af9041be47b77",
-                "sha256:fd7614a31923569545f05da11823ffef657cb2aa40b7e8e182c9bfbdbebc11dc"
+                "sha256:0180a5463f68e2e0110f382b4248d2284bc68481db4a16fcbf61f4f55801c31f",
+                "sha256:f40f54505da1be96160ef571363903c8d2d1eae8fa706dbe701211833f440b80"
             ],
             "index": "pypi",
-            "version": "==1.8.0.0a0"
-        },
-        "pytz": {
-            "hashes": [
-                "sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0",
-                "sha256:78f4f37d8198e0627c5f1143240bb0206b8691d8d7ac6d78fee88b78733f8c4a"
-            ],
-            "version": "==2022.7.1"
+            "version": "==1.8.0"
         },
         "pywin32": {
             "hashes": [
-                "sha256:109f98980bfb27e78f4df8a51a8198e10b0f347257d1e265bb1a32993d0c973d",
-                "sha256:13362cc5aa93c2beaf489c9c9017c793722aeb56d3e5166dadd5ef82da021fe1",
-                "sha256:19ca459cd2e66c0e2cc9a09d589f71d827f26d47fe4a9d09175f6aa0256b51c2",
-                "sha256:326f42ab4cfff56e77e3e595aeaf6c216712bbdd91e464d167c6434b28d65990",
-                "sha256:421f6cd86e84bbb696d54563c48014b12a23ef95a14e0bdba526be756d89f116",
-                "sha256:48d8b1659284f3c17b68587af047d110d8c44837736b8932c034091683e05863",
-                "sha256:4ecd404b2c6eceaca52f8b2e3e91b2187850a1ad3f8b746d0796a98b4cea04db",
-                "sha256:50768c6b7c3f0b38b7fb14dd4104da93ebced5f1a50dc0e834594bff6fbe1271",
-                "sha256:56d7a9c6e1a6835f521788f53b5af7912090674bb84ef5611663ee1595860fc7",
-                "sha256:73e819c6bed89f44ff1d690498c0a811948f73777e5f97c494c152b850fad478",
-                "sha256:742eb905ce2187133a29365b428e6c3b9001d79accdc30aa8969afba1d8470f4",
-                "sha256:9d968c677ac4d5cbdaa62fd3014ab241718e619d8e36ef8e11fb930515a1e918",
-                "sha256:9dd98384da775afa009bc04863426cb30596fd78c6f8e4e2e5bbf4edf8029504",
-                "sha256:a55db448124d1c1484df22fa8bbcbc45c64da5e6eae74ab095b9ea62e6d00496"
+                "sha256:06d3420a5155ba65f0b72f2699b5bacf3109f36acbe8923765c22938a69dfc8d",
+                "sha256:1c73ea9a0d2283d889001998059f5eaaba3b6238f767c9cf2833b13e6a685f65",
+                "sha256:37257794c1ad39ee9be652da0462dc2e394c8159dfd913a8a4e8eb6fd346da0e",
+                "sha256:383229d515657f4e3ed1343da8be101000562bf514591ff383ae940cad65458b",
+                "sha256:39b61c15272833b5c329a2989999dcae836b1eed650252ab1b7bfbe1d59f30f4",
+                "sha256:5821ec52f6d321aa59e2db7e0a35b997de60c201943557d108af9d4ae1ec7040",
+                "sha256:70dba0c913d19f942a2db25217d9a1b726c278f483a919f1abfed79c9cf64d3a",
+                "sha256:72c5f621542d7bdd4fdb716227be0dd3f8565c11b280be6315b06ace35487d36",
+                "sha256:84f4471dbca1887ea3803d8848a1616429ac94a4a8d05f4bc9c5dcfd42ca99c8",
+                "sha256:a7639f51c184c0272e93f244eb24dafca9b1855707d94c192d4a0b4c01e1100e",
+                "sha256:e25fd5b485b55ac9c057f67d94bc203f3f6595078d1fb3b458c9c28b7153a802",
+                "sha256:e4c092e2589b5cf0d365849e73e02c391c1349958c5ac3e9d5ccb9a28e017b3a",
+                "sha256:e65028133d15b64d2ed8f06dd9fbc268352478d4f9289e69c190ecd6818b6407",
+                "sha256:e8ac1ae3601bee6ca9f7cb4b5363bf1c0badb935ef243c4733ff9a393b1690c0"
             ],
             "index": "pypi",
             "markers": "sys_platform == 'win32' or platform_system == 'Windows' or os_name == 'nt'",
-            "version": "==305"
+            "version": "==306"
         },
         "pywin32-ctypes": {
             "hashes": [
-                "sha256:24ffc3b341d457d48e8922352130cf2644024a4ff09762a2261fd34c36ee5942",
-                "sha256:9dc2d991b3479cc2df15930958b674a48a227d5361d413827a4cfd0b5876fc98"
+                "sha256:3426e063bdd5fd4df74a14fa3cf80a0b42845a87e1d1e81f6549f9daec593a60",
+                "sha256:bf490a1a709baf35d688fe0ecf980ed4de11d2b3e37b51e5442587a75d9957e7"
             ],
             "markers": "sys_platform == 'win32'",
-            "version": "==0.2.0"
+            "version": "==0.2.2"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -1169,67 +1144,67 @@
                 "sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.1"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
-                "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
+                "sha256:9f77b519d96d03d7d7dce44977ba543090a14397c4f60de5b6eb5b8048110aa4",
+                "sha256:e18feb2a1e7706f2865b81ebb460056d93fb29d69daa10b223c00faa7bd9a00a"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==37.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==40.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "requests-futures": {
             "hashes": [
-                "sha256:35547502bf1958044716a03a2f47092a89efe8f9789ab0c4c528d9c9c30bc148",
-                "sha256:633804c773b960cef009efe2a5585483443c6eac3c39cc64beba2884013bcdd9"
+                "sha256:4a2f5472e9911a79532137d156aa937cd9cd90fec55677f71b2976d1f7a66d38",
+                "sha256:f55a4ef80070e2858e7d1e73123d2bfaeaf25b93fd34384d8ddf148e2b676373"
             ],
             "index": "pypi",
-            "version": "==1.0.0"
+            "version": "==1.0.1"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:125d96d20c92b946b983d0d392b84ff945461e5a06d3867e9f9e575f8697b67f",
-                "sha256:8aa57747f3fc3e977684f0176a88e789be314a99f99b43b75d1e9cb5dc6db9e9"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.1"
+            "version": "==13.4.2"
         },
         "setuptools": {
             "hashes": [
-                "sha256:16ccf598aab3b506593c17378473978908a2734d7336755a8769b480906bec1c",
-                "sha256:b440ee5f7e607bb8c9de15259dba2583dd41a38879a7abc1d43a71c59524da48"
+                "sha256:4d3c92fac8f1118bb77a22181355e29c239cabfe2b9effdaa665c66b711136d7",
+                "sha256:8ab4f1dbf2b4a65f7eec5ad0c620e84c34111a68d3349833494b9088212214dd"
             ],
-            "index": "pypi",
-            "version": "==67.2.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==65.7.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1240,19 +1215,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:060ca5c9f7ba57a08a1219e547b269fadf125ae25b06b9fa7f66768efb652d6d",
-                "sha256:51026de0a9ff9fc13c05d74913ad66047e104f56a129ff73e174eb5c3ee794b5"
+                "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616",
+                "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==5.3.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==7.0.1"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
                 "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
                 "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
             "markers": "python_version >= '3.8'",
@@ -1296,19 +1271,19 @@
                 "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.1.5"
         },
         "termcolor": {
             "hashes": [
-                "sha256:91ddd848e7251200eac969846cbae2dacd7d71c2871e92733289e7e3666f48e7",
-                "sha256:dfc8ac3f350788f23b2947b3e6cfa5a53b630b612e6cd8965a015a776020b99a"
+                "sha256:3afb05607b89aed0ffe25202399ee0867ad4d3cb4180d98aaf8eefa6a5f7d475",
+                "sha256:b5b08f68937f138fe92f6c089b99f1e2da0ae56c52b78bf7075fd95420fd9a5a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
+            "version": "==2.3.0"
         },
         "toml": {
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
@@ -1320,108 +1295,107 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b",
-                "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.11.6"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.8"
         },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
-                "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
+                "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
+                "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==4.4.0"
+            "markers": "python_version < '3.11'",
+            "version": "==4.7.1"
         },
         "urllib3": {
             "hashes": [
                 "sha256:47cc05d99aaa09c9e72ed5809b60e7ba354e64b59c9c173ac3018642d8bb41fc",
                 "sha256:c083dd0dce68dbfbe1129d5271cb90f9447dea7d52097c6e0126120c521ddea8"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.13"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:37a640ba82ed40b226599c522d411e4be5edb339a0c0de030c0dc7b646d61590",
-                "sha256:54eb59e7352b573aa04d53f80fc9736ed0ad5143af445a1e539aada6eb947dd1"
+                "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419",
+                "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.19.0"
+            "version": "==20.23.1"
         },
         "watchdog": {
             "hashes": [
-                "sha256:102a60093090fc3ff76c983367b19849b7cc24ec414a43c0333680106e62aae1",
-                "sha256:17f1708f7410af92ddf591e94ae71a27a13974559e72f7e9fde3ec174b26ba2e",
-                "sha256:195ab1d9d611a4c1e5311cbf42273bc541e18ea8c32712f2fb703cfc6ff006f9",
-                "sha256:4cb5ecc332112017fbdb19ede78d92e29a8165c46b68a0b8ccbd0a154f196d5e",
-                "sha256:5100eae58133355d3ca6c1083a33b81355c4f452afa474c2633bd2fbbba398b3",
-                "sha256:61fdb8e9c57baf625e27e1420e7ca17f7d2023929cd0065eb79c83da1dfbeacd",
-                "sha256:6ccd8d84b9490a82b51b230740468116b8205822ea5fdc700a553d92661253a3",
-                "sha256:6e01d699cd260d59b84da6bda019dce0a3353e3fcc774408ae767fe88ee096b7",
-                "sha256:748ca797ff59962e83cc8e4b233f87113f3cf247c23e6be58b8a2885c7337aa3",
-                "sha256:83a7cead445008e880dbde833cb9e5cc7b9a0958edb697a96b936621975f15b9",
-                "sha256:8586d98c494690482c963ffb24c49bf9c8c2fe0589cec4dc2f753b78d1ec301d",
-                "sha256:8b5cde14e5c72b2df5d074774bdff69e9b55da77e102a91f36ef26ca35f9819c",
-                "sha256:8c28c23972ec9c524967895ccb1954bc6f6d4a557d36e681a36e84368660c4ce",
-                "sha256:967636031fa4c4955f0f3f22da3c5c418aa65d50908d31b73b3b3ffd66d60640",
-                "sha256:96cbeb494e6cbe3ae6aacc430e678ce4b4dd3ae5125035f72b6eb4e5e9eb4f4e",
-                "sha256:978a1aed55de0b807913b7482d09943b23a2d634040b112bdf31811a422f6344",
-                "sha256:a09483249d25cbdb4c268e020cb861c51baab2d1affd9a6affc68ffe6a231260",
-                "sha256:a480d122740debf0afac4ddd583c6c0bb519c24f817b42ed6f850e2f6f9d64a8",
-                "sha256:adaf2ece15f3afa33a6b45f76b333a7da9256e1360003032524d61bdb4c422ae",
-                "sha256:bc43c1b24d2f86b6e1cc15f68635a959388219426109233e606517ff7d0a5a73",
-                "sha256:c27d8c1535fd4474e40a4b5e01f4ba6720bac58e6751c667895cbc5c8a7af33c",
-                "sha256:cdcc23c9528601a8a293eb4369cbd14f6b4f34f07ae8769421252e9c22718b6f",
-                "sha256:cece1aa596027ff56369f0b50a9de209920e1df9ac6d02c7f9e5d8162eb4f02b",
-                "sha256:d0f29fd9f3f149a5277929de33b4f121a04cf84bb494634707cfa8ea8ae106a8",
-                "sha256:d6b87477752bd86ac5392ecb9eeed92b416898c30bd40c7e2dd03c3146105646",
-                "sha256:e038be858425c4f621900b8ff1a3a1330d9edcfeaa1c0468aeb7e330fb87693e",
-                "sha256:e618a4863726bc7a3c64f95c218437f3349fb9d909eb9ea3a1ed3b567417c661",
-                "sha256:f8ac23ff2c2df4471a61af6490f847633024e5aa120567e08d07af5718c9d092"
+                "sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a",
+                "sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100",
+                "sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8",
+                "sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc",
+                "sha256:2b57a1e730af3156d13b7fdddfc23dea6487fceca29fc75c5a868beed29177ae",
+                "sha256:336adfc6f5cc4e037d52db31194f7581ff744b67382eb6021c868322e32eef41",
+                "sha256:3aa7f6a12e831ddfe78cdd4f8996af9cf334fd6346531b16cec61c3b3c0d8da0",
+                "sha256:3ed7c71a9dccfe838c2f0b6314ed0d9b22e77d268c67e015450a29036a81f60f",
+                "sha256:4c9956d27be0bb08fc5f30d9d0179a855436e655f046d288e2bcc11adfae893c",
+                "sha256:4d98a320595da7a7c5a18fc48cb633c2e73cda78f93cac2ef42d42bf609a33f9",
+                "sha256:4f94069eb16657d2c6faada4624c39464f65c05606af50bb7902e036e3219be3",
+                "sha256:5113334cf8cf0ac8cd45e1f8309a603291b614191c9add34d33075727a967709",
+                "sha256:51f90f73b4697bac9c9a78394c3acbbd331ccd3655c11be1a15ae6fe289a8c83",
+                "sha256:5d9f3a10e02d7371cd929b5d8f11e87d4bad890212ed3901f9b4d68767bee759",
+                "sha256:7ade88d0d778b1b222adebcc0927428f883db07017618a5e684fd03b83342bd9",
+                "sha256:7c5f84b5194c24dd573fa6472685b2a27cc5a17fe5f7b6fd40345378ca6812e3",
+                "sha256:7e447d172af52ad204d19982739aa2346245cc5ba6f579d16dac4bfec226d2e7",
+                "sha256:8ae9cda41fa114e28faf86cb137d751a17ffd0316d1c34ccf2235e8a84365c7f",
+                "sha256:8f3ceecd20d71067c7fd4c9e832d4e22584318983cabc013dbf3f70ea95de346",
+                "sha256:9fac43a7466eb73e64a9940ac9ed6369baa39b3bf221ae23493a9ec4d0022674",
+                "sha256:a70a8dcde91be523c35b2bf96196edc5730edb347e374c7de7cd20c43ed95397",
+                "sha256:adfdeab2da79ea2f76f87eb42a3ab1966a5313e5a69a0213a3cc06ef692b0e96",
+                "sha256:ba07e92756c97e3aca0912b5cbc4e5ad802f4557212788e72a72a47ff376950d",
+                "sha256:c07253088265c363d1ddf4b3cdb808d59a0468ecd017770ed716991620b8f77a",
+                "sha256:c9d8c8ec7efb887333cf71e328e39cffbf771d8f8f95d308ea4125bf5f90ba64",
+                "sha256:d00e6be486affb5781468457b21a6cbe848c33ef43f9ea4a73b4882e5f188a44",
+                "sha256:d429c2430c93b7903914e4db9a966c7f2b068dd2ebdd2fa9b9ce094c7d459f33"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.2.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.0.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:3f09e6d8230892547132177f575a4e3e73cfdf06526e20cc02aa1c3b47184d40",
-                "sha256:cdf5877568b7e83aa7cf2244ab56a3213de587bbe0ce9d8b9600fc77b455d89e"
+                "sha256:c951af98631d24f8df89ab1019fc365f2227c0892f12fd150e935607c79dd0dd",
+                "sha256:f1f9f2ad5291f0225a49efad77abf9e700b6fef553900623060dad6e26503b9d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.1"
+            "version": "==1.6.1"
         },
         "wheel": {
             "hashes": [
-                "sha256:965f5259b566725405b05e7cf774052044b1ed30119b5d586b2703aafe8719ac",
-                "sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8"
+                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
+                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
             ],
             "index": "pypi",
-            "version": "==0.38.4"
+            "version": "==0.40.0"
         },
         "windows-curses": {
             "hashes": [
                 "sha256:25e7ff3d77aed6c747456b06fbc1528d67fc59d1ef3be9ca244774e65e6bdbb2",
                 "sha256:2644f4547ae5124ce5129b66faa59ee0995b7b7205ed5e3920f6ecfef2e46275",
                 "sha256:395656bfe88d6f60cb18604605d423e0f2d1c3a8f550507dca5877a9d0b3a0f3",
                 "sha256:59856b41676c4b3eb527eb6b1478803d4dc92413b2e63aea762407807ffcd3ac",
@@ -1436,108 +1410,116 @@
             ],
             "index": "pypi",
             "markers": "sys_platform == 'win32' or platform_system == 'Windows' or os_name == 'nt'",
             "version": "==2.3.1"
         },
         "wrapt": {
             "hashes": [
-                "sha256:09fbbcfb17be9464c18f3e54457e4907a3913f836a691552ae1c967df4d6e4b4",
-                "sha256:0d47527c5c8f9fa6d20fd72e87c39c1cad627f8c7f11b62af05e27ddcd443ba3",
-                "sha256:107415c7367bf5489ab7b16f5348216a1a1c4ff8d5ec08612cf6f64321f9ad3c",
-                "sha256:123de234ee3f528ae817a4be29f811b9ce25f9f48ed446fbd5adcf68b7abb869",
-                "sha256:1b2975c345967fbbff2fa9ffc45c60c30de005e753b6c01135ba4fbb788d3f38",
-                "sha256:21c1487e21979ba8a6a1d6e2e2d026bfeb57aebec0e25da2f7960938e99a9e8c",
-                "sha256:25be3596f51338a6043c6679870d95eb0636e02bb1e6ccf63da61e8021e533d0",
-                "sha256:26bc4fe48eb78cc6a1328b70fe720555b4d31321b060b69fc03a1f8296ee40de",
-                "sha256:30201cbcfea303e345b3c83fb7217e34c46c87df897d3a6f9e0cb840cc0f81c9",
-                "sha256:32960f2f9e5f53ff8c75ef9704d03114fc14c8f604a75323aa7b907f65bfcb6b",
-                "sha256:338dd5c161be7c981f8afb597dac0f5d26e9310d66bbf612209fa29c21a7da33",
-                "sha256:3a8981cbf86e0a004160cbd299af99cb251f93a49d58032bd7400b23f40839e5",
-                "sha256:3cdfb26e3e9fec79e04af3e37b0576c12ee3cd5aa7ba3f041b92aa323fb7f997",
-                "sha256:401a64a7cdfe4d00edcd6a36666e6fba0f61291f6bacf686baf918182f02cf2d",
-                "sha256:42a271aac91a2c74ea6a6b869219cff14404e9362de05c4b83f65dfed7e9b12c",
-                "sha256:44bd131dab4ed4d6221fa78277b6ccbcfa9b439629ffa930b1d1ddc38a88a224",
-                "sha256:45d9589ff8649934c2106d57b85405777e9ce1278eaf0f0fec70f5e037d82c48",
-                "sha256:485cdea587ccc1e8d483855e4e26ab4397b6455e2b416c1f8034ac0acd820da8",
-                "sha256:49e9cb44795b512097f09d9df29e0d83d5f2a517a00eec47d886c0ded5be4496",
-                "sha256:4c08d4c4698e3119408acfa48871ed210a9c40d566b0426eee0b2bd0bc638c0e",
-                "sha256:4c74bf0a62faed5e40431fa846f278420d2356fe2a781b5f601946749f9ac914",
-                "sha256:5053e18f970b38e2e8cb4f635bba79ef1a22d236795af73017b415e9a9aeba48",
-                "sha256:50bfbb843e37e767634102eaf284def65a381061ca762f536c6b5a40e4aed4f4",
-                "sha256:515ab064a2163a05a3b6460137dc4c28c091a58853ed4a0b48b100089a29cb55",
-                "sha256:57ec643799932381502c3f0db4ef5de25bc10b0adc02b0de5fb2a61f23ca7562",
-                "sha256:5951d10d4cac32454c0a65e83330f832db7c4208eee82a69cd7e9be06bbecb70",
-                "sha256:59caed62ad5f7ce1a917e758e15bd2f0bfe2fd6817d0cf8c5e1a713203481669",
-                "sha256:5ac1a93b98c131aabc145a8712e01ed0241c66cb5940fe69ba34c61d59d8b31a",
-                "sha256:5cc4a8d20edb25b395c62e6932e5a1c8afe1aaf45bf2acd876ba683306f9dfa0",
-                "sha256:5d972d3a48c199564e0659d62de4a39d123a547dc25eba548e97b42e4733c0a8",
-                "sha256:5f3a8c55f27524c0426b07232dbfb7f2e0ba414dcb57ebc66054f0a170a0fc49",
-                "sha256:62324e76ea16e5b0339de237edfc1df338442308c599ad3ca02a22e5b3d847db",
-                "sha256:654160de93ee85253d426d9390a649bf2b91e3f79560410644664fd284bc2be8",
-                "sha256:66938fd0469076f8fb1064b24778756b47d71348e5ca7bde5f3cec303ed90676",
-                "sha256:67cad5aae1d0934b02f6a15fa6f181ef83e86d5d8dee2b26873ff57cdd4c0f4f",
-                "sha256:698e03c02d501681939f8a4376afb5521ec04dcca9bfdc023cc968e457e50410",
-                "sha256:6d03a9c18017976265d07e40236dd09278a387cdf3870487060ecf4f48ea5252",
-                "sha256:72d9f2ff2fb3e5c2bfcf891152995b8589c5e735045fbbaae00bd776a6dc9a6b",
-                "sha256:73942a75f7d8b78630076075848d303be3d68798f0462073639583616f0f65a0",
-                "sha256:77cb6f9eae637b1d19b78738602317f788df1896b79f8d81b829d186ff8154c3",
-                "sha256:7963d8049c452e9462e9ea9bc1a20aa31bda4ce667a39b38013e84ae1e6185b0",
-                "sha256:79662ce899950115f33f657b1558a83f631b2a2f91d6fcfdd09a6cbe378cbd2f",
-                "sha256:798bb2eb07988514ee3d213d8ab35e6677c86215190896970b1c407b84ce791a",
-                "sha256:7afabb46692c9dc3053a526915a05ddbc41266082ee505c64fc5aa1fd8ccfdd9",
-                "sha256:7bf51f7815f15d6655c67d32ceedc97787e88c41d1c9cfab19c5f54982d09c41",
-                "sha256:81cf008c5ef139b63dac5df0035eb597bc0b5818d321219d41da2c1aa2fa8ce3",
-                "sha256:88b8bfb2ce44d91789a566cd2be7083e0520208977322bf84ddd215fbee81b58",
-                "sha256:8ee0105bca55eb430ef949eadea557915a183810f25f396e91b5587b7aff3348",
-                "sha256:8f0a1f9d970d4af52c4b696022268b710e19f446423a59cf1d9c393b98c0d985",
-                "sha256:93d95f9007cdcd2ab1c31761840434aff21bc75859110b28dd77a1016fa39202",
-                "sha256:94f9d8cd233b0654c3c38b0855e872716a5b358203a42d41275acb09f3526f0a",
-                "sha256:99011767b4b383706ac749d52b6e2b1f7335e45a72ba604465aa097cca61da3d",
-                "sha256:9c025bbc3b29ca7d56cdbe8dd88e7c90a4caea59af1a236cc17222b114047342",
-                "sha256:9da305a413ac7be48dbcc2eda0a6376235a9cd437a3eb106e67cca36f50f9c12",
-                "sha256:9f74533bf0490662451e520450111548cd669440bb30f0400abe9e778789f5b9",
-                "sha256:a7f4fbef92c3b507232c65b9504c1f23dd5faede097b55ac5ffa599ae775c6e8",
-                "sha256:b51f96d1cd7a88baa373bbb39433d09326fd204c8bf95c2f53b81c530df688ef",
-                "sha256:b53b375ef6028136856aca7c22126de55343035d60198d32d32a90e156be857a",
-                "sha256:b86269bf2657876413a34c84fe205e853aa28ea84d7d044b6a58fd59f6c84e7c",
-                "sha256:bb6182ff6760da884274150af7b7dd3b1a71b49e7c2daa1398e48929b453022a",
-                "sha256:c47994d3ac60e235614235aef76fae1d41a2f882f5fbd62b6fde92f29d84d785",
-                "sha256:c4e87511f8b06cfdf8555701abe64bd2bd0951d1c2a5e66f9ee652ea38edeb5c",
-                "sha256:c588d8e582f07ae24133a4e12ff10e09789763a55acc2317760507492d0d482e",
-                "sha256:c9239fef921d5503c1b4489861ecabe246f56791c0804b1afb6917ba0f328002",
-                "sha256:d46da7b89f9b09c232528b395e9e27be7a73a2b70745eca2e4580f06fe622be4",
-                "sha256:d79b8d62443414fd8790e5b3f89365161957b40e1275888f8e9390a778553bb9",
-                "sha256:ddf53a1f0184a9d9bd72af31cbd639e48e5affc8cc473246a5fe2f89e7b01741",
-                "sha256:e3855ef2ffebca0fb8a1e80bfde292bcb19cdd43c73b94b2b91c874cca1116b9",
-                "sha256:e494137d27700a3a3b020c903d511f1f9fc7ecec406991266a023a756e61db2e",
-                "sha256:e7e3ba93fdec4e044a98c955641dd4e978513854d4a9425fd19f15143bc6af02",
-                "sha256:e8666f3b83285e84a081fc4260fd044f7ef06843691a3fa5e87432152ceeb7c3",
-                "sha256:e999014967cf06782702c7308c3e7977035f548217743eba752b2f8e0b576ee9",
-                "sha256:f50f3bb2ba9d914830ac351a6fce9fd3a5b8ff28124966941f0ea1a4789339a4",
-                "sha256:f6c7af527e9757af49b0de3f9447a61ad3ebc0cedb8e2ecd900265f715944a16",
-                "sha256:f6d36e191323cef8143915e0acc708fd222179311daec90a677f06270367fe8b"
+                "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
+                "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
+                "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
+                "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
+                "sha256:1286eb30261894e4c70d124d44b7fd07825340869945c79d05bda53a40caa079",
+                "sha256:21f6d9a0d5b3a207cdf7acf8e58d7d13d463e639f0c7e01d82cdb671e6cb7923",
+                "sha256:230ae493696a371f1dbffaad3dafbb742a4d27a0afd2b1aecebe52b740167e7f",
+                "sha256:26458da5653aa5b3d8dc8b24192f574a58984c749401f98fff994d41d3f08da1",
+                "sha256:2cf56d0e237280baed46f0b5316661da892565ff58309d4d2ed7dba763d984b8",
+                "sha256:2e51de54d4fb8fb50d6ee8327f9828306a959ae394d3e01a1ba8b2f937747d86",
+                "sha256:2fbfbca668dd15b744418265a9607baa970c347eefd0db6a518aaf0cfbd153c0",
+                "sha256:38adf7198f8f154502883242f9fe7333ab05a5b02de7d83aa2d88ea621f13364",
+                "sha256:3a8564f283394634a7a7054b7983e47dbf39c07712d7b177b37e03f2467a024e",
+                "sha256:3abbe948c3cbde2689370a262a8d04e32ec2dd4f27103669a45c6929bcdbfe7c",
+                "sha256:3bbe623731d03b186b3d6b0d6f51865bf598587c38d6f7b0be2e27414f7f214e",
+                "sha256:40737a081d7497efea35ab9304b829b857f21558acfc7b3272f908d33b0d9d4c",
+                "sha256:41d07d029dd4157ae27beab04d22b8e261eddfc6ecd64ff7000b10dc8b3a5727",
+                "sha256:46ed616d5fb42f98630ed70c3529541408166c22cdfd4540b88d5f21006b0eff",
+                "sha256:493d389a2b63c88ad56cdc35d0fa5752daac56ca755805b1b0c530f785767d5e",
+                "sha256:4ff0d20f2e670800d3ed2b220d40984162089a6e2c9646fdb09b85e6f9a8fc29",
+                "sha256:54accd4b8bc202966bafafd16e69da9d5640ff92389d33d28555c5fd4f25ccb7",
+                "sha256:56374914b132c702aa9aa9959c550004b8847148f95e1b824772d453ac204a72",
+                "sha256:578383d740457fa790fdf85e6d346fda1416a40549fe8db08e5e9bd281c6a475",
+                "sha256:58d7a75d731e8c63614222bcb21dd992b4ab01a399f1f09dd82af17bbfc2368a",
+                "sha256:5c5aa28df055697d7c37d2099a7bc09f559d5053c3349b1ad0c39000e611d317",
+                "sha256:5fc8e02f5984a55d2c653f5fea93531e9836abbd84342c1d1e17abc4a15084c2",
+                "sha256:63424c681923b9f3bfbc5e3205aafe790904053d42ddcc08542181a30a7a51bd",
+                "sha256:64b1df0f83706b4ef4cfb4fb0e4c2669100fd7ecacfb59e091fad300d4e04640",
+                "sha256:74934ebd71950e3db69960a7da29204f89624dde411afbfb3b4858c1409b1e98",
+                "sha256:75669d77bb2c071333417617a235324a1618dba66f82a750362eccbe5b61d248",
+                "sha256:75760a47c06b5974aa5e01949bf7e66d2af4d08cb8c1d6516af5e39595397f5e",
+                "sha256:76407ab327158c510f44ded207e2f76b657303e17cb7a572ffe2f5a8a48aa04d",
+                "sha256:76e9c727a874b4856d11a32fb0b389afc61ce8aaf281ada613713ddeadd1cfec",
+                "sha256:77d4c1b881076c3ba173484dfa53d3582c1c8ff1f914c6461ab70c8428b796c1",
+                "sha256:780c82a41dc493b62fc5884fb1d3a3b81106642c5c5c78d6a0d4cbe96d62ba7e",
+                "sha256:7dc0713bf81287a00516ef43137273b23ee414fe41a3c14be10dd95ed98a2df9",
+                "sha256:7eebcdbe3677e58dd4c0e03b4f2cfa346ed4049687d839adad68cc38bb559c92",
+                "sha256:896689fddba4f23ef7c718279e42f8834041a21342d95e56922e1c10c0cc7afb",
+                "sha256:96177eb5645b1c6985f5c11d03fc2dbda9ad24ec0f3a46dcce91445747e15094",
+                "sha256:96e25c8603a155559231c19c0349245eeb4ac0096fe3c1d0be5c47e075bd4f46",
+                "sha256:9d37ac69edc5614b90516807de32d08cb8e7b12260a285ee330955604ed9dd29",
+                "sha256:9ed6aa0726b9b60911f4aed8ec5b8dd7bf3491476015819f56473ffaef8959bd",
+                "sha256:a487f72a25904e2b4bbc0817ce7a8de94363bd7e79890510174da9d901c38705",
+                "sha256:a4cbb9ff5795cd66f0066bdf5947f170f5d63a9274f99bdbca02fd973adcf2a8",
+                "sha256:a74d56552ddbde46c246b5b89199cb3fd182f9c346c784e1a93e4dc3f5ec9975",
+                "sha256:a89ce3fd220ff144bd9d54da333ec0de0399b52c9ac3d2ce34b569cf1a5748fb",
+                "sha256:abd52a09d03adf9c763d706df707c343293d5d106aea53483e0ec8d9e310ad5e",
+                "sha256:abd8f36c99512755b8456047b7be10372fca271bf1467a1caa88db991e7c421b",
+                "sha256:af5bd9ccb188f6a5fdda9f1f09d9f4c86cc8a539bd48a0bfdc97723970348418",
+                "sha256:b02f21c1e2074943312d03d243ac4388319f2456576b2c6023041c4d57cd7019",
+                "sha256:b06fa97478a5f478fb05e1980980a7cdf2712015493b44d0c87606c1513ed5b1",
+                "sha256:b0724f05c396b0a4c36a3226c31648385deb6a65d8992644c12a4963c70326ba",
+                "sha256:b130fe77361d6771ecf5a219d8e0817d61b236b7d8b37cc045172e574ed219e6",
+                "sha256:b56d5519e470d3f2fe4aa7585f0632b060d532d0696c5bdfb5e8319e1d0f69a2",
+                "sha256:b67b819628e3b748fd3c2192c15fb951f549d0f47c0449af0764d7647302fda3",
+                "sha256:ba1711cda2d30634a7e452fc79eabcadaffedf241ff206db2ee93dd2c89a60e7",
+                "sha256:bbeccb1aa40ab88cd29e6c7d8585582c99548f55f9b2581dfc5ba68c59a85752",
+                "sha256:bd84395aab8e4d36263cd1b9308cd504f6cf713b7d6d3ce25ea55670baec5416",
+                "sha256:c99f4309f5145b93eca6e35ac1a988f0dc0a7ccf9ccdcd78d3c0adf57224e62f",
+                "sha256:ca1cccf838cd28d5a0883b342474c630ac48cac5df0ee6eacc9c7290f76b11c1",
+                "sha256:cd525e0e52a5ff16653a3fc9e3dd827981917d34996600bbc34c05d048ca35cc",
+                "sha256:cdb4f085756c96a3af04e6eca7f08b1345e94b53af8921b25c72f096e704e145",
+                "sha256:ce42618f67741d4697684e501ef02f29e758a123aa2d669e2d964ff734ee00ee",
+                "sha256:d06730c6aed78cee4126234cf2d071e01b44b915e725a6cb439a879ec9754a3a",
+                "sha256:d5fe3e099cf07d0fb5a1e23d399e5d4d1ca3e6dfcbe5c8570ccff3e9208274f7",
+                "sha256:d6bcbfc99f55655c3d93feb7ef3800bd5bbe963a755687cbf1f490a71fb7794b",
+                "sha256:d787272ed958a05b2c86311d3a4135d3c2aeea4fc655705f074130aa57d71653",
+                "sha256:e169e957c33576f47e21864cf3fc9ff47c223a4ebca8960079b8bd36cb014fd0",
+                "sha256:e20076a211cd6f9b44a6be58f7eeafa7ab5720eb796975d0c03f05b47d89eb90",
+                "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
+                "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
+                "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
+                "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
+                "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
+                "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==1.15.0rc1"
+            "markers": "python_version < '3.11'",
+            "version": "==1.15.0"
         },
         "xmltodict": {
             "hashes": [
                 "sha256:341595a488e3e01a85a9d8911d8912fd922ede5fecc4dce437eb4b6c8d037e56",
                 "sha256:aa89e8fd76320154a40d19a0df04a4695fb9dc5ba977cbb68ab3e4eb225e7852"
             ],
             "index": "pypi",
             "version": "==0.13.0"
         },
+        "yamllint": {
+            "hashes": [
+                "sha256:d01dde008c65de5b235188ab3110bebc59d18e5c65fc8a58267cd211cd9df34a",
+                "sha256:d97a66e48da820829d96077d76b8dfbe6c6140f106e558dae87e81ac4e6b30b7"
+            ],
+            "index": "pypi",
+            "version": "==1.32.0"
+        },
         "yapf": {
             "hashes": [
-                "sha256:8fea849025584e486fd06d6ba2bed717f396080fd3cc236ba10cb97c4c51cf32",
-                "sha256:a3f5085d37ef7e3e004c4ba9f9b3e40c54ff1901cd111f05145ae313a7c67d1b"
+                "sha256:958587eb5c8ec6c860119a9c25d02addf30a44f75aa152a4220d30e56a98037c",
+                "sha256:b8bfc1f280949153e795181768ca14ef43d7312629a06c43e7abd279323af313"
             ],
             "index": "pypi",
-            "version": "==0.32.0"
+            "version": "==0.40.1"
         },
         "yaspin": {
             "hashes": [
                 "sha256:17b5548479b3d5b30adec7a87ffcdcddb403d14a2bb86fbcee97f37951e13427",
                 "sha256:547afd1a9700ac3a29a9f5591c70343bef186ed5dfb5e545a9bb0c77e561a1c9"
             ],
             "index": "pypi",
@@ -1545,15 +1527,15 @@
         },
         "yojenkins": {
             "editable": true,
             "path": "."
         },
         "zipp": {
             "hashes": [
-                "sha256:23f70e964bc11a34cef175bc90ba2914e1e4545ea1e3e2f67c079671883f9cb6",
-                "sha256:e8b2a36ea17df80ffe9e2c4fda3f693c3dad6df1697d3cd3af232db680950b0b"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.13.0"
+            "version": "==3.15.0"
         }
     }
 }
```

### Comparing `yojenkins-0.0.85/README.md` & `yojenkins-0.0.86/README.md`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/pyproject.toml` & `yojenkins-0.0.86/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/setup.py` & `yojenkins-0.0.86/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import sys
 
 import setuptools
 
 # Package version number (Updated via bump2version tool)
-__version__ = "0.0.85"
+__version__ = "0.0.86"
 
 def check_py_version():
     """Check the python version"""
     if sys.version_info < (3, 7):
         print('Your Python version ({}.{}) is not supported'.format(sys.version_info.major, sys.version_info.minor))
         print('You must have Python version 3.7 or higher to run this program')
         if sys.version_info.major < 3:
```

### Comparing `yojenkins-0.0.85/yojenkins/__main__.py` & `yojenkins-0.0.86/yojenkins/__main__.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_account.py` & `yojenkins-0.0.86/yojenkins/cli/cli_account.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_auth.py` & `yojenkins-0.0.86/yojenkins/cli/cli_auth.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_build.py` & `yojenkins-0.0.86/yojenkins/cli/cli_build.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_credential.py` & `yojenkins-0.0.86/yojenkins/cli/cli_credential.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_decorators.py` & `yojenkins-0.0.86/yojenkins/cli/cli_decorators.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_folder.py` & `yojenkins-0.0.86/yojenkins/cli/cli_folder.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_job.py` & `yojenkins-0.0.86/yojenkins/cli/cli_job.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_node.py` & `yojenkins-0.0.86/yojenkins/cli/cli_node.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_server.py` & `yojenkins-0.0.86/yojenkins/cli/cli_server.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_stage.py` & `yojenkins-0.0.86/yojenkins/cli/cli_stage.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_step.py` & `yojenkins-0.0.86/yojenkins/cli/cli_step.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_tools.py` & `yojenkins-0.0.86/yojenkins/cli/cli_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tools Menu CLI Entrypoints"""
 
 import json
 import logging
 import os
 import sys
 from pathlib import Path
-from typing import NoReturn, Union
+from typing import Any, Dict, List, NoReturn, Union
 
 import click
 
 from yojenkins.cli import cli_utility as cu
 from yojenkins.cli.cli_utility import log_to_history
 from yojenkins.tools import Package, SharedLibrary
 from yojenkins.utility.utility import (
@@ -72,15 +72,15 @@
     """
     if click.confirm('Are you sure you want to remove yojenkins?'):
         Package.uninstall()
 
 
 @log_to_history
 def bug_report() -> None:
-    """TODO Docstring
+    """Report a bug for yojenkins.
 
     Details: TODO
 
     Args:
         TODO
     """
     logger.debug(f'Opening bug report webpage in web browser: "{BUG_REPORT_URL}" ...')
@@ -89,15 +89,15 @@
         logger.debug('Successfully opened in web browser')
     else:
         logger.debug('Failed to open in web browser')
 
 
 @log_to_history
 def feature_request() -> None:
-    """TODO Docstring
+    """Request a new feature for yojenkins.
 
     Details: TODO
 
     Args:
         TODO
     """
     logger.debug(f'Opening feature request webpage in web browser: "{FEATURE_REQUEST_URL}" ...')
@@ -105,66 +105,66 @@
     if success:
         logger.debug('Successfully opened in web browser')
     else:
         logger.debug('Failed to open in web browser')
 
 
 def history(profile: str, clear: bool) -> None:
-    """Displaying the command history and clearing the history file if requested.
+    """Display the command history and clearing the history file if requested.
 
     ### TODO: Ability to clear only for a specific profile.
 
     Args:
         profile: The name of the profile to to filter history with
         clear:   Clearing the history file
     """
-    # Load contents from history file
     history_file_path = os.path.join(os.path.join(Path.home(), cu.CONFIG_DIR_NAME), cu.HISTORY_FILE_NAME)
-    contents = load_contents_from_local_file('json', history_file_path)
-    if not contents:
-        click.secho('No history found', fg='bright_red', bold=True)
-        sys.exit(1)
 
     # Clearing the history file if requested
     if clear:
         logger.debug(f'Removing history file: {history_file_path} ...')
         try:
             os.remove(history_file_path)
         except (OSError, IOError, PermissionError) as error:
             fail_out(f'Failed to clear history file. Exception: {error}')
         logger.debug('Successfully cleared history file')
         click.secho('success', fg='bright_green', bold=True)
         sys.exit(0)
 
+    # Load contents from history file
+    contents = load_contents_from_local_file('jsonl', history_file_path)
+    if not contents:
+        click.secho('No history found', fg='bright_red', bold=True)
+        sys.exit(1)
+
     # Displaying the command history
     logger.debug(f'Displaying command history for profile "{profile}" ...')
 
-    def output_history_to_console(command_list: list, profile_name: str) -> None:
-        """Helper function to format and output to console"""
+    def output_history_to_console(command_list: List, profile_name: str = "") -> None:
+        """Help to format and output to console."""
         for command_info in command_list:
-            profile_str = f'{click.style("[" + profile_name + "]", fg="yellow", bold=True)}'
+            if profile_name:
+                if command_info["profile"] != profile_name:
+                    continue
+            profile_str = f'{click.style("[" + command_info["profile"] + "]", fg="yellow", bold=True)}'
             datetime_str = f'{click.style("[" + command_info["datetime"] + "]", fg="green", bold=False)}'
             tool_version = f'{click.style("[" + "v" + command_info["tool_version"] + "]", fg="green", bold=False)}'
 
             command_info = f'{profile_str} {datetime_str} {tool_version} - {command_info["tool_path"]} {command_info["arguments"]}'
             click.echo(command_info)
 
     if profile:
-        if profile in contents:
-            output_history_to_console(contents[profile], profile)
-        else:
-            fail_out(f'No history found for profile: {profile}')
+        output_history_to_console(contents, profile)
     else:
-        for profile_name in contents:
-            output_history_to_console(contents[profile_name], profile_name)
+        output_history_to_console(contents)
 
 
 @log_to_history
 def rest_request(profile: str, token: str, request_text: str, request_type: str, raw: bool, clean_html: bool) -> None:
-    """Send a generic REST request to Jenkins Server using the loaded credentials
+    """Send a generic REST request to Jenkins Server using the loaded credentials.
 
     Args:
         profile: The name of the credentials profile
         token:   API token for Jenkins server
         request_text: The text of the request to send
         request_type: The type of request to send
         raw: Whether to return the raw response or formatted JSON
```

### Comparing `yojenkins-0.0.85/yojenkins/cli/cli_utility.py` & `yojenkins-0.0.86/yojenkins/cli/cli_utility.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 from yojenkins.utility.utility import iter_data_empty_item_stripper, load_contents_from_local_file, am_i_inside_docker, am_i_bundled, print2, create_new_history_file  # isort:skip
 
 # Getting the logger reference
 logger = logging.getLogger()
 
 CONFIG_DIR_NAME = '.yojenkins'
-HISTORY_FILE_NAME = 'history'
-COMMAND_HISTORY_FORMAT = 'json'
+HISTORY_FILE_NAME = 'history.jsonl'
+COMMAND_HISTORY_FORMAT = 'jsonl'
 DEFAULT_PROFILE_NAME = 'default'
 MAX_PROFILE_HISTORY_LENGTH = 1000
 
 CLI_CMD_PATH = sys.argv[0]
 CLI_CMD_ARGS = ' '.join([quote(arg) for arg in sys.argv[1:]])
 
 
@@ -191,24 +191,24 @@
 
 def server_target_check(target: str) -> bool:
     """TODO"""
     pass
 
 
 def log_to_history(decorated_function) -> Callable:
-    """This function decorates a function that is a cli command.
+    """Decorate/wrap a function that is a cli command.
     The function will log the CLI command and its info to the command history.
 
     Details: Add this function like "@log_to_history" to a function
 
     Args:
         decorated_function : Function that is decorated
 
     Returns:
-        None
+        The decorated function
     """
     # Get the profile argument index
     argspec = getfullargspec(decorated_function)
     try:
         arg_index = argspec.args.index('profile')
     except ValueError:
         arg_index = -1
@@ -223,46 +223,32 @@
             # If no profile is used by the decorated function, use the default profile name
             profile_name = DEFAULT_PROFILE_NAME
 
         if profile_name is None:
             # If function has profile argument, but none was passed, use the default profile name
             profile_name = DEFAULT_PROFILE_NAME
 
-        # Check if history file exists
+        # Check if history file exists, if not create it
         history_file_path = os.path.join(os.path.join(Path.home(), CONFIG_DIR_NAME), HISTORY_FILE_NAME)
         if not os.path.isfile(history_file_path):
             create_new_history_file(history_file_path)
 
-        # Load the history file content
-        file_contents = load_contents_from_local_file(COMMAND_HISTORY_FORMAT, history_file_path)
-        if not file_contents:
-            logger.debug("Command history file is blank")
-
-        # If profile history length is too long, remove the oldest history item
-        if profile_name in file_contents:
-            if len(file_contents[profile_name]) > MAX_PROFILE_HISTORY_LENGTH:
-                file_contents[profile_name].pop(0)
-
-        # Add the command to the history file
         logger.debug(f'Logging command to command history file: "{history_file_path}" ...')
-        if profile_name not in file_contents:
-            file_contents[profile_name] = []
-
         command_info = {
+            'profile': profile_name,
             'tool_path': CLI_CMD_PATH,
             'arguments': CLI_CMD_ARGS,
             'timestamp': datetime.now().timestamp(),
             'datetime': datetime.now().strftime("%A, %B %d, %Y %I:%M:%S"),
             'tool_version': __version__
         }
-        file_contents[profile_name].append(command_info)
 
-        # Add to file, overwritting entire file
+        # Add line to history file
         try:
-            with open(history_file_path, 'w') as outfile:
-                json.dump(file_contents, outfile, indent=4)
+            with open(history_file_path, 'a', encoding="utf-8") as outfile:
+                outfile.write(json.dumps(command_info) + '\n')
         except Exception as error:
             logger.debug(f'Failed to write command history file: {error}')
 
         return decorated_function(*args, **kwargs)
 
     return wrapper
```

### Comparing `yojenkins-0.0.85/yojenkins/cli/logger_setup.py` & `yojenkins-0.0.86/yojenkins/cli/logger_setup.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/account.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/account.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/auth.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/auth.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/build.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/build.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/credential.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/credential.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/folder.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/folder.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/job.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/job.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/node.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/node.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/server.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/server.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/stage.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/stage.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/step.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/step.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/cli_sub_commands/tools.py` & `yojenkins-0.0.86/yojenkins/cli_sub_commands/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 @tools.command(short_help='\tShow detailed command usage history')
 @cli_decorators.debug
 @click.option('--profile', type=str, required=False, is_flag=False, help='Filter by profile name')
 @click.option('--clear', type=bool, required=False, default=False, is_flag=True, help='Clear the history file')
 def history(debug, **kwargs):
-    """Show detailed command usage history"""
+    """Show detailed command usage history."""
     set_debug_log_level(debug)
     cli_tools.history(**kwargs)
 
 
 @tools.command(short_help='\tSend a generic Rest request to server')
 @cli_decorators.debug
 @cli_decorators.profile
```

### Comparing `yojenkins-0.0.85/yojenkins/docker_container/docker_jenkins_server.py` & `yojenkins-0.0.86/yojenkins/docker_container/docker_jenkins_server.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/monitor/build_monitor.py` & `yojenkins-0.0.86/yojenkins/monitor/build_monitor.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/monitor/folder_monitor.py` & `yojenkins-0.0.86/yojenkins/monitor/folder_monitor.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/monitor/job_monitor.py` & `yojenkins-0.0.86/yojenkins/monitor/job_monitor.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/monitor/monitor.py` & `yojenkins-0.0.86/yojenkins/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/monitor/monitor_utility.py` & `yojenkins-0.0.86/yojenkins/monitor/monitor_utility.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/resources/scripts/node_prepare_amazonlinux2.sh` & `yojenkins-0.0.86/yojenkins/resources/scripts/node_prepare_amazonlinux2.sh`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/resources/server_docker_settings/Dockerfile` & `yojenkins-0.0.86/yojenkins/resources/server_docker_settings/Dockerfile`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/resources/server_docker_settings/config_as_code.yaml` & `yojenkins-0.0.86/yojenkins/resources/server_docker_settings/config_as_code.yaml`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/resources/server_docker_settings/plugins.txt` & `yojenkins-0.0.86/yojenkins/resources/server_docker_settings/plugins.txt`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/resources/sound/negative_alert_wooden_mallet_fast_negative_error_two_tone.wav` & `yojenkins-0.0.86/yojenkins/resources/sound/negative_alert_wooden_mallet_fast_negative_error_two_tone.wav`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/resources/sound/negative_notification_mallet_wooden_short_alert.wav` & `yojenkins-0.0.86/yojenkins/resources/sound/negative_notification_mallet_wooden_short_alert.wav`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/resources/sound/negative_ui_ping_chime_mallet_like.wav` & `yojenkins-0.0.86/yojenkins/resources/sound/negative_ui_ping_chime_mallet_like.wav`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/resources/sound/negative_ui_ping_chime_mallet_like_error.wav` & `yojenkins-0.0.86/yojenkins/resources/sound/negative_ui_ping_chime_mallet_like_error.wav`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/resources/sound/positive_alert_mallet_wood_simple_musical_003.wav` & `yojenkins-0.0.86/yojenkins/resources/sound/positive_alert_mallet_wood_simple_musical_003.wav`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/resources/sound/positive_alert_notification_musical_short_marimba_process_finished.wav` & `yojenkins-0.0.86/yojenkins/resources/sound/positive_alert_notification_musical_short_marimba_process_finished.wav`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/tools/package.py` & `yojenkins-0.0.86/yojenkins/tools/package.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/tools/shared_library.py` & `yojenkins-0.0.86/yojenkins/tools/shared_library.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/utility/utility.py` & `yojenkins-0.0.86/yojenkins/utility/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""General utility and tools"""
+"""General utility and tools."""
 
 import difflib
 import json
 import logging
 import os
 import re
 import sys
 import sysconfig
 import time
 import webbrowser
 from pathlib import Path
 from string import Template
-from typing import Any, Dict, List, Set, Tuple, Union
+from typing import Any, Dict, List, Literal, Set, Tuple, Union
 from urllib.parse import urljoin, urlparse
 
 import requests
 import toml
 import xmltodict
 import yaml
 from click import echo, secho, style
@@ -37,30 +37,29 @@
     "list": "opt_list",
     "json": "opt_json",
     "id": "opt_id",
 }
 
 
 class TextStyle:
-    """Text style definitions"""
+    """Text style definitions."""
 
     HEADER = "\033[95m"
     BLUE = "\033[94m"
     CYAN = "\033[96m"
     GREEN = "\033[92m"
     YELLOW = "\033[93m"
     RED = "\033[91m"
     BOLD = "\033[1m"
     UNDERLINE = "\033[4m"
     NORMAL = "\033[0m"
 
 
 def translate_kwargs(original_kwargs: Dict[str, Any]) -> Dict[str, Any]:
-    """Rename the key names of the provided kwargs based on
-    a set of translation rules.
+    """Rename the key names of the provided kwargs based on a set of translation rules.
 
     Details: This is primarirly used if kwarg keys are named like
              a module or python native object.
              Examples:
                 - pretty -> opt_pretty
                 - json -> opt_json
 
@@ -76,15 +75,15 @@
             new_kwargs[KWARG_TRANSLATE_MAP[key]] = value
         else:
             new_kwargs[key] = value
     return new_kwargs
 
 
 def print2(message: str, bold: bool = False, color: str = "reset") -> None:
-    """Print a message to the console using click
+    """Print a message to the console using click.
 
     Details:
         - Colors: `black` (might be a gray), `red`, `green`, `yellow` (might be an orange), `blue`,
           `magenta`, `cyan`, `white` (might be light gray), `reset` (reset the color code only)
 
     Example Usage:
         - `print2("Hey there!", bold=True, color="green")`
@@ -94,80 +93,82 @@
         bold   : Whether to bold the message
         color  : Color to use for the message ()
     """
     echo(style(message, fg=color, bold=bold))
 
 
 def fail_out(message: str) -> None:
-    """Output one failure message to the console, then exit
+    """Output one failure message to the console, then exit.
 
     Example Usage:
         - `fail_out("Something went wrong!")`
 
     Args:
         message: Message to output to console
     """
     echo(style(message, fg="bright_red", bold=True))
     sys.exit(1)
 
 
 def failures_out(messages: list) -> None:
-    """Output multiple failure messages to the console, then exit
+    """Output multiple failure messages to the console, then exit.
 
     Example Usage:
         - `failures_out(["Oh no!", "This is not good!"])`
 
     Args:
         message: Multiple messages to output to console
     """
     for message in messages:
         echo(style(message, fg="bright_red", bold=True))
     sys.exit(1)
 
 
-def load_contents_from_local_file(file_type: str, local_file_path: str) -> Dict:
-    """Loading a local file contents
+def load_contents_from_local_file(file_type: Literal['yaml', 'toml', 'json', 'jsonl'],
+                                  local_file_path: str) -> Union[Dict, List]:
+    """Load a local file contents.
 
     ### TODO: Add default option to load file as plain text
 
     Parameters:
-        file_type (str)       : Type of file to be loaded ie. 'yaml', 'toml', 'json'
-        local_file_path (str) : Path to a local TOML file to be loaded
+        file_type       : Type of file to be loaded (ie. json)
+        local_file_path : Path to a local TOML file to be loaded
     Returns:
-        file_contents (dict) : The contents of file
+        file_contents
     """
-    file_type = file_type.lower()
-
     # Check if file exists
     if not os.path.isfile(local_file_path):
         fail_out(f"Failed to find file: {local_file_path}")
 
     # Check if file is completely empty
     if os.stat(local_file_path).st_size == 0:
         return {}
 
     logger.debug(f"Loading specified local .{file_type} file: '{local_file_path}' ...")
+    file_contents: Union[List, Dict] = {}
     try:
         with open(local_file_path, "r") as open_file:
             if file_type == "yaml":
                 file_contents = yaml.safe_load(open_file)
             elif file_type == "toml":
                 file_contents = toml.load(open_file)
             elif file_type == "json":
                 file_contents = json.loads(open_file.read())
+            elif file_type == "jsonl":
+                file_contents = [json.loads(line) for line in open_file]
             else:
                 raise ValueError(f"Unknown file type passed: '{file_type}'")
         logger.debug(f"Successfully loaded local .{file_type} file")
     except Exception as error:
         fail_out(f"Failed to load specified local .{file_type} file: '{local_file_path}'. Exception: {error}")
     return file_contents
 
 
 def load_contents_from_string(file_type: str, text: str) -> Dict:
-    """Loading a local file contents
+    """Load a local file contents.
 
     Parameters:
         file_type (str) : Type of file to be loaded ie. 'yaml', 'toml', 'json'
         text (str)      : Text string to be loaded as specified filetype
     Returns:
         contents (dict) : The contents of file
     """
@@ -182,15 +183,15 @@
     else:
         raise ValueError(f'Unknown file type passed: "{file_type}"')
     logger.debug(f'Successfully loaded specified "{file_type}" contents from text string')
     return contents
 
 
 def load_contents_from_remote_file_url(file_type: str, remote_file_url: str, allow_redirects: bool = True) -> Dict:
-    """Loading a remote yaml file contents over HTTP
+    """Load a remote yaml file contents over HTTP.
 
     ### FIXME: Make it able to load toml, json, and yaml file types
 
     Args:
         file_type (str)       : Type of file to be loaded ie. 'yaml', 'toml', 'json'
         remote_file_url (url)  : Remote URL location of file to be loaded
         allow_redirects (bool) : If True allow redirects to another URL (default True)
@@ -329,15 +330,15 @@
     for key in dict_to_check:  # Looping top level dict keys
         if key in list_items:  # Check if the key is in one of the list items
             return list_items.index(key)
     return None
 
 
 def iter_data_empty_item_stripper(iter_data: Union[Dict, List, Set, Tuple]) -> Union[Dict, List, Set, Tuple]:
-    """Removes any empty data from a nested or un-nested iter item (list, dict, set, etc)
+    """Remove any empty data from a nested or un-nested iter item (list, dict, set, etc).
 
     Details: https://stackoverflow.com/a/27974027/11294572
 
     Args:
         iter_data : data in the from of iterable (ie. list, dict, set, etc)
 
     Returns:
@@ -353,33 +354,32 @@
         }
     if isinstance(iter_data, list):
         return [value for value in map(iter_data_empty_item_stripper, iter_data) if value not in empties]
     return iter_data
 
 
 def is_credential_id_format(text: str) -> bool:
-    """Checking if the passed text is in Jenkins credential ID format
+    """Check if the passed text is in Jenkins credential ID format.
 
     Args:
         text: The text to check
 
     Returns:
         True if the text is in credential ID format, else False
     """
     regex_pattern = (r"^[a-zA-Z0-9]{8}-[a-zA-Z0-9]{4}-[a-zA-Z0-9]{4}-[a-zA-Z0-9]{4}-[a-zA-Z0-9]{12}$")
     cred_match = re.match(regex_pattern, text)
     if cred_match:
         logger.debug(f"Successfully identified credential ID format")
-    else:
-        logger.debug(f"Failed to identify credential ID format")
-    return cred_match
+        return True
+    return False
 
 
 def is_full_url(url: str) -> bool:
-    """Check if passed string is a valid and full URL
+    """Check if passed string is a valid and full URL.
 
     Args:
         url: The text to check
 
     Returns:
         True if valid and full URL, else False
     """
@@ -395,15 +395,15 @@
     logger.debug(f'    - netloc:  {parsed_url.netloc} - {"OK" if parsed_url.netloc else "MISSING"}')
     logger.debug(f'    - path:    {parsed_url.path} - {"OK" if parsed_url.path else "MISSING"}')
 
     return is_valid_url
 
 
 def url_to_name(url: str) -> str:
-    """Convert the jenkins item URL to its name
+    """Convert the jenkins item URL to its name.
 
     Args:
         url : URL of the item (ie. folder, job, build)
 
     Returns:
         The full name of the item
     """
@@ -420,15 +420,15 @@
     name = "/".join(filtered_list)
 
     logger.debug(f'Converted URL "{url}" to fullname "{name}"')
     return name
 
 
 def format_name(name: str) -> str:
-    """Format / clean up the passed name
+    """Format / clean up the passed name.
 
     Details: The formatting includes it:
         - /Non-PAR/job/Non-Prod-Jobs/job/Something/job/job --> /Non-PAR/Non-Prod-Jobs/Something/job
         - remove `job/`, `view/`, `change-requests/`
         - remove leading or trailing `/`
 
     Args:
@@ -443,15 +443,15 @@
                                                                              "").replace("change-requests/", ""))
 
     logger.debug(f'Formatted "{name}" to "{name_formatted}"')
     return name_formatted
 
 
 def fullname_to_name(fullname: str) -> str:
-    """Convert the jenkins item full name to its name only
+    """Convert the jenkins item full name to its name only.
 
     Details: Hey/This/Is/A/Full/Job --> Job
 
     Args:
         url : Full name of the item (ie. Hey/This/Is/A/Full/Job)
 
     Returns:
@@ -459,15 +459,15 @@
     """
     name = fullname.strip().strip("/").split("/")[-1]
     logger.debug(f'Converted fullname "{fullname}" to name "{name}"')
     return name
 
 
 def name_to_url(server_base_url: str, name: str) -> str:
-    """Convert the item name to URL
+    """Convert the item name to URL.
 
     ** TODO **
 
     NOTE: Passed '.' will go to base url
 
     Args:
         name : The name of the item
@@ -487,15 +487,15 @@
     url = str(urljoin(server_base_url, short_name))
     logger.debug(f'Converted name "{name}" to URL "{url}"')
 
     return url
 
 
 def build_url_to_other_url(build_url: str, target_url: str = "job") -> str:
-    """From build_url get job or folder url
+    """From build_url get job or folder url.
 
     Args:
         build_url  : The URL of the build
         target_url : URL to derive. `job` or `folder` (default: `job`)
 
     Returns:
         The URL of the job or folder
@@ -522,15 +522,16 @@
     result_url = urljoin(base_url, path_new) + "/"
     logger.debug(f'From build URL "{build_url}" extracted {target_url} URL "{result_url}"')
 
     return result_url
 
 
 def build_url_to_build_number(build_url: str) -> Union[int, None]:
-    """If possible, extract the build number from a passed Jenkins URL
+    """If possible, extract the build number from a passed Jenkins URL.
+
     In order to extract the build number, the passed URL must be related to the
     build (ie. URL of build logs)
 
     Args:
         build_url : URL of anything build related
 
     Example Usage:
@@ -557,15 +558,15 @@
             build_number = None
 
     logger.debug(f'From build URL "{build_url}" extracted build number "{build_number}"')
     return build_number
 
 
 def is_complete_build_url(build_url: str) -> bool:
-    """Check if passed URL is a complete and valid build URL
+    """Check if passed URL is a complete and valid build URL.
 
     Args:
         build_url : URL of anything build related
 
     Returns:
         True if valid and complete, else False
     """
@@ -580,14 +581,15 @@
     except (ValueError, IndexError):
         is_complete = False
     return is_complete
 
 
 def build_url_complete(build_url: str) -> Union[str, None]:
     """If possible, extract only the build URL from a passed Jenkins URL.
+
     Will try to truncate anything after the build number.
     In order to extract the complete build URL, the passed URL must be related to the
     build (ie. URL of build logs).
 
     Args:
         build_url : URL of anything build related
 
@@ -631,15 +633,15 @@
     build_url_complete = urljoin(base_url, path_new) + "/"
 
     logger.debug(f'Extracted complete build URL "{build_url_complete}" from "{build_url}"')
     return build_url_complete
 
 
 def item_url_to_server_url(url: str, include_scheme: bool = True) -> str:
-    """From build_url get job or folder url
+    """From build_url get job or folder url.
 
     Args:
         url            : The URL of the build
         include_scheme : If True, include protocol scheme (ie. `https://`) (default: `True`)
 
     Returns:
         The URL of the server
@@ -649,43 +651,43 @@
         server_url = url_parsed.scheme + "://" + url_parsed.netloc
     else:
         server_url = url_parsed.netloc
     return server_url
 
 
 def has_build_number_started(job_info: dict, build_number: int) -> bool:
-    """Given the job info, check if build number has been started/run
+    """Given the job info, check if build number has been started/run.
 
     Args:
         job_info     : The job information
         build_number : The build number to be looked up
 
     Returns:
         True if build number has starated, else false
     """
     if "builds" not in job_info:
         return False
     for build in job_info["builds"]:
         if not "number" in build:
             continue
         if build["number"] == build_number:
-            logger.debug(f"Successfully found tha build {build_number} was previously started")
+            logger.debug(f"Successfully found the build {build_number} was previously started")
             return True
     logger.debug(f"Failed to find build {build_number} was previously started")
     return False
 
 
 def item_subitem_list(
     item_info: Dict,
     get_key_info: str,
     item_type: str,
     item_class_list: list = [],
     item_class_key: str = "_class",
 ) -> Tuple[list, list]:
-    """Given a item (job, build, etc) info, get the sub-items matching criteria
+    """Given a item (job, build, etc) info, get the sub-items matching criteria.
 
     Details: <DETAILED DESCRIPTION>
 
     Args:
         item_info       : Info dict of the item
         get_key_info    : The key value to get (ie. `url`, `name`)
         item_type       : Class type of sub-item to be matched (ie. `com.cloudbees.hudson.plugins.folder.Folder`) - See `JenkinsItemClasses.py`
@@ -710,16 +712,16 @@
     else:
         return [], []
 
     return item_list, item_name_list
 
 
 def to_seconds(time_quantity: int, time_unit_text: str) -> int:
-    """
-    Get the number of seconds from the time quantity and time unit type.
+    """Get the number of seconds from the time quantity and time unit type.
+
     Examples:
         - 45 min -> 2700 seconds
         - 2 days -> 432000 seconds
 
     Parameters:
         time_quantity (int)  : Number of time units
         time_unit_text (str) : Type of time units (ie. seconds, minutes, hours, etc)
@@ -745,15 +747,15 @@
         blue_moon = 41  # months
         return int(time_quantity * blue_moon * 2.628e6)
 
     return 0
 
 
 def html_clean(html: str) -> str:
-    """Clean up HTML format to text without HTML tags
+    """Clean up HTML format to text without HTML tags.
 
     Args:
         html : HTML content
 
     Returns:
         Cleaned text
     """
@@ -768,15 +770,15 @@
     cleaned_text = cleaned_text.replace("&nbsp;", "")
     cleaned_text = cleaned_text.replace("&amp;", "&")  # This has to be last
 
     return cleaned_text
 
 
 def browser_open(url: str, new: int = 2, autoraise: bool = True) -> bool:
-    """Clean up HTML format to text without HTML tags
+    """Clean up HTML format to text without HTML tags.
 
     Args:
         url       : Weblink URL
         new       : 0=Same browser window, 1=New browser window, 2=New Tab
         autoraise : True=Window is raised
 
     Returns:
@@ -787,15 +789,15 @@
     except Exception as error:
         logger.debug(f'Failed to open web browser for URL: {url.strip("/")}  Exception: {error}')
         return False
     return True
 
 
 def has_special_char(text: str, special_chars: str = "@!#$%^&*<>?/\|~:") -> bool:
-    """Check if passed text string contains any special characters
+    """Check if passed text string contains any special characters.
 
     Args:
         text          : Text to check
         special_chars : String with all special characters to check
 
     Returns:
         True if includes special characters, else False
@@ -806,15 +808,15 @@
         logger.debug(f'Item "{text}" includes special characters. Special characters: {special_chars}')
     else:
         logger.debug(f'Item "{text}" does not include special characters. Special characters: {special_chars}')
     return includes_special_chars
 
 
 def remove_special_char(text: str, special_chars: str = "@!#$%^&*<>?/\|~:") -> str:
-    """Remove any special characters from text string
+    """Remove any special characters from text string.
 
     Args:
         text          : Text to remove special characters from
         special_chars : String with all special characters to remove
 
     Returns:
         Text with special characters removed
@@ -822,15 +824,15 @@
     regex = re.compile("[" + special_chars + "]")
     text_new = re.sub(regex, "", text)
     logger.debug(f'Removed special characters "{special_chars}" from string')
     return text_new
 
 
 def queue_find(all_queue_info: dict, job_name: str = "", job_url: str = "", first: bool = True) -> list:
-    """Finding job in server build queue
+    """Find job in server build queue.
 
     Args:
         TODO
 
     Returns:
         TODO
     """
@@ -987,15 +989,15 @@
 
     Returns:
         True if running bundled, else False
     """
     return getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS")
 
 
-def parse_and_check_input_string_list(string_list: str, join_back_char: str = "", split_char: str = ",") -> list:
+def parse_and_check_input_string_list(string_list: str, join_back_char: str = "", split_char: str = ",") -> List[str]:
     """Parsing a string list into a list of strings
 
     Details:
         - `parse_string_list('a,b,c')` => ['a', 'b', 'c']
         - `parse_string_list('a,b,c', join_back_char=';')` => ['a;b;c']
 
     Args:
@@ -1215,31 +1217,30 @@
 
 
 def create_new_history_file(file_path: str) -> None:
     """Create a new blank command history file.
 
     Args:
         file_path: Full path to the history file
-
-    Returns:
-        None
     """
     try:
         # Creating configuration directory if it does not exist
         config_dir_abs_path = os.path.join(Path.home(), CONFIG_DIR_NAME)
 
         if not os.path.exists(config_dir_abs_path):
             logger.debug("Configuration directory does not exist. Creating it ...")
             os.makedirs(config_dir_abs_path)
 
         if not os.path.exists(file_path):
             logger.debug(f'Command history file NOT found: "{file_path}"')
             logger.debug("Creating a new command history file ...")
+
         with open(file_path, "w") as open_file:
-            json.dump({}, open_file)
+            # json.dump({}, open_file)
+            open_file.write("")
 
     except (FileNotFoundError, IOError, PermissionError) as error:
         fail_out(f"Failed to create history file ({file_path}). Exception: {error}")
     except Exception as error:
         logger.exception(f"Failed to create new command history file. Exception: {error}")
 
 
@@ -1292,15 +1293,15 @@
     label_2: str,
     line_pattern: tuple,
     char_ignore: int,
     no_color: bool,
     diff_only: bool,
     diff_guide: bool,
 ) -> None:
-    """Display/Show line diffs between two specified texts
+    """Display/Show line diffs between two specified texts.
 
     Args:
         text_1:       String text 1
         text_2:       String text 2 to compare to text 1
         label_1:      text_1 label/description
         label_2:      text_2 label/description
         line-pattern: Patterns to consider for diff for each line
```

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/account.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/account.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/auth.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/auth.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/build.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/build.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/credential.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/credential.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/folder.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/folder.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/user_create.groovy` & `yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/user_create.groovy`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/user_delete.groovy` & `yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/user_delete.groovy`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/user_list.groovy` & `yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/user_list.groovy`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/user_permission_add_remove.groovy` & `yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/user_permission_add_remove.groovy`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/groovy_scripts/user_permission_list.groovy` & `yojenkins-0.0.86/yojenkins/yo_jenkins/groovy_scripts/user_permission_list.groovy`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/jenkins_item_classes.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/jenkins_item_classes.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/jenkins_item_config.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/jenkins_item_config.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/jenkins_item_template.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/jenkins_item_template.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/job.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/job.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/node.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/node.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/rest.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/rest.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/server.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/server.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/stage.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/stage.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/status.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/status.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/step.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/step.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins/yo_jenkins/yojenkins.py` & `yojenkins-0.0.86/yojenkins/yo_jenkins/yojenkins.py`

 * *Files identical despite different names*

### Comparing `yojenkins-0.0.85/yojenkins.egg-info/PKG-INFO` & `yojenkins-0.0.86/yojenkins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yojenkins
-Version: 0.0.85
+Version: 0.0.86
 Summary: A CLI tool to manage and have fun with Jenkins server
 Home-page: https://github.com/ismet55555/yojenkins
 Author: Ismet Handzic
 Author-email: ismet.handzic@gmail.com
 Maintainer: Ismet Handzic
 Keywords: jenkins monitor manage job build fun
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yojenkins Version: 0.0.85 Summary: A CLI tool to
+Metadata-Version: 2.1 Name: yojenkins Version: 0.0.86 Summary: A CLI tool to
 manage and have fun with Jenkins server Home-page: https://github.com/
 ismet55555/yojenkins Author: Ismet Handzic Author-email:
 ismet.handzic@gmail.com Maintainer: Ismet Handzic Keywords: jenkins monitor
 manage job build fun Classifier: Development Status :: 3 - Alpha Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Intended Audience :: System Administrators Classifier:
 Intended Audience :: Developers Classifier: Topic :: Utilities Classifier:
```

### Comparing `yojenkins-0.0.85/yojenkins.egg-info/SOURCES.txt` & `yojenkins-0.0.86/yojenkins.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 Pipfile
 Pipfile.lock
 README.md
 pyproject.toml
 setup.py
-tests/test_test.py
 yojenkins/__init__.py
 yojenkins/__main__.py
 yojenkins.egg-info/PKG-INFO
 yojenkins.egg-info/SOURCES.txt
 yojenkins.egg-info/dependency_links.txt
 yojenkins.egg-info/entry_points.txt
 yojenkins.egg-info/requires.txt
```

