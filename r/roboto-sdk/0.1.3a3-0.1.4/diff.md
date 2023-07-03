# Comparing `tmp/roboto_sdk-0.1.3a3.tar.gz` & `tmp/roboto_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_sdk-0.1.3a3.tar", max compression
+gzip compressed data, was "roboto_sdk-0.1.4.tar", max compression
```

## Comparing `roboto_sdk-0.1.3a3.tar` & `roboto_sdk-0.1.4.tar`

### file list

```diff
@@ -1,87 +1,122 @@
--rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.3a3/README.md
--rw-r--r--   0        0        0      949 2023-07-03 17:26:10.562107 roboto_sdk-0.1.3a3/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-03 16:08:19.143854 roboto_sdk-0.1.3a3/src/roboto_sdk/__init__.py
--rw-r--r--   0        0        0       48 2023-07-03 16:08:19.141092 roboto_sdk-0.1.3a3/src/roboto_sdk/auth/__init__.py
--rw-r--r--   0        0        0     4037 2023-07-03 16:08:19.139811 roboto_sdk-0.1.3a3/src/roboto_sdk/auth/pat.py
--rw-r--r--   0        0        0      132 2023-07-03 16:08:19.152003 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/__init__.py
--rw-r--r--   0        0        0      334 2023-07-03 16:08:19.162015 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/command/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-03 16:08:19.164617 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/command/args.py
--rw-r--r--   0        0        0     2058 2023-07-03 16:28:40.380758 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/command/model.py
--rw-r--r--   0        0        0      822 2023-07-03 16:28:40.367049 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/context.py
--rw-r--r--   0        0        0      110 2023-07-03 16:08:19.148587 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/datasets/__init__.py
--rw-r--r--   0        0        0     6714 2023-07-03 16:08:19.150367 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/datasets/commands.py
--rw-r--r--   0        0        0     3659 2023-07-03 17:26:31.317426 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/entry.py
--rw-r--r--   0        0        0      108 2023-07-03 16:08:19.168666 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/help/__init__.py
--rw-r--r--   0        0        0      167 2023-07-03 16:08:19.169956 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/help/args.py
--rw-r--r--   0        0        0      110 2023-07-03 16:08:19.153590 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/orgs/__init__.py
--rw-r--r--   0        0        0     3386 2023-07-03 16:08:19.155109 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/orgs/commands.py
--rw-r--r--   0        0        0      110 2023-07-03 16:08:19.165930 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/tokens/__init__.py
--rw-r--r--   0        0        0     3301 2023-07-03 16:08:19.167288 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2023-07-03 16:08:19.145458 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/triggers/__init__.py
--rw-r--r--   0        0        0     2874 2023-07-03 16:08:19.147004 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2023-07-03 16:08:19.159379 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/users/__init__.py
--rw-r--r--   0        0        0      733 2023-07-03 16:08:19.160698 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/users/commands.py
--rw-r--r--   0        0        0       48 2023-07-03 16:08:19.198130 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-03 16:08:19.224521 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/__init__.py
--rw-r--r--   0        0        0     7427 2023-07-03 16:28:40.375211 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action.py
--rw-r--r--   0        0        0     3015 2023-07-03 16:28:40.382505 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_delegate.py
--rw-r--r--   0        0        0     5168 2023-07-03 16:28:40.356951 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_http_delegate.py
--rw-r--r--   0        0        0      640 2023-07-03 16:28:40.365100 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_http_resources.py
--rw-r--r--   0        0        0      808 2023-07-03 16:28:40.372147 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_record.py
--rw-r--r--   0        0        0      106 2023-07-03 16:08:19.223131 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/error.py
--rw-r--r--   0        0        0     4499 2023-07-03 16:28:40.370371 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation.py
--rw-r--r--   0        0        0     1726 2023-07-03 16:28:40.384071 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_delegate.py
--rw-r--r--   0        0        0     4768 2023-07-03 16:28:40.366150 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      566 2023-07-03 16:30:28.384279 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_http_resources.py
--rw-r--r--   0        0        0     1652 2023-07-03 16:30:28.386808 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_record.py
--rw-r--r--   0        0        0      546 2023-07-03 16:08:19.192761 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/__init__.py
--rw-r--r--   0        0        0     9836 2023-07-03 16:28:40.373480 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/dataset.py
--rw-r--r--   0        0        0     2215 2023-07-03 16:28:40.371324 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/delegate.py
--rw-r--r--   0        0        0     4911 2023-07-03 16:28:40.387575 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/http_delegate.py
--rw-r--r--   0        0        0      340 2023-07-03 16:08:19.190087 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/http_resources.py
--rw-r--r--   0        0        0      867 2023-07-03 16:08:19.196854 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/record.py
--rw-r--r--   0        0        0      436 2023-07-03 16:08:19.238248 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/__init__.py
--rw-r--r--   0        0        0     1181 2023-07-03 16:28:40.353092 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/delegate.py
--rw-r--r--   0        0        0      802 2023-07-03 16:30:28.392185 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/file.py
--rw-r--r--   0        0        0     2166 2023-07-03 16:30:27.887912 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/http_delegate.py
--rw-r--r--   0        0        0      168 2023-07-03 16:08:19.235599 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/http_resources.py
--rw-r--r--   0        0        0      382 2023-07-03 16:08:19.242205 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/record.py
--rw-r--r--   0        0        0     2358 2023-07-03 16:30:27.887409 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/s3_delegate.py
--rw-r--r--   0        0        0      728 2023-07-03 16:08:19.204997 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/__init__.py
--rw-r--r--   0        0        0     1893 2023-07-03 16:28:40.348041 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/delegate.py
--rw-r--r--   0        0        0     4103 2023-07-03 16:28:40.383366 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      359 2023-07-03 16:08:19.200791 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     1815 2023-07-03 16:28:40.378431 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org.py
--rw-r--r--   0        0        0     1680 2023-07-03 16:28:40.364446 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org_invite.py
--rw-r--r--   0        0        0     1158 2023-07-03 16:28:40.351236 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org_role.py
--rw-r--r--   0        0        0      722 2023-07-03 16:08:19.209463 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/record.py
--rw-r--r--   0        0        0      387 2023-07-03 16:08:19.249174 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/__init__.py
--rw-r--r--   0        0        0      888 2023-07-03 16:28:40.360553 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/delegate.py
--rw-r--r--   0        0        0     2038 2023-07-03 16:28:40.386560 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      216 2023-07-03 16:30:28.394782 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      455 2023-07-03 16:30:28.399700 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/record.py
--rw-r--r--   0        0        0     1832 2023-07-03 16:30:28.395655 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/token.py
--rw-r--r--   0        0        0      391 2023-07-03 16:08:19.184598 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/__init__.py
--rw-r--r--   0        0        0     2280 2023-07-03 16:28:40.388369 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0      205 2023-07-03 16:08:19.182005 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/http_resources.py
--rw-r--r--   0        0        0     2683 2023-07-03 16:28:40.381687 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/trigger.py
--rw-r--r--   0        0        0      882 2023-07-03 16:28:40.352187 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0      249 2023-07-03 16:08:19.188733 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      262 2023-07-03 16:08:19.215749 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/__init__.py
--rw-r--r--   0        0        0     1051 2023-07-03 16:28:40.361652 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/http_delegate.py
--rw-r--r--   0        0        0     1213 2023-07-03 16:28:40.362745 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/user.py
--rw-r--r--   0        0        0      485 2023-07-03 16:28:40.384945 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/user_delegate.py
--rw-r--r--   0        0        0      194 2023-07-03 16:30:28.374240 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/user_record.py
--rw-r--r--   0        0        0      704 2023-07-03 16:08:19.177982 roboto_sdk-0.1.3a3/src/roboto_sdk/http/__init__.py
--rw-r--r--   0        0        0      216 2023-07-03 16:08:19.176698 roboto_sdk-0.1.3a3/src/roboto_sdk/http/constants.py
--rw-r--r--   0        0        0     9060 2023-07-03 16:28:40.379809 roboto_sdk-0.1.3a3/src/roboto_sdk/http/http_client.py
--rw-r--r--   0        0        0     3161 2023-07-03 16:30:28.347765 roboto_sdk-0.1.3a3/src/roboto_sdk/http/request_decorators.py
--rw-r--r--   0        0        0     1004 2023-07-03 16:28:40.363668 roboto_sdk-0.1.3a3/src/roboto_sdk/http/testing_util.py
--rw-r--r--   0        0        0      158 2023-07-03 16:08:19.138394 roboto_sdk-0.1.3a3/src/roboto_sdk/logging.py
--rw-r--r--   0        0        0      224 2023-07-03 16:30:28.318993 roboto_sdk-0.1.3a3/src/roboto_sdk/pagination.py
--rw-r--r--   0        0        0      168 2023-07-03 16:08:19.172598 roboto_sdk-0.1.3a3/src/roboto_sdk/profile/__init__.py
--rw-r--r--   0        0        0     2977 2023-07-03 16:28:40.376360 roboto_sdk-0.1.3a3/src/roboto_sdk/profile/profile.py
--rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.3a3/src/roboto_sdk/py.typed
--rw-r--r--   0        0        0      651 2023-07-03 16:08:19.142504 roboto_sdk-0.1.3a3/src/roboto_sdk/serde.py
--rw-r--r--   0        0        0      112 2023-07-03 16:08:19.137067 roboto_sdk-0.1.3a3/src/roboto_sdk/time.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 roboto_sdk-0.1.3a3/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-07-03 22:07:17.479285 roboto_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0      948 2023-07-03 22:08:50.756074 roboto_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-03 22:07:17.483285 roboto_sdk-0.1.4/src/roboto_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/auth/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-03 22:08:20.863767 roboto_sdk-0.1.4/src/roboto_sdk/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3811 2023-07-03 22:08:20.863767 roboto_sdk-0.1.4/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc
+-rw-r--r--   0        0        0     4037 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/auth/pat.py
+-rw-r--r--   0        0        0      132 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      334 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/cli/command/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/cli/command/args.py
+-rw-r--r--   0        0        0     2058 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/cli/command/model.py
+-rw-r--r--   0        0        0      822 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/cli/context.py
+-rw-r--r--   0        0        0      110 2023-07-03 22:07:17.491285 roboto_sdk-0.1.4/src/roboto_sdk/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     6774 2023-07-03 22:07:17.491285 roboto_sdk-0.1.4/src/roboto_sdk/cli/datasets/commands.py
+-rw-r--r--   0        0        0     3659 2023-07-03 22:07:17.491285 roboto_sdk-0.1.4/src/roboto_sdk/cli/entry.py
+-rw-r--r--   0        0        0      108 2023-07-03 22:07:17.491285 roboto_sdk-0.1.4/src/roboto_sdk/cli/help/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-03 22:07:17.491285 roboto_sdk-0.1.4/src/roboto_sdk/cli/help/args.py
+-rw-r--r--   0        0        0      110 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/orgs/__init__.py
+-rw-r--r--   0        0        0     4074 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/orgs/commands.py
+-rw-r--r--   0        0        0      110 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/tokens/__init__.py
+-rw-r--r--   0        0        0     3301 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/triggers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2023-07-03 22:07:17.499285 roboto_sdk-0.1.4/src/roboto_sdk/cli/users/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-03 22:07:17.499285 roboto_sdk-0.1.4/src/roboto_sdk/cli/users/commands.py
+-rw-r--r--   0        0        0       48 2023-07-03 22:07:17.499285 roboto_sdk-0.1.4/src/roboto_sdk/domain/__init__.py
+-rw-r--r--   0        0        0      324 2023-07-03 22:08:20.471761 roboto_sdk-0.1.4/src/roboto_sdk/domain/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1641 2023-07-03 22:07:17.499285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__init__.py
+-rw-r--r--   0        0        0     1510 2023-07-03 22:08:20.471761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6438 2023-07-03 22:08:20.475761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc
+-rw-r--r--   0        0        0     3737 2023-07-03 22:08:20.475761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5170 2023-07-03 22:08:20.487762 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1383 2023-07-03 22:08:20.899767 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1124 2023-07-03 22:08:20.475761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc
+-rw-r--r--   0        0        0      636 2023-07-03 22:08:20.479761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc
+-rw-r--r--   0        0        0     4784 2023-07-03 22:08:20.483761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc
+-rw-r--r--   0        0        0     2321 2023-07-03 22:08:20.483761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     4685 2023-07-03 22:08:20.903767 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1310 2023-07-03 22:08:20.903767 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     2340 2023-07-03 22:08:20.483761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc
+-rw-r--r--   0        0        0     7427 2023-07-03 22:07:17.499285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action.py
+-rw-r--r--   0        0        0     3015 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_delegate.py
+-rw-r--r--   0        0        0     5168 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_http_delegate.py
+-rw-r--r--   0        0        0      640 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_http_resources.py
+-rw-r--r--   0        0        0      808 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_record.py
+-rw-r--r--   0        0        0      106 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/error.py
+-rw-r--r--   0        0        0     4499 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation.py
+-rw-r--r--   0        0        0     1726 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     4768 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      566 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0     1652 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_record.py
+-rw-r--r--   0        0        0      546 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__init__.py
+-rw-r--r--   0        0        0      735 2023-07-03 22:08:20.919767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7400 2023-07-03 22:08:20.923767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     3184 2023-07-03 22:08:20.931767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5064 2023-07-03 22:08:20.935767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      867 2023-07-03 22:08:20.935767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1263 2023-07-03 22:08:20.931767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     9836 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/dataset.py
+-rw-r--r--   0        0        0     2215 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/delegate.py
+-rw-r--r--   0        0        0     4911 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/http_delegate.py
+-rw-r--r--   0        0        0      340 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/http_resources.py
+-rw-r--r--   0        0        0      867 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/record.py
+-rw-r--r--   0        0        0      436 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__init__.py
+-rw-r--r--   0        0        0      712 2023-07-03 22:08:20.923767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1916 2023-07-03 22:08:20.927767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1536 2023-07-03 22:08:20.927767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc
+-rw-r--r--   0        0        0     2835 2023-07-03 22:08:20.927767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      723 2023-07-03 22:08:20.927767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0      696 2023-07-03 22:08:20.927767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     3232 2023-07-03 22:08:20.931767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1181 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/delegate.py
+-rw-r--r--   0        0        0      802 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/file.py
+-rw-r--r--   0        0        0     2166 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/http_delegate.py
+-rw-r--r--   0        0        0      168 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/http_resources.py
+-rw-r--r--   0        0        0      382 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/record.py
+-rw-r--r--   0        0        0     2358 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/s3_delegate.py
+-rw-r--r--   0        0        0      728 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/__init__.py
+-rw-r--r--   0        0        0     2052 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     4674 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      359 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     1815 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org.py
+-rw-r--r--   0        0        0     1680 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org_invite.py
+-rw-r--r--   0        0        0     1432 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      722 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/record.py
+-rw-r--r--   0        0        0      387 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      888 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     2038 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      216 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      455 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/record.py
+-rw-r--r--   0        0        0     1832 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/token.py
+-rw-r--r--   0        0        0      391 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/__init__.py
+-rw-r--r--   0        0        0     2280 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0      205 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0     2683 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/trigger.py
+-rw-r--r--   0        0        0      882 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0      249 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      262 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/users/__init__.py
+-rw-r--r--   0        0        0     1051 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     1213 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/users/user.py
+-rw-r--r--   0        0        0      485 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      194 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/users/user_record.py
+-rw-r--r--   0        0        0      704 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/http/__init__.py
+-rw-r--r--   0        0        0      841 2023-07-03 22:08:20.491762 roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      500 2023-07-03 22:08:20.491762 roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     9636 2023-07-03 22:08:20.491762 roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc
+-rw-r--r--   0        0        0     3963 2023-07-03 22:08:20.531762 roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc
+-rw-r--r--   0        0        0     1666 2023-07-03 22:08:20.899767 roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc
+-rw-r--r--   0        0        0      216 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/http/constants.py
+-rw-r--r--   0        0        0     9060 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/http/http_client.py
+-rw-r--r--   0        0        0     3161 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/http/request_decorators.py
+-rw-r--r--   0        0        0     1004 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/http/testing_util.py
+-rw-r--r--   0        0        0      158 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/logging.py
+-rw-r--r--   0        0        0      224 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/pagination.py
+-rw-r--r--   0        0        0      168 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/profile/__init__.py
+-rw-r--r--   0        0        0      428 2023-07-03 22:08:20.895767 roboto_sdk-0.1.4/src/roboto_sdk/profile/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2991 2023-07-03 22:08:20.899767 roboto_sdk-0.1.4/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc
+-rw-r--r--   0        0        0     2977 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/py.typed
+-rw-r--r--   0        0        0     1250 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/serde.py
+-rw-r--r--   0        0        0      112 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/time.py
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 roboto_sdk-0.1.4/PKG-INFO
```

### Comparing `roboto_sdk-0.1.3a3/pyproject.toml` & `roboto_sdk-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires-python = ">=3.10"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto_sdk"
-version = "0.1.3a3"
+version = "0.1.4"
 description = "Tools for interacting with roboto.ai"
 license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -28,8 +28,8 @@
 
 [tool.poetry.scripts]
 roboto = 'roboto_sdk.cli:entry'
 
 [tool.pytest.ini_options]
 markers = [
     "cli: tests which assume that the CLI is available on ${PATH}. (deselect with '-m \"not cli\"')",
-]
+]
```

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/auth/pat.py` & `roboto_sdk-0.1.4/src/roboto_sdk/auth/pat.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/command/args.py` & `roboto_sdk-0.1.4/src/roboto_sdk/cli/command/args.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/command/model.py` & `roboto_sdk-0.1.4/src/roboto_sdk/cli/command/model.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/context.py` & `roboto_sdk-0.1.4/src/roboto_sdk/cli/context.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/datasets/commands.py` & `roboto_sdk-0.1.4/src/roboto_sdk/cli/datasets/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,32 @@
 def get_setup_parser(parser):
     parser.add_argument(
         "-d", "--dataset-id", type=str, required=True, help=DATASET_ARG_HELP
     )
 
 
 def query(args, context: CLIContext, parser: argparse.ArgumentParser):
-    records = Dataset.query(filters={}, dataset_delegate=context.datasets)
+    records = Dataset.query(
+        filters=args.filter, dataset_delegate=context.datasets, org_id=args.org
+    )
     for record in records:
         sys.stdout.write(json.dumps(record.to_dict()) + "\n")
 
 
 def query_setup_parser(parser):
     parser.add_argument("-o", "--org", type=str, help=ORG_ARG_HELP)
     parser.add_argument(
         "-f",
         "--filter",
         metavar="KEY=VALUE",
         nargs="*",
         action=KeyValuePairsAction,
         help="Zero or more 'key=value' formatted conditions which will perform equality checks against "
         + "datasets and filter results accordingly.",
+        default={},
     )
 
 
 def list_files(args, context: CLIContext, parser: argparse.ArgumentParser):
     record = Dataset.from_id(
         dataset_delegate=context.datasets,
         dataset_id=args.dataset_id,
```

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/entry.py` & `roboto_sdk-0.1.4/src/roboto_sdk/cli/entry.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/orgs/commands.py` & `roboto_sdk-0.1.4/src/roboto_sdk/cli/orgs/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -77,14 +77,29 @@
 
 def list_roles(args, context: CLIContext, parser: argparse.ArgumentParser):
     records = OrgRole.by_user_id(user_id=None, org_delegate=context.orgs)
     for record in records:
         sys.stdout.write(json.dumps(record.to_dict()) + "\n")
 
 
