# Comparing `tmp/roboto_sdk-0.1.3a2.tar.gz` & `tmp/roboto_sdk-0.1.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_sdk-0.1.3a2.tar", max compression
+gzip compressed data, was "roboto_sdk-0.1.3a3.tar", max compression
```

## Comparing `roboto_sdk-0.1.3a2.tar` & `roboto_sdk-0.1.3a3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.3a2/README.md
--rw-r--r--   0        0        0      949 2023-07-03 16:21:54.874816 roboto_sdk-0.1.3a2/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-03 16:08:19.143854 roboto_sdk-0.1.3a2/src/roboto_sdk/__init__.py
--rw-r--r--   0        0        0       48 2023-07-03 16:08:19.141092 roboto_sdk-0.1.3a2/src/roboto_sdk/auth/__init__.py
--rw-r--r--   0        0        0     4037 2023-07-03 16:08:19.139811 roboto_sdk-0.1.3a2/src/roboto_sdk/auth/pat.py
--rw-r--r--   0        0        0      132 2023-07-03 16:08:19.152003 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/__init__.py
--rw-r--r--   0        0        0      334 2023-07-03 16:08:19.162015 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/command/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-03 16:08:19.164617 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/command/args.py
--rw-r--r--   0        0        0     2058 2023-07-03 16:28:40.380758 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/command/model.py
--rw-r--r--   0        0        0      822 2023-07-03 16:28:40.367049 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/context.py
--rw-r--r--   0        0        0      110 2023-07-03 16:08:19.148587 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/datasets/__init__.py
--rw-r--r--   0        0        0     6714 2023-07-03 16:08:19.150367 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/datasets/commands.py
--rw-r--r--   0        0        0     3603 2023-07-03 16:08:19.157982 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/entry.py
--rw-r--r--   0        0        0      108 2023-07-03 16:08:19.168666 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/help/__init__.py
--rw-r--r--   0        0        0      167 2023-07-03 16:08:19.169956 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/help/args.py
--rw-r--r--   0        0        0      110 2023-07-03 16:08:19.153590 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/orgs/__init__.py
--rw-r--r--   0        0        0     3386 2023-07-03 16:08:19.155109 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/orgs/commands.py
--rw-r--r--   0        0        0      110 2023-07-03 16:08:19.165930 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/tokens/__init__.py
--rw-r--r--   0        0        0     3301 2023-07-03 16:08:19.167288 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2023-07-03 16:08:19.145458 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/triggers/__init__.py
--rw-r--r--   0        0        0     2874 2023-07-03 16:08:19.147004 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2023-07-03 16:08:19.159379 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/users/__init__.py
--rw-r--r--   0        0        0      733 2023-07-03 16:08:19.160698 roboto_sdk-0.1.3a2/src/roboto_sdk/cli/users/commands.py
--rw-r--r--   0        0        0       48 2023-07-03 16:08:19.198130 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-03 16:08:19.224521 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/__init__.py
--rw-r--r--   0        0        0     7427 2023-07-03 16:28:40.375211 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action.py
--rw-r--r--   0        0        0     3015 2023-07-03 16:28:40.382505 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_delegate.py
--rw-r--r--   0        0        0     5168 2023-07-03 16:28:40.356951 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_http_delegate.py
--rw-r--r--   0        0        0      640 2023-07-03 16:28:40.365100 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_http_resources.py
--rw-r--r--   0        0        0      808 2023-07-03 16:28:40.372147 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_record.py
--rw-r--r--   0        0        0      106 2023-07-03 16:08:19.223131 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/error.py
--rw-r--r--   0        0        0     4499 2023-07-03 16:28:40.370371 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation.py
--rw-r--r--   0        0        0     1726 2023-07-03 16:28:40.384071 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_delegate.py
--rw-r--r--   0        0        0     4768 2023-07-03 16:28:40.366150 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      566 2023-07-03 16:30:28.384279 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_http_resources.py
--rw-r--r--   0        0        0     1652 2023-07-03 16:30:28.386808 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_record.py
--rw-r--r--   0        0        0      546 2023-07-03 16:08:19.192761 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/__init__.py
--rw-r--r--   0        0        0     9836 2023-07-03 16:28:40.373480 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/dataset.py
--rw-r--r--   0        0        0     2215 2023-07-03 16:28:40.371324 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/delegate.py
--rw-r--r--   0        0        0     4911 2023-07-03 16:28:40.387575 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/http_delegate.py
--rw-r--r--   0        0        0      340 2023-07-03 16:08:19.190087 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/http_resources.py
--rw-r--r--   0        0        0      867 2023-07-03 16:08:19.196854 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/record.py
--rw-r--r--   0        0        0      436 2023-07-03 16:08:19.238248 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/__init__.py
--rw-r--r--   0        0        0     1181 2023-07-03 16:28:40.353092 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/delegate.py
--rw-r--r--   0        0        0      802 2023-07-03 16:30:28.392185 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/file.py
--rw-r--r--   0        0        0     2166 2023-07-03 16:30:27.887912 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/http_delegate.py
--rw-r--r--   0        0        0      168 2023-07-03 16:08:19.235599 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/http_resources.py
--rw-r--r--   0        0        0      382 2023-07-03 16:08:19.242205 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/record.py
--rw-r--r--   0        0        0     2358 2023-07-03 16:30:27.887409 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/s3_delegate.py
--rw-r--r--   0        0        0      728 2023-07-03 16:08:19.204997 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/__init__.py
--rw-r--r--   0        0        0     1893 2023-07-03 16:28:40.348041 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/delegate.py
--rw-r--r--   0        0        0     4103 2023-07-03 16:28:40.383366 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      359 2023-07-03 16:08:19.200791 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     1815 2023-07-03 16:28:40.378431 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org.py
--rw-r--r--   0        0        0     1680 2023-07-03 16:28:40.364446 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org_invite.py
--rw-r--r--   0        0        0     1158 2023-07-03 16:28:40.351236 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org_role.py
--rw-r--r--   0        0        0      722 2023-07-03 16:08:19.209463 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/record.py
--rw-r--r--   0        0        0      387 2023-07-03 16:08:19.249174 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/__init__.py
--rw-r--r--   0        0        0      888 2023-07-03 16:28:40.360553 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/delegate.py
--rw-r--r--   0        0        0     2038 2023-07-03 16:28:40.386560 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      216 2023-07-03 16:30:28.394782 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      455 2023-07-03 16:30:28.399700 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/record.py
--rw-r--r--   0        0        0     1832 2023-07-03 16:30:28.395655 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/token.py
--rw-r--r--   0        0        0      391 2023-07-03 16:08:19.184598 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/__init__.py
--rw-r--r--   0        0        0     2280 2023-07-03 16:28:40.388369 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0      205 2023-07-03 16:08:19.182005 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/http_resources.py
--rw-r--r--   0        0        0     2683 2023-07-03 16:28:40.381687 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/trigger.py
--rw-r--r--   0        0        0      882 2023-07-03 16:28:40.352187 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0      249 2023-07-03 16:08:19.188733 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      262 2023-07-03 16:08:19.215749 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/__init__.py
--rw-r--r--   0        0        0     1051 2023-07-03 16:28:40.361652 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/http_delegate.py
--rw-r--r--   0        0        0     1213 2023-07-03 16:28:40.362745 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/user.py
--rw-r--r--   0        0        0      485 2023-07-03 16:28:40.384945 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/user_delegate.py
--rw-r--r--   0        0        0      194 2023-07-03 16:30:28.374240 roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/user_record.py
--rw-r--r--   0        0        0      704 2023-07-03 16:08:19.177982 roboto_sdk-0.1.3a2/src/roboto_sdk/http/__init__.py
--rw-r--r--   0        0        0      216 2023-07-03 16:08:19.176698 roboto_sdk-0.1.3a2/src/roboto_sdk/http/constants.py
--rw-r--r--   0        0        0     9060 2023-07-03 16:28:40.379809 roboto_sdk-0.1.3a2/src/roboto_sdk/http/http_client.py
--rw-r--r--   0        0        0     3161 2023-07-03 16:30:28.347765 roboto_sdk-0.1.3a2/src/roboto_sdk/http/request_decorators.py
--rw-r--r--   0        0        0     1004 2023-07-03 16:28:40.363668 roboto_sdk-0.1.3a2/src/roboto_sdk/http/testing_util.py
--rw-r--r--   0        0        0      158 2023-07-03 16:08:19.138394 roboto_sdk-0.1.3a2/src/roboto_sdk/logging.py
--rw-r--r--   0        0        0      224 2023-07-03 16:30:28.318993 roboto_sdk-0.1.3a2/src/roboto_sdk/pagination.py
--rw-r--r--   0        0        0      168 2023-07-03 16:08:19.172598 roboto_sdk-0.1.3a2/src/roboto_sdk/profile/__init__.py
--rw-r--r--   0        0        0     2977 2023-07-03 16:28:40.376360 roboto_sdk-0.1.3a2/src/roboto_sdk/profile/profile.py
--rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.3a2/src/roboto_sdk/py.typed
--rw-r--r--   0        0        0      651 2023-07-03 16:08:19.142504 roboto_sdk-0.1.3a2/src/roboto_sdk/serde.py
--rw-r--r--   0        0        0      112 2023-07-03 16:08:19.137067 roboto_sdk-0.1.3a2/src/roboto_sdk/time.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 roboto_sdk-0.1.3a2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.3a3/README.md
+-rw-r--r--   0        0        0      949 2023-07-03 17:26:10.562107 roboto_sdk-0.1.3a3/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-03 16:08:19.143854 roboto_sdk-0.1.3a3/src/roboto_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-03 16:08:19.141092 roboto_sdk-0.1.3a3/src/roboto_sdk/auth/__init__.py
+-rw-r--r--   0        0        0     4037 2023-07-03 16:08:19.139811 roboto_sdk-0.1.3a3/src/roboto_sdk/auth/pat.py
+-rw-r--r--   0        0        0      132 2023-07-03 16:08:19.152003 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      334 2023-07-03 16:08:19.162015 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/command/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-03 16:08:19.164617 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/command/args.py
+-rw-r--r--   0        0        0     2058 2023-07-03 16:28:40.380758 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/command/model.py
+-rw-r--r--   0        0        0      822 2023-07-03 16:28:40.367049 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/context.py
+-rw-r--r--   0        0        0      110 2023-07-03 16:08:19.148587 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     6714 2023-07-03 16:08:19.150367 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/datasets/commands.py
+-rw-r--r--   0        0        0     3659 2023-07-03 17:26:31.317426 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/entry.py
+-rw-r--r--   0        0        0      108 2023-07-03 16:08:19.168666 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/help/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-03 16:08:19.169956 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/help/args.py
+-rw-r--r--   0        0        0      110 2023-07-03 16:08:19.153590 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/orgs/__init__.py
+-rw-r--r--   0        0        0     3386 2023-07-03 16:08:19.155109 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/orgs/commands.py
+-rw-r--r--   0        0        0      110 2023-07-03 16:08:19.165930 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/tokens/__init__.py
+-rw-r--r--   0        0        0     3301 2023-07-03 16:08:19.167288 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2023-07-03 16:08:19.145458 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/triggers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-07-03 16:08:19.147004 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2023-07-03 16:08:19.159379 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/users/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-03 16:08:19.160698 roboto_sdk-0.1.3a3/src/roboto_sdk/cli/users/commands.py
+-rw-r--r--   0        0        0       48 2023-07-03 16:08:19.198130 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-03 16:08:19.224521 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/__init__.py
+-rw-r--r--   0        0        0     7427 2023-07-03 16:28:40.375211 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action.py
+-rw-r--r--   0        0        0     3015 2023-07-03 16:28:40.382505 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_delegate.py
+-rw-r--r--   0        0        0     5168 2023-07-03 16:28:40.356951 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_http_delegate.py
+-rw-r--r--   0        0        0      640 2023-07-03 16:28:40.365100 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_http_resources.py
+-rw-r--r--   0        0        0      808 2023-07-03 16:28:40.372147 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_record.py
+-rw-r--r--   0        0        0      106 2023-07-03 16:08:19.223131 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/error.py
+-rw-r--r--   0        0        0     4499 2023-07-03 16:28:40.370371 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation.py
+-rw-r--r--   0        0        0     1726 2023-07-03 16:28:40.384071 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     4768 2023-07-03 16:28:40.366150 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      566 2023-07-03 16:30:28.384279 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0     1652 2023-07-03 16:30:28.386808 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_record.py
+-rw-r--r--   0        0        0      546 2023-07-03 16:08:19.192761 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/__init__.py
+-rw-r--r--   0        0        0     9836 2023-07-03 16:28:40.373480 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/dataset.py
+-rw-r--r--   0        0        0     2215 2023-07-03 16:28:40.371324 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/delegate.py
+-rw-r--r--   0        0        0     4911 2023-07-03 16:28:40.387575 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/http_delegate.py
+-rw-r--r--   0        0        0      340 2023-07-03 16:08:19.190087 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/http_resources.py
+-rw-r--r--   0        0        0      867 2023-07-03 16:08:19.196854 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/record.py
+-rw-r--r--   0        0        0      436 2023-07-03 16:08:19.238248 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/__init__.py
+-rw-r--r--   0        0        0     1181 2023-07-03 16:28:40.353092 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/delegate.py
+-rw-r--r--   0        0        0      802 2023-07-03 16:30:28.392185 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/file.py
+-rw-r--r--   0        0        0     2166 2023-07-03 16:30:27.887912 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/http_delegate.py
+-rw-r--r--   0        0        0      168 2023-07-03 16:08:19.235599 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/http_resources.py
+-rw-r--r--   0        0        0      382 2023-07-03 16:08:19.242205 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/record.py
+-rw-r--r--   0        0        0     2358 2023-07-03 16:30:27.887409 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/s3_delegate.py
+-rw-r--r--   0        0        0      728 2023-07-03 16:08:19.204997 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/__init__.py
+-rw-r--r--   0        0        0     1893 2023-07-03 16:28:40.348041 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     4103 2023-07-03 16:28:40.383366 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      359 2023-07-03 16:08:19.200791 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     1815 2023-07-03 16:28:40.378431 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org.py
+-rw-r--r--   0        0        0     1680 2023-07-03 16:28:40.364446 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org_invite.py
+-rw-r--r--   0        0        0     1158 2023-07-03 16:28:40.351236 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      722 2023-07-03 16:08:19.209463 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/record.py
+-rw-r--r--   0        0        0      387 2023-07-03 16:08:19.249174 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      888 2023-07-03 16:28:40.360553 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     2038 2023-07-03 16:28:40.386560 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      216 2023-07-03 16:30:28.394782 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      455 2023-07-03 16:30:28.399700 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/record.py
+-rw-r--r--   0        0        0     1832 2023-07-03 16:30:28.395655 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/token.py
+-rw-r--r--   0        0        0      391 2023-07-03 16:08:19.184598 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/__init__.py
+-rw-r--r--   0        0        0     2280 2023-07-03 16:28:40.388369 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0      205 2023-07-03 16:08:19.182005 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0     2683 2023-07-03 16:28:40.381687 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/trigger.py
+-rw-r--r--   0        0        0      882 2023-07-03 16:28:40.352187 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0      249 2023-07-03 16:08:19.188733 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      262 2023-07-03 16:08:19.215749 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/__init__.py
+-rw-r--r--   0        0        0     1051 2023-07-03 16:28:40.361652 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     1213 2023-07-03 16:28:40.362745 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/user.py
+-rw-r--r--   0        0        0      485 2023-07-03 16:28:40.384945 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      194 2023-07-03 16:30:28.374240 roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/user_record.py
+-rw-r--r--   0        0        0      704 2023-07-03 16:08:19.177982 roboto_sdk-0.1.3a3/src/roboto_sdk/http/__init__.py
+-rw-r--r--   0        0        0      216 2023-07-03 16:08:19.176698 roboto_sdk-0.1.3a3/src/roboto_sdk/http/constants.py
+-rw-r--r--   0        0        0     9060 2023-07-03 16:28:40.379809 roboto_sdk-0.1.3a3/src/roboto_sdk/http/http_client.py
+-rw-r--r--   0        0        0     3161 2023-07-03 16:30:28.347765 roboto_sdk-0.1.3a3/src/roboto_sdk/http/request_decorators.py
+-rw-r--r--   0        0        0     1004 2023-07-03 16:28:40.363668 roboto_sdk-0.1.3a3/src/roboto_sdk/http/testing_util.py
+-rw-r--r--   0        0        0      158 2023-07-03 16:08:19.138394 roboto_sdk-0.1.3a3/src/roboto_sdk/logging.py
+-rw-r--r--   0        0        0      224 2023-07-03 16:30:28.318993 roboto_sdk-0.1.3a3/src/roboto_sdk/pagination.py
+-rw-r--r--   0        0        0      168 2023-07-03 16:08:19.172598 roboto_sdk-0.1.3a3/src/roboto_sdk/profile/__init__.py
+-rw-r--r--   0        0        0     2977 2023-07-03 16:28:40.376360 roboto_sdk-0.1.3a3/src/roboto_sdk/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.3a3/src/roboto_sdk/py.typed
+-rw-r--r--   0        0        0      651 2023-07-03 16:08:19.142504 roboto_sdk-0.1.3a3/src/roboto_sdk/serde.py
+-rw-r--r--   0        0        0      112 2023-07-03 16:08:19.137067 roboto_sdk-0.1.3a3/src/roboto_sdk/time.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 roboto_sdk-0.1.3a3/PKG-INFO
```

### Comparing `roboto_sdk-0.1.3a2/pyproject.toml` & `roboto_sdk-0.1.3a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires-python = ">=3.10"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto_sdk"
-version = "0.1.3a2"
+version = "0.1.3a3"
 description = "Tools for interacting with roboto.ai"
 license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/auth/pat.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/auth/pat.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/command/args.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/command/args.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/command/model.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/command/model.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/context.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/context.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/datasets/commands.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/entry.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,15 +102,16 @@
         required=False,
     )
 
     context = CLIContext()
 
     logging.basicConfig(level=logging.ERROR, stream=sys.stderr)
 
