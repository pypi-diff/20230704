# Comparing `tmp/infrahouse-toolkit-1.2.0.tar.gz` & `tmp/infrahouse-toolkit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrahouse-toolkit-1.2.0.tar", last modified: Sun Feb 26 18:14:07 2023, max compression
+gzip compressed data, was "infrahouse-toolkit-1.3.0.tar", last modified: Tue Jul  4 21:23:12 2023, max compression
```

## Comparing `infrahouse-toolkit-1.2.0.tar` & `infrahouse-toolkit-1.3.0.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.066698 infrahouse-toolkit-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-02-26 18:14:07.066698 infrahouse-toolkit-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.cli.ih_plan.rst
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.cli.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.backends.rst
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.backends.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.tests.status.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_download/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/tests/test_get_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/s3backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.066698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.066698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tests/s3backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tfbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/githubpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.066698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.066698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/github_pr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.066698 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 18:14:07.062698 infrahouse-toolkit-1.2.0/infrahouse_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-02-26 18:14:07.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-26 18:14:07.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 18:14:07.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-26 18:14:07.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 18:14:01.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-26 18:14:07.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-26 18:14:07.000000 infrahouse-toolkit-1.2.0/infrahouse_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-02-26 18:14:07.066698 infrahouse-toolkit-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-02-26 18:13:30.000000 infrahouse-toolkit-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.460747 infrahouse-toolkit-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 21:23:12.464747 infrahouse-toolkit-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.452747 infrahouse-toolkit-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.cli.ih_plan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.cli.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.backends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.backends.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.tests.status.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.452747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.456747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.456747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.456747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_download/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.456747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.456747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.456747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.456747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/tests/test_get_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.456747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.460747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/s3backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.460747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.460747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tests/s3backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tfbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/githubpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.460747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.460747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/github_pr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.460747 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:23:12.452747 infrahouse-toolkit-1.3.0/infrahouse_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 21:23:12.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-04 21:23:12.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:23:12.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 21:23:12.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:23:05.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 21:23:12.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 21:23:12.000000 infrahouse-toolkit-1.3.0/infrahouse_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-04 21:23:12.464747 infrahouse-toolkit-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-04 21:22:29.000000 infrahouse-toolkit-1.3.0/setup.py
```

### Comparing `infrahouse-toolkit-1.2.0/CONTRIBUTING.rst` & `infrahouse-toolkit-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/LICENSE` & `infrahouse-toolkit-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/PKG-INFO` & `infrahouse-toolkit-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 1.2.0
+Version: 1.3.0
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -27,14 +27,16 @@
 .. image:: https://img.shields.io/pypi/v/infrahouse_toolkit.svg
         :target: https://pypi.python.org/pypi/infrahouse_toolkit
 
 .. image:: https://readthedocs.org/projects/infrahouse-toolkit/badge/?version=latest
         :target: https://infrahouse-toolkit.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+.. image:: https://app.codacy.com/project/badge/Grade/26f8863a19434e3fb578bfa254328e9d
+    :target: https://app.codacy.com/gh/infrahouse/infrahouse-toolkit/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
 
 A collection of tools for building infrastructure.
 
 
 * Free software: Apache Software License 2.0
 * Documentation: https://infrahouse-toolkit.readthedocs.io.
```

### Comparing `infrahouse-toolkit-1.2.0/README.rst` & `infrahouse-toolkit-1.3.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 .. image:: https://img.shields.io/pypi/v/infrahouse_toolkit.svg
         :target: https://pypi.python.org/pypi/infrahouse_toolkit
 
 .. image:: https://readthedocs.org/projects/infrahouse-toolkit/badge/?version=latest
         :target: https://infrahouse-toolkit.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+.. image:: https://app.codacy.com/project/badge/Grade/26f8863a19434e3fb578bfa254328e9d
+    :target: https://app.codacy.com/gh/infrahouse/infrahouse-toolkit/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
 
 A collection of tools for building infrastructure.
 
 
 * Free software: Apache Software License 2.0
 * Documentation: https://infrahouse-toolkit.readthedocs.io.
```

### Comparing `infrahouse-toolkit-1.2.0/docs/Makefile` & `infrahouse-toolkit-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/conf.py` & `infrahouse-toolkit-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.cli.tests.rst` & `infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.cli.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.backends.rst` & `infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.backends.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.backends.tests.rst` & `infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.backends.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst` & `infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.rst` & `infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst` & `infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.tests.rst` & `infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/infrahouse_toolkit.terraform.tests.status.rst` & `infrahouse-toolkit-1.3.0/docs/infrahouse_toolkit.terraform.tests.status.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/installation.rst` & `infrahouse-toolkit-1.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/docs/usage.rst` & `infrahouse-toolkit-1.3.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/__init__.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     A ``ih-plan download`` subcommand.
 
     See ``ih-plan download --help`` for more details.
 """
 
 from os import path as osp
 
-import boto3
 import click
 
 from infrahouse_toolkit.cli.lib import get_bucket, get_s3_client
 
 
 @click.command(name="download")
 @click.argument("key_name")
```

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .. topic:: ``ih-plan remove``
 
     A ``ih-plan remove`` subcommand.
 
     See ``ih-plan remove --help`` for more details.
 """
 
