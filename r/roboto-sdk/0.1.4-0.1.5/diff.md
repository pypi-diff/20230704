# Comparing `tmp/roboto_sdk-0.1.4.tar.gz` & `tmp/roboto_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_sdk-0.1.4.tar", max compression
+gzip compressed data, was "roboto_sdk-0.1.5.tar", max compression
```

## Comparing `roboto_sdk-0.1.4.tar` & `roboto_sdk-0.1.5.tar`

### file list

```diff
@@ -1,122 +1,149 @@
--rw-r--r--   0        0        0       22 2023-07-03 22:07:17.479285 roboto_sdk-0.1.4/README.md
--rw-r--r--   0        0        0      948 2023-07-03 22:08:50.756074 roboto_sdk-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-03 22:07:17.483285 roboto_sdk-0.1.4/src/roboto_sdk/__init__.py
--rw-r--r--   0        0        0       48 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/auth/__init__.py
--rw-r--r--   0        0        0      322 2023-07-03 22:08:20.863767 roboto_sdk-0.1.4/src/roboto_sdk/auth/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3811 2023-07-03 22:08:20.863767 roboto_sdk-0.1.4/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc
--rw-r--r--   0        0        0     4037 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/auth/pat.py
--rw-r--r--   0        0        0      132 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/cli/__init__.py
--rw-r--r--   0        0        0      334 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/cli/command/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/cli/command/args.py
--rw-r--r--   0        0        0     2058 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/cli/command/model.py
--rw-r--r--   0        0        0      822 2023-07-03 22:07:17.487285 roboto_sdk-0.1.4/src/roboto_sdk/cli/context.py
--rw-r--r--   0        0        0      110 2023-07-03 22:07:17.491285 roboto_sdk-0.1.4/src/roboto_sdk/cli/datasets/__init__.py
--rw-r--r--   0        0        0     6774 2023-07-03 22:07:17.491285 roboto_sdk-0.1.4/src/roboto_sdk/cli/datasets/commands.py
--rw-r--r--   0        0        0     3659 2023-07-03 22:07:17.491285 roboto_sdk-0.1.4/src/roboto_sdk/cli/entry.py
--rw-r--r--   0        0        0      108 2023-07-03 22:07:17.491285 roboto_sdk-0.1.4/src/roboto_sdk/cli/help/__init__.py
--rw-r--r--   0        0        0      167 2023-07-03 22:07:17.491285 roboto_sdk-0.1.4/src/roboto_sdk/cli/help/args.py
--rw-r--r--   0        0        0      110 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/orgs/__init__.py
--rw-r--r--   0        0        0     4074 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/orgs/commands.py
--rw-r--r--   0        0        0      110 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/tokens/__init__.py
--rw-r--r--   0        0        0     3301 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/triggers/__init__.py
--rw-r--r--   0        0        0     2874 2023-07-03 22:07:17.495285 roboto_sdk-0.1.4/src/roboto_sdk/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2023-07-03 22:07:17.499285 roboto_sdk-0.1.4/src/roboto_sdk/cli/users/__init__.py
--rw-r--r--   0        0        0      733 2023-07-03 22:07:17.499285 roboto_sdk-0.1.4/src/roboto_sdk/cli/users/commands.py
--rw-r--r--   0        0        0       48 2023-07-03 22:07:17.499285 roboto_sdk-0.1.4/src/roboto_sdk/domain/__init__.py
--rw-r--r--   0        0        0      324 2023-07-03 22:08:20.471761 roboto_sdk-0.1.4/src/roboto_sdk/domain/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1641 2023-07-03 22:07:17.499285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__init__.py
--rw-r--r--   0        0        0     1510 2023-07-03 22:08:20.471761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6438 2023-07-03 22:08:20.475761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc
--rw-r--r--   0        0        0     3737 2023-07-03 22:08:20.475761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     5170 2023-07-03 22:08:20.487762 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1383 2023-07-03 22:08:20.899767 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1124 2023-07-03 22:08:20.475761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc
--rw-r--r--   0        0        0      636 2023-07-03 22:08:20.479761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc
--rw-r--r--   0        0        0     4784 2023-07-03 22:08:20.483761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc
--rw-r--r--   0        0        0     2321 2023-07-03 22:08:20.483761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     4685 2023-07-03 22:08:20.903767 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1310 2023-07-03 22:08:20.903767 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     2340 2023-07-03 22:08:20.483761 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc
--rw-r--r--   0        0        0     7427 2023-07-03 22:07:17.499285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action.py
--rw-r--r--   0        0        0     3015 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_delegate.py
--rw-r--r--   0        0        0     5168 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_http_delegate.py
--rw-r--r--   0        0        0      640 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_http_resources.py
--rw-r--r--   0        0        0      808 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_record.py
--rw-r--r--   0        0        0      106 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/error.py
--rw-r--r--   0        0        0     4499 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation.py
--rw-r--r--   0        0        0     1726 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_delegate.py
--rw-r--r--   0        0        0     4768 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      566 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_http_resources.py
--rw-r--r--   0        0        0     1652 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_record.py
--rw-r--r--   0        0        0      546 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__init__.py
--rw-r--r--   0        0        0      735 2023-07-03 22:08:20.919767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7400 2023-07-03 22:08:20.923767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc
--rw-r--r--   0        0        0     3184 2023-07-03 22:08:20.931767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     5064 2023-07-03 22:08:20.935767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      867 2023-07-03 22:08:20.935767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1263 2023-07-03 22:08:20.931767 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     9836 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/dataset.py
--rw-r--r--   0        0        0     2215 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/delegate.py
--rw-r--r--   0        0        0     4911 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/http_delegate.py
--rw-r--r--   0        0        0      340 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/http_resources.py
--rw-r--r--   0        0        0      867 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/record.py
--rw-r--r--   0        0        0      436 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__init__.py
--rw-r--r--   0        0        0      712 2023-07-03 22:08:20.923767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1916 2023-07-03 22:08:20.927767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1536 2023-07-03 22:08:20.927767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc
--rw-r--r--   0        0        0     2835 2023-07-03 22:08:20.927767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      723 2023-07-03 22:08:20.927767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0      696 2023-07-03 22:08:20.927767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     3232 2023-07-03 22:08:20.931767 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1181 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/delegate.py
--rw-r--r--   0        0        0      802 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/file.py
--rw-r--r--   0        0        0     2166 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/http_delegate.py
--rw-r--r--   0        0        0      168 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/http_resources.py
--rw-r--r--   0        0        0      382 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/record.py
--rw-r--r--   0        0        0     2358 2023-07-03 22:07:17.503285 roboto_sdk-0.1.4/src/roboto_sdk/domain/files/s3_delegate.py
--rw-r--r--   0        0        0      728 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/__init__.py
--rw-r--r--   0        0        0     2052 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/delegate.py
--rw-r--r--   0        0        0     4674 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      359 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     1815 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org.py
--rw-r--r--   0        0        0     1680 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org_invite.py
--rw-r--r--   0        0        0     1432 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org_role.py
--rw-r--r--   0        0        0      722 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/record.py
--rw-r--r--   0        0        0      387 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/__init__.py
--rw-r--r--   0        0        0      888 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/delegate.py
--rw-r--r--   0        0        0     2038 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      216 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      455 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/record.py
--rw-r--r--   0        0        0     1832 2023-07-03 22:07:17.507285 roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/token.py
--rw-r--r--   0        0        0      391 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/__init__.py
--rw-r--r--   0        0        0     2280 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0      205 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/http_resources.py
--rw-r--r--   0        0        0     2683 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/trigger.py
--rw-r--r--   0        0        0      882 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0      249 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      262 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/users/__init__.py
--rw-r--r--   0        0        0     1051 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/users/http_delegate.py
--rw-r--r--   0        0        0     1213 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/users/user.py
--rw-r--r--   0        0        0      485 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/users/user_delegate.py
--rw-r--r--   0        0        0      194 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/domain/users/user_record.py
--rw-r--r--   0        0        0      704 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/http/__init__.py
--rw-r--r--   0        0        0      841 2023-07-03 22:08:20.491762 roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      500 2023-07-03 22:08:20.491762 roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0     9636 2023-07-03 22:08:20.491762 roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc
--rw-r--r--   0        0        0     3963 2023-07-03 22:08:20.531762 roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc
--rw-r--r--   0        0        0     1666 2023-07-03 22:08:20.899767 roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc
--rw-r--r--   0        0        0      216 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/http/constants.py
--rw-r--r--   0        0        0     9060 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/http/http_client.py
--rw-r--r--   0        0        0     3161 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/http/request_decorators.py
--rw-r--r--   0        0        0     1004 2023-07-03 22:07:17.511285 roboto_sdk-0.1.4/src/roboto_sdk/http/testing_util.py
--rw-r--r--   0        0        0      158 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/logging.py
--rw-r--r--   0        0        0      224 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/pagination.py
--rw-r--r--   0        0        0      168 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/profile/__init__.py
--rw-r--r--   0        0        0      428 2023-07-03 22:08:20.895767 roboto_sdk-0.1.4/src/roboto_sdk/profile/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2991 2023-07-03 22:08:20.899767 roboto_sdk-0.1.4/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc
--rw-r--r--   0        0        0     2977 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/profile/profile.py
--rw-r--r--   0        0        0        0 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/py.typed
--rw-r--r--   0        0        0     1250 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/serde.py
--rw-r--r--   0        0        0      112 2023-07-03 22:07:17.515285 roboto_sdk-0.1.4/src/roboto_sdk/time.py
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 roboto_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-07-04 01:18:05.605793 roboto_sdk-0.1.5/README.md
+-rw-r--r--   0        0        0      948 2023-07-04 01:19:42.474094 roboto_sdk-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-04 01:18:05.609793 roboto_sdk-0.1.5/src/roboto_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-04 01:18:05.609793 roboto_sdk-0.1.5/src/roboto_sdk/auth/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-04 01:19:08.421988 roboto_sdk-0.1.5/src/roboto_sdk/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3811 2023-07-04 01:19:08.421988 roboto_sdk-0.1.5/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc
+-rw-r--r--   0        0        0     4037 2023-07-04 01:18:05.609793 roboto_sdk-0.1.5/src/roboto_sdk/auth/pat.py
+-rw-r--r--   0        0        0      132 2023-07-04 01:18:05.613793 roboto_sdk-0.1.5/src/roboto_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      334 2023-07-04 01:18:05.613793 roboto_sdk-0.1.5/src/roboto_sdk/cli/command/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-04 01:18:05.613793 roboto_sdk-0.1.5/src/roboto_sdk/cli/command/args.py
+-rw-r--r--   0        0        0     2058 2023-07-04 01:18:05.613793 roboto_sdk-0.1.5/src/roboto_sdk/cli/command/model.py
+-rw-r--r--   0        0        0      822 2023-07-04 01:18:05.613793 roboto_sdk-0.1.5/src/roboto_sdk/cli/context.py
+-rw-r--r--   0        0        0      110 2023-07-04 01:18:05.617793 roboto_sdk-0.1.5/src/roboto_sdk/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     6774 2023-07-04 01:18:05.617793 roboto_sdk-0.1.5/src/roboto_sdk/cli/datasets/commands.py
+-rw-r--r--   0        0        0     3659 2023-07-04 01:18:05.617793 roboto_sdk-0.1.5/src/roboto_sdk/cli/entry.py
+-rw-r--r--   0        0        0      108 2023-07-04 01:18:05.617793 roboto_sdk-0.1.5/src/roboto_sdk/cli/help/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-04 01:18:05.617793 roboto_sdk-0.1.5/src/roboto_sdk/cli/help/args.py
+-rw-r--r--   0        0        0      110 2023-07-04 01:18:05.621793 roboto_sdk-0.1.5/src/roboto_sdk/cli/orgs/__init__.py
+-rw-r--r--   0        0        0     4074 2023-07-04 01:18:05.621793 roboto_sdk-0.1.5/src/roboto_sdk/cli/orgs/commands.py
+-rw-r--r--   0        0        0      110 2023-07-04 01:18:05.621793 roboto_sdk-0.1.5/src/roboto_sdk/cli/tokens/__init__.py
+-rw-r--r--   0        0        0     3301 2023-07-04 01:18:05.621793 roboto_sdk-0.1.5/src/roboto_sdk/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2023-07-04 01:18:05.625793 roboto_sdk-0.1.5/src/roboto_sdk/cli/triggers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-07-04 01:18:05.625793 roboto_sdk-0.1.5/src/roboto_sdk/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2023-07-04 01:18:05.625793 roboto_sdk-0.1.5/src/roboto_sdk/cli/users/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-04 01:18:05.625793 roboto_sdk-0.1.5/src/roboto_sdk/cli/users/commands.py
+-rw-r--r--   0        0        0      120 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-04 01:19:08.069987 roboto_sdk-0.1.5/src/roboto_sdk/domain/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1849 2023-07-04 01:19:08.069987 roboto_sdk-0.1.5/src/roboto_sdk/domain/__pycache__/http_delegates.cpython-310.pyc
+-rw-r--r--   0        0        0     1641 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__init__.py
+-rw-r--r--   0        0        0     1510 2023-07-04 01:19:08.453988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6438 2023-07-04 01:19:08.453988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc
+-rw-r--r--   0        0        0     3737 2023-07-04 01:19:08.457988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5170 2023-07-04 01:19:08.469988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1383 2023-07-04 01:19:08.469988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1124 2023-07-04 01:19:08.457988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc
+-rw-r--r--   0        0        0      636 2023-07-04 01:19:08.461988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc
+-rw-r--r--   0        0        0     4784 2023-07-04 01:19:08.461988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc
+-rw-r--r--   0        0        0     2321 2023-07-04 01:19:08.461988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     4685 2023-07-04 01:19:08.473988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1310 2023-07-04 01:19:08.473988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     2340 2023-07-04 01:19:08.461988 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc
+-rw-r--r--   0        0        0     7427 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action.py
+-rw-r--r--   0        0        0     3015 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_delegate.py
+-rw-r--r--   0        0        0     5168 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_http_delegate.py
+-rw-r--r--   0        0        0      640 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_http_resources.py
+-rw-r--r--   0        0        0      808 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_record.py
+-rw-r--r--   0        0        0      106 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/error.py
+-rw-r--r--   0        0        0     4499 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation.py
+-rw-r--r--   0        0        0     1726 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     4768 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      566 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0     1652 2023-07-04 01:18:05.629793 roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_record.py
+-rw-r--r--   0        0        0      546 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__init__.py
+-rw-r--r--   0        0        0      735 2023-07-04 01:19:08.477988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7400 2023-07-04 01:19:08.477988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     3184 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5064 2023-07-04 01:19:08.489988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      867 2023-07-04 01:19:08.489988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1263 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     9836 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/dataset.py
+-rw-r--r--   0        0        0     2215 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/delegate.py
+-rw-r--r--   0        0        0     4911 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/http_delegate.py
+-rw-r--r--   0        0        0      340 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/http_resources.py
+-rw-r--r--   0        0        0      867 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/record.py
+-rw-r--r--   0        0        0      436 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__init__.py
+-rw-r--r--   0        0        0      712 2023-07-04 01:19:08.481988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1916 2023-07-04 01:19:08.481988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1536 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc
+-rw-r--r--   0        0        0     2835 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      723 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0      696 2023-07-04 01:19:08.481988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     3232 2023-07-04 01:19:08.485988 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1181 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/delegate.py
+-rw-r--r--   0        0        0      802 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/file.py
+-rw-r--r--   0        0        0     2166 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/http_delegate.py
+-rw-r--r--   0        0        0      168 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/http_resources.py
+-rw-r--r--   0        0        0      382 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/record.py
+-rw-r--r--   0        0        0     2358 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/files/s3_delegate.py
+-rw-r--r--   0        0        0     1974 2023-07-04 01:18:05.633793 roboto_sdk-0.1.5/src/roboto_sdk/domain/http_delegates.py
+-rw-r--r--   0        0        0      728 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__init__.py
+-rw-r--r--   0        0        0      896 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2758 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5097 2023-07-04 01:19:08.501988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1012 2023-07-04 01:19:08.501988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     2574 2023-07-04 01:19:08.501988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/org.cpython-310.pyc
+-rw-r--r--   0        0        0     2178 2023-07-04 01:19:08.501988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/org_invite.cpython-310.pyc
+-rw-r--r--   0        0        0     2413 2023-07-04 01:19:08.501988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/org_role.cpython-310.pyc
+-rw-r--r--   0        0        0     1709 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     2052 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     4674 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      359 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     1815 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org.py
+-rw-r--r--   0        0        0     1680 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org_invite.py
+-rw-r--r--   0        0        0     1432 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      722 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/record.py
+-rw-r--r--   0        0        0      387 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      640 2023-07-04 01:19:08.505988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-07-04 01:19:08.505988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     2697 2023-07-04 01:19:08.505988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      685 2023-07-04 01:19:08.505988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1003 2023-07-04 01:19:08.505988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     2542 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/token.cpython-310.pyc
+-rw-r--r--   0        0        0      888 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     2038 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      216 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      455 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/record.py
+-rw-r--r--   0        0        0     1832 2023-07-04 01:18:05.637793 roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/token.py
+-rw-r--r--   0        0        0      391 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2758 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      657 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     2388 2023-07-04 01:19:08.513988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/trigger.cpython-310.pyc
+-rw-r--r--   0        0        0     1488 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      617 2023-07-04 01:19:08.509988 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/trigger_record.cpython-310.pyc
+-rw-r--r--   0        0        0     2280 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0      205 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0     2683 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/trigger.py
+-rw-r--r--   0        0        0      882 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0      249 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      262 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__init__.py
+-rw-r--r--   0        0        0      554 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1617 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1940 2023-07-04 01:19:08.497988 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1172 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/user_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      658 2023-07-04 01:19:08.493988 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/__pycache__/user_record.cpython-310.pyc
+-rw-r--r--   0        0        0     1051 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     1213 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/user.py
+-rw-r--r--   0        0        0      485 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      194 2023-07-04 01:18:05.641793 roboto_sdk-0.1.5/src/roboto_sdk/domain/users/user_record.py
+-rw-r--r--   0        0        0      704 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/http/__init__.py
+-rw-r--r--   0        0        0      841 2023-07-04 01:19:08.069987 roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      500 2023-07-04 01:19:08.069987 roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     9636 2023-07-04 01:19:08.073987 roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc
+-rw-r--r--   0        0        0     3963 2023-07-04 01:19:08.109987 roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc
+-rw-r--r--   0        0        0     1666 2023-07-04 01:19:08.453988 roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc
+-rw-r--r--   0        0        0      216 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/http/constants.py
+-rw-r--r--   0        0        0     9060 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/http/http_client.py
+-rw-r--r--   0        0        0     3161 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/http/request_decorators.py
+-rw-r--r--   0        0        0     1004 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/http/testing_util.py
+-rw-r--r--   0        0        0      158 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/logging.py
+-rw-r--r--   0        0        0      224 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/pagination.py
+-rw-r--r--   0        0        0      168 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/profile/__init__.py
+-rw-r--r--   0        0        0      428 2023-07-04 01:19:08.449988 roboto_sdk-0.1.5/src/roboto_sdk/profile/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2991 2023-07-04 01:19:08.453988 roboto_sdk-0.1.5/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc
+-rw-r--r--   0        0        0     2977 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/py.typed
+-rw-r--r--   0        0        0     1250 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/serde.py
+-rw-r--r--   0        0        0      112 2023-07-04 01:18:05.645793 roboto_sdk-0.1.5/src/roboto_sdk/time.py
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 roboto_sdk-0.1.5/PKG-INFO
```

### Comparing `roboto_sdk-0.1.4/pyproject.toml` & `roboto_sdk-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires-python = ">=3.10"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto_sdk"
-version = "0.1.4"
+version = "0.1.5"
 description = "Tools for interacting with roboto.ai"
 license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 4037 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 c50f 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 c50f 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6403  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 0100 6403 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6508 8300 5a0b 6401 5a0c  m.Z...e...Z.d.Z.
@@ -26,16 +26,16 @@
 00000190: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
 000001a0: 005a 0264 0153 0029 02da 1652 656a 6563  .Z.d.S.)...Rejec
 000001b0: 7465 6454 6f6b 656e 4578 6365 7074 696f  tedTokenExceptio
 000001c0: 6e4e 2903 da08 5f5f 6e61 6d65 5f5f da0a  nN)...__name__..
 000001d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 000001e0: 616c 6e61 6d65 5f5f a900 720b 0000 0072  alname__..r....r
 000001f0: 0b00 0000 fae0 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000200: 2f6f 7574 7075 742f 7372 6334 3039 3837  /output/src40987
-00000210: 3536 3136 392f 7372 632f 636f 6465 7374  56169/src/codest
+00000200: 2f6f 7574 7075 742f 7372 6333 3439 3732  /output/src34972
+00000210: 3638 3637 302f 7372 632f 636f 6465 7374  68670/src/codest
 00000220: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000230: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000240: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000250: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000260: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000270: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000280: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
@@ -156,15 +156,15 @@
 000009b0: 0100 6400 5300 3100 7381 7701 0100 0100  ..d.S.1.s.w.....
 000009c0: 0100 5900 0100 6400 5300 290b 4efa 012f  ..Y...d.S.).N../
 000009d0: 7211 0000 00da 0172 5a10 7665 7269 6679  r......rZ.verify
 000009e0: 5f73 6967 6e61 7475 7265 4629 01da 076f  _signatureF)...o
 000009f0: 7074 696f 6e73 da03 6578 7054 2902 da07  ptions..expT)...
 00000a00: 7061 7265 6e74 73da 0865 7869 7374 5f6f  parents..exist_o
 00000a10: 6bda 0177 2914 7219 0000 0072 1a00 0000  k..w).r....r....
-00000a20: 7212 0000 005a 0967 6574 5f65 6e74 7279  r....Z.get_entry
+00000a20: 7212 0000 00da 0967 6574 5f65 6e74 7279  r......get_entry
 00000a30: da07 7061 7468 6c69 62da 0450 6174 68da  ..pathlib..Path.
 00000a40: 0e52 4f42 4f54 4f5f 5445 4d50 4449 5272  .ROBOTO_TEMPDIRr
 00000a50: 1e00 0000 da06 6578 6973 7473 da04 6f70  ......exists..op
 00000a60: 656e da04 7265 6164 da03 6a77 74da 0664  en..read..jwt..d
 00000a70: 6563 6f64 65da 0d66 726f 6d74 696d 6573  ecode..fromtimes
 00000a80: 7461 6d70 7210 0000 0072 1100 0000 722c  tampr....r....r,
 00000a90: 0000 0072 1d00 0000 da05 6d6b 6469 72da  ...r......mkdir.
@@ -189,49 +189,49 @@
 00000bc0: 3149 4420 546f 6b65 6e20 6973 2075 6e61  1ID Token is una
 00000bd0: 7661 696c 6162 6c65 206f 7220 7374 616c  vailable or stal
 00000be0: 652c 2072 6567 656e 6572 6174 696e 6720  e, regenerating 
 00000bf0: 6974 7a1e 4944 2054 6f6b 656e 2069 7320  itz.ID Token is 
 00000c00: 616c 7265 6164 7920 6176 6169 6c61 626c  already availabl
 00000c10: 6521 2907 7219 0000 0072 1a00 0000 7211  e!).r....r....r.
 00000c20: 0000 0072 1000 0000 da03 6c6f 67da 0564  ...r......log..d
-00000c30: 6562 7567 7243 0000 0029 0272 1b00 0000  ebugrC...).r....
+00000c30: 6562 7567 7244 0000 0029 0272 1b00 0000  ebugrD...).r....
 00000c40: 721a 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
 00000c50: 0c00 0000 da0c 6765 745f 6964 5f74 6f6b  ......get_id_tok
 00000c60: 656e 7100 0000 730e 0000 000a 0114 010a  enq...s.........
 00000c70: 0108 0106 040a fe06 027a 1e42 6561 7265  .........z.Beare
 00000c80: 7254 6f6b 656e 5665 6e64 6f72 2e67 6574  rTokenVendor.get
 00000c90: 5f69 645f 746f 6b65 6e63 0100 0000 0000  _id_tokenc......
 00000ca0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
 00000cb0: 0000 730e 0000 0064 017c 00a0 00a1 009b  ..s....d.|......
 00000cc0: 009d 0253 0029 024e 7a07 4265 6172 6572  ...S.).Nz.Bearer
-00000cd0: 2029 0172 4600 0000 2901 721b 0000 0072   ).rF...).r....r
+00000cd0: 2029 0172 4700 0000 2901 721b 0000 0072   ).rG...).r....r
 00000ce0: 0b00 0000 720b 0000 0072 0c00 0000 da0f  ....r....r......
 00000cf0: 6765 745f 6175 7468 5f68 6561 6465 727b  get_auth_header{
 00000d00: 0000 0073 0200 0000 0e01 7a21 4265 6172  ...s......z!Bear
 00000d10: 6572 546f 6b65 6e56 656e 646f 722e 6765  erTokenVendor.ge
 00000d20: 745f 6175 7468 5f68 6561 6465 7229 0e72  t_auth_header).r
 00000d30: 0800 0000 7209 0000 0072 0a00 0000 da03  ....r....r......
 00000d40: 7374 72da 0f5f 5f61 6e6e 6f74 6174 696f  str..__annotatio
 00000d50: 6e73 5f5f 7202 0000 0072 1900 0000 7203  ns__r....r....r.
 00000d60: 0000 0072 0600 0000 721c 0000 0072 2c00  ...r....r....r,.
-00000d70: 0000 7243 0000 0072 4600 0000 7247 0000  ..rC...rF...rG..
+00000d70: 0000 7244 0000 0072 4700 0000 7248 0000  ..rD...rG...rH..
 00000d80: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
 00000d90: 720c 0000 0072 0d00 0000 1e00 0000 7326  r....r........s&
 00000da0: 0000 000a 0008 0108 010a 010c 0108 0102  ................
 00000db0: 0504 0104 fc02 0202 fe06 0302 fd02 040a  ................
 00000dc0: fc12 1008 1f08 1d0c 0a72 0d00 0000 2918  .........r....).
-00000dd0: 7219 0000 0072 3400 0000 da06 7479 7069  r....r4.....typi
+00000dd0: 7219 0000 0072 3500 0000 da06 7479 7069  r....r5.....typi
 00000de0: 6e67 7202 0000 0072 0300 0000 7217 0000  ngr....r....r...
-00000df0: 0072 3a00 0000 da07 6c6f 6767 696e 6772  .r:.....loggingr
-00000e00: 0500 0000 7215 0000 0072 0600 0000 7244  ....r....r....rD
+00000df0: 0072 3b00 0000 da07 6c6f 6767 696e 6772  .r;.....loggingr
+00000e00: 0500 0000 7215 0000 0072 0600 0000 7245  ....r....r....rE
 00000e10: 0000 005a 1362 6561 7265 725f 746f 6b65  ...Z.bearer_toke
 00000e20: 6e5f 7665 6e64 6f72 5a0b 6372 6564 5f66  n_vendorZ.cred_f
-00000e30: 696e 6465 7272 3500 0000 da04 686f 6d65  inderr5.....home
+00000e30: 696e 6465 7272 3600 0000 da04 686f 6d65  inderr6.....home
 00000e40: 5a10 4352 4544 454e 5449 414c 535f 4649  Z.CREDENTIALS_FI
-00000e50: 4c45 7236 0000 005a 0f50 524f 4649 4c45  LEr6...Z.PROFILE
+00000e50: 4c45 7237 0000 005a 0f50 524f 4649 4c45  LEr7...Z.PROFILE
 00000e60: 5f45 4e56 5f56 4152 5a0c 5553 4552 5f45  _ENV_VARZ.USER_E
 00000e70: 4e56 5f56 4152 5a0d 544f 4b45 4e5f 454e  NV_VARZ.TOKEN_EN
 00000e80: 565f 5641 52da 0945 7863 6570 7469 6f6e  V_VAR..Exception
 00000e90: 7207 0000 0072 0d00 0000 720b 0000 0072  r....r....r....r
 00000ea0: 0b00 0000 720b 0000 0072 0c00 0000 da08  ....r....r......
 00000eb0: 3c6d 6f64 756c 653e 0100 0000 7322 0000  <module>....s"..
 00000ec0: 0008 0308 0110 0108 0208 010c 020c 0106  ................
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/auth/pat.py` & `roboto_sdk-0.1.5/src/roboto_sdk/auth/pat.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/cli/command/args.py` & `roboto_sdk-0.1.5/src/roboto_sdk/cli/command/args.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/cli/command/model.py` & `roboto_sdk-0.1.5/src/roboto_sdk/cli/command/model.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/cli/context.py` & `roboto_sdk-0.1.5/src/roboto_sdk/cli/context.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/cli/datasets/commands.py` & `roboto_sdk-0.1.5/src/roboto_sdk/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/cli/entry.py` & `roboto_sdk-0.1.5/src/roboto_sdk/cli/entry.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/cli/orgs/commands.py` & `roboto_sdk-0.1.5/src/roboto_sdk/cli/orgs/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/cli/tokens/commands.py` & `roboto_sdk-0.1.5/src/roboto_sdk/cli/tokens/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/cli/triggers/commands.py` & `roboto_sdk-0.1.5/src/roboto_sdk/cli/triggers/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/cli/users/commands.py` & `roboto_sdk-0.1.5/src/roboto_sdk/cli/users/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__init__.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 1641 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 6906 0000  o........F.di...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 6906 0000  o.......Ms.di...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
@@ -72,15 +72,15 @@
 00000470: 7210 0000 0072 1100 0000 7212 0000 005a  r....r....r....Z
 00000480: 1169 6e76 6f63 6174 696f 6e5f 7265 636f  .invocation_reco
 00000490: 7264 7213 0000 0072 1400 0000 7215 0000  rdr....r....r...
 000004a0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
 000004b0: 7219 0000 00da 075f 5f61 6c6c 5f5f a900  r......__all__..
 000004c0: 721d 0000 0072 1d00 0000 faef 2f63 6f64  r....r....../cod
 000004d0: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-000004e0: 6334 3039 3837 3536 3136 392f 7372 632f  c4098756169/src/