-    subcommands = parser.add_subparsers()
+    # https://bugs.python.org/issue29298
+    subcommands = parser.add_subparsers(dest="function")
     subcommands.required = True
 
     for command_set in COMMAND_SETS:
         command_set.add_to_subparsers(subcommands, context)
 
     args = parser.parse_args()
     __populate_context(args, context)
```

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/orgs/commands.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/orgs/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/tokens/commands.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/tokens/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/triggers/commands.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/triggers/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/cli/users/commands.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/cli/users/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/__init__.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_http_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_http_resources.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/action_record.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/action_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_http_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_http_resources.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/actions/invocation_record.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/actions/invocation_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/__init__.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/dataset.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/http_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/datasets/record.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/datasets/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/file.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/file.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/http_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/files/s3_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/files/s3_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/__init__.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/http_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org_invite.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org_invite.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/org_role.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/org_role.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/orgs/record.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/orgs/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/http_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/tokens/token.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/tokens/token.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/http_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/trigger.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/trigger.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/triggers/trigger_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/triggers/trigger_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/http_delegate.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/domain/users/user.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/domain/users/user.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/http/__init__.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/http/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/http/http_client.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/http/http_client.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/http/request_decorators.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/http/request_decorators.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/http/testing_util.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/http/testing_util.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/profile/profile.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/profile/profile.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/src/roboto_sdk/serde.py` & `roboto_sdk-0.1.3a3/src/roboto_sdk/serde.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a2/PKG-INFO` & `roboto_sdk-0.1.3a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto-sdk
-Version: 0.1.3a2
+Version: 0.1.3a3
 Summary: Tools for interacting with roboto.ai
 License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