-import boto3
 import click
 
 from infrahouse_toolkit.cli.lib import get_bucket, get_s3_client
 
 
 def validate_key_name(ctx, param, value):  # pylint: disable=unused-argument
     """Check if passed value ends with a ".state"."""
```

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     A ``ih-plan upload`` subcommand.
 
     See ``ih-plan upload --help`` for more details.
 """
 
 from os import path as osp
 
-import boto3
 import click
 
 from infrahouse_toolkit.cli.lib import get_bucket, get_s3_client
 
 
 @click.command(name="upload")
 @click.option("--key-name", help="Path to the file in the S3 bucket. Default is pending/<plan_file>", default=None)
```

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/lib.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/lib.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/cli/tests/conftest.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/cli/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/__init__.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/s3backend.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/s3backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/backends/tfbackend.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/backends/tfbackend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/githubpr.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/githubpr.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/status.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/status.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/test_eq.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/test_eq.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit.egg-info/PKG-INFO` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 1.2.0
+Version: 1.3.0
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -27,14 +27,16 @@
 .. image:: https://img.shields.io/pypi/v/infrahouse_toolkit.svg
         :target: https://pypi.python.org/pypi/infrahouse_toolkit
 
 .. image:: https://readthedocs.org/projects/infrahouse-toolkit/badge/?version=latest
         :target: https://infrahouse-toolkit.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+.. image:: https://app.codacy.com/project/badge/Grade/26f8863a19434e3fb578bfa254328e9d
+    :target: https://app.codacy.com/gh/infrahouse/infrahouse-toolkit/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
 
 A collection of tools for building infrastructure.
 
 
 * Free software: Apache Software License 2.0
 * Documentation: https://infrahouse-toolkit.readthedocs.io.
```

### Comparing `infrahouse-toolkit-1.2.0/infrahouse_toolkit.egg-info/SOURCES.txt` & `infrahouse-toolkit-1.3.0/infrahouse_toolkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 docs/infrahouse_toolkit.terraform.tests.status.rst
 docs/installation.rst
 docs/modules.rst
 docs/readme.rst
 docs/usage.rst
 infrahouse_toolkit/__init__.py
 infrahouse_toolkit/exceptions.py
+infrahouse_toolkit/logging.py
 infrahouse_toolkit.egg-info/PKG-INFO
 infrahouse_toolkit.egg-info/SOURCES.txt
 infrahouse_toolkit.egg-info/dependency_links.txt
 infrahouse_toolkit.egg-info/entry_points.txt
 infrahouse_toolkit.egg-info/not-zip-safe
 infrahouse_toolkit.egg-info/requires.txt
 infrahouse_toolkit.egg-info/top_level.txt
```

### Comparing `infrahouse-toolkit-1.2.0/setup.py` & `infrahouse-toolkit-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-with open("README.rst") as readme_file:
+CODEC = "utf-8"
+
+with open("README.rst", encoding=CODEC) as readme_file:
     readme = readme_file.read()
 
-history = "See git log"
+HISTORY = "See git log"
 
 
 def parse_requirements(req_file):
     """
     Parse file with requirements and return a dictionary
     consumable by setuptools.
 
     :param req_file: path to requirements file.
     :type req_file: str
     :return: Dictionary with requirements.
     :rtype: dict
     """
-    with open(req_file) as f_descr:
+    with open(req_file, encoding=CODEC) as f_descr:
         reqs = f_descr.read().strip().split("\n")
     return [x for x in reqs if x and not x.strip().startswith("#")]
 
 
 requirements = parse_requirements("requirements.txt")
 test_requirements = parse_requirements("requirements_dev.txt")
 
@@ -46,18 +48,18 @@
     entry_points={
         "console_scripts": [
             "ih-plan=infrahouse_toolkit.cli.ih_plan:ih_plan",
         ],
     },
     install_requires=requirements,
     license="Apache Software License 2.0",
-    long_description=readme + "\n\n" + history,
+    long_description=readme + "\n\n" + HISTORY,
     include_package_data=True,
     keywords="infrahouse-toolkit",
     name="infrahouse-toolkit",
     packages=find_packages(include=["infrahouse_toolkit", "infrahouse_toolkit.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/infrahouse/infrahouse-toolkit",
-    version="1.2.0",
+    version="1.3.0",
     zip_safe=False,
 )
```