+000004e0: 6333 3439 3732 3638 3637 302f 7372 632f  c3497268670/src/
 000004f0: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000500: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000510: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000520: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 00000530: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000540: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 00000550: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 7427 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 031d 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 031d 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6403 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 6d0a 5a0a 0100 6405 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6408 6c0d 6d0e 5a0e 0100 6405  ..d.d.l.m.Z...d.
@@ -56,43 +56,43 @@
 00000370: 0c66 0219 0066 0864 2d64 2e84 055a 2164  .f...f.d-d...Z!d
 00000380: 0f65 0d65 0c65 0e66 0219 0066 0264 2f64  .e.e.e.f...f.d/d
 00000390: 3084 045a 2209 0509 0509 0564 3864 3165  0..Z"......d8d1e
 000003a0: 0d65 0c65 0e66 0219 0064 3265 0965 0f65  .e.e.f...d2e.e.e
 000003b0: 2319 0019 0064 0a65 0965 0c19 0064 3365  #....d.e.e...d3e
 000003c0: 0965 0c19 0064 0f64 0566 0a64 3464 3584  .e...d.d.f.d4d5.
 000003d0: 055a 2464 0553 0029 39da 0641 6374 696f  .Z$d.S.)9..Actio
-000003e0: 6e3e 0700 0000 da03 7572 69da 066f 7267  n>......uri..org
-000003f0: 5f69 645a 0a63 7265 6174 6564 5f61 74da  _idZ.created_at.
-00000400: 086d 6f64 6966 6965 645a 0b6d 6f64 6966  .modifiedZ.modif
-00000410: 6965 645f 6279 da0a 6372 6561 7465 645f  ied_by..created_
-00000420: 6279 da04 6e61 6d65 da18 5f41 6374 696f  by..name.._Actio
+000003e0: 6e3e 0700 0000 da08 6d6f 6469 6669 6564  n>......modified
+000003f0: da04 6e61 6d65 da0a 6372 6561 7465 645f  ..name..created_
+00000400: 6279 da06 6f72 675f 6964 da03 7572 695a  by..org_id..uriZ
+00000410: 0a63 7265 6174 6564 5f61 745a 0b6d 6f64  .created_atZ.mod
+00000420: 6966 6965 645f 6279 da18 5f41 6374 696f  ified_by.._Actio
 00000430: 6e5f 5f61 6374 696f 6e5f 6465 6c65 6761  n__action_delega
 00000440: 7465 da1c 5f41 6374 696f 6e5f 5f69 6e76  te.._Action__inv
 00000450: 6f63 6174 696f 6e5f 6465 6c65 6761 7465  ocation_delegate
 00000460: da0f 5f41 6374 696f 6e5f 5f72 6563 6f72  .._Action__recor
 00000470: 644e da23 5f41 6374 696f 6e5f 5f74 656d  dN.#_Action__tem
 00000480: 705f 636f 6e74 6169 6e65 725f 6372 6564  p_container_cred
-00000490: 656e 7469 616c 7372 1500 0000 da0f 6163  entialsr......ac
+00000490: 656e 7469 616c 7372 1200 0000 da0f 6163  entialsr......ac
 000004a0: 7469 6f6e 5f64 656c 6567 6174 65da 1369  tion_delegate..i
 000004b0: 6e76 6f63 6174 696f 6e5f 6465 6c65 6761  nvocation_delega
-000004c0: 7465 7212 0000 00da 0b64 6573 6372 6970  ter......descrip
+000004c0: 7465 7214 0000 00da 0b64 6573 6372 6970  ter......descrip
 000004d0: 7469 6f6e da08 6d65 7461 6461 7461 da04  tion..metadata..
-000004e0: 7461 6773 7214 0000 00da 0672 6574 7572  tagsr......retur
+000004e0: 7461 6773 7213 0000 00da 0672 6574 7572  tagsr......retur
 000004f0: 6e63 0900 0000 0000 0000 0000 0000 0a00  nc..............
 00000500: 0000 0800 0000 4300 0000 7320 0000 007c  ......C...s ...|
 00000510: 02a0 007c 017c 047c 087c 057c 067c 07a1  ...|.|.|.|.|.|..
 00000520: 067d 097c 007c 097c 027c 0383 0353 00a9  .}.|.|.|.|...S..
 00000530: 014e 2901 5a0d 6372 6561 7465 5f61 6374  .N).Z.create_act
-00000540: 696f 6e29 0ada 0363 6c73 7215 0000 0072  ion)...clsr....r
-00000550: 1a00 0000 721b 0000 0072 1200 0000 721c  ....r....r....r.
-00000560: 0000 0072 1d00 0000 721e 0000 0072 1400  ...r....r....r..
+00000540: 696f 6e29 0ada 0363 6c73 7212 0000 0072  ion)...clsr....r
+00000550: 1a00 0000 721b 0000 0072 1400 0000 721c  ....r....r....r.
+00000560: 0000 0072 1d00 0000 721e 0000 0072 1300  ...r....r....r..
 00000570: 0000 da06 7265 636f 7264 a900 7223 0000  ....record..r#..
 00000580: 00fa ed2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000590: 7470 7574 2f73 7263 3430 3938 3735 3631  tput/src40987561
-000005a0: 3639 2f73 7263 2f63 6f64 6573 7461 722d  69/src/codestar-
+00000590: 7470 7574 2f73 7263 3334 3937 3236 3836  tput/src34972686
+000005a0: 3730 2f73 7263 2f63 6f64 6573 7461 722d  70/src/codestar-
 000005b0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000005c0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000005d0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 000005e0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 000005f0: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 00000600: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000610: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
@@ -106,16 +106,16 @@
 00000690: fa0c 087a 0d41 6374 696f 6e2e 6372 6561  ...z.Action.crea
 000006a0: 7465 6305 0000 0000 0000 0000 0000 0006  tec.............
 000006b0: 0000 0004 0000 0043 0000 0073 1800 0000  .......C...s....
 000006c0: 7c02 a000 7c01 7c04 a102 7d05 7c00 7c05  |...|.|...}.|.|.
 000006d0: 7c02 7c03 8303 5300 7220 0000 0029 015a  |.|...S.r ...).Z
 000006e0: 1967 6574 5f61 6374 696f 6e5f 6279 5f70  .get_action_by_p
 000006f0: 7269 6d61 7279 5f6b 6579 2906 7221 0000  rimary_key).r!..
-00000700: 0072 1500 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000710: 7212 0000 0072 2200 0000 7223 0000 0072  r....r"...r#...r
+00000700: 0072 1200 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000710: 7214 0000 0072 2200 0000 7223 0000 0072  r....r"...r#...r
 00000720: 2300 0000 7224 0000 00da 0966 726f 6d5f  #...r$.....from_
 00000730: 6e61 6d65 3c00 0000 7304 0000 000c 080c  name<...s.......
 00000740: 017a 1041 6374 696f 6e2e 6672 6f6d 5f6e  .z.Action.from_n
 00000750: 616d 65da 0766 696c 7465 7273 2903 7210  ame..filters).r.
 00000760: 0000 004e 4e63 0500 0000 0000 0000 0000  ...NNc..........
 00000770: 0000 0c00 0000 0600 0000 6300 0000 73a2  ..........c...s.
 00000780: 0000 0081 0074 0074 016a 02a0 03a1 0083  .....t.t.j......
@@ -131,23 +131,23 @@
 00000820: 0053 0071 3429 094e 7206 0000 007a 2261  .S.q4).Nr....z"a
 00000830: 7265 206e 6f74 206b 6e6f 776e 2061 7474  re not known att
 00000840: 7269 6275 7465 7320 6f66 2041 6374 696f  ributes of Actio
 00000850: 6e7a 2269 7320 6e6f 7420 6120 6b6e 6f77  nz"is not a know
 00000860: 6e20 6174 7472 6962 7574 6520 6f66 2041  n attribute of A
 00000870: 6374 696f 6eda 0120 7a14 2e20 4b6e 6f77  ction.. z.. Know
 00000880: 6e20 6174 7472 6962 7574 6573 3a20 2901  n attributes: ).
-00000890: 7212 0000 0054 2902 7212 0000 005a 0a70  r....T).r....Z.p
+00000890: 7214 0000 0054 2902 7214 0000 005a 0a70  r....T).r....Z.p
 000008a0: 6167 655f 746f 6b65 6e29 09da 0373 6574  age_token)...set
 000008b0: 720a 0000 00da 0a5f 5f66 6965 6c64 735f  r......__fields_
 000008c0: 5fda 046b 6579 73da 036c 656e da0a 5661  _..keys..len..Va
 000008d0: 6c75 6545 7272 6f72 5a0d 7175 6572 795f  lueErrorZ.query_
-000008e0: 6163 7469 6f6e 73da 0569 7465 6d73 5a0a  actions..itemsZ.
+000008e0: 6163 7469 6f6e 73da 0569 7465 6d73 da0a  actions..items..
 000008f0: 6e65 7874 5f74 6f6b 656e 290c 7221 0000  next_token).r!..
 00000900: 0072 2700 0000 721a 0000 0072 1b00 0000  .r'...r....r....
-00000910: 7212 0000 00da 0a6b 6e6f 776e 5f6b 6579  r......known_key
+00000910: 7214 0000 00da 0a6b 6e6f 776e 5f6b 6579  r......known_key
 00000920: 735a 0b61 6374 7561 6c5f 6b65 7973 5a0c  sZ.actual_keysZ.
 00000930: 756e 6b6e 6f77 6e5f 6b65 7973 da06 706c  unknown_keys..pl
 00000940: 7572 616c da03 6d73 675a 1170 6167 696e  ural..msgZ.pagin
 00000950: 6174 6564 5f72 6573 756c 7473 7222 0000  ated_resultsr"..
 00000960: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
 00000970: da05 7175 6572 7947 0000 0073 2a00 0000  ..queryG...s*...
 00000980: 0280 0e08 0c01 0801 0401 0c01 0203 06ff  ................
@@ -162,41 +162,41 @@
 00000a10: 2200 0000 721a 0000 0072 1b00 0000 7223  "...r....r....r#
 00000a20: 0000 0072 2300 0000 7224 0000 00da 085f  ...r#...r$....._
 00000a30: 5f69 6e69 745f 5f66 0000 0073 0600 0000  _init__f...s....
 00000a40: 0606 0601 0a01 7a0f 4163 7469 6f6e 2e5f  ......z.Action._
 00000a50: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
 00000a60: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
 00000a70: f308 0000 007c 006a 006a 0153 0072 2000  .....|.j.j.S.r .
-00000a80: 0000 2902 7218 0000 0072 1500 0000 a901  ..).r....r......
-00000a90: 7233 0000 0072 2300 0000 7223 0000 0072  r3...r#...r#...r
-00000aa0: 2400 0000 7215 0000 0070 0000 00f3 0200  $...r....p......
+00000a80: 0000 2902 7218 0000 0072 1200 0000 a901  ..).r....r......
+00000a90: 7234 0000 0072 2300 0000 7223 0000 0072  r4...r#...r#...r
+00000aa0: 2400 0000 7212 0000 0070 0000 00f3 0200  $...r....p......
 00000ab0: 0000 0802 7a0b 4163 7469 6f6e 2e6e 616d  ....z.Action.nam
 00000ac0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-00000ad0: 0000 0100 0000 4300 0000 7235 0000 0072  ......C...r5...r
-00000ae0: 2000 0000 2902 7218 0000 0072 1200 0000   ...).r....r....
-00000af0: 7236 0000 0072 2300 0000 7223 0000 0072  r6...r#...r#...r
-00000b00: 2400 0000 7212 0000 0074 0000 0072 3700  $...r....t...r7.
+00000ad0: 0000 0100 0000 4300 0000 7236 0000 0072  ......C...r6...r
+00000ae0: 2000 0000 2902 7218 0000 0072 1400 0000   ...).r....r....
+00000af0: 7237 0000 0072 2300 0000 7223 0000 0072  r7...r#...r#...r
+00000b00: 2400 0000 7214 0000 0074 0000 0072 3800  $...r....t...r8.
 00000b10: 0000 7a0d 4163 7469 6f6e 2e6f 7267 5f69  ..z.Action.org_i
 00000b20: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
-00000b30: 0000 0100 0000 4300 0000 7235 0000 0072  ......C...r5...r
-00000b40: 2000 0000 2902 7218 0000 0072 1100 0000   ...).r....r....
-00000b50: 7236 0000 0072 2300 0000 7223 0000 0072  r6...r#...r#...r
-00000b60: 2400 0000 7211 0000 0078 0000 0072 3700  $...r....x...r7.
+00000b30: 0000 0100 0000 4300 0000 7236 0000 0072  ......C...r6...r
+00000b40: 2000 0000 2902 7218 0000 0072 1500 0000   ...).r....r....
+00000b50: 7237 0000 0072 2300 0000 7223 0000 0072  r7...r#...r#...r
+00000b60: 2400 0000 7215 0000 0078 0000 0072 3800  $...r....x...r8.
 00000b70: 0000 7a0a 4163 7469 6f6e 2e75 7269 da06  ..z.Action.uri..
 00000b80: 6361 6c6c 6572 6302 0000 0000 0000 0000  callerc.........
 00000b90: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
 00000ba0: 3000 0000 7c00 6a00 6400 7500 730a 7c00  0...|.j.d.u.s.|.
 00000bb0: 6a00 a001 a100 7215 7c00 6a02 a003 7c00  j.....r.|.j...|.
 00000bc0: 6a04 7c01 a102 7d02 7c02 7c00 5f00 7c00  j.|...}.|.|._.|.
 00000bd0: 6a00 5300 7220 0000 0029 0572 1900 0000  j.S.r ...).r....
 00000be0: da0a 6973 5f65 7870 6972 6564 7216 0000  ..is_expiredr...
 00000bf0: 005a 1e67 6574 5f74 656d 705f 636f 6e74  .Z.get_temp_cont
 00000c00: 6169 6e65 725f 6372 6564 656e 7469 616c  ainer_credential
-00000c10: 7372 1800 0000 2903 7233 0000 0072 3800  sr....).r3...r8.
-00000c20: 0000 5a05 6372 6564 7372 2300 0000 7223  ..Z.credsr#...r#
+00000c10: 7372 1800 0000 2903 7234 0000 0072 3900  sr....).r4...r9.
+00000c20: 0000 da05 6372 6564 7372 2300 0000 7223  ....credsr#...r#
 00000c30: 0000 0072 2400 0000 da23 6765 745f 7465  ...r$....#get_te
 00000c40: 6d70 6f72 6172 795f 636f 6e74 6169 6e65  mporary_containe
 00000c50: 725f 6372 6564 656e 7469 616c 737c 0000  r_credentials|..
 00000c60: 0073 1000 0000 0a04 0801 02ff 0603 0601  .s..............
 00000c70: 04ff 0603 0602 7a2a 4163 7469 6f6e 2e67  ......z*Action.g
 00000c80: 6574 5f74 656d 706f 7261 7279 5f63 6f6e  et_temporary_con
 00000c90: 7461 696e 6572 5f63 7265 6465 6e74 6961  tainer_credentia
@@ -216,18 +216,18 @@
 00000d70: 7573 7420 6265 2061 7373 6f63 6961 7465  ust be associate
 00000d80: 6420 7769 7468 2074 6869 7320 4163 7469  d with this Acti
 00000d90: 6f6e 2061 6e64 2070 7573 6865 6420 6265  on and pushed be
 00000da0: 666f 7265 2069 7420 6361 6e20 6265 2069  fore it can be i
 00000db0: 6e76 6f6b 6564 2908 7218 0000 005a 0c69  nvoked).r....Z.i
 00000dc0: 735f 6176 6169 6c61 626c 6572 0b00 0000  s_availabler....
 00000dd0: 7217 0000 005a 1163 7265 6174 655f 696e  r....Z.create_in
-00000de0: 766f 6361 7469 6f6e 7215 0000 0072 1200  vocationr....r..
-00000df0: 0000 720c 0000 0029 0772 3300 0000 723b  ..r....).r3...r;
-00000e00: 0000 0072 3c00 0000 723d 0000 0072 3e00  ...r<...r=...r>.
-00000e10: 0000 723f 0000 0072 2200 0000 7223 0000  ..r?...r"...r#..
+00000de0: 766f 6361 7469 6f6e 7212 0000 0072 1400  vocationr....r..
+00000df0: 0000 720c 0000 0029 0772 3400 0000 723d  ..r....).r4...r=
+00000e00: 0000 0072 3e00 0000 723f 0000 0072 4000  ...r>...r?...r@.
+00000e10: 0000 7241 0000 0072 2200 0000 7223 0000  ..rA...r"...r#..
 00000e20: 0072 2300 0000 7224 0000 00da 0669 6e76  .r#...r$.....inv
 00000e30: 6f6b 658a 0000 0073 2200 0000 0c08 0201  oke....s".......
 00000e40: 0201 04ff 0604 0601 0201 0201 0201 0201  ................
 00000e50: 0201 0601 04f9 0209 0201 0401 04fe 7a0d  ..............z.
 00000e60: 4163 7469 6f6e 2e69 6e76 6f6b 65da 0a69  Action.invoke..i
 00000e70: 6d61 6765 5f6e 616d 65da 0969 6d61 6765  mage_name..image
 00000e80: 5f74 6167 6304 0000 0000 0000 0000 0000  _tagc...........
@@ -303,24 +303,24 @@
 000012e0: 206f 6e20 7468 6520 636c 6965 6e74 2e20   on the client. 
 000012f0: 4974 2069 7320 6465 7465 726d 696e 6564  It is determined
 00001300: 2073 6572 7665 722d 7369 6465 2076 6961   server-side via
 00001310: 2074 6865 2069 6465 6e74 6974 792f 6163   the identity/ac
 00001320: 6365 7373 206d 6563 6861 6e69 736d 2e0a  cess mechanism..
 00001330: 2020 2020 2020 2020 2903 7216 0000 00da          ).r.....
 00001340: 1272 6567 6973 7465 725f 636f 6e74 6169  .register_contai
-00001350: 6e65 7272 1800 0000 2904 7233 0000 0072  nerr....).r3...r
-00001360: 4100 0000 7242 0000 0072 3800 0000 7223  A...rB...r8...r#
-00001370: 0000 0072 2300 0000 7224 0000 0072 4300  ...r#...r$...rC.
+00001350: 6e65 7272 1800 0000 2904 7234 0000 0072  nerr....).r4...r
+00001360: 4300 0000 7244 0000 0072 3900 0000 7223  C...rD...r9...r#
+00001370: 0000 0072 2300 0000 7224 0000 0072 4500  ...r#...r$...rE.
 00001380: 0000 a500 0000 7306 0000 0006 180a 0104  ......s.........
 00001390: ff7a 1941 6374 696f 6e2e 7265 6769 7374  .z.Action.regist
 000013a0: 6572 5f63 6f6e 7461 696e 6572 6301 0000  er_containerc...
 000013b0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
 000013c0: 0043 0000 0073 0a00 0000 7400 7c00 6a01  .C...s....t.|.j.
 000013d0: 8301 5300 7220 0000 0029 0272 0500 0000  ..S.r ...).r....
-000013e0: 7218 0000 0072 3600 0000 7223 0000 0072  r....r6...r#...r
+000013e0: 7218 0000 0072 3700 0000 7223 0000 0072  r....r7...r#...r
 000013f0: 2300 0000 7224 0000 00da 0774 6f5f 6469  #...r$.....to_di
 00001400: 6374 c100 0000 7302 0000 000a 017a 0e41  ct....s......z.A
 00001410: 6374 696f 6e2e 746f 5f64 6963 74da 0775  ction.to_dict..u
 00001420: 7064 6174 6573 da0a 636f 6e64 6974 696f  pdates..conditio
 00001430: 6e73 da0a 7570 6461 7465 645f 6279 6305  ns..updated_byc.
 00001440: 0000 0000 0000 0000 0000 000b 0000 0007  ................
 00001450: 0000 0043 0000 0073 8000 0000 7400 7401  ...C...s....t.t.
@@ -339,41 +339,41 @@
 00001520: 7574 6572 2800 0000 7a19 2e20 5570 6461  uter(...z.. Upda
 00001530: 7465 6162 6c65 2061 7474 7269 6275 7465  teable attribute
 00001540: 733a 2029 0b72 2900 0000 720a 0000 0072  s: ).r)...r....r
 00001550: 2a00 0000 722b 0000 0072 1000 0000 da15  *...r+...r......
 00001560: 4449 5341 4c4c 4f57 4544 5f46 4f52 5f55  DISALLOWED_FOR_U
 00001570: 5044 4154 4572 2c00 0000 722d 0000 0072  PDATEr,...r-...r
 00001580: 1600 0000 da06 7570 6461 7465 7218 0000  ......updater...
-00001590: 0029 0b72 3300 0000 7245 0000 0072 4600  .).r3...rE...rF.
-000015a0: 0000 7212 0000 0072 4700 0000 722f 0000  ..r....rG...r/..
+00001590: 0029 0b72 3400 0000 7247 0000 0072 4800  .).r4...rG...rH.
+000015a0: 0000 7214 0000 0072 4900 0000 7230 0000  ..r....rI...r0..
 000015b0: 00da 0c61 6c6c 6f77 6564 5f6b 6579 735a  ...allowed_keysZ
-000015c0: 0975 6e61 6c6c 6f77 6564 7230 0000 0072  .unallowedr0...r
-000015d0: 3100 0000 da07 7570 6461 7465 6472 2300  1.....updatedr#.
-000015e0: 0000 7223 0000 0072 2400 0000 7249 0000  ..r#...r$...rI..
+000015c0: 0975 6e61 6c6c 6f77 6564 7231 0000 0072  .unallowedr1...r
+000015d0: 3200 0000 da07 7570 6461 7465 6472 2300  2.....updatedr#.
+000015e0: 0000 7223 0000 0072 2400 0000 724b 0000  ..r#...r$...rK..
 000015f0: 00c4 0000 0073 2000 0000 0e07 0a01 1001  .....s .........
 00001600: 0801 0c01 0203 06ff 0202 02fd 0205 1201  ................
 00001610: 04ff 0604 0c01 04ff 0a03 7a0d 4163 7469  ..........z.Acti
 00001620: 6f6e 2e75 7064 6174 6529 054e 4e4e 4e4e  on.update).NNNNN
 00001630: 7220 0000 0029 034e 4e4e 2925 da08 5f5f  r ...).NNN)%..__
 00001640: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 00001650: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00001660: 7248 0000 0072 0700 0000 da0f 5f5f 616e  rH...r......__an
+00001660: 724a 0000 0072 0700 0000 da0f 5f5f 616e  rJ...r......__an
 00001670: 6e6f 7461 7469 6f6e 735f 5f72 0d00 0000  notations__r....
 00001680: 720a 0000 0072 1900 0000 7203 0000 0072  r....r....r....r
 00001690: 0800 0000 da0b 636c 6173 736d 6574 686f  ......classmetho
 000016a0: 64da 0373 7472 da04 6469 6374 7202 0000  d..str..dictr...
 000016b0: 00da 046c 6973 7472 2500 0000 7226 0000  ...listr%...r&..
 000016c0: 00da 0b63 6f6c 6c65 6374 696f 6e73 da03  ...collections..
-000016d0: 6162 63da 0947 656e 6572 6174 6f72 7232  abc..Generatorr2
-000016e0: 0000 0072 3400 0000 da08 7072 6f70 6572  ...r4.....proper
-000016f0: 7479 7215 0000 0072 1200 0000 7211 0000  tyr....r....r...
-00001700: 0072 3a00 0000 720e 0000 0072 0f00 0000  .r:...r....r....
-00001710: 720c 0000 0072 4000 0000 da05 7475 706c  r....r@.....tupl
-00001720: 6572 4300 0000 7244 0000 0072 0900 0000  erC...rD...r....
-00001730: 7249 0000 0072 2300 0000 7223 0000 0072  rI...r#...r#...r
+000016d0: 6162 63da 0947 656e 6572 6174 6f72 7233  abc..Generatorr3
+000016e0: 0000 0072 3500 0000 da08 7072 6f70 6572  ...r5.....proper
+000016f0: 7479 7212 0000 0072 1400 0000 7215 0000  tyr....r....r...
+00001700: 0072 3c00 0000 720e 0000 0072 0f00 0000  .r<...r....r....
+00001710: 720c 0000 0072 4200 0000 da05 7475 706c  r....rB.....tupl
+00001720: 6572 4500 0000 7246 0000 0072 0900 0000  erE...rF...r....
+00001730: 724b 0000 0072 2300 0000 7223 0000 0072  rK...r#...r#...r
 00001740: 2300 0000 7224 0000 0072 1000 0000 1600  #...r$...r......
 00001750: 0000 73e8 0000 000a 0008 0108 0a08 0108  ..s.............
 00001760: 0110 0102 0202 0602 0102 0102 0102 0104  ................
 00001770: f702 0202 fe02 0302 fd02 0402 fc06 0502  ................
 00001780: fb06 0602 fa0e 0702 f90a 0802 f806 0902  ................
 00001790: f702 0a0c f602 1502 0604 fb02 0202 fe02  ................
 000017a0: 0302 fd02 0402 fc06 0502 fb02 060c fa02  ................
@@ -383,15 +383,15 @@
 000017e0: 0310 0102 0314 0102 0404 ff06 0102 ff02  ................
 000017f0: 020a fe02 0e06 0202 fe02 0302 fd02 0402  ................
 00001800: fc02 0502 fb06 0602 fa02 070a f902 1f04  ................
 00001810: fc02 0202 fe02 0302 fd06 0402 fc0a 050a  ................
 00001820: fb16 1c02 0602 0102 0104 fb0a 0202 fe0a  ................
 00001830: 0302 fd06 0402 fc06 0502 fb02 060e fa72  ...............r
 00001840: 1000 0000 2917 da0f 636f 6c6c 6563 7469  ....)...collecti
-00001850: 6f6e 732e 6162 6372 5400 0000 da06 7479  ons.abcrT.....ty
+00001850: 6f6e 732e 6162 6372 5600 0000 da06 7479  ons.abcrV.....ty
 00001860: 7069 6e67 7202 0000 0072 0300 0000 da05  pingr....r......
 00001870: 7365 7264 6572 0500 0000 721a 0000 0072  serder....r....r
 00001880: 0700 0000 7208 0000 0072 0900 0000 da0d  ....r....r......
 00001890: 6163 7469 6f6e 5f72 6563 6f72 6472 0a00  action_recordr..
 000018a0: 0000 da05 6572 726f 7272 0b00 0000 da0a  ....errorr......
 000018b0: 696e 766f 6361 7469 6f6e 720c 0000 0072  invocationr....r
 000018c0: 1b00 0000 720d 0000 00da 1169 6e76 6f63  ....r......invoc
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 3015 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 c70b 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 c70b 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6401 6c06 5a06 6403 6404 6c07  ..d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 0100 6403 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6403 6406 6c0b 6d0c 5a0c 0100 6407  ..d.d.l.m.Z...d.
@@ -31,15 +31,15 @@
 000001e0: 6cda 0a65 7870 6972 6174 696f 6eda 0672  l..expiration..r
 000001f0: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
 00000200: 0000 0100 0000 0200 0000 4300 0000 730c  ..........C...s.
 00000210: 0000 0074 0083 007c 006a 016b 0553 00a9  ...t...|.j.k.S..
 00000220: 014e 2902 7209 0000 0072 1000 0000 a901  .N).r....r......
 00000230: da04 7365 6c66 a900 7215 0000 00fa f62f  ..self..r....../
 00000240: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000250: 2f73 7263 3430 3938 3735 3631 3639 2f73  /src4098756169/s
+00000250: 2f73 7263 3334 3937 3236 3836 3730 2f73  /src3497268670/s
 00000260: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000270: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000280: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000290: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 000002a0: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 000002b0: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 000002c0: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
@@ -95,15 +95,15 @@
 000005e0: 6d61 7a6f 6e2e 636f 6d2f 616d 617a 6f6e  mazon.com/amazon
 000005f0: 6479 6e61 6d6f 6462 2f6c 6174 6573 742f  dynamodb/latest/
 00000600: 6465 7665 6c6f 7065 7267 7569 6465 2f45  developerguide/E
 00000610: 7870 7265 7373 696f 6e73 2e4f 7065 7261  xpressions.Opera
 00000620: 746f 7273 416e 6446 756e 6374 696f 6e73  torsAndFunctions
 00000630: 2e68 746d 6c0a 2020 2020 da03 6b65 79da  .html.    ..key.
 00000640: 0576 616c 7565 2902 da02 6571 da02 6e65  .value)...eq..ne