+def list_org_members(args, context: CLIContext, parser: argparse.ArgumentParser):
+    records = OrgRole.by_org_id(org_id=args.org, org_delegate=context.orgs)
+    for record in records:
+        sys.stdout.write(json.dumps(record.to_dict()) + "\n")
+
+
+def list_org_members_setup_parser(parser):
+    parser.add_argument(
+        "--org",
+        type=str,
+        required=True,
+        help="The org_id for the org you want to see.",
+    )
+
+
 create_command = RobotoCommand(
     name="create",
     logic=create,
     setup_parser=create_setup_parser,
     command_kwargs={"help": "Creates a new organization"},
 )
 
@@ -116,20 +131,28 @@
     name="list-roles",
     logic=list_roles,
     command_kwargs={
         "help": "Lists the roles that you have in orgs that you're a member of"
     },
 )
 
+list_org_members_command = RobotoCommand(
+    name="list-org-members",
+    logic=list_org_members,
+    setup_parser=list_org_members_setup_parser,
+    command_kwargs={"help": "Lists the members of an organization"},
+)
+
 
 commands = [
     create_command,
     delete_command,
     get_command,
     list_orgs_command,
+    list_org_members_command,
     list_roles_command,
 ]
 
 command_set = RobotoCommandSet(
     name="orgs",
     help="Commands for interacting with orgs.",
     commands=commands,
```

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/tokens/commands.py` & `roboto_sdk-0.1.4/src/roboto_sdk/cli/tokens/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/triggers/commands.py` & `roboto_sdk-0.1.4/src/roboto_sdk/cli/triggers/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/users/commands.py` & `roboto_sdk-0.1.4/src/roboto_sdk/cli/users/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/__init__.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_http_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_http_resources.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_record.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_http_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_http_resources.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_record.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/__init__.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/dataset.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/http_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/record.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/file.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/file.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/http_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/s3_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/s3_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/__init__.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/delegate.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,18 @@
         raise NotImplementedError("orgs_for_user")
 
     @abc.abstractmethod
     def org_roles_for_user(self, user_id: Optional[str]) -> list[OrgRoleRecord]:
         raise NotImplementedError("org_roles_for_user")
 
     @abc.abstractmethod
+    def org_roles_for_org(self, org_id: Optional[str]) -> list[OrgRoleRecord]:
+        raise NotImplementedError("org_roles_for_org")
+
+    @abc.abstractmethod
     def get_org_by_id(self, org_id: str) -> OrgRecord:
         raise NotImplementedError("get_org_by_id")
 
     @abc.abstractmethod
     def delete_org(self, org_id: str):
         raise NotImplementedError("delete_org")
```

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/http_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/http_delegate.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,16 +55,34 @@
         response = self.__http_client.get(url=url)
         return [
             OrgRecord.parse_obj(record)
             for record in response.from_json(json_path=["data"])
         ]
 
     def org_roles_for_user(self, user_id: Optional[str]) -> list[OrgRoleRecord]:
+        url = self.__http_client.url("v1/orgs/roles/user")
+
+        headers = {}
+        if user_id is not None:
+            headers[USER_OVERRIDE_HEADER] = user_id
+
+        response = self.__http_client.get(url=url, headers=headers)
+        return [
+            OrgRoleRecord.parse_obj(record)
+            for record in response.from_json(json_path=["data"])
+        ]
+
+    def org_roles_for_org(self, org_id: Optional[str]) -> list[OrgRoleRecord]:
         url = self.__http_client.url("v1/orgs/roles")
-        response = self.__http_client.get(url=url)
+
+        headers = {}
+        if org_id is not None:
+            headers[ORG_OVERRIDE_HEADER] = org_id
+
+        response = self.__http_client.get(url=url, headers=headers)
         return [
             OrgRoleRecord.parse_obj(record)
             for record in response.from_json(json_path=["data"])
         ]
 
     def get_org_by_id(self, org_id: str) -> OrgRecord:
         url = self.__http_client.url("v1/orgs")
```

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org_invite.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org_invite.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org_role.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org_role.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,21 @@
     @classmethod
     def by_user_id(
         cls, user_id: Optional[str], org_delegate: OrgDelegate
     ) -> list["OrgRole"]:
         records = org_delegate.org_roles_for_user(user_id=user_id)
         return [cls(record=record, org_delegate=org_delegate) for record in records]
 
+    @classmethod
+    def by_org_id(
+        cls, org_id: Optional[str], org_delegate: OrgDelegate
+    ) -> list["OrgRole"]:
+        records = org_delegate.org_roles_for_org(org_id=org_id)
+        return [cls(record=record, org_delegate=org_delegate) for record in records]
+
     def __init__(self, record: OrgRoleRecord, org_delegate: OrgDelegate):
         self.__record = record
         self.__org_delegate = org_delegate
         self.__org = Org(record=record.org, org_delegate=org_delegate)
 
     def to_dict(self) -> dict[str, Any]:
         return pydantic_jsonable_dict(self.__record)
```

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/record.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/http_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/token.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/token.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/http_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/trigger.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/trigger.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/trigger_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/trigger_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/http_delegate.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/users/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/user.py` & `roboto_sdk-0.1.4/src/roboto_sdk/domain/users/user.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/http/__init__.py` & `roboto_sdk-0.1.4/src/roboto_sdk/http/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/http/http_client.py` & `roboto_sdk-0.1.4/src/roboto_sdk/http/http_client.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/http/request_decorators.py` & `roboto_sdk-0.1.4/src/roboto_sdk/http/request_decorators.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/http/testing_util.py` & `roboto_sdk-0.1.4/src/roboto_sdk/http/testing_util.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/src/roboto_sdk/profile/profile.py` & `roboto_sdk-0.1.4/src/roboto_sdk/profile/profile.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a3/PKG-INFO` & `roboto_sdk-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto-sdk
-Version: 0.1.3a3
+Version: 0.1.4
 Summary: Tools for interacting with roboto.ai
 License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