-00000650: 5a0a 636f 6d70 6172 6174 6f72 4e29 0872  Z.comparatorN).r
+00000650: da0a 636f 6d70 6172 6174 6f72 4e29 0872  ..comparatorN).r
 00000660: 1900 0000 721a 0000 0072 1b00 0000 da07  ....r....r......
 00000670: 5f5f 646f 635f 5f72 1c00 0000 721d 0000  __doc__r....r...
 00000680: 0072 0200 0000 7203 0000 0072 1500 0000  .r....r....r....
 00000690: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
 000006a0: 2100 0000 1a00 0000 730a 0000 000a 0004  !.......s.......
 000006b0: 0108 0908 0110 0372 2100 0000 6300 0000  .......r!...c...
 000006c0: 0000 0000 0000 0000 0000 0000 0010 0000  ................
@@ -136,99 +136,99 @@
 00000870: 0b64 6573 6372 6970 7469 6f6e da08 6d65  .description..me
 00000880: 7461 6461 7461 da04 7461 6773 7211 0000  tadata..tagsr...
 00000890: 0063 0700 0000 0000 0000 0000 0000 0700  .c..............
 000008a0: 0000 0200 0000 4300 0000 f308 0000 0074  ......C........t
 000008b0: 0064 0183 0182 0129 024e da0d 6372 6561  .d.....).N..crea
 000008c0: 7465 5f61 6374 696f 6ea9 01da 134e 6f74  te_action....Not
 000008d0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-000008e0: 2907 7214 0000 0072 2800 0000 7229 0000  ).r....r(...r)..
-000008f0: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-00000900: 722d 0000 0072 1500 0000 7215 0000 0072  r-...r....r....r
-00000910: 1600 0000 722f 0000 002c 0000 0073 0200  ....r/...,...s..
+000008e0: 2907 7214 0000 0072 2900 0000 722a 0000  ).r....r)...r*..
+000008f0: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+00000900: 722e 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
+00000910: 1600 0000 7230 0000 002c 0000 0073 0200  ....r0...,...s..
 00000920: 0000 080a 7a1c 4163 7469 6f6e 4465 6c65  ....z.ActionDele
 00000930: 6761 7465 2e63 7265 6174 655f 6163 7469  gate.create_acti
 00000940: 6f6e 6303 0000 0000 0000 0000 0000 0003  onc.............
-00000950: 0000 0002 0000 0043 0000 0072 2e00 0000  .......C...r....
+00000950: 0000 0002 0000 0043 0000 0072 2f00 0000  .......C...r/...
 00000960: 2902 4eda 1967 6574 5f61 6374 696f 6e5f  ).N..get_action_
-00000970: 6279 5f70 7269 6d61 7279 5f6b 6579 7230  by_primary_keyr0
-00000980: 0000 0029 0372 1400 0000 7228 0000 0072  ...).r....r(...r
-00000990: 2900 0000 7215 0000 0072 1500 0000 7216  )...r....r....r.
-000009a0: 0000 0072 3200 0000 3800 0000 7302 0000  ...r2...8...s...
+00000970: 6279 5f70 7269 6d61 7279 5f6b 6579 7231  by_primary_keyr1
+00000980: 0000 0029 0372 1400 0000 7229 0000 0072  ...).r....r)...r
+00000990: 2a00 0000 7215 0000 0072 1500 0000 7216  *...r....r....r.
+000009a0: 0000 0072 3300 0000 3800 0000 7302 0000  ...r3...8...s...
 000009b0: 0008 047a 2841 6374 696f 6e44 656c 6567  ...z(ActionDeleg
 000009c0: 6174 652e 6765 745f 6163 7469 6f6e 5f62  ate.get_action_b
 000009d0: 795f 7072 696d 6172 795f 6b65 79da 0672  y_primary_key..r
 000009e0: 6563 6f72 64da 0a69 6d61 6765 5f6e 616d  ecord..image_nam
 000009f0: 65da 0969 6d61 6765 5f74 6167 da06 6361  e..image_tag..ca
 00000a00: 6c6c 6572 6305 0000 0000 0000 0000 0000  llerc...........
-00000a10: 0005 0000 0002 0000 0043 0000 0072 2e00  .........C...r..
+00000a10: 0005 0000 0002 0000 0043 0000 0072 2f00  .........C...r/.
 00000a20: 0000 2902 4eda 1272 6567 6973 7465 725f  ..).N..register_
-00000a30: 636f 6e74 6169 6e65 7272 3000 0000 2905  containerr0...).
-00000a40: 7214 0000 0072 3300 0000 7234 0000 0072  r....r3...r4...r
-00000a50: 3500 0000 7236 0000 0072 1500 0000 7215  5...r6...r....r.
-00000a60: 0000 0072 1600 0000 7237 0000 003e 0000  ...r....r7...>..
+00000a30: 636f 6e74 6169 6e65 7272 3100 0000 2905  containerr1...).
+00000a40: 7214 0000 0072 3400 0000 7235 0000 0072  r....r4...r5...r
+00000a50: 3600 0000 7237 0000 0072 1500 0000 7215  6...r7...r....r.
+00000a60: 0000 0072 1600 0000 7238 0000 003e 0000  ...r....r8...>..
 00000a70: 0073 0200 0000 0808 7a21 4163 7469 6f6e  .s......z!Action
 00000a80: 4465 6c65 6761 7465 2e72 6567 6973 7465  Delegate.registe
 00000a90: 725f 636f 6e74 6169 6e65 7263 0300 0000  r_containerc....
 00000aa0: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00000ab0: 4300 0000 722e 0000 0029 024e da1e 6765  C...r....).N..ge
+00000ab0: 4300 0000 722f 0000 0029 024e da1e 6765  C...r/...).N..ge
 00000ac0: 745f 7465 6d70 5f63 6f6e 7461 696e 6572  t_temp_container
-00000ad0: 5f63 7265 6465 6e74 6961 6c73 7230 0000  _credentialsr0..
-00000ae0: 0029 0372 1400 0000 7233 0000 0072 3600  .).r....r3...r6.
+00000ad0: 5f63 7265 6465 6e74 6961 6c73 7231 0000  _credentialsr1..
+00000ae0: 0029 0372 1400 0000 7234 0000 0072 3700  .).r....r4...r7.
 00000af0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000b00: 0072 3800 0000 4800 0000 7302 0000 0008  .r8...H...s.....
+00000b00: 0072 3900 0000 4800 0000 7302 0000 0008  .r9...H...s.....
 00000b10: 067a 2d41 6374 696f 6e44 656c 6567 6174  .z-ActionDelegat
 00000b20: 652e 6765 745f 7465 6d70 5f63 6f6e 7461  e.get_temp_conta
 00000b30: 696e 6572 5f63 7265 6465 6e74 6961 6c73  iner_credentials
 00000b40: da07 6669 6c74 6572 73da 0a70 6167 655f  ..filters..page_
 00000b50: 746f 6b65 6e63 0400 0000 0000 0000 0000  tokenc..........
-00000b60: 0000 0400 0000 0200 0000 4300 0000 722e  ..........C...r.
+00000b60: 0000 0400 0000 0200 0000 4300 0000 722f  ..........C...r/
 00000b70: 0000 0029 024e da0d 7175 6572 795f 6163  ...).N..query_ac
-00000b80: 7469 6f6e 7372 3000 0000 2904 7214 0000  tionsr0...).r...
-00000b90: 0072 3900 0000 7229 0000 0072 3a00 0000  .r9...r)...r:...
+00000b80: 7469 6f6e 7372 3100 0000 2904 7214 0000  tionsr1...).r...
+00000b90: 0072 3a00 0000 722a 0000 0072 3b00 0000  .r:...r*...r;...
 00000ba0: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000bb0: 3b00 0000 5000 0000 7302 0000 0008 077a  ;...P...s......z
+00000bb0: 3c00 0000 5000 0000 7302 0000 0008 077a  <...P...s......z
 00000bc0: 1c41 6374 696f 6e44 656c 6567 6174 652e  .ActionDelegate.
 00000bd0: 7175 6572 795f 6163 7469 6f6e 73da 0775  query_actions..u
 00000be0: 7064 6174 6573 da0a 636f 6e64 6974 696f  pdates..conditio
 00000bf0: 6e73 da0a 7570 6461 7465 645f 6279 6306  ns..updated_byc.
 00000c00: 0000 0000 0000 0000 0000 0006 0000 0002  ................
-00000c10: 0000 0043 0000 0072 2e00 0000 2902 4eda  ...C...r....).N.
-00000c20: 0675 7064 6174 6572 3000 0000 2906 7214  .updater0...).r.
-00000c30: 0000 0072 3300 0000 723c 0000 0072 3d00  ...r3...r<...r=.
-00000c40: 0000 7229 0000 0072 3e00 0000 7215 0000  ..r)...r>...r...
-00000c50: 0072 1500 0000 7216 0000 0072 3f00 0000  .r....r....r?...
+00000c10: 0000 0043 0000 0072 2f00 0000 2902 4eda  ...C...r/...).N.
+00000c20: 0675 7064 6174 6572 3100 0000 2906 7214  .updater1...).r.
+00000c30: 0000 0072 3400 0000 723d 0000 0072 3e00  ...r4...r=...r>.
+00000c40: 0000 722a 0000 0072 3f00 0000 7215 0000  ..r*...r?...r...
+00000c50: 0072 1500 0000 7216 0000 0072 4000 0000  .r....r....r@...
 00000c60: 5900 0000 7302 0000 0008 097a 1541 6374  Y...s......z.Act
 00000c70: 696f 6e44 656c 6567 6174 652e 7570 6461  ionDelegate.upda
 00000c80: 7465 2905 4e4e 4e4e 4e72 1200 0000 2902  te).NNNNNr....).
 00000c90: 4e4e 2915 7219 0000 0072 1a00 0000 721b  NN).r....r....r.
 00000ca0: 0000 00da 0361 6263 da0e 6162 7374 7261  .....abc..abstra
 00000cb0: 6374 6d65 7468 6f64 721c 0000 0072 0400  ctmethodr....r..
 00000cc0: 0000 7220 0000 0072 0200 0000 da04 6c69  ..r ...r......li
-00000cd0: 7374 720b 0000 0072 2f00 0000 7232 0000  str....r/...r2..
-00000ce0: 00da 0574 7570 6c65 7237 0000 0072 0c00  ...tupler7...r..
-00000cf0: 0000 7238 0000 0072 0600 0000 723b 0000  ..r8...r....r;..
-00000d00: 0072 2100 0000 723f 0000 0072 1500 0000  .r!...r?...r....
+00000cd0: 7374 720b 0000 0072 3000 0000 7233 0000  str....r0...r3..
+00000ce0: 00da 0574 7570 6c65 7238 0000 0072 0c00  ...tupler8...r..
+00000cf0: 0000 7239 0000 0072 0600 0000 723c 0000  ..r9...r....r<..
+00000d00: 0072 2100 0000 7240 0000 0072 1500 0000  .r!...r@...r....
 00000d10: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000d20: 2700 0000 2b00 0000 73a2 0000 0008 0004  '...+...s.......
+00000d20: 2800 0000 2b00 0000 73a2 0000 0008 0004  (...+...s.......
 00000d30: 0102 0402 0102 0102 0102 0104 f902 0202  ................
 00000d40: fe06 0302 fd06 0402 fc06 0502 fb0e 0602  ................
 00000d50: fa0a 0702 f902 080c f804 0b02 0204 ff02  ................
 00000d60: 0102 ff06 0102 ff02 020c fe04 0502 0604  ................
 00000d70: fb02 0202 fe02 0302 fd02 0402 fc06 0502  ................
 00000d80: fb0a 060c fa04 0902 0404 fd02 0202 fe06  ................
 00000d90: 0302 fd02 040c fc04 0702 0402 0104 fc0a  ................
 00000da0: 0202 fe06 0302 fd0e 0402 fc06 050c fb04  ................
 00000db0: 0802 0602 0104 fa02 0202 fe0a 0302 fd0a  ................
 00000dc0: 0402 fc06 0502 fb06 0602 fa02 0710 f972  ...............r
-00000dd0: 2700 0000 2914 7240 0000 0072 1e00 0000  '...).r@...r....
+00000dd0: 2800 0000 2914 7241 0000 0072 1e00 0000  (...).rA...r....
 00000de0: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
 00000df0: 0000 7204 0000 00da 0870 7964 616e 7469  ..r......pydanti
-00000e00: 635a 0a70 6167 696e 6174 696f 6e72 0600  cZ.paginationr..
+00000e00: 63da 0a70 6167 696e 6174 696f 6e72 0600  c..paginationr..
 00000e10: 0000 da05 7365 7264 6572 0800 0000 da04  ....serder......
 00000e20: 7469 6d65 7209 0000 00da 0d61 6374 696f  timer......actio
 00000e30: 6e5f 7265 636f 7264 720b 0000 00da 0942  n_recordr......B
 00000e40: 6173 654d 6f64 656c 720c 0000 0072 2100  aseModelr....r!.
-00000e50: 0000 da03 4142 4372 2700 0000 7215 0000  ....ABCr'...r...
+00000e50: 0000 da03 4142 4372 2800 0000 7215 0000  ....ABCr(...r...
 00000e60: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
 00000e70: da08 3c6d 6f64 756c 653e 0100 0000 7316  ..<module>....s.
 00000e80: 0000 0008 0008 0114 0108 020c 020c 010c  ................
 00000e90: 010c 0112 0312 0d16 11                   .........
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 5168 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 3014 0000  o........F.d0...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 3014 0000  o.......Ms.d0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6403  d.l.m.Z.m.Z...d.
 00000050: 6404 6c00 6d05 5a05 6d06 5a06 6d07 5a07  d.l.m.Z.m.Z.m.Z.
 00000060: 6d08 5a08 0100 6403 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6403 6406 6c0b 6d0c 5a0c 0100 6403  ..d.d.l.m.Z...d.
@@ -78,16 +78,16 @@
 000004d0: 0000 0003 0000 0073 1a00 0000 7400 8300  .......s....t...
 000004e0: a001 a100 0100 7c02 7c00 5f02 7c01 7c00  ......|.|._.|.|.
 000004f0: 5f03 6400 5300 a901 4e29 04da 0573 7570  _.d.S...N)...sup
 00000500: 6572 da08 5f5f 696e 6974 5f5f 7215 0000  er..__init__r...
 00000510: 0072 1600 0000 2903 da04 7365 6c66 7217  .r....)...selfr.
 00000520: 0000 0072 1800 0000 a901 da09 5f5f 636c  ...r........__cl
 00000530: 6173 735f 5fa9 00fa fb2f 636f 6465 6275  ass__..../codebu
-00000540: 696c 642f 6f75 7470 7574 2f73 7263 3430  ild/output/src40
-00000550: 3938 3735 3631 3639 2f73 7263 2f63 6f64  98756169/src/cod
+00000540: 696c 642f 6f75 7470 7574 2f73 7263 3334  ild/output/src34
+00000550: 3937 3236 3836 3730 2f73 7263 2f63 6f64  97268670/src/cod
 00000560: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 00000570: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 00000580: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 00000590: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 000005a0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 000005b0: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 000005c0: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
@@ -125,22 +125,22 @@
 000007c0: 027c 00a0 057c 027c 03a1 0264 058d 037d  .|...|.|...d...}
 000007d0: 0974 06a0 077c 096a 0864 0667 0164 078d  .t...|.j.d.g.d..
 000007e0: 01a1 0153 0029 084e 7a0b 2f76 312f 6163  ...S.).Nz./v1/ac
 000007f0: 7469 6f6e 7329 0472 2500 0000 7227 0000  tions).r%...r'..
 00000800: 0072 2800 0000 7229 0000 0054 2901 da0c  .r(...r)...T)...
 00000810: 6578 636c 7564 655f 6e6f 6e65 a902 da04  exclude_none....
 00000820: 6461 7461 7224 0000 0072 2c00 0000 a901  datar$...r,.....
-00000830: 5a09 6a73 6f6e 5f70 6174 6829 0972 1600  Z.json_path).r..
+00000830: da09 6a73 6f6e 5f70 6174 6829 0972 1600  ..json_path).r..
 00000840: 0000 7210 0000 0072 1500 0000 da04 706f  ..r....r......po
 00000850: 7374 720b 0000 0072 2400 0000 7212 0000  str....r$...r...
 00000860: 00da 0970 6172 7365 5f6f 626a da09 6672  ...parse_obj..fr
 00000870: 6f6d 5f6a 736f 6e29 0a72 1d00 0000 7225  om_json).r....r%
 00000880: 0000 0072 2200 0000 7226 0000 0072 2700  ...r"...r&...r'.
 00000890: 0000 7228 0000 0072 2900 0000 da03 7572  ..r(...r).....ur
-000008a0: 6c5a 0c72 6571 7565 7374 5f62 6f64 79da  lZ.request_body.
+000008a0: 6cda 0c72 6571 7565 7374 5f62 6f64 79da  l..request_body.
 000008b0: 0872 6573 706f 6e73 6572 2000 0000 7220  .responser ...r 
 000008c0: 0000 0072 2100 0000 da0d 6372 6561 7465  ...r!.....create
 000008d0: 5f61 6374 696f 6e36 0000 0073 1a00 0000  _action6...s....
 000008e0: 0c09 0201 0201 0201 0201 0201 06fc 0606  ................
 000008f0: 0201 0a01 0a01 06fd 1405 7a20 4163 7469  ..........z Acti
 00000900: 6f6e 4874 7470 4465 6c65 6761 7465 2e63  onHttpDelegate.c
 00000910: 7265 6174 655f 6163 7469 6f6e 6303 0000  reate_actionc...
@@ -149,16 +149,16 @@
 00000940: 6401 7c01 9b00 9d03 7d03 7c00 6a01 6a02  d.|.....}.|.j.j.
 00000950: 7c03 7c00 a003 7c02 a101 6402 8d02 7d04  |.|...|...d...}.
 00000960: 7404 a005 7c04 6a06 6403 6701 6404 8d01  t...|.j.d.g.d...
 00000970: a101 5300 2905 4efa 0c2f 7631 2f61 6374  ..S.).N../v1/act
 00000980: 696f 6e73 2fa9 0172 2400 0000 722c 0000  ions/..r$...r,..
 00000990: 0072 2d00 0000 2907 7216 0000 0072 1500  .r-...).r....r..
 000009a0: 0000 da03 6765 7472 2400 0000 7212 0000  ....getr$...r...
-000009b0: 0072 2f00 0000 7230 0000 0029 0572 1d00  .r/...r0...).r..
-000009c0: 0000 7225 0000 0072 2200 0000 7231 0000  ..r%...r"...r1..
+000009b0: 0072 3000 0000 7231 0000 0029 0572 1d00  .r0...r1...).r..
+000009c0: 0000 7225 0000 0072 2200 0000 7232 0000  ..r%...r"...r2..
 000009d0: 00da 0372 6573 7220 0000 0072 2000 0000  ...resr ...r ...
 000009e0: 7221 0000 00da 1967 6574 5f61 6374 696f  r!.....get_actio
 000009f0: 6e5f 6279 5f70 7269 6d61 7279 5f6b 6579  n_by_primary_key
 00000a00: 4d00 0000 7306 0000 0010 0316 0114 017a  M...s..........z
 00000a10: 2c41 6374 696f 6e48 7474 7044 656c 6567  ,ActionHttpDeleg
 00000a20: 6174 652e 6765 745f 6163 7469 6f6e 5f62  ate.get_action_b
 00000a30: 795f 7072 696d 6172 795f 6b65 79da 0672  y_primary_key..r
@@ -167,45 +167,45 @@
 00000a60: 6c6c 6572 6305 0000 0000 0000 0000 0000  llerc...........
 00000a70: 0009 0000 0006 0000 0043 0000 0073 5600  .........C...sV.
 00000a80: 0000 7c00 6a00 9b00 6401 7c01 6a01 9b00  ..|.j...d.|.j...
 00000a90: 6402 9d04 7d05 7c02 7c03 6403 9c02 7d06  d...}.|.|.d...}.
 00000aa0: 7c00 6a02 6a03 7c05 7c06 7c00 6a04 7c04  |.j.j.|.|.|.j.|.
 00000ab0: 6404 8d01 6405 8d03 7d07 7c07 6a05 6406  d...d...}.|.j.d.
 00000ac0: 6701 6407 8d01 7d08 7c08 6408 1900 7c08  g.d...}.|.d...|.
-00000ad0: 6409 1900 6602 5300 290a 4e72 3400 0000  d...f.S.).Nr4...
-00000ae0: 7a0a 2f63 6f6e 7461 696e 6572 2902 723a  z./container).r:
-00000af0: 0000 0072 3b00 0000 a901 7223 0000 0072  ...r;.....r#...r
+00000ad0: 6409 1900 6602 5300 290a 4e72 3600 0000  d...f.S.).Nr6...
+00000ae0: 7a0a 2f63 6f6e 7461 696e 6572 2902 723c  z./container).r<
+00000af0: 0000 0072 3d00 0000 a901 7223 0000 0072  ...r=.....r#...r
 00000b00: 2b00 0000 722c 0000 0072 2d00 0000 5a0e  +...r,...r-...Z.
 00000b10: 7265 706f 7369 746f 7279 5f75 7269 5a09  repository_uriZ.
 00000b20: 696d 6167 655f 7572 6929 0672 1600 0000  image_uri).r....
 00000b30: 7225 0000 0072 1500 0000 da03 7075 7472  r%...r......putr
-00000b40: 2400 0000 7230 0000 0029 0972 1d00 0000  $...r0...).r....
-00000b50: 7239 0000 0072 3a00 0000 723b 0000 0072  r9...r:...r;...r
-00000b60: 3c00 0000 7231 0000 0072 2c00 0000 7237  <...r1...r,...r7
+00000b40: 2400 0000 7231 0000 0029 0972 1d00 0000  $...r1...).r....
+00000b50: 723b 0000 0072 3c00 0000 723d 0000 0072  r;...r<...r=...r
+00000b60: 3e00 0000 7232 0000 0072 2c00 0000 7239  >...r2...r,...r9
 00000b70: 0000 005a 0a70 6172 7365 645f 7265 7372  ...Z.parsed_resr
 00000b80: 2000 0000 7220 0000 0072 2100 0000 da12   ...r ...r!.....
 00000b90: 7265 6769 7374 6572 5f63 6f6e 7461 696e  register_contain
 00000ba0: 6572 5400 0000 7312 0000 0014 0702 0202  erT...s.........
 00000bb0: 0106 fe06 050e 0106 ff0e 0310 017a 2541  .............z%A
 00000bc0: 6374 696f 6e48 7474 7044 656c 6567 6174  ctionHttpDelegat
 00000bd0: 652e 7265 6769 7374 6572 5f63 6f6e 7461  e.register_conta
 00000be0: 696e 6572 6303 0000 0000 0000 0000 0000  inerc...........
 00000bf0: 0005 0000 0005 0000 0043 0000 0073 4000  .........C...s@.
 00000c00: 0000 7c00 6a00 9b00 6401 7c01 6a01 9b00  ..|.j...d.|.j...
 00000c10: 6402 9d04 7d03 7c00 6a02 6a03 7c03 7c00  d...}.|.j.j.|.|.
 00000c20: 6a04 7c02 6403 8d01 6404 8d02 7d04 7405  j.|.d...d...}.t.
 00000c30: a006 7c04 6a07 6405 6701 6406 8d01 a101  ..|.j.d.g.d.....
-00000c40: 5300 2907 4e72 3400 0000 7a16 2f63 6f6e  S.).Nr4...z./con
+00000c40: 5300 2907 4e72 3600 0000 7a16 2f63 6f6e  S.).Nr6...z./con
 00000c50: 7461 696e 6572 2f63 7265 6465 6e74 6961  tainer/credentia
-00000c60: 6c73 723d 0000 0072 3500 0000 722c 0000  lsr=...r5...r,..
+00000c60: 6c73 723f 0000 0072 3700 0000 722c 0000  lsr?...r7...r,..
 00000c70: 0072 2d00 0000 2908 7216 0000 0072 2500  .r-...).r....r%.
-00000c80: 0000 7215 0000 0072 3600 0000 7224 0000  ..r....r6...r$..
-00000c90: 0072 0e00 0000 722f 0000 0072 3000 0000  .r....r/...r0...
-00000ca0: 2905 721d 0000 0072 3900 0000 723c 0000  ).r....r9...r<..
-00000cb0: 0072 3100 0000 7237 0000 0072 2000 0000  .r1...r7...r ...
+00000c80: 0000 7215 0000 0072 3800 0000 7224 0000  ..r....r8...r$..
+00000c90: 0072 0e00 0000 7230 0000 0072 3100 0000  .r....r0...r1...
+00000ca0: 2905 721d 0000 0072 3b00 0000 723e 0000  ).r....r;...r>..
+00000cb0: 0072 3200 0000 7239 0000 0072 2000 0000  .r2...r9...r ...
 00000cc0: 7220 0000 0072 2100 0000 da1e 6765 745f  r ...r!.....get_
 00000cd0: 7465 6d70 5f63 6f6e 7461 696e 6572 5f63  temp_container_c
 00000ce0: 7265 6465 6e74 6961 6c73 6700 0000 7306  redentialsg...s.
 00000cf0: 0000 0014 0518 0114 017a 3141 6374 696f  .........z1Actio
 00000d00: 6e48 7474 7044 656c 6567 6174 652e 6765  nHttpDelegate.ge
 00000d10: 745f 7465 6d70 5f63 6f6e 7461 696e 6572  t_temp_container
 00000d20: 5f63 7265 6465 6e74 6961 6c73 da07 6669  _credentials..fi
@@ -214,37 +214,37 @@
 00000d50: 0000 0600 0000 4300 0000 736c 0000 007c  ......C...sl...|
 00000d60: 0372 067c 037c 0164 013c 0074 00a0 0174  .r.|.|.d.<.t...t
 00000d70: 00a0 027c 01a1 01a1 017d 047c 006a 039b  ...|.....}.|.j..
 00000d80: 0064 029d 027d 057c 006a 046a 057c 057c  .d...}.|.j.j.|.|
 00000d90: 047c 00a0 067c 02a1 0164 038d 037d 067c  .|...|...d...}.|
 00000da0: 066a 0764 0467 0164 058d 017d 0774 0864  .j.d.g.d...}.t.d
 00000db0: 0664 0784 007c 0764 0819 0044 0083 017c  .d...|.d...D...|
-00000dc0: 0764 0919 0064 0a8d 0253 0029 0b4e 7242  .d...d...S.).NrB
+00000dc0: 0764 0919 0064 0a8d 0253 0029 0b4e 7244  .d...d...S.).NrD
 00000dd0: 0000 007a 112f 7631 2f61 6374 696f 6e73  ...z./v1/actions
 00000de0: 2f71 7565 7279 722b 0000 0072 2c00 0000  /queryr+...r,...
 00000df0: 722d 0000 0063 0100 0000 0000 0000 0000  r-...c..........
 00000e00: 0000 0200 0000 0500 0000 5300 0000 7316  ..........S...s.
 00000e10: 0000 0067 007c 005d 077d 0174 00a0 017c  ...g.|.].}.t...|
 00000e20: 01a1 0191 0271 0253 0072 2000 0000 2902  .....q.S.r ...).
-00000e30: 7212 0000 0072 2f00 0000 2902 da02 2e30  r....r/...)....0
+00000e30: 7212 0000 0072 3000 0000 2902 da02 2e30  r....r0...)....0
 00000e40: 5a07 6461 7461 7365 7472 2000 0000 7220  Z.datasetr ...r 
 00000e50: 0000 0072 2100 0000 da0a 3c6c 6973 7463  ...r!.....<listc
 00000e60: 6f6d 703e 8000 0000 7306 0000 0006 000a  omp>....s.......
 00000e70: 0106 ff7a 3441 6374 696f 6e48 7474 7044  ...z4ActionHttpD
 00000e80: 656c 6567 6174 652e 7175 6572 795f 6163  elegate.query_ac
 00000e90: 7469 6f6e 732e 3c6c 6f63 616c 733e 2e3c  tions.<locals>.<
 00000ea0: 6c69 7374 636f 6d70 3eda 0569 7465 6d73  listcomp>..items
-00000eb0: da0a 6e65 7874 5f74 6f6b 656e 2902 7245  ..next_token).rE
-00000ec0: 0000 0072 4600 0000 2909 da04 6a73 6f6e  ...rF...)...json
+00000eb0: da0a 6e65 7874 5f74 6f6b 656e 2902 7247  ..next_token).rG
+00000ec0: 0000 0072 4800 0000 2909 da04 6a73 6f6e  ...rH...)...json
 00000ed0: da05 6c6f 6164 73da 0564 756d 7073 7216  ..loads..dumpsr.
-00000ee0: 0000 0072 1500 0000 722e 0000 0072 2400  ...r....r....r$.
-00000ef0: 0000 7230 0000 0072 0a00 0000 2908 721d  ..r0...r....).r.
-00000f00: 0000 0072 4100 0000 7222 0000 0072 4200  ...rA...r"...rB.
+00000ee0: 0000 0072 1500 0000 722f 0000 0072 2400  ...r....r/...r$.
+00000ef0: 0000 7231 0000 0072 0a00 0000 2908 721d  ..r1...r....).r.
+00000f00: 0000 0072 4300 0000 7222 0000 0072 4400  ...rC...r"...rD.
 00000f10: 0000 5a0c 7361 6665 5f66 696c 7465 7273  ..Z.safe_filters
-00000f20: 7231 0000 0072 3700 0000 5a0c 756e 6d61  r1...r7...Z.unma
+00000f20: 7232 0000 0072 3900 0000 5a0c 756e 6d61  r2...r9...Z.unma
 00000f30: 7273 6861 6c6c 6564 7220 0000 0072 2000  rshalledr ...r .
 00000f40: 0000 7221 0000 00da 0d71 7565 7279 5f61  ..r!.....query_a
 00000f50: 6374 696f 6e73 7000 0000 731c 0000 0004  ctionsp...s.....
 00000f60: 0608 0110 020c 0106 010c 0106 ff0e 0302  ................
 00000f70: 0106 0106 0104 ff06 0306 fc7a 2041 6374  ...........z Act
 00000f80: 696f 6e48 7474 7044 656c 6567 6174 652e  ionHttpDelegate.
 00000f90: 7175 6572 795f 6163 7469 6f6e 73da 0775  query_actions..u
@@ -257,58 +257,58 @@
 00001000: 6402 8d02 7d07 7a1a 7c00 6a03 6a04 7c06  d...}.z.|.j.j.|.
 00001010: 7c07 a005 a100 7c00 a006 7c04 7c05 a102  |.....|...|.|...
 00001020: 6403 8d03 7d08 7407 a008 7c08 6a09 6404  d...}.t...|.j.d.
 00001030: 6701 6405 8d01 a101 5700 5300 0400 740a  g.d.....W.S...t.
 00001040: 7949 0100 7d09 0100 7a0e 7c09 6a0b 740c  yI..}...z.|.j.t.
 00001050: 6a0d 6a0e 6b02 7244 740f 7c09 6a10 8301  j.j.k.rDt.|.j...
 00001060: 6400 8202 8200 6400 7d09 7e09 7701 7700  d.....d.}.~.w.w.
-00001070: 2906 4e72 3400 0000 2902 724b 0000 0072  ).Nr4...).rK...r
-00001080: 4c00 0000 722b 0000 0072 2c00 0000 722d  L...r+...r,...r-
+00001070: 2906 4e72 3600 0000 2902 724d 0000 0072  ).Nr6...).rM...r
+00001080: 4e00 0000 722b 0000 0072 2c00 0000 722d  N...r+...r,...r-
 00001090: 0000 0029 1172 1600 0000 7225 0000 0072  ...).r....r%...r
-000010a0: 1100 0000 7215 0000 005a 0570 6174 6368  ....r....Z.patch
+000010a0: 1100 0000 7215 0000 00da 0570 6174 6368  ....r......patch
 000010b0: da04 6469 6374 7224 0000 0072 1200 0000  ..dictr$...r....
-000010c0: 722f 0000 0072 3000 0000 7207 0000 00da  r/...r0...r.....
-000010d0: 0673 7461 7475 73da 0468 7474 705a 0a48  .status..httpZ.H
-000010e0: 5454 5053 7461 7475 735a 0843 4f4e 464c  TTPStatusZ.CONFL
+000010c0: 7230 0000 0072 3100 0000 7207 0000 00da  r0...r1...r.....
+000010d0: 0673 7461 7475 73da 0468 7474 70da 0a48  .status..http..H
+000010e0: 5454 5053 7461 7475 73da 0843 4f4e 464c  TTPStatus..CONFL
 000010f0: 4943 5472 1300 0000 da03 6d73 6729 0a72  ICTr......msg).r
-00001100: 1d00 0000 7239 0000 0072 4b00 0000 724c  ....r9...rK...rL
-00001110: 0000 0072 2200 0000 724d 0000 0072 3100  ...r"...rM...r1.
-00001120: 0000 da07 7061 796c 6f61 6472 3700 0000  ....payloadr7...
+00001100: 1d00 0000 723b 0000 0072 4d00 0000 724e  ....r;...rM...rN
+00001110: 0000 0072 2200 0000 724f 0000 0072 3200  ...r"...rO...r2.
+00001120: 0000 da07 7061 796c 6f61 6472 3900 0000  ....payloadr9...
 00001130: da03 6578 6372 2000 0000 7220 0000 0072  ..excr ...r ...r
 00001140: 2100 0000 da06 7570 6461 7465 8600 0000  !.....update....
 00001150: 7320 0000 0012 0802 0102 010e 0106 fe02  s ..............
 00001160: 0406 0112 0106 ff16 030e 010e 010c 0102  ................
 00001170: 0108 8002 fd7a 1941 6374 696f 6e48 7474  .....z.ActionHtt
 00001180: 7044 656c 6567 6174 652e 7570 6461 7465  pDelegate.update
 00001190: 2902 4e4e 2905 4e4e 4e4e 4e72 1a00 0000  ).NN).NNNNNr....
 000011a0: 2919 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000011b0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 000011c0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
 000011d0: 0800 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
 000011e0: 6f6e 735f 5fda 0373 7472 721c 0000 0072  ons__..strr....r
-000011f0: 0300 0000 724e 0000 0072 2400 0000 7202  ....rN...r$...r.
-00001200: 0000 00da 046c 6973 7472 1200 0000 7233  .....listr....r3
-00001210: 0000 0072 3800 0000 da05 7475 706c 6572  ...r8.....tupler
-00001220: 3f00 0000 720e 0000 0072 4000 0000 720a  ?...r....r@...r.
-00001230: 0000 0072 4a00 0000 720f 0000 0072 5400  ...rJ...r....rT.
+000011f0: 0300 0000 7251 0000 0072 2400 0000 7202  ....rQ...r$...r.
+00001200: 0000 00da 046c 6973 7472 1200 0000 7235  .....listr....r5
+00001210: 0000 0072 3a00 0000 da05 7475 706c 6572  ...r:.....tupler
+00001220: 4100 0000 720e 0000 0072 4200 0000 720a  A...r....rB...r.
+00001230: 0000 0072 4c00 0000 720f 0000 0072 5900  ...rL...r....rY.
 00001240: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
 00001250: 5f72 2000 0000 7220 0000 0072 1e00 0000  _r ...r ...r....
 00001260: 7221 0000 0072 1400 0000 1f00 0000 73ae  r!...r........s.
 00001270: 0000 000a 0004 0108 0408 011a 0202 0604  ................
 00001280: ff06 0102 ff06 0102 ff0a 020a fe02 0d02  ................
 00001290: 0102 0102 0102 0104 f902 0202 fe06 0302  ................
 000012a0: fd06 0402 fc06 0502 fb0e 0602 fa0a 0702  ................
 000012b0: f902 080a f802 1804 ff02 0102 ff06 0102  ................
 000012c0: ff02 020a fe02 0c04 fb02 0202 fe02 0302  ................
 000012d0: fd02 0402 fc06 0502 fb0a 060a fa02 1604  ................
 000012e0: fd02 0202 fe06 0302 fd02 040a fc02 0c02  ................
 000012f0: 0104 fc0a 0202 fe06 0302 fd0e 0402 fc06  ................
 00001300: 050a fb02 1b02 0104 fa02 0202 fe0a 0302  ................
 00001310: fd0a 0402 fc06 0502 fb06 0602 fa02 0712  ................
-00001320: f972 1400 0000 291c 7250 0000 0072 4700  .r....).rP...rG.
+00001320: f972 1400 0000 291c 7253 0000 0072 4900  .r....).rS...rI.
 00001330: 0000 da06 7479 7069 6e67 7202 0000 0072  ....typingr....r
 00001340: 0300 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
 00001350: 0000 0072 0800 0000 da07 6c6f 6767 696e  ...r......loggin
 00001360: 6772 0900 0000 da0a 7061 6769 6e61 7469  gr......paginati
 00001370: 6f6e 720a 0000 00da 0573 6572 6465 720b  onr......serder.
 00001380: 0000 00da 0f61 6374 696f 6e5f 6465 6c65  .....action_dele
 00001390: 6761 7465 720d 0000 0072 0e00 0000 720f  gater....r....r.
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 640 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 8002 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 8002 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6403 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 4700 6405 6406 8400 6406 6503 6a06  ..G.d.d...d.e.j.
 00000060: 8303 5a07 4700 6407 6408 8400 6408 6503  ..Z.G.d.d...d.e.
 00000070: 6a06 8303 5a08 4700 6409 640a 8400 640a  j...Z.G.d.d...d.
@@ -28,15 +28,15 @@
 000001b0: 5fda 0373 7472 da0f 5f5f 616e 6e6f 7461  _..str..__annota
 000001c0: 7469 6f6e 735f 5f72 0800 0000 7203 0000  tions__r....r...
 000001d0: 00da 0870 7964 616e 7469 63da 0546 6965  ...pydantic..Fie
 000001e0: 6c64 da04 6469 6374 720a 0000 0072 0200  ld..dictr....r..
 000001f0: 0000 da04 6c69 7374 720b 0000 00a9 0072  ....listr......r
 00000200: 1500 0000 7215 0000 00fa fc2f 636f 6465  ....r....../code
 00000210: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000220: 3430 3938 3735 3631 3639 2f73 7263 2f63  4098756169/src/c
+00000220: 3334 3937 3236 3836 3730 2f73 7263 2f63  3497268670/src/c
 00000230: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 00000240: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 00000250: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 00000260: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 00000270: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 00000280: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 00000290: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 808 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 2803 0000  o........F.d(...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 2803 0000  o.......Ms.d(...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 5a04 4700  m.Z...d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6504 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6401 5300 2905 e900 0000 004e 2902 da03  d.S.)......N)...
 00000070: 416e 79da 084f 7074 696f 6e61 6c63 0000  Any..Optionalc..
@@ -41,15 +41,15 @@
 00000280: 6461 7465 7469 6d65 da0f 5f5f 616e 6e6f  datetime..__anno
 00000290: 7461 7469 6f6e 735f 5fda 0373 7472 720b  tations__..strr.
 000002a0: 0000 0072 0300 0000 720c 0000 00da 0462  ...r....r......b
 000002b0: 6f6f 6c72 0d00 0000 da04 6469 6374 7202  oolr......dictr.
 000002c0: 0000 0072 0e00 0000 da04 6c69 7374 720f  ...r......listr.
 000002d0: 0000 00a9 0072 1a00 0000 721a 0000 00fa  .....r....r.....
 000002e0: f42f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000002f0: 7574 2f73 7263 3430 3938 3735 3631 3639  ut/src4098756169
+000002f0: 7574 2f73 7263 3334 3937 3236 3836 3730  ut/src3497268670
 00000300: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 00000310: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000320: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000330: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000340: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000350: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000360: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 106 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 6a00 0000  o........F.dj...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 6a00 0000  o.......Ms.dj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2400 0000 4700  .....@...s$...G.
 00000030: 6400 6401 8400 6401 6500 8303 5a01 4700  d.d...d.e...Z.G.
 00000040: 6402 6403 8400 6403 6500 8303 5a02 6404  d.d...d.e...Z.d.
 00000050: 5300 2905 6300 0000 0000 0000 0000 0000  S.).c...........
 00000060: 0000 0000 0001 0000 0040 0000 00f3 0c00  .........@......
 00000070: 0000 6500 5a01 6400 5a02 6401 5300 2902  ..e.Z.d.Z.d.S.).
 00000080: da21 4163 7469 6f6e 5570 6461 7465 436f  .!ActionUpdateCo
 00000090: 6e64 6974 696f 6e43 6865 636b 4661 696c  nditionCheckFail
 000000a0: 7572 654e a903 da08 5f5f 6e61 6d65 5f5f  ureN....__name__
 000000b0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 000000c0: 7175 616c 6e61 6d65 5f5f a900 7207 0000  qualname__..r...
 000000d0: 0072 0700 0000 faec 2f63 6f64 6562 7569  .r....../codebui
-000000e0: 6c64 2f6f 7574 7075 742f 7372 6334 3039  ld/output/src409
-000000f0: 3837 3536 3136 392f 7372 632f 636f 6465  8756169/src/code
+000000e0: 6c64 2f6f 7574 7075 742f 7372 6333 3439  ld/output/src349
+000000f0: 3732 3638 3637 302f 7372 632f 636f 6465  7268670/src/code
 00000100: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000110: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000120: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000130: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000140: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000150: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000160: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 4499 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 9311 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 9311 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6403 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c07 6d08 5a08 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6407 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 4700 6408 6409 8400 6409 8302 5a0d  ..G.d.d...d...Z.
@@ -52,15 +52,15 @@
 00000330: 0000 0400 0000 4300 0000 7316 0000 007c  ......C...s....|
 00000340: 02a0 007c 017c 03a1 027d 047c 007c 047c  ...|.|...}.|.|.|
 00000350: 0283 0253 00a9 014e 2901 5a09 6765 745f  ...S...N).Z.get_
 00000360: 6279 5f69 6429 05da 0363 6c73 720e 0000  by_id)...clsr...
 00000370: 0072 0f00 0000 7210 0000 00da 0672 6563  .r....r......rec
 00000380: 6f72 64a9 0072 1500 0000 faf1 2f63 6f64  ord..r....../cod
 00000390: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-000003a0: 6334 3039 3837 3536 3136 392f 7372 632f  c4098756169/src/
+000003a0: 6333 3439 3732 3638 3637 302f 7372 632f  c3497268670/src/
 000003b0: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 000003c0: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 000003d0: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 000003e0: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 000003f0: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000400: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 00000410: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 1726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 be06 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 be06 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
 00000070: 8400 6408 6500 6a0b 8303 5a0c 6401 5300  ..d.e.j...Z.d.S.
@@ -47,16 +47,16 @@
 000002e0: 6e76 6f63 6174 696f 6eda 1163 7265 6174  nvocation..creat
 000002f0: 655f 696e 766f 6361 7469 6f6e a901 da13  e_invocation....
 00000300: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
 00000310: 726f 7229 08da 0473 656c 6672 0c00 0000  ror)...selfr....
 00000320: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
 00000330: 1000 0000 7211 0000 0072 1200 0000 a900  ....r....r......
 00000340: 7219 0000 00fa fa2f 636f 6465 6275 696c  r....../codebuil
-00000350: 642f 6f75 7470 7574 2f73 7263 3430 3938  d/output/src4098
-00000360: 3735 3631 3639 2f73 7263 2f63 6f64 6573  756169/src/codes
+00000350: 642f 6f75 7470 7574 2f73 7263 3334 3937  d/output/src3497
+00000360: 3236 3836 3730 2f73 7263 2f63 6f64 6573  268670/src/codes
 00000370: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 00000380: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 00000390: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 000003a0: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 000003b0: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 000003c0: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 000003d0: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 4768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 a012 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 a012 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6403 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6403 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6403 6407 6c0c 6d0d 5a0d 0100 6408  ..d.d.l.m.Z...d.
@@ -71,15 +71,15 @@
 00000460: 0000 7400 8300 a001 a100 0100 7c02 7c00  ..t.........|.|.
 00000470: 5f02 7c01 7c00 5f03 6400 5300 a901 4e29  _.|.|._.d.S...N)
 00000480: 04da 0573 7570 6572 da08 5f5f 696e 6974  ...super..__init
 00000490: 5f5f 7214 0000 0072 1500 0000 2903 da04  __r....r....)...
 000004a0: 7365 6c66 7216 0000 0072 1700 0000 a901  selfr....r......
 000004b0: da09 5f5f 636c 6173 735f 5fa9 00fa ff2f  ..__class__..../
 000004c0: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-000004d0: 2f73 7263 3430 3938 3735 3631 3639 2f73  /src4098756169/s
+000004d0: 2f73 7263 3334 3937 3236 3836 3730 2f73  /src3497268670/s
 000004e0: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 000004f0: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000500: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000510: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000520: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000530: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000540: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 566 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 3602 0000  o........F.d6...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 3602 0000  o.......Ms.d6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6403 6404 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 6502 6a07 8303 5a08 4700 6407 6408 8400  e.j...Z.G.d.d...
 00000070: 6408 6502 6a07 8303 5a09 4700 6409 640a  d.e.j...Z.G.d.d.
@@ -28,16 +28,16 @@
 000001b0: 7572 6365 5f69 644e 2909 da08 5f5f 6e61  urce_idN)...__na
 000001c0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 000001d0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da04  ..__qualname__..
 000001e0: 6c69 7374 da03 7374 72da 0f5f 5f61 6e6e  list..str..__ann
 000001f0: 6f74 6174 696f 6e73 5f5f 7204 0000 0072  otations__r....r
 00000200: 0500 0000 7202 0000 00a9 0072 1300 0000  ....r......r....
 00000210: 7213 0000 00e1 0001 0000 2f63 6f64 6562  r........./codeb
-00000220: 7569 6c64 2f6f 7574 7075 742f 7372 6334  uild/output/src4
-00000230: 3039 3837 3536 3136 392f 7372 632f 636f  098756169/src/co
+00000220: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+00000230: 3439 3732 3638 3637 302f 7372 632f 636f  497268670/src/co
 00000240: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 00000250: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000260: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000270: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000280: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000290: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 000002a0: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 1652 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 7406 0000  o........F.dt...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 7406 0000  o.......Ms.dt...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6501 6a05  Z.G.d.d...d.e.j.
 00000060: 8303 5a06 4700 6405 6406 8400 6406 6504  ..Z.G.d.d...d.e.
 00000070: 6a07 8303 5a08 4700 6407 6408 8400 6408  j...Z.G.d.d...d.
@@ -22,15 +22,15 @@
 00000150: 7469 6f6e 2773 2049 6e70 7574 4269 6e64  tion's InputBind
 00000160: 696e 67da 0744 6174 6173 6574 4e29 05da  ing..DatasetN)..
 00000170: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
 00000180: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
 00000190: 655f 5fda 075f 5f64 6f63 5f5f 7205 0000  e__..__doc__r...
 000001a0: 00a9 0072 0a00 0000 720a 0000 00fa f82f  ...r....r....../
 000001b0: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-000001c0: 2f73 7263 3430 3938 3735 3631 3639 2f73  /src4098756169/s
+000001c0: 2f73 7263 3334 3937 3236 3836 3730 2f73  /src3497268670/s
 000001d0: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 000001e0: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 000001f0: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000200: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000210: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000220: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000230: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_http_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_http_resources.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/action_record.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/action_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_http_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_http_resources.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/actions/invocation_record.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/actions/invocation_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__init__.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 546 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 2202 0000  o........F.d"...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 2202 0000  o.......Ms.d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6406 5a0e 6407  m.Z.m.Z...d.Z.d.
@@ -24,15 +24,15 @@
 00000170: 0400 0000 7205 0000 005a 0d68 7474 705f  ....r....Z.http_
 00000180: 6465 6c65 6761 7465 7206 0000 005a 0e68  delegater....Z.h
 00000190: 7474 705f 7265 736f 7572 6365 7372 0700  ttp_resourcesr..
 000001a0: 0000 da06 7265 636f 7264 7208 0000 0072  ....recordr....r
 000001b0: 0900 0000 720a 0000 00da 075f 5f61 6c6c  ....r......__all
 000001c0: 5f5f a900 720e 0000 0072 0e00 0000 faf0  __..r....r......
 000001d0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000001e0: 742f 7372 6334 3039 3837 3536 3136 392f  t/src4098756169/
+000001e0: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
 000001f0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000200: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000210: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000220: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000230: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000240: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000250: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 9836 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 6c26 0000  o........F.dl&..
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 6c26 0000  o.......Ms.dl&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c06 5a06 6403 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6405 6406 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6407 6408 6c0e  m.Z.m.Z...d.d.l.
@@ -69,22 +69,22 @@
 00000440: 6174 6564 5f62 79da 086d 6574 6164 6174  ated_by..metadat
 00000450: 61da 0474 6167 73da 0e66 696c 6573 5f64  a..tags..files_d
 00000460: 656c 6567 6174 65da 0672 6574 7572 6e63  elegate..returnc
 00000470: 0900 0000 0000 0000 0000 0000 0a00 0000  ................
 00000480: 0800 0000 4300 0000 7320 0000 007c 01a0  ....C...s ...|..
 00000490: 007c 027c 067c 037c 077c 047c 05a1 067d  .|.|.|.|.|.|...}
 000004a0: 097c 007c 097c 017c 0883 0353 00a9 014e  .|.|.|.|...S...N
-000004b0: 2901 da0e 6372 6561 7465 5f64 6174 6173  )...create_datas
+000004b0: 2901 5a0e 6372 6561 7465 5f64 6174 6173  ).Z.create_datas
 000004c0: 6574 290a da03 636c 7372 1700 0000 7218  et)...clsr....r.
 000004d0: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
 000004e0: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-000004f0: 00da 0672 6563 6f72 64a9 0072 2400 0000  ...record..r$...
+000004f0: 00da 0672 6563 6f72 64a9 0072 2300 0000  ...record..r#...
 00000500: faef 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-00000510: 7075 742f 7372 6334 3039 3837 3536 3136  put/src409875616
-00000520: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+00000510: 7075 742f 7372 6333 3439 3732 3638 3637  put/src349726867
+00000520: 302f 7372 632f 636f 6465 7374 6172 2d63  0/src/codestar-c
 00000530: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 00000540: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 00000550: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 00000560: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 00000570: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 00000580: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000590: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
@@ -96,19 +96,19 @@
 000005f0: 79da 0663 7265 6174 651d 0000 0073 0800  y..create....s..
 00000600: 0000 040c 0c01 04ff 0c03 7a0e 4461 7461  ..........z.Data
 00000610: 7365 742e 6372 6561 7465 da0a 6461 7461  set.create..data
 00000620: 7365 745f 6964 6305 0000 0000 0000 0000  set_idc.........
 00000630: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
 00000640: 1800 0000 7c02 a000 7c01 7c03 a102 7d05  ....|...|.|...}.
 00000650: 7c00 7c05 7c02 7c04 8303 5300 7220 0000  |.|.|.|...S.r ..
-00000660: 0029 01da 1a67 6574 5f64 6174 6173 6574  .)...get_dataset
+00000660: 0029 015a 1a67 6574 5f64 6174 6173 6574  .).Z.get_dataset
 00000670: 5f62 795f 7072 696d 6172 795f 6b65 7929  _by_primary_key)
-00000680: 0672 2200 0000 7227 0000 0072 1700 0000  .r"...r'...r....
-00000690: 721a 0000 0072 1e00 0000 7223 0000 0072  r....r....r#...r
-000006a0: 2400 0000 7224 0000 0072 2500 0000 da07  $...r$...r%.....
+00000680: 0672 2100 0000 7226 0000 0072 1700 0000  .r!...r&...r....
+00000690: 721a 0000 0072 1e00 0000 7222 0000 0072  r....r....r"...r
+000006a0: 2300 0000 7223 0000 0072 2400 0000 da07  #...r#...r$.....
 000006b0: 6672 6f6d 5f69 642e 0000 0073 0400 0000  from_id....s....
 000006c0: 0c08 0c01 7a0f 4461 7461 7365 742e 6672  ....z.Dataset.fr
 000006d0: 6f6d 5f69 64da 0766 696c 7465 7273 2903  om_id..filters).
 000006e0: 7212 0000 004e 4e63 0500 0000 0000 0000  r....NNc........
 000006f0: 0000 0000 0c00 0000 0600 0000 6300 0000  ............c...
 00000700: 73a2 0000 0081 0074 0074 016a 02a0 03a1  s......t.t.j....
 00000710: 0083 017d 0574 007c 01a0 03a1 0083 017d  ...}.t.|.......}
@@ -127,37 +127,37 @@
 000007e0: 6e6f 776e 2061 7474 7269 6275 7465 206f  nown attribute o
 000007f0: 6620 4461 7461 7365 74da 0120 7a14 2e20  f Dataset.. z.. 
 00000800: 4b6e 6f77 6e20 6174 7472 6962 7574 6573  Known attributes
 00000810: 3a20 2901 721a 0000 0054 2902 721a 0000  : ).r....T).r...
 00000820: 00da 0a70 6167 655f 746f 6b65 6e29 09da  ...page_token)..
 00000830: 0373 6574 7211 0000 00da 0a5f 5f66 6965  .setr......__fie
 00000840: 6c64 735f 5fda 046b 6579 73da 036c 656e  lds__..keys..len
-00000850: da0a 5661 6c75 6545 7272 6f72 da0e 7175  ..ValueError..qu
+00000850: da0a 5661 6c75 6545 7272 6f72 5a0e 7175  ..ValueErrorZ.qu
 00000860: 6572 795f 6461 7461 7365 7473 da05 6974  ery_datasets..it
 00000870: 656d 73da 0a6e 6578 745f 746f 6b65 6e29  ems..next_token)
-00000880: 0c72 2200 0000 722a 0000 0072 1700 0000  .r"...r*...r....
+00000880: 0c72 2100 0000 7228 0000 0072 1700 0000  .r!...r(...r....
 00000890: 721e 0000 0072 1a00 0000 da0a 6b6e 6f77  r....r......know
 000008a0: 6e5f 6b65 7973 da0b 6163 7475 616c 5f6b  n_keys..actual_k
 000008b0: 6579 73da 0c75 6e6b 6e6f 776e 5f6b 6579  eys..unknown_key
 000008c0: 73da 0670 6c75 7261 6cda 036d 7367 da11  s..plural..msg..
 000008d0: 7061 6769 6e61 7465 645f 7265 7375 6c74  paginated_result
-000008e0: 7372 2300 0000 7224 0000 0072 2400 0000  sr#...r$...r$...
-000008f0: 7225 0000 00da 0571 7565 7279 3900 0000  r%.....query9...
+000008e0: 7372 2200 0000 7223 0000 0072 2300 0000  sr"...r#...r#...
+000008f0: 7224 0000 00da 0571 7565 7279 3900 0000  r$.....query9...
 00000900: 732a 0000 0002 800e 080c 0108 0104 010c  s*..............
 00000910: 0102 0306 ff02 0202 fd18 050e 0202 010a  ................
 00000920: 0110 0106 0104 0108 0108 ff04 0402 f87a  ...............z
-00000930: 0d44 6174 6173 6574 2e71 7565 7279 7223  .Dataset.queryr#
+00000930: 0d44 6174 6173 6574 2e71 7565 7279 7222  .Dataset.queryr"
 00000940: 0000 00da 0864 656c 6567 6174 6563 0400  .....delegatec..
 00000950: 0000 0000 0000 0000 0000 0400 0000 0200  ................
 00000960: 0000 4300 0000 7316 0000 007c 027c 005f  ..C...s....|.|._
 00000970: 007c 037c 005f 017c 017c 005f 0264 0053  .|.|._.|.|._.d.S
 00000980: 0072 2000 0000 2903 7213 0000 0072 1500  .r ...).r....r..
 00000990: 0000 7214 0000 0029 04da 0473 656c 6672  ..r....)...selfr
-000009a0: 2300 0000 723c 0000 0072 1e00 0000 7224  #...r<...r....r$
-000009b0: 0000 0072 2400 0000 7225 0000 00da 085f  ...r$...r%....._
+000009a0: 2200 0000 7239 0000 0072 1e00 0000 7223  "...r9...r....r#
+000009b0: 0000 0072 2300 0000 7224 0000 00da 085f  ...r#...r$....._
 000009c0: 5f69 6e69 745f 5f58 0000 0073 0600 0000  _init__X...s....
 000009d0: 0606 0601 0a01 7a10 4461 7461 7365 742e  ......z.Dataset.
 000009e0: 5f5f 696e 6974 5f5f da08 6f75 745f 7061  __init__..out_pa
 000009f0: 7468 da10 696e 636c 7564 655f 7061 7474  th..include_patt
 00000a00: 6572 6e73 da10 6578 636c 7564 655f 7061  erns..exclude_pa
 00000a10: 7474 6572 6e73 6304 0000 0000 0000 0000  tternsc.........
 00000a20: 0000 000a 0000 0005 0000 0043 0000 0073  ...........C...s
@@ -232,64 +232,64 @@
 00000e70: da19 6765 745f 7465 6d70 6f72 6172 795f  ..get_temporary_
 00000e80: 6372 6564 656e 7469 616c 7372 0c00 0000  credentialsr....
 00000e90: da08 5265 6164 4f6e 6c79 7215 0000 0072  ..ReadOnlyr....r
 00000ea0: 0900 0000 da06 6275 636b 6574 da0a 6c69  ......bucket..li
 00000eb0: 7374 5f66 696c 6573 da0a 6d61 7463 685f  st_files..match_
 00000ec0: 6669 6c65 da0d 7265 6c61 7469 7665 5f70  file..relative_p
 00000ed0: 6174 68da 0d64 6f77 6e6c 6f61 645f 6669  ath..download_fi
-00000ee0: 6c65 da03 6b65 7929 0a72 3d00 0000 723f  le..key).r=...r?
-00000ef0: 0000 0072 4000 0000 7241 0000 005a 1469  ...r@...rA...Z.i
+00000ee0: 6c65 da03 6b65 7929 0a72 3a00 0000 723c  le..key).r:...r<
+00000ef0: 0000 0072 3d00 0000 723e 0000 005a 1469  ...r=...r>...Z.i
 00000f00: 6e63 6c75 6465 5f70 6174 7465 726e 5f73  nclude_pattern_s
 00000f10: 7065 635a 1465 7863 6c75 6465 5f70 6174  pecZ.exclude_pat
-00000f20: 7465 726e 5f73 7065 6372 4600 0000 721e  tern_specrF...r.
+00000f20: 7465 726e 5f73 7065 6372 4300 0000 721e  tern_specrC...r.
 00000f30: 0000 00da 0466 696c 655a 0a6c 6f63 616c  .....fileZ.local
-00000f40: 5f70 6174 6872 2400 0000 7224 0000 0072  _pathr$...r$...r
-00000f50: 2500 0000 da0e 646f 776e 6c6f 6164 5f66  %.....download_f
+00000f40: 5f70 6174 6872 2300 0000 7223 0000 0072  _pathr#...r#...r
+00000f50: 2400 0000 da0e 646f 776e 6c6f 6164 5f66  $.....download_f
 00000f60: 696c 6573 6200 0000 734a 0000 000e 180e  ilesb...sJ......
 00000f70: 0102 0202 0104 ff04 0408 0106 0108 0104  ................
 00000f80: ff04 0408 010c 0108 020c 010c 020a 0306  ................
 00000f90: ff02 0204 0102 0104 fe02 fd0c 0808 0104  ................
 00000fa0: 0104 ff02 0302 0108 0104 0104 ff02 0302  ................
 00000fb0: 010a 0210 0104 f37a 1644 6174 6173 6574  .......z.Dataset
 00000fc0: 2e64 6f77 6e6c 6f61 645f 6669 6c65 73da  .download_files.
 00000fd0: 046d 6f64 65da 0663 616c 6c65 7263 0300  .mode..callerc..
 00000fe0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
 00000ff0: 0000 4300 0000 732e 0000 007c 006a 0064  ..C...s....|.j.d
 00001000: 0075 0073 0a7c 006a 00a0 01a1 0072 147c  .u.s.|.j.....r.|
 00001010: 006a 02a0 037c 006a 047c 017c 02a1 037c  .j...|.j.|.|...|
 00001020: 005f 007c 006a 0053 0072 2000 0000 2905  ._.|.j.S.r ...).
 00001030: 7216 0000 00da 0a69 735f 6578 7069 7265  r......is_expire
-00001040: 6472 1300 0000 7250 0000 0072 1400 0000  dr....rP...r....
-00001050: 2903 723d 0000 0072 5a00 0000 725b 0000  ).r=...rZ...r[..
-00001060: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
-00001070: 7250 0000 00a6 0000 0073 0a00 0000 1405  rP.......s......
+00001040: 6472 1300 0000 724d 0000 0072 1400 0000  dr....rM...r....
+00001050: 2903 723a 0000 0072 5700 0000 7258 0000  ).r:...rW...rX..
+00001060: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00001070: 724d 0000 00a6 0000 0073 0a00 0000 1405  rM.......s......
 00001080: 0601 0801 06ff 0603 7a21 4461 7461 7365  ........z!Datase
 00001090: 742e 6765 745f 7465 6d70 6f72 6172 795f  t.get_temporary_
 000010a0: 6372 6564 656e 7469 616c 7363 0100 0000  credentialsc....
 000010b0: 0000 0000 0000 0000 0300 0000 0500 0000  ................
 000010c0: 6300 0000 7358 0000 0081 007c 006a 00a0  c...sX.....|.j..
 000010d0: 017c 006a 026a 037c 006a 026a 04a1 027d  .|.j.j.|.j.j...}
 000010e0: 0109 007c 016a 0544 005d 077d 0274 067c  ...|.j.D.].}.t.|
 000010f0: 0283 0156 0001 0071 107c 016a 0772 297c  ...V...q.|.j.r)|
 00001100: 006a 00a0 017c 006a 026a 037c 006a 026a  .j...|.j.j.|.j.j
 00001110: 047c 016a 07a1 037d 016e 0264 0053 0071  .|.j...}.n.d.S.q
-00001120: 0d72 2000 0000 2908 7213 0000 0072 5300  .r ...).r....rS.
-00001130: 0000 7214 0000 0072 2700 0000 721a 0000  ..r....r'...r...
-00001140: 0072 3300 0000 7207 0000 0072 3400 0000  .r3...r....r4...
-00001150: 2903 723d 0000 0072 3a00 0000 7223 0000  ).r=...r:...r#..
-00001160: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
-00001170: 7253 0000 00b1 0000 0073 1e00 0000 0280  rS.......s......
+00001120: 0d72 2000 0000 2908 7213 0000 0072 5000  .r ...).r....rP.
+00001130: 0000 7214 0000 0072 2600 0000 721a 0000  ..r....r&...r...
+00001140: 0072 3000 0000 7207 0000 0072 3100 0000  .r0...r....r1...
+00001150: 2903 723a 0000 0072 3700 0000 7222 0000  ).r:...r7...r"..
+00001160: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00001170: 7250 0000 00b1 0000 0073 1e00 0000 0280  rP.......s......
 00001180: 0601 0c01 04ff 0203 0a01 0c01 0601 0601  ................
 00001190: 0601 0601 0401 06fd 0406 02f6 7a12 4461  ............z.Da
 000011a0: 7461 7365 742e 6c69 7374 5f66 696c 6573  taset.list_files
 000011b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
 000011c0: 0002 0000 0043 0000 0073 0a00 0000 7400  .....C...s....t.
 000011d0: 7c00 6a01 8301 5300 7220 0000 0029 0272  |.j...S.r ...).r
-000011e0: 0500 0000 7214 0000 0029 0172 3d00 0000  ....r....).r=...
-000011f0: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+000011e0: 0500 0000 7214 0000 0029 0172 3a00 0000  ....r....).r:...
+000011f0: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
 00001200: 0774 6f5f 6469 6374 c100 0000 7302 0000  .to_dict....s...
 00001210: 000a 017a 0f44 6174 6173 6574 2e74 6f5f  ...z.Dataset.to_
 00001220: 6469 6374 da0e 6469 7265 6374 6f72 795f  dict..directory_
 00001230: 7061 7468 6303 0000 0000 0000 0000 0000  pathc...........
 00001240: 0003 0000 0006 0000 0003 0000 0073 5c00  .............s\.
 00001250: 0000 7c01 a000 a100 730b 7401 7c01 9b00  ..|.....s.t.|...
 00001260: 6401 9d02 8301 8201 6402 8901 7c02 6402  d.......d...|.d.
@@ -328,47 +328,47 @@
 00001470: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
 00001480: 6465 5f6d 6f64 756c 6573 2f22 2c0a 2020  de_modules/",.  
 00001490: 2020 2020 2020 2020 2020 2020 2020 222a                "*
 000014a0: 2a2f 2a2e 6c6f 6722 2c0a 2020 2020 2020  */*.log",.      
 000014b0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
 000014c0: 2029 0a20 2020 2020 2020 2060 6060 0a20   ).        ```. 
 000014d0: 2020 2020 2020 207a 1320 6973 206e 6f74         z. is not
-000014e0: 2061 2064 6972 6563 746f 7279 4e72 5e00   a directoryNr^.
+000014e0: 2061 2064 6972 6563 746f 7279 4e72 5b00   a directoryNr[.
 000014f0: 0000 da0a 6b65 795f 7072 6566 6978 721f  ....key_prefixr.
 00001500: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
 00001510: 0300 0000 0700 0000 1300 0000 735e 0000  ............s^..
 00001520: 007c 00a0 00a1 0044 005d 287d 027c 02a0  .|.....D.](}.|..
 00001530: 01a1 0072 1688 007c 027c 019b 0064 017c  ...r...|.|...d.|
 00001540: 026a 029b 009d 0383 0201 0071 0488 0164  .j.........q...d
 00001550: 0075 0172 2088 01a0 037c 02a1 0172 2071  .u.r ....|...r q
 00001560: 0488 02a0 047c 027c 019b 0064 017c 026a  .....|.|...d.|.j
 00001570: 029b 009d 03a1 0201 0071 0464 0053 0029  .........q.d.S.)
 00001580: 024e fa01 2f29 05da 0769 7465 7264 6972  .N../)...iterdir
-00001590: 724e 0000 00da 046e 616d 6572 5400 0000  rN.....namerT...
+00001590: 724b 0000 00da 046e 616d 6572 5100 0000  rK.....namerQ...
 000015a0: da0b 7570 6c6f 6164 5f66 696c 6529 0372  ..upload_file).r
-000015b0: 5e00 0000 725f 0000 00da 0470 6174 68a9  ^...r_.....path.
+000015b0: 5b00 0000 725c 0000 00da 0470 6174 68a9  [...r\.....path.
 000015c0: 03da 115f 7570 6c6f 6164 5f64 6972 6563  ..._upload_direc
 000015d0: 746f 7279 5a0c 6578 636c 7564 655f 7370  toryZ.exclude_sp
-000015e0: 6563 723d 0000 0072 2400 0000 7225 0000  ecr=...r$...r%..
-000015f0: 0072 6600 0000 e500 0000 730e 0000 000c  .rf.......s.....
+000015e0: 6563 723a 0000 0072 2300 0000 7224 0000  ecr:...r#...r$..
+000015f0: 0072 6300 0000 e500 0000 730e 0000 000c  .rc.......s.....
 00001600: 0108 0118 0112 0202 011a 0104 fa7a 3344  .............z3D
 00001610: 6174 6173 6574 2e75 706c 6f61 645f 6469  ataset.upload_di
 00001620: 7265 6374 6f72 792e 3c6c 6f63 616c 733e  rectory.<locals>
 00001630: 2e5f 7570 6c6f 6164 5f64 6972 6563 746f  ._upload_directo
-00001640: 7279 da00 2908 724e 0000 0072 3100 0000  ry..).rN...r1...
-00001650: 724a 0000 0072 4d00 0000 724b 0000 00da  rJ...rM...rK....
+00001640: 7279 da00 2908 724b 0000 0072 2f00 0000  ry..).rK...r/...
+00001650: 7247 0000 0072 4a00 0000 7248 0000 00da  rG...rJ...rH....
 00001660: 0770 6174 686c 6962 da04 5061 7468 da03  .pathlib..Path..
-00001670: 7374 7229 0372 3d00 0000 725e 0000 0072  str).r=...r^...r
-00001680: 4100 0000 7224 0000 0072 6500 0000 7225  A...r$...re...r%
+00001670: 7374 7229 0372 3a00 0000 725b 0000 0072  str).r:...r[...r
+00001680: 3e00 0000 7223 0000 0072 6200 0000 7224  >...r#...rb...r$
 00001690: 0000 00da 1075 706c 6f61 645f 6469 7265  .....upload_dire
 000016a0: 6374 6f72 79c4 0000 0073 1200 0000 0818  ctory....s......
 000016b0: 0e01 0402 0801 0601 0201 04ff 2004 0e09  ............ ...
 000016c0: 7a18 4461 7461 7365 742e 7570 6c6f 6164  z.Dataset.upload
 000016d0: 5f64 6972 6563 746f 7279 da0f 6c6f 6361  _directory..loca
-000016e0: 6c5f 6669 6c65 5f70 6174 6872 5700 0000  l_file_pathrW...
+000016e0: 6c5f 6669 6c65 5f70 6174 6872 5400 0000  l_file_pathrT...
 000016f0: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
 00001700: 0009 0000 0043 0000 0073 aa00 0000 7c01  .....C...s....|.
 00001710: a000 a100 730b 7401 7c01 9b00 6401 9d02  ....s.t.|...d...
 00001720: 8301 8201 7c00 6a02 6a03 7404 6a05 6b03  ....|.j.j.t.j.k.
 00001730: 7319 7c00 6a02 6a06 7407 6a08 6b03 721d  s.|.j.j.t.j.k.r.
 00001740: 7409 6402 8301 8201 7c00 a00a 740b 6a0c  t.d.....|...t.j.
 00001750: a101 7d03 7c00 6a0d 6403 7501 722b 7c00  ..}.|.j.d.u.r+|.
@@ -392,52 +392,52 @@
 00001870: 7365 7427 7320 7374 6f72 6167 6520 6c6f  set's storage lo
 00001880: 6361 7469 6f6e 2e0a 2020 2020 2020 2020  cation..        
 00001890: 2020 2020 2020 2020 2020 2020 4974 2077              It w
 000018a0: 696c 6c20 6265 2070 7265 6669 7865 6420  ill be prefixed 
 000018b0: 7769 7468 2074 6865 2064 6174 6173 6574  with the dataset
 000018c0: 2773 2073 746f 7261 6765 2070 7265 6669  's storage prefi
 000018d0: 782e 0a20 2020 2020 2020 207a 0e20 6973  x..        z. is
-000018e0: 206e 6f74 2061 2066 696c 6572 4200 0000   not a filerB...
-000018f0: 4e72 4400 0000 7260 0000 0029 0172 1d00  NrD...r`...).r..
-00001900: 0000 2919 da07 6973 5f66 696c 6572 3100  ..)...is_filer1.
+000018e0: 206e 6f74 2061 2066 696c 6572 3f00 0000   not a filer?...
+000018f0: 4e72 4100 0000 725d 0000 0029 0172 1d00  NrA...r]...).r..
+00001900: 0000 2919 da07 6973 5f66 696c 6572 2f00  ..)...is_filer/.
 00001910: 0000 7214 0000 0072 1900 0000 720f 0000  ..r....r....r...
-00001920: 0072 4700 0000 7218 0000 0072 1000 0000  .rG...r....r....
-00001930: 7248 0000 0072 4900 0000 7250 0000 0072  rH...rI...rP...r
+00001920: 0072 4400 0000 7218 0000 0072 1000 0000  .rD...r....r....
+00001930: 7245 0000 0072 4600 0000 724d 0000 0072  rE...rF...rM...r
 00001940: 0c00 0000 5a09 5265 6164 5772 6974 6572  ....Z.ReadWriter
-00001950: 1500 0000 7209 0000 0072 5200 0000 da0f  ....r....rR.....
+00001950: 1500 0000 7209 0000 0072 4f00 0000 5a0f  ....r....rO...Z.
 00001960: 7265 7175 6972 6564 5f70 7265 6669 78da  required_prefix.
-00001970: 066c 7374 7269 7072 6300 0000 720a 0000  .lstriprc...r...
-00001980: 005a 0944 6174 6173 6574 4964 7227 0000  .Z.DatasetIdr'..
+00001970: 066c 7374 7269 7072 6000 0000 720a 0000  .lstripr`...r...
+00001980: 005a 0944 6174 6173 6574 4964 7226 0000  .Z.DatasetIdr&..
 00001990: 005a 054f 7267 4964 721a 0000 005a 0c43  .Z.OrgIdr....Z.C
-000019a0: 6f6d 6d6f 6e50 7265 6669 7829 0572 3d00  ommonPrefix).r=.
-000019b0: 0000 726c 0000 0072 5700 0000 7246 0000  ..rl...rW...rF..
-000019c0: 0072 1e00 0000 7224 0000 0072 2400 0000  .r....r$...r$...
-000019d0: 7225 0000 0072 6300 0000 f000 0000 7330  r%...rc.......s0
+000019a0: 6f6d 6d6f 6e50 7265 6669 7829 0572 3a00  ommonPrefix).r:.
+000019b0: 0000 7269 0000 0072 5400 0000 7243 0000  ..ri...rT...rC..
+000019c0: 0072 1e00 0000 7223 0000 0072 2300 0000  .r....r#...r#...
+000019d0: 7224 0000 0072 6000 0000 f000 0000 7330  r$...r`.......s0
 000019e0: 0000 0008 0c0e 010e 030e 0102 0202 0104  ................
 000019f0: ff0c 040a 0306 ff02 0204 0102 0104 fe02  ................
 00001a00: fd16 0804 0102 0102 010a 020a 0108 0102  ................
 00001a10: fd0a fd7a 1344 6174 6173 6574 2e75 706c  ...z.Dataset.upl
 00001a20: 6f61 645f 6669 6c65 2902 4e4e 7220 0000  oad_file).NNr ..
 00001a30: 0029 26da 085f 5f6e 616d 655f 5fda 0a5f  .)&..__name__.._
 00001a40: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00001a50: 6c6e 616d 655f 5f72 0e00 0000 da0f 5f5f  lname__r......__
 00001a60: 616e 6e6f 7461 7469 6f6e 735f 5f72 1100  annotations__r..
 00001a70: 0000 7215 0000 0072 0300 0000 7208 0000  ..r....r....r...
 00001a80: 0072 1600 0000 720d 0000 00da 0b63 6c61  .r....r......cla
-00001a90: 7373 6d65 7468 6f64 7210 0000 0072 4800  ssmethodr....rH.
-00001aa0: 0000 720f 0000 0072 4700 0000 726a 0000  ..r....rG...rj..
+00001a90: 7373 6d65 7468 6f64 7210 0000 0072 4500  ssmethodr....rE.
+00001aa0: 0000 720f 0000 0072 4400 0000 7267 0000  ..r....rD...rg..
 00001ab0: 00da 0464 6963 7472 0200 0000 da04 6c69  ...dictr......li
-00001ac0: 7374 7226 0000 0072 2900 0000 da0b 636f  str&...r).....co
+00001ac0: 7374 7225 0000 0072 2700 0000 da0b 636f  str%...r'.....co
 00001ad0: 6c6c 6563 7469 6f6e 73da 0361 6263 da09  llections..abc..
-00001ae0: 4765 6e65 7261 746f 7272 3b00 0000 723e  Generatorr;...r>
-00001af0: 0000 0072 6800 0000 7269 0000 0072 5900  ...rh...ri...rY.
-00001b00: 0000 720c 0000 0072 5100 0000 7250 0000  ..r....rQ...rP..
-00001b10: 0072 0700 0000 7253 0000 0072 5d00 0000  .r....rS...r]...
-00001b20: 726b 0000 0072 6300 0000 7224 0000 0072  rk...rc...r$...r
-00001b30: 2400 0000 7224 0000 0072 2500 0000 7212  $...r$...r%...r.
+00001ae0: 4765 6e65 7261 746f 7272 3800 0000 723b  Generatorr8...r;
+00001af0: 0000 0072 6500 0000 7266 0000 0072 5600  ...re...rf...rV.
+00001b00: 0000 720c 0000 0072 4e00 0000 724d 0000  ..r....rN...rM..
+00001b10: 0072 0700 0000 7250 0000 0072 5a00 0000  .r....rP...rZ...
+00001b20: 7268 0000 0072 6000 0000 7223 0000 0072  rh...r`...r#...r
+00001b30: 2300 0000 7223 0000 0072 2400 0000 7212  #...r#...r$...r.
 00001b40: 0000 0017 0000 0073 d600 0000 0a00 0801  .......s........
 00001b50: 0801 1001 1001 0202 0404 0401 0201 0201  ................
 00001b60: 0201 0201 0201 04f7 0202 02fe 0203 02fd  ................
 00001b70: 0204 02fc 0605 02fb 0606 02fa 0e07 02f9  ................
 00001b80: 0a08 02f8 0609 02f7 020a 0cf6 0210 0205  ................
 00001b90: 0201 04fb 0202 02fe 0203 02fd 0604 02fc  ................
 00001ba0: 0605 02fb 0206 0cfa 020a 0205 0201 04fb  ................
@@ -445,19 +445,19 @@
 00001bc0: 0a06 0cfa 0222 04fc 0202 02fe 0203 02fd  ....."..........
 00001bd0: 0604 02fc 0205 0afb 020d 0201 04fc 0402  ................
 00001be0: 02fe 0a03 02fd 0a04 02fc 0205 0afb 0446  ...............F
 00001bf0: 0201 04fd 0202 02fe 0603 02fd 0204 0afc  ................
 00001c00: 1c0b 1610 0206 04fd 0402 02fe 0a03 02fd  ................
 00001c10: 0204 0afc 022c 0402 02fe 0203 02fd 0204  .....,..........
 00001c20: 0efc 7212 0000 0029 17da 0f63 6f6c 6c65  ..r....)...colle
-00001c30: 6374 696f 6e73 2e61 6263 7277 0000 0072  ctions.abcrw...r
-00001c40: 6800 0000 da06 7479 7069 6e67 7202 0000  h.....typingr...
-00001c50: 0072 0300 0000 724a 0000 00da 0573 6572  .r....rJ.....ser
+00001c30: 6374 696f 6e73 2e61 6263 7273 0000 0072  ctions.abcrs...r
+00001c40: 6500 0000 da06 7479 7069 6e67 7202 0000  e.....typingr...
+00001c50: 0072 0300 0000 7247 0000 00da 0573 6572  .r....rG.....ser
 00001c60: 6465 7205 0000 00da 0566 696c 6573 7207  der......filesr.
 00001c70: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00001c80: 0000 723c 0000 0072 0c00 0000 720d 0000  ..r<...r....r...
-00001c90: 0072 0e00 0000 720f 0000 0072 2300 0000  .r....r....r#...
+00001c80: 0000 7239 0000 0072 0c00 0000 720d 0000  ..r9...r....r...
+00001c90: 0072 0e00 0000 720f 0000 0072 2200 0000  .r....r....r"...
 00001ca0: 7210 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00001cb0: 2400 0000 7224 0000 0072 2400 0000 7225  $...r$...r$...r%
+00001cb0: 2300 0000 7223 0000 0072 2300 0000 7224  #...r#...r#...r$
 00001cc0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
 00001cd0: 0073 1200 0000 0800 0801 1001 0802 0c02  .s..............
 00001ce0: 1801 1806 1006 1203                      ........
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 2215 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 a708 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 a708 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6401 6c06 5a06 6403  m.Z...d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 0100 6403 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6403 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -28,15 +28,15 @@
 000001b0: 6365 7373 4d6f 6465 da08 5265 6164 4f6e  cessMode..ReadOn
 000001c0: 6c79 da09 5265 6164 5772 6974 654e 2905  ly..ReadWriteN).
 000001d0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 000001e0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 000001f0: 6d65 5f5f 7210 0000 0072 1100 0000 a900  me__r....r......
 00000200: 7215 0000 0072 1500 0000 faf0 2f63 6f64  r....r....../cod
 00000210: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000220: 6334 3039 3837 3536 3136 392f 7372 632f  c4098756169/src/
+00000220: 6333 3439 3732 3638 3637 302f 7372 632f  c3497268670/src/
 00000230: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000240: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000250: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000260: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 00000270: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000280: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 00000290: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 4911 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 2f13 0000  o........F.d/...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 2f13 0000  o.......Ms.d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 5a05 6403  m.Z...d.d.l.Z.d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6403 6405 6c0a 6d0b 5a0b 0100 6403  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6407 6408 6c0e  d.l.m.Z...d.d.l.
@@ -66,16 +66,16 @@
 00000410: 0000 0300 0000 731a 0000 0074 0083 00a0  ......s....t....
 00000420: 01a1 0001 007c 027c 005f 027c 017c 005f  .....|.|._.|.|._
 00000430: 0364 0053 00a9 014e 2904 da05 7375 7065  .d.S...N)...supe
 00000440: 72da 085f 5f69 6e69 745f 5f72 1500 0000  r..__init__r....
 00000450: 7216 0000 0029 03da 0473 656c 6672 1700  r....)...selfr..
 00000460: 0000 7218 0000 00a9 01da 095f 5f63 6c61  ..r........__cla
 00000470: 7373 5f5f a900 faf5 2f63 6f64 6562 7569  ss__..../codebui
-00000480: 6c64 2f6f 7574 7075 742f 7372 6334 3039  ld/output/src409
-00000490: 3837 3536 3136 392f 7372 632f 636f 6465  8756169/src/code
+00000480: 6c64 2f6f 7574 7075 742f 7372 6333 3439  ld/output/src349
+00000490: 3732 3638 3637 302f 7372 632f 636f 6465  7268670/src/code
 000004a0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 000004b0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 000004c0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 000004d0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 000004e0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 000004f0: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000500: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 867 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 6303 0000  o........F.dc...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 6303 0000  o.......Ms.dc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6505 6501  Z.G.d.d...d.e.e.
 00000060: 6a06 8304 5a07 4700 6405 6406 8400 6406  j...Z.G.d.d...d.
 00000070: 6505 6501 6a06 8304 5a08 4700 6407 6408  e.e.j...Z.G.d.d.
@@ -13,15 +13,15 @@
 000000c0: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
 000000d0: 0d41 646d 696e 6973 7472 6174 6f72 da06  .Administrator..
 000000e0: 526f 626f 746f 4e29 04da 085f 5f6e 616d  RobotoN)...__nam
 000000f0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 00000100: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0500  .__qualname__r..
 00000110: 0000 a900 7209 0000 0072 0900 0000 faee  ....r....r......
 00000120: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000130: 742f 7372 6334 3039 3837 3536 3136 392f  t/src4098756169/
+00000130: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
 00000140: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000150: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000160: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000170: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000180: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000190: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000001a0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/dataset.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/http_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/datasets/record.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/datasets/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 436 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 b401 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 b401 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6407  ..d.d.l.m.Z...d.
@@ -22,16 +22,16 @@
 00000150: 6572 0400 0000 da0d 6874 7470 5f64 656c  er......http_del
 00000160: 6567 6174 6572 0500 0000 da0e 6874 7470  egater......http
 00000170: 5f72 6573 6f75 7263 6573 7206 0000 0072  _resourcesr....r
 00000180: 0700 0000 da06 7265 636f 7264 7208 0000  ......recordr...
 00000190: 005a 0b73 335f 6465 6c65 6761 7465 7209  .Z.s3_delegater.
 000001a0: 0000 00da 075f 5f61 6c6c 5f5f a900 7210  .....__all__..r.
 000001b0: 0000 0072 1000 0000 faed 2f63 6f64 6562  ...r....../codeb
-000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6334  uild/output/src4
-000001d0: 3039 3837 3536 3136 392f 7372 632f 636f  098756169/src/co
+000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+000001d0: 3439 3732 3638 3637 302f 7372 632f 636f  497268670/src/co
 000001e0: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 000001f0: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000200: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000210: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000220: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000230: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000240: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 1181 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 9d04 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 9d04 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6403 6404 6c05 6d06 5a06 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6501 6a07 8303 5a08  d.d...d.e.j...Z.
 00000070: 4700 6407 6408 8400 6408 6500 6a09 8303  G.d.d...d.e.j...
@@ -17,16 +17,16 @@
 00000100: 6964 5a0d 636f 6d6d 6f6e 5f70 7265 6669  idZ.common_prefi
 00000110: 784e 2906 da08 5f5f 6e61 6d65 5f5f da0a  xN)...__name__..
 00000120: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 00000130: 616c 6e61 6d65 5f5f da09 4461 7461 7365  alname__..Datase
 00000140: 7449 64da 054f 7267 4964 da0c 436f 6d6d  tId..OrgId..Comm
 00000150: 6f6e 5072 6566 6978 a900 720e 0000 0072  onPrefix..r....r
 00000160: 0e00 0000 faed 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000170: 2f6f 7574 7075 742f 7372 6334 3039 3837  /output/src40987
-00000180: 3536 3136 392f 7372 632f 636f 6465 7374  56169/src/codest
+00000170: 2f6f 7574 7075 742f 7372 6333 3439 3732  /output/src34972
+00000180: 3638 3637 302f 7372 632f 636f 6465 7374  68670/src/codest
 00000190: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 000001a0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000001b0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000001c0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000001d0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000001e0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000001f0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 802 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 2203 0000  o........F.d"...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 2203 0000  o.......Ms.d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 6403 6404 6c04 6d05 5a05 0100 4700  Z.d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 8302 5a06 6402 5300  d.d...d...Z.d.S.
 00000060: 2907 e900 0000 0029 01da 084f 7074 696f  )......)...Optio
 00000070: 6e61 6c4e e901 0000 0029 01da 0a46 696c  nalN.....)...Fil
@@ -21,15 +21,15 @@
 00000140: 4669 6c65 5f5f 7061 7273 6564 5f75 7269  File__parsed_uri
 00000150: da06 7265 636f 7264 6302 0000 0000 0000  ..recordc.......
 00000160: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00000170: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
 00000180: a901 4e29 0172 0600 0000 2902 da04 7365  ..N).r....)...se
 00000190: 6c66 7208 0000 00a9 0072 0b00 0000 fae9  lfr......r......
 000001a0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000001b0: 742f 7372 6334 3039 3837 3536 3136 392f  t/src4098756169/
+000001b0: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
 000001c0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 000001d0: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 000001e0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 000001f0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000200: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000210: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000220: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 2166 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 7608 0000  o........F.dv...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 7608 0000  o.......Ms.dv...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 0100 6406 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6406 6408 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6406 6409 6c0d  m.Z.m.Z...d.d.l.
@@ -56,15 +56,15 @@
 00000370: 0000 0074 0083 00a0 01a1 0001 007c 027c  ...t.........|.|
 00000380: 005f 027c 017c 005f 0364 0053 00a9 014e  ._.|.|._.d.S...N
 00000390: 2904 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
 000003a0: 745f 5f72 0d00 0000 720e 0000 0029 03da  t__r....r....)..
 000003b0: 0473 656c 6672 0f00 0000 7210 0000 00a9  .selfr....r.....
 000003c0: 01da 095f 5f63 6c61 7373 5f5f a900 faf2  ...__class__....
 000003d0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000003e0: 742f 7372 6334 3039 3837 3536 3136 392f  t/src4098756169/
+000003e0: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
 000003f0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000400: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000410: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000420: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000430: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000440: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000450: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 168 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 a800 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 cd00 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
+00000020: 0004 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
-00000040: 6500 6a01 8303 5a02 4700 6404 6405 8400  e.j...Z.G.d.d...
-00000050: 6405 6500 6a01 8303 5a03 6401 5300 2906  d.e.j...Z.d.S.).
-00000060: e900 0000 004e 6300 0000 0000 0000 0000  .....Nc.........
-00000070: 0000 0000 0000 0003 0000 0040 0000 00f3  ...........@....
-00000080: 1e00 0000 6500 5a01 6400 5a02 5500 6503  ....e.Z.d.Z.U.e.
-00000090: 6504 6401 3c00 6503 6504 6402 3c00 6403  e.d.<.e.e.d.<.d.
-000000a0: 5300 2904 da11 4372 6561 7465 4669 6c65  S.)...CreateFile
-000000b0: 5265 7175 6573 74da 0662 7563 6b65 74da  Request..bucket.
-000000c0: 036b 6579 4ea9 05da 085f 5f6e 616d 655f  .keyN....__name_
-000000d0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000000e0: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
-000000f0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-00000100: 5fa9 0072 0c00 0000 720c 0000 00fa f32f  _..r....r....../
-00000110: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000120: 2f73 7263 3430 3938 3735 3631 3639 2f73  /src4098756169/s
-00000130: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
-00000140: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
-00000150: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
-00000160: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
-00000170: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
-00000180: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
-00000190: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
-000001a0: 3639 3964 2f72 6f62 6f74 6f2d 6169 2f72  699d/roboto-ai/r
-000001b0: 6f62 6f74 6f2d 686f 7374 6564 2d61 7070  oboto-hosted-app
-000001c0: 2f70 6163 6b61 6765 732f 726f 626f 746f  /packages/roboto
-000001d0: 5f73 646b 2f73 7263 2f72 6f62 6f74 6f5f  _sdk/src/roboto_
-000001e0: 7364 6b2f 646f 6d61 696e 2f66 696c 6573  sdk/domain/files
-000001f0: 2f68 7474 705f 7265 736f 7572 6365 732e  /http_resources.
-00000200: 7079 7203 0000 0004 0000 00f3 0600 0000  pyr.............
-00000210: 0a00 0801 0c01 7203 0000 0063 0000 0000  ......r....c....
-00000220: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000230: 4000 0000 7202 0000 0029 04da 1144 656c  @...r....)...Del
-00000240: 6574 6546 696c 6552 6571 7565 7374 7204  eteFileRequestr.
-00000250: 0000 0072 0500 0000 4e72 0600 0000 720c  ...r....Nr....r.
-00000260: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000270: 0000 720f 0000 0009 0000 0072 0e00 0000  ..r........r....
-00000280: 720f 0000 0029 04da 0870 7964 616e 7469  r....)...pydanti
-00000290: 63da 0942 6173 654d 6f64 656c 7203 0000  c..BaseModelr...
-000002a0: 0072 0f00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-000002b0: 720c 0000 0072 0d00 0000 da08 3c6d 6f64  r....r......<mod
-000002c0: 756c 653e 0100 0000 7306 0000 0008 0012  ule>....s.......
-000002d0: 0316 05                                  ...
+00000040: 6500 6a01 8303 5a02 6401 5300 2904 e900  e.j...Z.d.S.)...
+00000050: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
+00000060: 0000 0000 0003 0000 0040 0000 0073 2a00  .........@...s*.
+00000070: 0000 6500 5a01 6400 5a02 5500 6503 6a04  ..e.Z.d.Z.U.e.j.
+00000080: 6401 6402 8d01 5a05 6506 6507 6403 3c00  d.d...Z.e.e.d.<.
+00000090: 6506 6507 6404 3c00 6405 5300 2906 da14  e.e.d.<.d.S.)...
+000000a0: 4372 6561 7465 5472 6967 6765 7252 6571  CreateTriggerReq
+000000b0: 7565 7374 7a0d 5b5c 775c 2d5d 7b31 2c32  uestz.[\w\-]{1,2
+000000c0: 3536 7d29 01da 0572 6567 6578 da04 6e61  56})...regex..na
+000000d0: 6d65 da0b 6163 7469 6f6e 5f6e 616d 654e  me..action_nameN
+000000e0: 2908 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000000f0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000100: 6e61 6d65 5f5f da08 7079 6461 6e74 6963  name__..pydantic
+00000110: da05 4669 656c 6472 0400 0000 da03 7374  ..Fieldr......st
+00000120: 72da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  r..__annotations
+00000130: 5f5f a900 720d 0000 0072 0d00 0000 faf6  __..r....r......
+00000140: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
+00000150: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
+00000160: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
+00000170: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
+00000180: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
+00000190: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
+000001a0: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
+000001b0: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
+000001c0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
+000001d0: 3336 3939 642f 726f 626f 746f 2d61 692f  3699d/roboto-ai/
+000001e0: 726f 626f 746f 2d68 6f73 7465 642d 6170  roboto-hosted-ap
+000001f0: 702f 7061 636b 6167 6573 2f72 6f62 6f74  p/packages/robot
+00000200: 6f5f 7364 6b2f 7372 632f 726f 626f 746f  o_sdk/src/roboto
+00000210: 5f73 646b 2f64 6f6d 6169 6e2f 7472 6967  _sdk/domain/trig
+00000220: 6765 7273 2f68 7474 705f 7265 736f 7572  gers/http_resour
+00000230: 6365 732e 7079 7202 0000 0005 0000 0073  ces.pyr........s
+00000240: 0600 0000 0a00 1402 0c01 7202 0000 0029  ..........r....)
+00000250: 0372 0900 0000 da09 4261 7365 4d6f 6465  .r......BaseMode
+00000260: 6c72 0200 0000 720d 0000 0072 0d00 0000  lr....r....r....
+00000270: 720d 0000 0072 0e00 0000 da08 3c6d 6f64  r....r......<mod
+00000280: 756c 653e 0100 0000 7304 0000 0008 0116  ule>....s.......
+00000290: 03                                       .
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 382 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 7e01 0000  o........F.d~...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 d800 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 4700  d.l.Z.d.d.l.Z.G.
-00000040: 6402 6403 8400 6403 6501 6a02 8303 5a03  d.d...d.e.j...Z.
-00000050: 6401 5300 2904 e900 0000 004e 6300 0000  d.S.)......Nc...
-00000060: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000070: 0040 0000 0073 4000 0000 6500 5a01 6400  .@...s@...e.Z.d.
-00000080: 5a02 5500 6503 6504 6401 3c00 6505 6a05  Z.U.e.e.d.<.e.j.
-00000090: 6504 6402 3c00 6503 6504 6403 3c00 6506  e.d.<.e.e.d.<.e.
-000000a0: 6504 6404 3c00 6503 6504 6405 3c00 6503  e.d.<.e.e.d.<.e.
-000000b0: 6504 6406 3c00 6407 5300 2908 da0a 4669  e.d.<.d.S.)...Fi
-000000c0: 6c65 5265 636f 7264 da0e 6173 736f 6369  leRecord..associ
-000000d0: 6174 696f 6e5f 6964 da08 6d6f 6469 6669  ation_id..modifi
-000000e0: 6564 da0d 7265 6c61 7469 7665 5f70 6174  ed..relative_pat
-000000f0: 68da 0473 697a 65da 066f 7267 5f69 64da  h..size..org_id.
-00000100: 0375 7269 4e29 07da 085f 5f6e 616d 655f  .uriN)...__name_
-00000110: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000120: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
-00000130: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-00000140: 5fda 0864 6174 6574 696d 65da 0369 6e74  _..datetime..int
-00000150: a900 7210 0000 0072 1000 0000 faeb 2f63  ..r....r....../c
-00000160: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000170: 7372 6334 3039 3837 3536 3136 392f 7372  src4098756169/sr
-00000180: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
-00000190: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
-000001a0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
-000001b0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
-000001c0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
-000001d0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
-000001e0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
-000001f0: 3939 642f 726f 626f 746f 2d61 692f 726f  99d/roboto-ai/ro
-00000200: 626f 746f 2d68 6f73 7465 642d 6170 702f  boto-hosted-app/
-00000210: 7061 636b 6167 6573 2f72 6f62 6f74 6f5f  packages/roboto_
-00000220: 7364 6b2f 7372 632f 726f 626f 746f 5f73  sdk/src/roboto_s
-00000230: 646b 2f64 6f6d 6169 6e2f 6669 6c65 732f  dk/domain/files/
-00000240: 7265 636f 7264 2e70 7972 0200 0000 0600  record.pyr......
-00000250: 0000 730e 0000 000a 0008 010a 0108 0108  ..s.............
-00000260: 0108 010c 0172 0200 0000 2904 720e 0000  .....r....).r...
-00000270: 00da 0870 7964 616e 7469 63da 0942 6173  ...pydantic..Bas
-00000280: 654d 6f64 656c 7202 0000 0072 1000 0000  eModelr....r....
-00000290: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-000002a0: 083c 6d6f 6475 6c65 3e01 0000 0073 0600  .<module>....s..
-000002b0: 0000 0800 0802 1603                      ........
+00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 5a02 4700 6403 6404 8400 6404 6502 6a03  Z.G.d.d...d.e.j.
+00000050: 8303 5a04 6402 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 084f 7074 696f 6e61 6c4e 6300 0000  ...OptionalNc...
+00000070: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000080: 0040 0000 0073 2e00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000090: 5a02 5500 6503 6504 6401 3c00 6505 6504  Z.U.e.e.d.<.e.e.
+000000a0: 6402 3c00 6403 5a06 6507 6505 1900 6504  d.<.d.Z.e.e...e.
+000000b0: 6404 3c00 6403 5300 2905 da12 4372 6561  d.<.d.S.)...Crea
+000000c0: 7465 546f 6b65 6e52 6571 7565 7374 da0b  teTokenRequest..
+000000d0: 6578 7069 7279 5f64 6179 73da 046e 616d  expiry_days..nam
+000000e0: 654e da0b 6465 7363 7269 7074 696f 6e29  eN..description)
+000000f0: 08da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000100: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000110: 616d 655f 5fda 0369 6e74 da0f 5f5f 616e  ame__..int..__an
+00000120: 6e6f 7461 7469 6f6e 735f 5fda 0373 7472  notations__..str
+00000130: 7206 0000 0072 0200 0000 a900 720d 0000  r....r......r...
+00000140: 0072 0d00 0000 faf4 2f63 6f64 6562 7569  .r....../codebui
+00000150: 6c64 2f6f 7574 7075 742f 7372 6333 3439  ld/output/src349
+00000160: 3732 3638 3637 302f 7372 632f 636f 6465  7268670/src/code
+00000170: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
+00000180: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
+00000190: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
+000001a0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
+000001b0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
+000001c0: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
+000001d0: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
+000001e0: 626f 746f 2d61 692f 726f 626f 746f 2d68  boto-ai/roboto-h
+000001f0: 6f73 7465 642d 6170 702f 7061 636b 6167  osted-app/packag
+00000200: 6573 2f72 6f62 6f74 6f5f 7364 6b2f 7372  es/roboto_sdk/sr
+00000210: 632f 726f 626f 746f 5f73 646b 2f64 6f6d  c/roboto_sdk/dom
+00000220: 6169 6e2f 746f 6b65 6e73 2f68 7474 705f  ain/tokens/http_
+00000230: 7265 736f 7572 6365 732e 7079 7203 0000  resources.pyr...
+00000240: 0009 0000 0073 0800 0000 0a00 0801 0801  .....s..........
+00000250: 1401 7203 0000 0029 05da 0674 7970 696e  ..r....)...typin
+00000260: 6772 0200 0000 da08 7079 6461 6e74 6963  gr......pydantic
+00000270: da09 4261 7365 4d6f 6465 6c72 0300 0000  ..BaseModelr....
+00000280: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00000290: 0e00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000002a0: 0000 7306 0000 000c 0308 0216 03         ..s..........
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 2358 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 3609 0000  o........F.d6...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 3609 0000  o.......Ms.d6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6401 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a06 6400 6401 6c07 5a07 6403 6404 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6403 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
@@ -22,16 +22,16 @@
 00000150: 6563 7265 745f 6163 6365 7373 5f6b 6579  ecret_access_key
 00000160: da0d 7365 7373 696f 6e5f 746f 6b65 6e4e  ..session_tokenN
 00000170: 2905 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 00000180: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000190: 6e61 6d65 5f5f da03 7374 72da 0f5f 5f61  name__..str..__a
 000001a0: 6e6e 6f74 6174 696f 6e73 5f5f a900 7212  nnotations__..r.
 000001b0: 0000 0072 1200 0000 faf0 2f63 6f64 6562  ...r....../codeb
-000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6334  uild/output/src4
-000001d0: 3039 3837 3536 3136 392f 7372 632f 636f  098756169/src/co
+000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+000001d0: 3439 3732 3638 3637 302f 7372 632f 636f  497268670/src/co
 000001e0: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 000001f0: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000200: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000210: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000220: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000230: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000240: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/file.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/file.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/http_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/files/s3_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/files/s3_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/__init__.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/http_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org_invite.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org_invite.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/org_role.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/org_role.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/orgs/record.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/orgs/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/http_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/tokens/token.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/tokens/token.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/http_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/trigger.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/trigger.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/triggers/trigger_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/triggers/trigger_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/users/http_delegate.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/users/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/domain/users/user.py` & `roboto_sdk-0.1.5/src/roboto_sdk/domain/users/user.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/http/__init__.py` & `roboto_sdk-0.1.5/src/roboto_sdk/http/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 704 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 c002 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 c002 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6403 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6404 6c0e 6d0f 5a0f 0100 6405  ..d.d.l.m.Z...d.
@@ -31,16 +31,16 @@
 000001e0: 636c 6965 6e74 7206 0000 0072 0700 0000  clientr....r....
 000001f0: 7208 0000 0072 0900 0000 5a12 7265 7175  r....r....Z.requ
 00000200: 6573 745f 6465 636f 7261 746f 7273 720a  est_decoratorsr.
 00000210: 0000 0072 0b00 0000 720c 0000 005a 0c74  ...r....r....Z.t
 00000220: 6573 7469 6e67 5f75 7469 6c72 0d00 0000  esting_utilr....
 00000230: da07 5f5f 616c 6c5f 5fa9 0072 1100 0000  ..__all__..r....
 00000240: 7211 0000 00fa e52f 636f 6465 6275 696c  r....../codebuil
-00000250: 642f 6f75 7470 7574 2f73 7263 3430 3938  d/output/src4098
-00000260: 3735 3631 3639 2f73 7263 2f63 6f64 6573  756169/src/codes
+00000250: 642f 6f75 7470 7574 2f73 7263 3334 3937  d/output/src3497
+00000260: 3236 3836 3730 2f73 7263 2f63 6f64 6573  268670/src/codes
 00000270: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 00000280: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 00000290: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 000002a0: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 000002b0: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 000002c0: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 000002d0: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 9060 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 6423 0000  o........F.dd#..
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 6423 0000  o.......Ms.dd#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a07 6400 6401 6c08 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c09 5a07 6400 6401 6c0a 5a07 6400  d.l.Z.d.d.l.Z.d.
@@ -35,22 +35,22 @@
 00000220: 5300 6401 5300 2903 4e46 7a24 5465 6d70  S.d.S.).NFz$Temp
 00000230: 6f72 6172 7920 6661 696c 7572 6520 696e  orary failure in
 00000240: 206e 616d 6520 7265 736f 6c75 7469 6f6e   name resolution
 00000250: 290e da0a 6973 696e 7374 616e 6365 da06  )...isinstance..
 00000260: 7572 6c6c 6962 da05 6572 726f 72da 0948  urllib..error..H
 00000270: 5454 5045 7272 6f72 da04 6874 7470 da0a  TTPError..http..
 00000280: 4854 5450 5374 6174 7573 da03 696e 74da  HTTPStatus..int.
-00000290: 0463 6f64 65da 1154 4f4f 5f4d 414e 595f  .code..TOO_MANY_
-000002a0: 5245 5155 4553 5453 da13 5345 5256 4943  REQUESTS..SERVIC
+00000290: 0463 6f64 655a 1154 4f4f 5f4d 414e 595f  .codeZ.TOO_MANY_
+000002a0: 5245 5155 4553 5453 5a13 5345 5256 4943  REQUESTSZ.SERVIC
 000002b0: 455f 554e 4156 4149 4c41 424c 45da 0a56  E_UNAVAILABLE..V
 000002c0: 616c 7565 4572 726f 72da 0855 524c 4572  alueError..URLEr
 000002d0: 726f 72da 0373 7472 da06 7265 6173 6f6e  ror..str..reason
-000002e0: 2901 7205 0000 00a9 0072 1500 0000 fae8  ).r......r......
+000002e0: 2901 7205 0000 00a9 0072 1300 0000 fae8  ).r......r......
 000002f0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000300: 742f 7372 6334 3039 3837 3536 3136 392f  t/src4098756169/
+00000300: 742f 7372 6333 3439 3732 3638 3637 302f  t/src3497268670/
 00000310: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000320: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000330: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000340: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000350: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000360: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000370: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
@@ -59,22 +59,22 @@
 000003a0: 702f 7061 636b 6167 6573 2f72 6f62 6f74  p/packages/robot
 000003b0: 6f5f 7364 6b2f 7372 632f 726f 626f 746f  o_sdk/src/roboto
 000003c0: 5f73 646b 2f68 7474 702f 6874 7470 5f63  _sdk/http/http_c
 000003d0: 6c69 656e 742e 7079 da1b 6973 5f65 7870  lient.py..is_exp
 000003e0: 6563 7465 645f 746f 5f62 655f 7472 616e  ected_to_be_tran
 000003f0: 7369 656e 7417 0000 0073 1800 0000 0e01  sient....s......
 00000400: 0201 0e01 0601 0601 08fe 0c04 0601 02ff  ................
-00000410: 0e05 0e02 0402 7217 0000 00da 045f 6578  ......r......_ex
+00000410: 0e05 0e02 0402 7215 0000 00da 045f 6578  ......r......_ex
 00000420: 6363 0100 0000 0000 0000 0000 0000 0100  cc..............
 00000430: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
 00000440: 0153 0029 024e 6700 0000 0000 00f0 3f72  .S.).Ng.......?r
-00000450: 1500 0000 2901 7218 0000 0072 1500 0000  ....).r....r....
-00000460: 7215 0000 0072 1600 0000 da12 6465 6661  r....r......defa
+00000450: 1300 0000 2901 7216 0000 0072 1300 0000  ....).r....r....
+00000460: 7213 0000 0072 1400 0000 da12 6465 6661  r....r......defa
 00000470: 756c 745f 7265 7472 795f 7761 6974 2a00  ult_retry_wait*.
-00000480: 0000 7302 0000 0004 0172 1900 0000 6300  ..s......r....c.
+00000480: 0000 7302 0000 0004 0172 1700 0000 6300  ..s......r....c.
 00000490: 0000 0000 0000 0000 0000 0000 0000 0004  ................
 000004a0: 0000 0000 0000 0073 a400 0000 6500 5a01  .......s....e.Z.
 000004b0: 6400 5a02 5500 6503 6a04 6a05 6506 6401  d.Z.U.e.j.j.e.d.
 000004c0: 3c00 6402 5a07 6508 6a09 6506 6403 3c00  <.d.Z.e.j.e.d.<.
 000004d0: 6402 5a0a 6508 6a0b 650c 6a0d 1900 6506  d.Z.e.j.e.j...e.
 000004e0: 6404 3c00 6405 6503 6a04 6a05 6406 6402  d.<.d.e.j.j.d.d.
 000004f0: 6604 8700 6601 6407 6408 840c 5a0e 6406  f...f.d.d...Z.d.
@@ -88,164 +88,164 @@
 00000570: 6578 634e da0f 5f48 7474 7045 7272 6f72  excN.._HttpError
 00000580: 5f5f 6d73 67da 125f 4874 7470 4572 726f  __msg.._HttpErro
 00000590: 725f 5f73 7461 7475 7372 0500 0000 7206  r__statusr....r.
 000005a0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
 000005b0: 0200 0000 0200 0000 0300 0000 f314 0000  ................
 000005c0: 0074 0083 00a0 01a1 0001 007c 017c 005f  .t.........|.|._
 000005d0: 0264 0053 00a9 014e 2903 da05 7375 7065  .d.S...N)...supe
-000005e0: 72da 085f 5f69 6e69 745f 5f72 1b00 0000  r..__init__r....
+000005e0: 72da 085f 5f69 6e69 745f 5f72 1900 0000  r..__init__r....
 000005f0: 2902 da04 7365 6c66 7205 0000 00a9 01da  )...selfr.......
-00000600: 095f 5f63 6c61 7373 5f5f 7215 0000 0072  .__class__r....r
-00000610: 1600 0000 7221 0000 0033 0000 00f3 0400  ....r!...3......
+00000600: 095f 5f63 6c61 7373 5f5f 7213 0000 0072  .__class__r....r
+00000610: 1400 0000 721f 0000 0033 0000 00f3 0400  ....r....3......
 00000620: 0000 0a01 0a01 7a12 4874 7470 4572 726f  ......z.HttpErro
 00000630: 722e 5f5f 696e 6974 5f5f 6301 0000 0000  r.__init__c.....
 00000640: 0000 0000 0000 0001 0000 0006 0000 0043  ...............C
 00000650: 0000 0073 1e00 0000 7c00 6a00 6a01 9b00  ...s....|.j.j...
 00000660: 6401 7c00 6a02 9b02 6402 7c00 6a03 9b02  d.|.j...d.|.j...
 00000670: 6403 9d06 5300 2904 4efa 0128 7a02 2c20  d...S.).N..(z., 
-00000680: fa01 2929 0472 2400 0000 da08 5f5f 6e61  ..)).r$.....__na
+00000680: fa01 2929 0472 2200 0000 da08 5f5f 6e61  ..)).r".....__na
 00000690: 6d65 5f5f da03 6d73 67da 0673 7461 7475  me__..msg..statu
-000006a0: 73a9 0172 2200 0000 7215 0000 0072 1500  s..r"...r....r..
-000006b0: 0000 7216 0000 00da 085f 5f72 6570 725f  ..r......__repr_
+000006a0: 73a9 0172 2000 0000 7213 0000 0072 1300  s..r ...r....r..
+000006b0: 0000 7214 0000 00da 085f 5f72 6570 725f  ..r......__repr_
 000006c0: 5f37 0000 0073 0200 0000 1e01 7a12 4874  _7...s......z.Ht
 000006d0: 7470 4572 726f 722e 5f5f 7265 7072 5f5f  tpError.__repr__
 000006e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
 000006f0: 0001 0000 0043 0000 0073 0800 0000 7c00  .....C...s....|.
-00000700: 6a00 9b02 5300 721f 0000 0029 0172 2900  j...S.r....).r).
-00000710: 0000 722b 0000 0072 1500 0000 7215 0000  ..r+...r....r...
-00000720: 0072 1600 0000 da07 5f5f 7374 725f 5f3a  .r......__str__:
+00000700: 6a00 9b02 5300 721d 0000 0029 0172 2700  j...S.r....).r'.
+00000710: 0000 7229 0000 0072 1300 0000 7213 0000  ..r)...r....r...
+00000720: 0072 1400 0000 da07 5f5f 7374 725f 5f3a  .r......__str__:
 00000730: 0000 0073 0200 0000 0801 7a11 4874 7470  ...s......z.Http
 00000740: 4572 726f 722e 5f5f 7374 725f 5f63 0100  Error.__str__c..
 00000750: 0000 0000 0000 0000 0000 0100 0000 0800  ................
 00000760: 0000 4300 0000 734a 0000 007c 006a 0064  ..C...sJ...|.j.d
 00000770: 0075 0072 227a 0e74 01a0 0274 037c 006a  .u.r"z.t...t.|.j
 00000780: 046a 0583 01a1 017c 005f 0057 007c 006a  .j.....|._.W.|.j
 00000790: 0053 0004 0074 0679 2101 0001 0001 0064  .S...t.y!......d
 000007a0: 007c 005f 0059 007c 006a 0053 0077 007c  .|._.Y.|.j.S.w.|
-000007b0: 006a 0053 0072 1f00 0000 2907 721d 0000  .j.S.r....).r...
+000007b0: 006a 0053 0072 1d00 0000 2907 721b 0000  .j.S.r....).r...
 000007c0: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000007d0: 721b 0000 0072 0e00 0000 7211 0000 0072  r....r....r....r
-000007e0: 2b00 0000 7215 0000 0072 1500 0000 7216  +...r....r....r.
-000007f0: 0000 0072 2a00 0000 3d00 0000 7312 0000  ...r*...=...s...
+000007d0: 7219 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+000007e0: 2900 0000 7213 0000 0072 1300 0000 7214  )...r....r....r.
+000007f0: 0000 0072 2800 0000 3d00 0000 7312 0000  ...r(...=...s...
 00000800: 000a 0202 0116 0106 030c fe08 0106 0102  ................
 00000810: fe06 027a 1048 7474 7045 7272 6f72 2e73  ...z.HttpError.s
 00000820: 7461 7475 7363 0100 0000 0000 0000 0000  tatusc..........
 00000830: 0000 0200 0000 0800 0000 4300 0000 7354  ..........C...sT
 00000840: 0000 007c 006a 0064 0075 0072 277c 006a  ...|.j.d.u.r'|.j
 00000850: 01a0 02a1 00a0 0364 01a1 017d 017a 0a74  .......d...}.z.t
 00000860: 04a0 057c 01a1 017c 005f 0057 007c 006a  ...|...|._.W.|.j
 00000870: 0053 0004 0074 046a 0679 2601 0001 0001  .S...t.j.y&.....
 00000880: 007c 017c 005f 0059 007c 006a 0053 0077  .|.|._.Y.|.j.S.w
 00000890: 007c 006a 0053 00a9 024e 7a05 7574 662d  .|.j.S...Nz.utf-
-000008a0: 3829 0772 1c00 0000 721b 0000 00da 0472  8).r....r......r
+000008a0: 3829 0772 1a00 0000 7219 0000 00da 0472  8).r....r......r
 000008b0: 6561 64da 0664 6563 6f64 65da 046a 736f  ead..decode..jso
 000008c0: 6eda 056c 6f61 6473 da0f 4a53 4f4e 4465  n..loads..JSONDe
-000008d0: 636f 6465 4572 726f 7229 0272 2200 0000  codeError).r"...
-000008e0: da07 6465 636f 6465 6472 1500 0000 7215  ..decodedr....r.
-000008f0: 0000 0072 1600 0000 7229 0000 0046 0000  ...r....r)...F..
+000008d0: 636f 6465 4572 726f 7229 0272 2000 0000  codeError).r ...
+000008e0: da07 6465 636f 6465 6472 1300 0000 7213  ..decodedr....r.
+000008f0: 0000 0072 1400 0000 7227 0000 0046 0000  ...r....r'...F..
 00000900: 0073 1400 0000 0a02 1001 0201 0e01 0603  .s..............
 00000910: 0efe 0801 0601 02fe 0602 7a0d 4874 7470  ..........z.Http
-00000920: 4572 726f 722e 6d73 6729 1672 2800 0000  Error.msg).r(...
+00000920: 4572 726f 722e 6d73 6729 1672 2600 0000  Error.msg).r&...
 00000930: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 00000940: 7175 616c 6e61 6d65 5f5f 7208 0000 0072  qualname__r....r
 00000950: 0900 0000 720a 0000 00da 0f5f 5f61 6e6e  ....r......__ann
-00000960: 6f74 6174 696f 6e73 5f5f 721c 0000 00da  otations__r.....
-00000970: 0674 7970 696e 67da 0341 6e79 721d 0000  .typing..Anyr...
+00000960: 6f74 6174 696f 6e73 5f5f 721a 0000 00da  otations__r.....
+00000970: 0674 7970 696e 67da 0341 6e79 721b 0000  .typing..Anyr...
 00000980: 00da 084f 7074 696f 6e61 6c72 0b00 0000  ...Optionalr....
-00000990: 720c 0000 0072 2100 0000 7213 0000 0072  r....r!...r....r
-000009a0: 2c00 0000 722d 0000 00da 0870 726f 7065  ,...r-.....prope
-000009b0: 7274 7972 2a00 0000 7229 0000 00da 0d5f  rtyr*...r)....._
-000009c0: 5f63 6c61 7373 6365 6c6c 5f5f 7215 0000  _classcell__r...
-000009d0: 0072 1500 0000 7223 0000 0072 1600 0000  .r....r#...r....
-000009e0: 721a 0000 002e 0000 0073 1600 0000 0a00  r........s......
+00000990: 720c 0000 0072 1f00 0000 7211 0000 0072  r....r....r....r
+000009a0: 2a00 0000 722b 0000 00da 0870 726f 7065  *...r+.....prope
+000009b0: 7274 7972 2800 0000 7227 0000 00da 0d5f  rtyr(...r'....._
+000009c0: 5f63 6c61 7373 6365 6c6c 5f5f 7213 0000  _classcell__r...
+000009d0: 0072 1300 0000 7221 0000 0072 1400 0000  .r....r!...r....
+000009e0: 7218 0000 002e 0000 0073 1600 0000 0a00  r........s......
 000009f0: 0c01 0e01 1401 1a02 0e04 0e03 0203 1801  ................
-00000a00: 0208 1a01 721a 0000 0063 0000 0000 0000  ....r....c......
+00000a00: 0208 1a01 7218 0000 0063 0000 0000 0000  ....r....c......
 00000a10: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
 00000a20: 0000 f30c 0000 0065 005a 0164 005a 0264  .......e.Z.d.Z.d
 00000a30: 0153 0029 02da 0b43 6c69 656e 7445 7272  .S.)...ClientErr
-00000a40: 6f72 4ea9 0372 2800 0000 7235 0000 0072  orN..r(...r5...r
-00000a50: 3600 0000 7215 0000 0072 1500 0000 7215  6...r....r....r.
-00000a60: 0000 0072 1600 0000 723e 0000 0051 0000  ...r....r>...Q..
-00000a70: 00f3 0400 0000 0800 0401 723e 0000 0063  ..........r>...c
+00000a40: 6f72 4ea9 0372 2600 0000 7233 0000 0072  orN..r&...r3...r
+00000a50: 3400 0000 7213 0000 0072 1300 0000 7213  4...r....r....r.
+00000a60: 0000 0072 1400 0000 723c 0000 0051 0000  ...r....r<...Q..
+00000a70: 00f3 0400 0000 0800 0401 723c 0000 0063  ..........r<...c
 00000a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000a90: 0100 0000 4000 0000 723d 0000 0029 02da  ....@...r=...)..
-00000aa0: 0b53 6572 7665 7245 7272 6f72 4e72 3f00  .ServerErrorNr?.
-00000ab0: 0000 7215 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00000ac0: 0072 1600 0000 7241 0000 0055 0000 0072  .r....rA...U...r
-00000ad0: 4000 0000 7241 0000 0063 0000 0000 0000  @...rA...c......
+00000a90: 0100 0000 4000 0000 723b 0000 0029 02da  ....@...r;...)..
+00000aa0: 0b53 6572 7665 7245 7272 6f72 4e72 3d00  .ServerErrorNr=.
+00000ab0: 0000 7213 0000 0072 1300 0000 7213 0000  ..r....r....r...
+00000ac0: 0072 1400 0000 723f 0000 0055 0000 0072  .r....r?...U...r
+00000ad0: 3e00 0000 723f 0000 0063 0000 0000 0000  >...r?...c......
 00000ae0: 0000 0000 0000 0000 0000 0500 0000 0000  ................
 00000af0: 0000 7380 0000 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
 00000b00: 0065 036a 046a 0565 0664 013c 0064 0265  .e.j.j.e.d.<.d.e
 00000b10: 036a 046a 0564 0364 0466 0487 0066 0164  .j.j.d.d.f...f.d
 00000b20: 0564 0684 0c5a 0765 0864 0365 036a 046a  .d...Z.e.d.e.j.j
 00000b30: 0566 0264 0764 0884 0483 015a 0965 0864  .f.d.d.....Z.e.d
 00000b40: 0365 0a6a 0b66 0264 0964 0a84 0483 015a  .e.j.f.d.d.....Z
 00000b50: 0c64 0e64 0b65 0d6a 0e65 0f65 1019 0019  .d.d.e.j.e.e....
 00000b60: 0064 0365 1166 0464 0c64 0d84 055a 1287  .d.e.f.d.d...Z..
 00000b70: 0004 005a 1353 0029 0fda 0c48 7474 7052  ...Z.S.)...HttpR
 00000b80: 6573 706f 6e73 65da 175f 4874 7470 5265  esponse.._HttpRe
 00000b90: 7370 6f6e 7365 5f5f 7265 7370 6f6e 7365  sponse__response
 00000ba0: da08 7265 7370 6f6e 7365 7206 0000 004e  ..responser....N
 00000bb0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000bc0: 0002 0000 0003 0000 0072 1e00 0000 721f  .........r....r.
-00000bd0: 0000 0029 0372 2000 0000 7221 0000 0072  ...).r ...r!...r
-00000be0: 4300 0000 2902 7222 0000 0072 4400 0000  C...).r"...rD...
-00000bf0: 7223 0000 0072 1500 0000 7216 0000 0072  r#...r....r....r
-00000c00: 2100 0000 5c00 0000 7225 0000 007a 1548  !...\...r%...z.H
+00000bc0: 0002 0000 0003 0000 0072 1c00 0000 721d  .........r....r.
+00000bd0: 0000 0029 0372 1e00 0000 721f 0000 0072  ...).r....r....r
+00000be0: 4100 0000 2902 7220 0000 0072 4200 0000  A...).r ...rB...
+00000bf0: 7221 0000 0072 1300 0000 7214 0000 0072  r!...r....r....r
+00000c00: 1f00 0000 5c00 0000 7223 0000 007a 1548  ....\...r#...z.H
 00000c10: 7474 7052 6573 706f 6e73 652e 5f5f 696e  ttpResponse.__in
 00000c20: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
 00000c30: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00000c40: 0000 7c00 6a00 5300 721f 0000 0029 0172  ..|.j.S.r....).r
-00000c50: 4300 0000 722b 0000 0072 1500 0000 7215  C...r+...r....r.
-00000c60: 0000 0072 1600 0000 da11 7265 6164 6162  ...r......readab
+00000c40: 0000 7c00 6a00 5300 721d 0000 0029 0172  ..|.j.S.r....).r
+00000c50: 4100 0000 7229 0000 0072 1300 0000 7213  A...r)...r....r.
+00000c60: 0000 0072 1400 0000 da11 7265 6164 6162  ...r......readab
 00000c70: 6c65 5f72 6573 706f 6e73 6560 0000 0073  le_response`...s
 00000c80: 0200 0000 0602 7a1e 4874 7470 5265 7370  ......z.HttpResp
 00000c90: 6f6e 7365 2e72 6561 6461 626c 655f 7265  onse.readable_re
 00000ca0: 7370 6f6e 7365 6301 0000 0000 0000 0000  sponsec.........
 00000cb0: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
 00000cc0: 2600 0000 7c00 6a00 6a01 7d01 7c01 6400  &...|.j.j.}.|.d.
 00000cd0: 7500 720c 7402 6401 8301 8201 7403 a004  u.r.t.d.....t...
 00000ce0: 7405 7c01 8301 a101 5300 2902 4e7a 1b52  t.|.....S.).Nz.R
 00000cf0: 6573 706f 6e73 6520 6861 7320 6e6f 2073  esponse has no s
-00000d00: 7461 7475 7320 636f 6465 2906 7243 0000  tatus code).rC..
-00000d10: 0072 2a00 0000 da0c 5275 6e74 696d 6545  .r*.....RuntimeE
+00000d00: 7461 7475 7320 636f 6465 2906 7241 0000  tatus code).rA..
+00000d10: 0072 2800 0000 da0c 5275 6e74 696d 6545  .r(.....RuntimeE
 00000d20: 7272 6f72 720b 0000 0072 0c00 0000 720d  rrorr....r....r.
-00000d30: 0000 0029 0272 2200 0000 da0b 7374 6174  ...).r".....stat
-00000d40: 7573 5f63 6f64 6572 1500 0000 7215 0000  us_coder....r...
-00000d50: 0072 1600 0000 722a 0000 0064 0000 0073  .r....r*...d...s
+00000d30: 0000 0029 0272 2000 0000 da0b 7374 6174  ...).r .....stat
+00000d40: 7573 5f63 6f64 6572 1300 0000 7213 0000  us_coder....r...
+00000d50: 0072 1400 0000 7228 0000 0064 0000 0073  .r....r(...d...s
 00000d60: 0800 0000 0802 0801 0801 0e01 7a13 4874  ............z.Ht
 00000d70: 7470 5265 7370 6f6e 7365 2e73 7461 7475  tpResponse.statu
 00000d80: 73da 096a 736f 6e5f 7061 7468 6302 0000  s..json_pathc...
 00000d90: 0000 0000 0000 0000 0003 0000 0008 0000  ................
 00000da0: 0043 0000 0073 6400 0000 7c00 6a00 8f25  .C...sd...|.j..%
 00000db0: 0100 7401 a002 7c00 6a00 a003 a100 a004  ..t...|.j.......
 00000dc0: 6401 a101 a101 7d02 7c01 6400 7500 721c  d.....}.|.d.u.r.
 00000dd0: 7c02 5700 0200 6400 0400 0400 8303 0100  |.W...d.........
 00000de0: 5300 7405 7c02 7c01 8302 5700 0200 6400  S.t.|.|...W...d.
 00000df0: 0400 0400 8303 0100 5300 3100 732b 7701  ........S.1.s+w.
-00000e00: 0100 0100 0100 5900 0100 6400 5300 722e  ......Y...d.S.r.
-00000e10: 0000 0029 0672 4300 0000 7231 0000 0072  ...).rC...r1...r
-00000e20: 3200 0000 722f 0000 0072 3000 0000 7204  2...r/...r0...r.
-00000e30: 0000 0029 0372 2200 0000 7248 0000 005a  ...).r"...rH...Z
-00000e40: 0b75 6e6d 6172 7361 6c6c 6564 7215 0000  .unmarsalledr...
-00000e50: 0072 1500 0000 7216 0000 00da 0966 726f  .r....r......fro
+00000e00: 0100 0100 0100 5900 0100 6400 5300 722c  ......Y...d.S.r,
+00000e10: 0000 0029 0672 4100 0000 722f 0000 0072  ...).rA...r/...r
+00000e20: 3000 0000 722d 0000 0072 2e00 0000 7204  0...r-...r....r.
+00000e30: 0000 0029 0372 2000 0000 7246 0000 005a  ...).r ...rF...Z
+00000e40: 0b75 6e6d 6172 7361 6c6c 6564 7213 0000  .unmarsalledr...
+00000e50: 0072 1300 0000 7214 0000 00da 0966 726f  .r....r......fro
 00000e60: 6d5f 6a73 6f6e 6b00 0000 730e 0000 0008  m_jsonk...s.....
 00000e70: 0116 0108 0102 0110 fd08 0524 fb7a 1648  ...........$.z.H
 00000e80: 7474 7052 6573 706f 6e73 652e 6672 6f6d  ttpResponse.from
-00000e90: 5f6a 736f 6e72 1f00 0000 2914 7228 0000  _jsonr....).r(..
-00000ea0: 0072 3500 0000 7236 0000 0072 0800 0000  .r5...r6...r....
-00000eb0: 7244 0000 005a 0a61 6464 696e 666f 7572  rD...Z.addinfour
-00000ec0: 6c72 3700 0000 7221 0000 0072 3b00 0000  lr7...r!...r;...
-00000ed0: 7245 0000 0072 0b00 0000 720c 0000 0072  rE...r....r....r
-00000ee0: 2a00 0000 7238 0000 0072 3a00 0000 da04  *...r8...r:.....
-00000ef0: 6c69 7374 7213 0000 00da 0464 6963 7472  listr......dictr
-00000f00: 4900 0000 723c 0000 0072 1500 0000 7215  I...r<...r....r.
-00000f10: 0000 0072 2300 0000 7216 0000 0072 4200  ...r#...r....rB.
+00000e90: 5f6a 736f 6e72 1d00 0000 2914 7226 0000  _jsonr....).r&..
+00000ea0: 0072 3300 0000 7234 0000 0072 0800 0000  .r3...r4...r....
+00000eb0: 7242 0000 005a 0a61 6464 696e 666f 7572  rB...Z.addinfour
+00000ec0: 6c72 3500 0000 721f 0000 0072 3900 0000  lr5...r....r9...
+00000ed0: 7243 0000 0072 0b00 0000 720c 0000 0072  rC...r....r....r
+00000ee0: 2800 0000 7236 0000 0072 3800 0000 da04  (...r6...r8.....
+00000ef0: 6c69 7374 7211 0000 00da 0464 6963 7472  listr......dictr
+00000f00: 4700 0000 723a 0000 0072 1300 0000 7213  G...r:...r....r.
+00000f10: 0000 0072 2100 0000 7214 0000 0072 4000  ...r!...r....r@.
 00000f20: 0000 5900 0000 7310 0000 000a 000c 011a  ..Y...s.........
-00000f30: 0202 0414 0102 0312 0126 0672 4200 0000  .........&.rB...
+00000f30: 0202 0414 0102 0312 0126 0672 4000 0000  .........&.r@...
 00000f40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000f50: 000c 0000 0040 0000 0073 cc00 0000 6500  .....@...s....e.
 00000f60: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
 00000f70: 6503 6504 6402 3c00 6505 6504 6403 3c00  e.e.d.<.e.e.d.<.
 00000f80: 6506 6504 6404 3c00 6405 5a07 6508 6a09  e.e.d.<.d.Z.e.j.
 00000f90: 6504 6406 3c00 0907 0905 0905 0905 6413  e.d.<.........d.
 00000fa0: 6401 6503 6402 6503 6403 6508 6a0a 6505  d.e.d.e.d.e.j.e.
@@ -262,84 +262,84 @@
 00001050: 0a72 6574 7279 5f77 6169 744e da04 6461  .retry_waitN..da
 00001060: 7461 da03 4745 5463 0600 0000 0000 0000  ta..GETc........
 00001070: 0000 0000 0600 0000 0200 0000 4300 0000  ............C...
 00001080: 7340 0000 007c 017c 005f 007c 027c 005f  s@...|.|._.|.|._
 00001090: 017c 0364 0075 0172 0c7c 036e 0169 007c  .|.d.u.r.|.n.i.|
 000010a0: 005f 027c 047c 005f 037c 0564 0075 0172  ._.|.|._.|.d.u.r
 000010b0: 1b7c 057c 005f 0564 0053 0074 047c 005f  .|.|._.d.S.t.|._
-000010c0: 0564 0053 0072 1f00 0000 2906 724d 0000  .d.S.r....).rM..
-000010d0: 0072 4e00 0000 724f 0000 0072 5100 0000  .rN...rO...rQ...
-000010e0: 7219 0000 0072 5000 0000 2906 7222 0000  r....rP...).r"..
-000010f0: 0072 4d00 0000 724e 0000 0072 4f00 0000  .rM...rN...rO...
-00001100: 7251 0000 0072 5000 0000 7215 0000 0072  rQ...rP...r....r
-00001110: 1500 0000 7216 0000 0072 2100 0000 7e00  ....r....r!...~.
+000010c0: 0564 0053 0072 1d00 0000 2906 724b 0000  .d.S.r....).rK..
+000010d0: 0072 4c00 0000 724d 0000 0072 4f00 0000  .rL...rM...rO...
+000010e0: 7217 0000 0072 4e00 0000 2906 7220 0000  r....rN...).r ..
+000010f0: 0072 4b00 0000 724c 0000 0072 4d00 0000  .rK...rL...rM...
+00001100: 724f 0000 0072 4e00 0000 7213 0000 0072  rO...rN...r....r
+00001110: 1300 0000 7214 0000 0072 1f00 0000 7e00  ....r....r....~.
 00001120: 0000 730a 0000 0006 0806 0112 0106 011c  ..s.............
 00001130: 017a 1448 7474 7052 6571 7565 7374 2e5f  .z.HttpRequest._
 00001140: 5f69 6e69 745f 5f72 0600 0000 6301 0000  _init__r....c...
 00001150: 0000 0000 0000 0000 0001 0000 0009 0000  ................
 00001160: 0043 0000 0073 2600 0000 6401 7c00 6a00  .C...s&...d.|.j.
 00001170: 9b00 6402 7c00 6a01 9b00 6403 7c00 6a02  ..d.|.j...d.|.j.
 00001180: 9b00 6404 7c00 6a03 9b00 6405 9d09 5300  ..d.|.j...d...S.
 00001190: 2906 4e7a 1048 7474 7052 6571 7565 7374  ).Nz.HttpRequest
 000011a0: 2875 726c 3d7a 092c 206d 6574 686f 643d  (url=z., method=
 000011b0: 7a0a 2c20 6865 6164 6572 733d 7a07 2c20  z., headers=z., 
-000011c0: 6461 7461 3d72 2700 0000 2904 724d 0000  data=r'...).rM..
-000011d0: 0072 4e00 0000 724f 0000 0072 5100 0000  .rN...rO...rQ...
-000011e0: 722b 0000 0072 1500 0000 7215 0000 0072  r+...r....r....r
-000011f0: 1600 0000 722c 0000 008c 0000 0073 0200  ....r,.......s..
+000011c0: 6461 7461 3d72 2500 0000 2904 724b 0000  data=r%...).rK..
+000011d0: 0072 4c00 0000 724d 0000 0072 4f00 0000  .rL...rM...rO...
+000011e0: 7229 0000 0072 1300 0000 7213 0000 0072  r)...r....r....r
+000011f0: 1400 0000 722a 0000 008c 0000 0073 0200  ....r*.......s..
 00001200: 0000 2601 7a14 4874 7470 5265 7175 6573  ..&.z.HttpReques
 00001210: 742e 5f5f 7265 7072 5f5f 6301 0000 0000  t.__repr__c.....
 00001220: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
 00001230: 0000 0073 4a00 0000 7c00 6a00 6400 7500  ...sJ...|.j.d.u.
 00001240: 7207 6400 5300 7401 7c00 6a00 7402 8302  r.d.S.t.|.j.t...
 00001250: 7210 7c00 6a00 5300 7401 7c00 6a00 7403  r.|.j.S.t.|.j.t.
 00001260: 8302 721c 7c00 6a00 a004 6401 a101 5300  ..r.|.j...d...S.
 00001270: 7405 a006 7c00 6a00 a101 a004 6401 a101  t...|.j.....d...
-00001280: 5300 722e 0000 0029 0772 5100 0000 7207  S.r....).rQ...r.
-00001290: 0000 00da 0562 7974 6573 7213 0000 00da  .....bytesr.....
-000012a0: 0665 6e63 6f64 6572 3100 0000 da05 6475  .encoder1.....du
-000012b0: 6d70 7372 2b00 0000 7215 0000 0072 1500  mpsr+...r....r..
-000012c0: 0000 7216 0000 00da 0462 6f64 798f 0000  ..r......body...
+00001280: 5300 722c 0000 0029 0772 4f00 0000 7207  S.r,...).rO...r.
+00001290: 0000 00da 0562 7974 6573 7211 0000 00da  .....bytesr.....
+000012a0: 0665 6e63 6f64 6572 2f00 0000 da05 6475  .encoder/.....du
+000012b0: 6d70 7372 2900 0000 7213 0000 0072 1300  mpsr)...r....r..
+000012c0: 0000 7214 0000 00da 0462 6f64 798f 0000  ..r......body...
 000012d0: 0073 0e00 0000 0a02 0401 0c02 0601 0c02  .s..............
 000012e0: 0c01 1202 7a10 4874 7470 5265 7175 6573  ....z.HttpReques
 000012f0: 742e 626f 6479 6301 0000 0000 0000 0000  t.bodyc.........
 00001300: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
 00001310: 2400 0000 7400 6a01 a002 7c00 6a03 a101  $...t.j...|.j...
 00001320: 7d01 7c01 6a04 6400 7501 720f 7c01 6a04  }.|.j.d.u.r.|.j.
-00001330: 5300 7c01 6a05 5300 721f 0000 0029 0672  S.|.j.S.r....).r
+00001330: 5300 7c01 6a05 5300 721d 0000 0029 0672  S.|.j.S.r....).r
 00001340: 0800 0000 da05 7061 7273 65da 0875 726c  ......parse..url
-00001350: 7061 7273 6572 4d00 0000 da08 686f 7374  parserM.....host
-00001360: 6e61 6d65 da06 6e65 746c 6f63 2902 7222  name..netloc).r"
+00001350: 7061 7273 6572 4b00 0000 da08 686f 7374  parserK.....host
+00001360: 6e61 6d65 da06 6e65 746c 6f63 2902 7220  name..netloc).r 
 00001370: 0000 005a 0a70 6172 7365 645f 7572 6c72  ...Z.parsed_urlr
-00001380: 1500 0000 7215 0000 0072 1600 0000 7259  ....r....r....rY
+00001380: 1300 0000 7213 0000 0072 1400 0000 7257  ....r....r....rW
 00001390: 0000 009c 0000 0073 0c00 0000 0e02 0a03  .......s........
 000013a0: 04ff 02ff 0403 02fd 7a14 4874 7470 5265  ........z.HttpRe
 000013b0: 7175 6573 742e 686f 7374 6e61 6d65 6302  quest.hostnamec.
 000013c0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
 000013d0: 0000 0043 0000 0073 1000 0000 7c00 6a00  ...C...s....|.j.
-000013e0: a001 7c01 a101 0100 6400 5300 721f 0000  ..|.....d.S.r...
-000013f0: 0029 0272 4f00 0000 da06 7570 6461 7465  .).rO.....update
-00001400: 2902 7222 0000 0072 4f00 0000 7215 0000  ).r"...rO...r...
-00001410: 0072 1500 0000 7216 0000 00da 0e61 7070  .r....r......app
+000013e0: a001 7c01 a101 0100 6400 5300 721d 0000  ..|.....d.S.r...
+000013f0: 0029 0272 4d00 0000 da06 7570 6461 7465  .).rM.....update
+00001400: 2902 7220 0000 0072 4d00 0000 7213 0000  ).r ...rM...r...
+00001410: 0072 1300 0000 7214 0000 00da 0e61 7070  .r....r......app
 00001420: 656e 645f 6865 6164 6572 73a5 0000 0073  end_headers....s
 00001430: 0200 0000 1001 7a1a 4874 7470 5265 7175  ......z.HttpRequ
 00001440: 6573 742e 6170 7065 6e64 5f68 6561 6465  est.append_heade
-00001450: 7273 2904 7252 0000 004e 4e4e 2912 7228  rs).rR...NNN).r(
-00001460: 0000 0072 3500 0000 7236 0000 0072 1300  ...r5...r6...r..
-00001470: 0000 7237 0000 0072 4b00 0000 da0b 5265  ..r7...rK.....Re
-00001480: 7472 7957 6169 7446 6e72 5100 0000 7238  tryWaitFnrQ...r8
-00001490: 0000 0072 3900 0000 723a 0000 0072 2100  ...r9...r:...r!.
-000014a0: 0000 722c 0000 0072 3b00 0000 7253 0000  ..r,...r;...rS..
-000014b0: 0072 5600 0000 7259 0000 0072 5c00 0000  .rV...rY...r\...
-000014c0: 7215 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-000014d0: 1600 0000 724c 0000 0077 0000 0073 3600  ....rL...w...s6.
+00001450: 7273 2904 7250 0000 004e 4e4e 2912 7226  rs).rP...NNN).r&
+00001460: 0000 0072 3300 0000 7234 0000 0072 1100  ...r3...r4...r..
+00001470: 0000 7235 0000 0072 4900 0000 da0b 5265  ..r5...rI.....Re
+00001480: 7472 7957 6169 7446 6e72 4f00 0000 7236  tryWaitFnrO...r6
+00001490: 0000 0072 3700 0000 7238 0000 0072 1f00  ...r7...r8...r..
+000014a0: 0000 722a 0000 0072 3900 0000 7251 0000  ..r*...r9...rQ..
+000014b0: 0072 5400 0000 7257 0000 0072 5a00 0000  .rT...rW...rZ...
+000014c0: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+000014d0: 1400 0000 724a 0000 0077 0000 0073 3600  ....rJ...w...s6.
 000014e0: 0000 0a00 0801 0801 0801 0801 0e01 0205  ................
 000014f0: 0201 0201 0201 04fa 0202 02fe 0203 02fd  ................
 00001500: 1004 02fc 0405 02fb 0806 0afa 0e0e 0203  ................
-00001510: 1601 020c 1001 1e08 724c 0000 0063 0000  ........rL...c..
+00001510: 1601 020c 1001 1e08 724a 0000 0063 0000  ........rJ...c..
 00001520: 0000 0000 0000 0000 0000 0000 0000 0900  ................
 00001530: 0000 4000 0000 7372 0100 0065 005a 0164  ..@...sr...e.Z.d
 00001540: 005a 0255 0065 0365 0465 0466 0219 0065  .Z.U.e.e.e.f...e
 00001550: 0564 013c 0065 066a 0765 0819 0065 0564  .d.<.e.j.e...e.d
 00001560: 023c 0065 066a 0765 0419 0065 0564 033c  .<.e.j.e...e.d.<
 00001570: 0009 0409 0409 0464 2564 0565 066a 0765  .......d%d.e.j.e
 00001580: 0365 0465 0466 0219 0019 0064 0665 066a  .e.e.f.....d.e.j
@@ -370,84 +370,84 @@
 00001710: 4eda 0c62 6173 655f 6865 6164 6572 73da  N..base_headers.
 00001720: 1064 6566 6175 6c74 5f65 6e64 706f 696e  .default_endpoin
 00001730: 74da 0c64 6566 6175 6c74 5f61 7574 6863  t..default_authc
 00001740: 0400 0000 0000 0000 0000 0000 0400 0000  ................
 00001750: 0200 0000 4300 0000 7322 0000 007c 0164  ....C...s"...|.d
 00001760: 0075 0172 067c 016e 0169 007c 005f 007c  .u.r.|.n.i.|._.|
 00001770: 037c 005f 017c 027c 005f 0264 0053 0072  .|._.|.|._.d.S.r
-00001780: 1f00 0000 2903 725f 0000 0072 6000 0000  ....).r_...r`...
-00001790: 7261 0000 0029 0472 2200 0000 7262 0000  ra...).r"...rb..
-000017a0: 0072 6300 0000 7264 0000 0072 1500 0000  .rc...rd...r....
-000017b0: 7215 0000 0072 1600 0000 7221 0000 00b1  r....r....r!....
+00001780: 1d00 0000 2903 725d 0000 0072 5e00 0000  ....).r]...r^...
+00001790: 725f 0000 0029 0472 2000 0000 7260 0000  r_...).r ...r`..
+000017a0: 0072 6100 0000 7262 0000 0072 1300 0000  .ra...rb...r....
+000017b0: 7213 0000 0072 1400 0000 721f 0000 00b1  r....r....r.....
 000017c0: 0000 0073 0600 0000 1206 0601 0a01 7a13  ...s..........z.
 000017d0: 4874 7470 436c 6965 6e74 2e5f 5f69 6e69  HttpClient.__ini
-000017e0: 745f 5f72 5100 0000 724f 0000 0072 0600  t__rQ...rO...r..
+000017e0: 745f 5f72 4f00 0000 724d 0000 0072 0600  t__rO...rM...r..
 000017f0: 0000 6304 0000 0000 0000 0000 0000 0005  ..c.............
 00001800: 0000 0006 0000 0043 0000 00f3 1a00 0000  .......C........
 00001810: 7400 7c01 6401 7c02 7c03 6402 8d04 7d04  t.|.d.|.|.d...}.
 00001820: 7c00 a001 7c04 a101 5300 2903 4e5a 0644  |...|...S.).NZ.D
-00001830: 454c 4554 45a9 0472 4d00 0000 724e 0000  ELETE..rM...rN..
-00001840: 0072 5100 0000 724f 0000 00a9 0272 4c00  .rQ...rO.....rL.
+00001830: 454c 4554 45a9 0472 4b00 0000 724c 0000  ELETE..rK...rL..
+00001840: 0072 4f00 0000 724d 0000 00a9 0272 4a00  .rO...rM.....rJ.
 00001850: 0000 da14 5f48 7474 7043 6c69 656e 745f  ...._HttpClient_
-00001860: 5f72 6571 7565 7374 a905 7222 0000 0072  _request..r"...r
-00001870: 4d00 0000 7251 0000 0072 4f00 0000 da07  M...rQ...rO.....
-00001880: 7265 7175 6573 7472 1500 0000 7215 0000  requestr....r...
-00001890: 0072 1600 0000 da06 6465 6c65 7465 bb00  .r......delete..
+00001860: 5f72 6571 7565 7374 a905 7220 0000 0072  _request..r ...r
+00001870: 4b00 0000 724f 0000 0072 4d00 0000 da07  K...rO...rM.....
+00001880: 7265 7175 6573 7472 1300 0000 7213 0000  requestr....r...
+00001890: 0072 1400 0000 da06 6465 6c65 7465 bb00  .r......delete..
 000018a0: 0000 f304 0000 0010 030a 017a 1148 7474  ...........z.Htt
-000018b0: 7043 6c69 656e 742e 6465 6c65 7465 724d  pClient.deleterM
-000018c0: 0000 0072 5000 0000 6304 0000 0000 0000  ...rP...c.......
+000018b0: 7043 6c69 656e 742e 6465 6c65 7465 724b  pClient.deleterK
+000018c0: 0000 0072 4e00 0000 6304 0000 0000 0000  ...rN...c.......
 000018d0: 0000 0000 0005 0000 0006 0000 0043 0000  .............C..
-000018e0: 0072 6500 0000 2903 4e72 5200 0000 2904  .re...).NrR...).
-000018f0: 724d 0000 0072 4e00 0000 724f 0000 0072  rM...rN...rO...r
-00001900: 5000 0000 7267 0000 0029 0572 2200 0000  P...rg...).r"...
-00001910: 724d 0000 0072 4f00 0000 7250 0000 0072  rM...rO...rP...r
-00001920: 6a00 0000 7215 0000 0072 1500 0000 7216  j...r....r....r.
+000018e0: 0072 6300 0000 2903 4e72 5000 0000 2904  .rc...).NrP...).
+000018f0: 724b 0000 0072 4c00 0000 724d 0000 0072  rK...rL...rM...r
+00001900: 4e00 0000 7265 0000 0029 0572 2000 0000  N...re...).r ...
+00001910: 724b 0000 0072 4d00 0000 724e 0000 0072  rK...rM...rN...r
+00001920: 6800 0000 7213 0000 0072 1300 0000 7214  h...r....r....r.
 00001930: 0000 00da 0367 6574 c100 0000 7308 0000  .....get....s...
 00001940: 0002 0608 0106 ff0a 037a 0e48 7474 7043  .........z.HttpC
 00001950: 6c69 656e 742e 6765 7463 0400 0000 0000  lient.getc......
 00001960: 0000 0000 0000 0500 0000 0600 0000 4300  ..............C.
-00001970: 0000 7265 0000 0029 034e 5a04 504f 5354  ..re...).NZ.POST
-00001980: 7266 0000 0072 6700 0000 7269 0000 0072  rf...rg...ri...r
-00001990: 1500 0000 7215 0000 0072 1600 0000 da04  ....r....r......
-000019a0: 706f 7374 cc00 0000 726c 0000 007a 0f48  post....rl...z.H
+00001970: 0000 7263 0000 0029 034e 5a04 504f 5354  ..rc...).NZ.POST
+00001980: 7264 0000 0072 6500 0000 7267 0000 0072  rd...re...rg...r
+00001990: 1300 0000 7213 0000 0072 1400 0000 da04  ....r....r......
+000019a0: 706f 7374 cc00 0000 726a 0000 007a 0f48  post....rj...z.H
 000019b0: 7474 7043 6c69 656e 742e 706f 7374 6304  ttpClient.postc.
 000019c0: 0000 0000 0000 0000 0000 0005 0000 0006  ................
-000019d0: 0000 0043 0000 0072 6500 0000 2903 4e5a  ...C...re...).NZ
-000019e0: 0550 4154 4348 7266 0000 0072 6700 0000  .PATCHrf...rg...
-000019f0: 7269 0000 0072 1500 0000 7215 0000 0072  ri...r....r....r
-00001a00: 1600 0000 da05 7061 7463 68d2 0000 0072  ......patch....r
-00001a10: 6c00 0000 7a10 4874 7470 436c 6965 6e74  l...z.HttpClient
+000019d0: 0000 0043 0000 0072 6300 0000 2903 4e5a  ...C...rc...).NZ
+000019e0: 0550 4154 4348 7264 0000 0072 6500 0000  .PATCHrd...re...
+000019f0: 7267 0000 0072 1300 0000 7213 0000 0072  rg...r....r....r
+00001a00: 1400 0000 da05 7061 7463 68d2 0000 0072  ......patch....r
+00001a10: 6a00 0000 7a10 4874 7470 436c 6965 6e74  j...z.HttpClient
 00001a20: 2e70 6174 6368 6304 0000 0000 0000 0000  .patchc.........
 00001a30: 0000 0005 0000 0006 0000 0043 0000 0072  ...........C...r
-00001a40: 6500 0000 2903 4eda 0350 5554 7266 0000  e...).N..PUTrf..
-00001a50: 0072 6700 0000 7269 0000 0072 1500 0000  .rg...ri...r....
-00001a60: 7215 0000 0072 1600 0000 da03 7075 74d8  r....r......put.
-00001a70: 0000 0072 6c00 0000 7a0e 4874 7470 436c  ...rl...z.HttpCl
+00001a40: 6300 0000 2903 4eda 0350 5554 7264 0000  c...).N..PUTrd..
+00001a50: 0072 6500 0000 7267 0000 0072 1300 0000  .re...rg...r....
+00001a60: 7213 0000 0072 1400 0000 da03 7075 74d8  r....r......put.
+00001a70: 0000 0072 6a00 0000 7a0e 4874 7470 436c  ...rj...z.HttpCl
 00001a80: 6965 6e74 2e70 7574 da06 7461 7267 6574  ient.put..target
 00001a90: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
 00001aa0: 0009 0000 0043 0000 0073 9600 0000 7400  .....C...s....t.
 00001ab0: a001 6401 7c01 a102 0100 7402 7c01 6402  ..d.|.....t.|.d.
 00001ac0: 6403 8d02 7d03 7c00 a003 7c03 a101 7d04  d...}.|...|...}.
 00001ad0: 7404 7c02 6404 8302 8f2b 7d05 7c04 6a05  t.|.d....+}.|.j.
 00001ae0: 8f0f 0100 7406 a007 7c04 6a05 7c05 a102  ....t...|.j.|...
 00001af0: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
 00001b00: 3100 732c 7701 0100 0100 0100 5900 0100  1.s,w.......Y...
 00001b10: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
 00001b20: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
 00001b30: 3100 7344 7701 0100 0100 0100 5900 0100  1.sDw.......Y...
 00001b40: 6400 5300 2905 4e7a 1648 5454 502e 646f  d.S.).Nz.HTTP.do
 00001b50: 776e 6c6f 6164 5f66 696c 653a 2025 7372  wnload_file: %sr
-00001b60: 5200 0000 2902 724d 0000 0072 4e00 0000  R...).rM...rN...
+00001b60: 5000 0000 2902 724b 0000 0072 4c00 0000  P...).rK...rL...
 00001b70: da02 7762 2908 da06 6c6f 6767 6572 da05  ..wb)...logger..
-00001b80: 6465 6275 6772 4c00 0000 7268 0000 00da  debugrL...rh....
-00001b90: 046f 7065 6e72 4500 0000 da06 7368 7574  .openrE.....shut
+00001b80: 6465 6275 6772 4a00 0000 7266 0000 00da  debugrJ...rf....
+00001b90: 046f 7065 6e72 4300 0000 da06 7368 7574  .openrC.....shut
 00001ba0: 696c da0b 636f 7079 6669 6c65 6f62 6a29  il..copyfileobj)
-00001bb0: 0672 2200 0000 724d 0000 0072 7200 0000  .r"...rM...rr...
-00001bc0: 726a 0000 0072 4400 0000 da08 6f75 745f  rj...rD.....out_
-00001bd0: 6669 6c65 7215 0000 0072 1500 0000 7216  filer....r....r.
+00001bb0: 0672 2000 0000 724b 0000 0072 7000 0000  .r ...rK...rp...
+00001bc0: 7268 0000 0072 4200 0000 da08 6f75 745f  rh...rB.....out_
+00001bd0: 6669 6c65 7213 0000 0072 1300 0000 7214  filer....r....r.
 00001be0: 0000 00da 0d64 6f77 6e6c 6f61 645f 6669  .....download_fi
 00001bf0: 6c65 de00 0000 731c 0000 000c 010c 010a  le....s.........
 00001c00: 010c 0108 0110 011e ff0a ff04 0302 fe0a  ................
 00001c10: ff04 0310 fd04 037a 1848 7474 7043 6c69  .......z.HttpCli
 00001c20: 656e 742e 646f 776e 6c6f 6164 5f66 696c  ent.download_fil
 00001c30: 65da 0470 6174 6863 0200 0000 0000 0000  e..pathc........
 00001c40: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
@@ -455,17 +455,17 @@
 00001c60: 0164 0183 0182 017c 006a 009b 0064 027c  .d.....|.j...d.|
 00001c70: 019b 009d 0353 0029 034e 7a53 4874 7470  .....S.).NzSHttp
 00001c80: 436c 6965 6e74 2e75 726c 2063 616c 6c65  Client.url calle
 00001c90: 6420 666f 7220 636c 6965 6e74 2077 6974  d for client wit
 00001ca0: 6820 6e6f 2064 6566 6175 6c74 2065 6e64  h no default end
 00001cb0: 706f 696e 742e 204a 7573 7420 7061 7373  point. Just pass
 00001cc0: 2074 6865 2055 524c 2063 6c65 6172 21fa   the URL clear!.
-00001cd0: 012f 2902 7261 0000 0072 1100 0000 2902  ./).ra...r....).
-00001ce0: 7222 0000 0072 7b00 0000 7215 0000 0072  r"...r{...r....r
-00001cf0: 1500 0000 7216 0000 0072 4d00 0000 e700  ....r....rM.....
+00001cd0: 012f 2902 725f 0000 0072 0f00 0000 2902  ./).r_...r....).
+00001ce0: 7220 0000 0072 7900 0000 7213 0000 0072  r ...ry...r....r
+00001cf0: 1300 0000 7214 0000 0072 4b00 0000 e700  ....r....rK.....
 00001d00: 0000 730a 0000 000a 0102 0102 0104 ff10  ..s.............
 00001d10: 037a 0e48 7474 7043 6c69 656e 742e 7572  .z.HttpClient.ur
 00001d20: 6cda 0b72 6571 7565 7374 5f63 7478 6302  l..request_ctxc.
 00001d30: 0000 0000 0000 0000 0000 000a 0000 000a  ................
 00001d40: 0000 0043 0000 0073 5a01 0000 7c00 6a00  ...C...sZ...|.j.
 00001d50: 6400 7501 720a 7c00 a000 7c01 a101 7d01  d.u.r.|...|...}.
 00001d60: 7401 a002 6401 7c01 a102 0100 7c00 6a03  t...d.|.....|.j.
@@ -487,36 +487,36 @@
 00001e60: 7c09 6407 6b00 7293 741c 7c08 8301 6400  |.d.k.r.t.|...d.
 00001e70: 8202 7c09 6408 6b04 729c 741d 7c08 8301  ..|.d.k.r.t.|...
 00001e80: 6400 8202 741e 7c08 8301 6400 8202 6400  d...t.|...d...d.
 00001e90: 7d08 7e08 7701 0400 741f 79ac 0100 0100  }.~.w...t.y.....
 00001ea0: 0100 8200 7700 290a 4e7a 0225 73e9 0300  ....w.).Nz.%s...
 00001eb0: 0000 5429 045a 0572 6574 7279 da04 7374  ..T).Z.retry..st
 00001ec0: 6f70 da07 7265 7261 6973 65da 0477 6169  op..reraise..wai
-00001ed0: 7429 0172 4e00 0000 698f 0100 0069 f401  t).rN...i....i..
+00001ed0: 7429 0172 4c00 0000 698f 0100 0069 f401  t).rL...i....i..
 00001ee0: 0000 69f3 0100 005a 0b55 6e72 6561 6368  ..i....Z.Unreach
-00001ef0: 6162 6c65 2921 7260 0000 0072 7400 0000  able)!r`...rt...
-00001f00: 7275 0000 0072 5f00 0000 da04 636f 7079  ru...r_.....copy
-00001f10: 724f 0000 0072 5b00 0000 da08 7465 6e61  rO...r[.....tena
+00001ef0: 6162 6c65 2921 725e 0000 0072 7200 0000  able)!r^...rr...
+00001f00: 7273 0000 0072 5d00 0000 da04 636f 7079  rs...r].....copy
+00001f10: 724d 0000 0072 5900 0000 da08 7465 6e61  rM...rY.....tena
 00001f20: 6369 7479 5a08 5265 7472 7969 6e67 5a12  cityZ.RetryingZ.
 00001f30: 7265 7472 795f 6966 5f65 7863 6570 7469  retry_if_excepti
-00001f40: 6f6e 7217 0000 005a 1273 746f 705f 6166  onr....Z.stop_af
+00001f40: 6f6e 7215 0000 005a 1273 746f 705f 6166  onr....Z.stop_af
 00001f50: 7465 725f 6174 7465 6d70 74da 055f 7761  ter_attempt.._wa
-00001f60: 6974 7250 0000 0072 0800 0000 726a 0000  itrP...r....rj..
-00001f70: 005a 0752 6571 7565 7374 724d 0000 0072  .Z.RequestrM...r
-00001f80: 4e00 0000 7256 0000 0072 5100 0000 da05  N...rV...rQ.....
+00001f60: 6974 724e 0000 0072 0800 0000 7268 0000  itrN...r....rh..
+00001f70: 005a 0752 6571 7565 7374 724b 0000 0072  .Z.RequestrK...r
+00001f80: 4c00 0000 7254 0000 0072 4f00 0000 da05  L...rT...rO.....
 00001f90: 6974 656d 73da 0a61 6464 5f68 6561 6465  items..add_heade
-00001fa0: 7272 4200 0000 da07 7572 6c6f 7065 6e72  rrB.....urlopenr
-00001fb0: 0900 0000 720a 0000 0072 0e00 0000 723e  ....r....r....r>
-00001fc0: 0000 0072 4100 0000 721a 0000 00da 0945  ...rA...r......E
-00001fd0: 7863 6570 7469 6f6e 7246 0000 0029 0a72  xceptionrF...).r
-00001fe0: 2200 0000 727d 0000 0072 4f00 0000 5a07  "...r}...rO...Z.
-00001ff0: 6174 7465 6d70 7472 6a00 0000 5a08 7265  attemptrj...Z.re
+00001fa0: 7272 4000 0000 da07 7572 6c6f 7065 6e72  rr@.....urlopenr
+00001fb0: 0900 0000 720a 0000 0072 0e00 0000 723c  ....r....r....r<
+00001fc0: 0000 0072 3f00 0000 7218 0000 00da 0945  ...r?...r......E
+00001fd0: 7863 6570 7469 6f6e 7244 0000 0029 0a72  xceptionrD...).r
+00001fe0: 2000 0000 727b 0000 0072 4d00 0000 5a07   ...r{...rM...Z.
+00001ff0: 6174 7465 6d70 7472 6800 0000 5a08 7265  attemptrh...Z.re
 00002000: 715f 626f 6479 da03 6b65 79da 0576 616c  q_body..key..val
-00002010: 7565 7205 0000 0072 4700 0000 7215 0000  uer....rG...r...
-00002020: 0072 1500 0000 7216 0000 005a 095f 5f72  .r....r....Z.__r
+00002010: 7565 7205 0000 0072 4500 0000 7213 0000  uer....rE...r...
+00002020: 0072 1300 0000 7214 0000 005a 095f 5f72  .r....r....Z.__r
 00002030: 6571 7565 7374 ee00 0000 734a 0000 000a  equest....sJ....
 00002040: 010a 010c 020a 0206 010c 0102 0204 0108  ................
 00002050: 0108 0102 010a 010a fc06 0606 0108 0106  ................
 00002060: ff06 0408 0106 0110 020e 010e 0228 f402  .............(..
 00002070: fa08 1e12 f506 0110 010a 0108 010a 010a  ................
 00002080: 0208 800c 0102 0102 ff7a 1448 7474 7043  .........z.HttpC
 00002090: 6c69 656e 742e 5f5f 7265 7175 6573 74da  lient.__request.
@@ -531,73 +531,73 @@
 00002120: 840c 5a06 6405 5300 2906 7a20 4874 7470  ..Z.d.S.).z Http
 00002130: 436c 6965 6e74 2e5f 7761 6974 2e3c 6c6f  Client._wait.<lo
 00002140: 6361 6c73 3e2e 5761 6974 6572 da0b 7265  cals>.Waiter..re
 00002150: 7472 795f 7374 6174 6572 0600 0000 6302  try_stater....c.
 00002160: 0000 0000 0000 0000 0000 0003 0000 0003  ................
 00002170: 0000 0013 0000 0073 2200 0000 7c01 6a00  .......s"...|.j.
 00002180: 7d02 7c02 6400 7500 720b 8800 6400 8301  }.|.d.u.r...d...
-00002190: 5300 8800 7c02 a001 a100 8301 5300 721f  S...|.......S.r.
+00002190: 5300 8800 7c02 a001 a100 8301 5300 721d  S...|.......S.r.
 000021a0: 0000 0029 02da 076f 7574 636f 6d65 da09  ...)...outcome..
-000021b0: 6578 6365 7074 696f 6e29 0372 2200 0000  exception).r"...
-000021c0: 728c 0000 0072 8d00 0000 a901 728b 0000  r....r......r...
-000021d0: 0072 1500 0000 7216 0000 00da 085f 5f63  .r....r......__c
+000021b0: 6578 6365 7074 696f 6e29 0372 2000 0000  exception).r ...
+000021c0: 728a 0000 0072 8b00 0000 a901 7289 0000  r....r......r...
+000021d0: 0072 1300 0000 7214 0000 00da 085f 5f63  .r....r......__c
 000021e0: 616c 6c5f 5f1b 0100 0073 0800 0000 0601  all__....s......
 000021f0: 0801 0801 0c01 7a29 4874 7470 436c 6965  ......z)HttpClie
 00002200: 6e74 2e5f 7761 6974 2e3c 6c6f 6361 6c73  nt._wait.<locals
 00002210: 3e2e 5761 6974 6572 2e5f 5f63 616c 6c5f  >.Waiter.__call_
-00002220: 5f4e 2907 7228 0000 0072 3500 0000 7236  _N).r(...r5...r6
-00002230: 0000 0072 8300 0000 5a0e 5265 7472 7943  ...r....Z.RetryC
+00002220: 5f4e 2907 7226 0000 0072 3300 0000 7234  _N).r&...r3...r4
+00002230: 0000 0072 8100 0000 5a0e 5265 7472 7943  ...r....Z.RetryC
 00002240: 616c 6c53 7461 7465 da05 666c 6f61 7472  allState..floatr
-00002250: 9000 0000 7215 0000 0072 8f00 0000 7215  ....r....r....r.
-00002260: 0000 0072 1600 0000 da06 5761 6974 6572  ...r......Waiter
-00002270: 1a01 0000 7304 0000 0008 001c 0172 9200  ....s........r..
-00002280: 0000 2903 7283 0000 0072 8100 0000 da09  ..).r....r......
-00002290: 7761 6974 5f62 6173 6529 0372 2200 0000  wait_base).r"...
-000022a0: 728b 0000 0072 9200 0000 7215 0000 0072  r....r....r....r
-000022b0: 8f00 0000 7216 0000 0072 8400 0000 1901  ....r....r......
+00002250: 8e00 0000 7213 0000 0072 8d00 0000 7213  ....r....r....r.
+00002260: 0000 0072 1400 0000 da06 5761 6974 6572  ...r......Waiter
+00002270: 1a01 0000 7304 0000 0008 001c 0172 9000  ....s........r..
+00002280: 0000 2903 7281 0000 0072 7f00 0000 da09  ..).r....r......
+00002290: 7761 6974 5f62 6173 6529 0372 2000 0000  wait_base).r ...
+000022a0: 7289 0000 0072 9000 0000 7213 0000 0072  r....r....r....r
+000022b0: 8d00 0000 7214 0000 0072 8200 0000 1901  ....r....r......
 000022c0: 0000 7304 0000 0018 0106 077a 1048 7474  ..s........z.Htt
 000022d0: 7043 6c69 656e 742e 5f77 6169 7429 034e  pClient._wait).N
-000022e0: 4e4e 2902 4e4e 291d 7228 0000 0072 3500  NN).NN).r(...r5.
-000022f0: 0000 7236 0000 0072 4b00 0000 7213 0000  ..r6...rK...r...
-00002300: 0072 3700 0000 7238 0000 0072 3a00 0000  .r7...r8...r:...
+000022e0: 4e4e 2902 4e4e 291d 7226 0000 0072 3300  NN).NN).r&...r3.
+000022f0: 0000 7234 0000 0072 4900 0000 7211 0000  ..r4...rI...r...
+00002300: 0072 3500 0000 7236 0000 0072 3800 0000  .r5...r6...r8...
 00002310: da14 4874 7470 5265 7175 6573 7444 6563  ..HttpRequestDec
-00002320: 6f72 6174 6f72 7221 0000 0072 3900 0000  oratorr!...r9...
-00002330: 7242 0000 0072 6b00 0000 7219 0000 0072  rB...rk...r....r
-00002340: 5d00 0000 726d 0000 0072 6e00 0000 726f  ]...rm...rn...ro
-00002350: 0000 0072 7100 0000 da07 7061 7468 6c69  ...rq.....pathli
-00002360: 62da 0450 6174 6872 7a00 0000 724d 0000  b..Pathrz...rM..
-00002370: 0072 4c00 0000 7268 0000 0072 8300 0000  .rL...rh...r....
-00002380: 7281 0000 0072 9300 0000 7284 0000 0072  r....r....r....r
-00002390: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-000023a0: 0000 0072 5e00 0000 ac00 0000 737a 0000  ...r^.......sz..
+00002320: 6f72 6174 6f72 721f 0000 0072 3700 0000  oratorr....r7...
+00002330: 7240 0000 0072 6900 0000 7217 0000 0072  r@...ri...r....r
+00002340: 5b00 0000 726b 0000 0072 6c00 0000 726d  [...rk...rl...rm
+00002350: 0000 0072 6f00 0000 da07 7061 7468 6c69  ...ro.....pathli
+00002360: 62da 0450 6174 6872 7800 0000 724b 0000  b..Pathrx...rK..
+00002370: 0072 4a00 0000 7266 0000 0072 8100 0000  .rJ...rf...r....
+00002380: 727f 0000 0072 9100 0000 7282 0000 0072  r....r....r....r
+00002390: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
+000023a0: 0000 0072 5c00 0000 ac00 0000 737a 0000  ...r\.......sz..
 000023b0: 000a 0010 010e 010e 0102 0402 0102 0104  ................
 000023c0: fc10 0202 fe08 0302 fd08 040a fc02 0b04  ................
 000023d0: ff04 0102 ff08 0102 ff02 020a fe02 0902  ................
 000023e0: 0104 fc02 0202 fe08 0302 fd02 0402 fc02  ................
 000023f0: 050a fb02 0c04 ff04 0102 ff08 0102 ff02  ................
 00002400: 020a fe02 0704 ff04 0102 ff08 0102 ff02  ................
 00002410: 020a fe02 0704 ff04 0102 ff08 0102 ff02  ................
-00002420: 020a fe18 0612 0912 071a 2b72 5e00 0000  ..........+r^...
-00002430: 2925 720b 0000 0072 3100 0000 da07 6c6f  )%r....r1.....lo
-00002440: 6767 696e 6772 9500 0000 7277 0000 0072  ggingr....rw...r
-00002450: 3800 0000 5a0c 7572 6c6c 6962 2e65 7272  8...Z.urllib.err
+00002420: 020a fe18 0612 0912 071a 2b72 5c00 0000  ..........+r\...
+00002430: 2925 720b 0000 0072 2f00 0000 da07 6c6f  )%r....r/.....lo
+00002440: 6767 696e 6772 9300 0000 7275 0000 0072  ggingr....ru...r
+00002450: 3600 0000 5a0c 7572 6c6c 6962 2e65 7272  6...Z.urllib.err
 00002460: 6f72 7208 0000 00da 0c75 726c 6c69 622e  orr......urllib.
 00002470: 7061 7273 65da 0e75 726c 6c69 622e 7265  parse..urllib.re
 00002480: 7175 6573 745a 0f75 726c 6c69 622e 7265  questZ.urllib.re
-00002490: 7370 6f6e 7365 7283 0000 005a 0d74 656e  sponser....Z.ten
+00002490: 7370 6f6e 7365 7281 0000 005a 0d74 656e  sponser....Z.ten
 000024a0: 6163 6974 792e 7761 6974 7203 0000 00da  acity.waitr.....
 000024b0: 0573 6572 6465 7204 0000 00da 0967 6574  .serder......get
-000024c0: 4c6f 6767 6572 7274 0000 00da 066f 626a  Loggerrt.....obj
+000024c0: 4c6f 6767 6572 7272 0000 00da 066f 626a  Loggerrr.....obj
 000024d0: 6563 745a 0f44 4546 4155 4c54 5f48 4541  ectZ.DEFAULT_HEA
-000024e0: 4445 5253 7239 0000 00da 0462 6f6f 6c72  DERSr9.....boolr
-000024f0: 1700 0000 723a 0000 00da 0d42 6173 6545  ....r:.....BaseE
-00002500: 7863 6570 7469 6f6e 7291 0000 0072 1900  xceptionr....r..
-00002510: 0000 7288 0000 0072 1a00 0000 723e 0000  ..r....r....r>..
-00002520: 0072 4100 0000 7242 0000 00da 0843 616c  .rA...rB.....Cal
-00002530: 6c61 626c 6572 5d00 0000 724c 0000 0072  labler]...rL...r
-00002540: 9400 0000 725e 0000 0072 1500 0000 7215  ....r^...r....r.
-00002550: 0000 0072 1500 0000 7216 0000 00da 083c  ...r....r......<
+000024e0: 4445 5253 7237 0000 00da 0462 6f6f 6c72  DERSr7.....boolr
+000024f0: 1500 0000 7238 0000 00da 0d42 6173 6545  ....r8.....BaseE
+00002500: 7863 6570 7469 6f6e 728f 0000 0072 1700  xceptionr....r..
+00002510: 0000 7286 0000 0072 1800 0000 723c 0000  ..r....r....r<..
+00002520: 0072 3f00 0000 7240 0000 00da 0843 616c  .r?...r@.....Cal
+00002530: 6c61 626c 6572 5b00 0000 724a 0000 0072  labler[...rJ...r
+00002540: 9200 0000 725c 0000 0072 1300 0000 7213  ....r\...r....r.
+00002550: 0000 0072 1300 0000 7214 0000 00da 083c  ...r....r......<
 00002560: 6d6f 6475 6c65 3e01 0000 0073 3400 0000  module>....s4...
 00002570: 0800 0801 0801 0801 0801 0801 0801 0801  ................
 00002580: 0801 0801 0802 0801 0c02 0c01 0a02 0602  ................
 00002590: 1403 1813 1004 1023 1004 0e04 161b 0e03  .......#........
 000025a0: 1032 1203                                .2..
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 3161 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 590c 0000  o........F.dY...
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 590c 0000  o.......Ms.dY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
@@ -33,16 +33,16 @@
 00000200: 7574 6844 6563 6f72 6174 6f72 5f5f 7573  uthDecorator__us
 00000210: 6572 5f69 64da 0775 7365 725f 6964 6302  er_id..user_idc.
 00000220: 0000 0000 0000 0000 0000 0002 0000 0002  ................
 00000230: 0000 0043 0000 00f3 0a00 0000 7c01 7c00  ...C........|.|.
 00000240: 5f00 6400 5300 a901 4e29 0172 0e00 0000  _.d.S...N).r....
 00000250: 2902 da04 7365 6c66 720f 0000 00a9 0072  )...selfr......r
 00000260: 1300 0000 faef 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000270: 2f6f 7574 7075 742f 7372 6334 3039 3837  /output/src40987
-00000280: 3536 3136 392f 7372 632f 636f 6465 7374  56169/src/codest
+00000270: 2f6f 7574 7075 742f 7372 6333 3439 3732  /output/src34972
+00000280: 3638 3637 302f 7372 632f 636f 6465 7374  68670/src/codest
 00000290: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 000002a0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000002b0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000002c0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000002d0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000002e0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000002f0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 1004 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 ec03 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 ec03 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6402 6403 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 4700 6404 6405 8400 6405 8302 5a08  ..G.d.d...d...Z.
 00000070: 6401 5300 2906 e900 0000 004e e901 0000  d.S.)......N....
@@ -36,16 +36,16 @@
 00000230: 5f00 7c04 7007 7401 8300 7c00 5f02 7c02  _.|.p.t...|._.|.
 00000240: 7c00 5f03 7c01 7c00 5f04 6400 5300 a901  |._.|.|._.d.S...
 00000250: 4e29 0572 0700 0000 da04 6469 6374 7205  N).r......dictr.
 00000260: 0000 0072 0600 0000 7208 0000 0029 05da  ...r....r....)..
 00000270: 0473 656c 6672 0a00 0000 720b 0000 0072  .selfr....r....r
 00000280: 0c00 0000 720d 0000 00a9 0072 1200 0000  ....r......r....
 00000290: fae9 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-000002a0: 7075 742f 7372 6334 3039 3837 3536 3136  put/src409875616
-000002b0: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+000002a0: 7075 742f 7372 6333 3439 3732 3638 3637  put/src349726867
+000002b0: 302f 7372 632f 636f 6465 7374 6172 2d63  0/src/codestar-c
 000002c0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 000002d0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 000002e0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 000002f0: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 00000300: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 00000310: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000320: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/http/http_client.py` & `roboto_sdk-0.1.5/src/roboto_sdk/http/http_client.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/http/request_decorators.py` & `roboto_sdk-0.1.5/src/roboto_sdk/http/request_decorators.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/http/testing_util.py` & `roboto_sdk-0.1.5/src/roboto_sdk/http/testing_util.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc` & `roboto_sdk-0.1.5/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 22:07:17 2023 UTC, .py size: 2977 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9546 a364 a10b 0000  o........F.d....
+00000000: 6f0d 0d0a 0000 0000 4d73 a364 a10b 0000  o.......Ms.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 6d06 5a06 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6401 6c07 5a07 6403 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6509 8300 5a0a 6405 5a0b 6406 5a0c  ..e...Z.d.Z.d.Z.
@@ -35,16 +35,16 @@
 00000220: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 00000230: 5f5f da03 7374 72da 0f5f 5f61 6e6e 6f74  __..str..__annot
 00000240: 6174 696f 6e73 5f5f da0d 5052 4f44 5f45  ations__..PROD_E
 00000250: 4e44 504f 494e 5472 0a00 0000 da18 5052  NDPOINTr......PR
 00000260: 4f44 5f55 5345 525f 504f 4f4c 5f43 4c49  OD_USER_POOL_CLI
 00000270: 454e 545f 4944 720b 0000 00a9 0072 1300  ENT_IDr......r..
 00000280: 0000 7213 0000 00fa e72f 636f 6465 6275  ..r....../codebu
-00000290: 696c 642f 6f75 7470 7574 2f73 7263 3430  ild/output/src40
-000002a0: 3938 3735 3631 3639 2f73 7263 2f63 6f64  98756169/src/cod
+00000290: 696c 642f 6f75 7470 7574 2f73 7263 3334  ild/output/src34
+000002a0: 3937 3236 3836 3730 2f73 7263 2f63 6f64  97268670/src/cod
 000002b0: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 000002c0: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 000002d0: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 000002e0: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 000002f0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 00000300: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 00000310: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/profile/profile.py` & `roboto_sdk-0.1.5/src/roboto_sdk/profile/profile.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/src/roboto_sdk/serde.py` & `roboto_sdk-0.1.5/src/roboto_sdk/serde.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.4/PKG-INFO` & `roboto_sdk-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools for interacting with roboto.ai
 License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

