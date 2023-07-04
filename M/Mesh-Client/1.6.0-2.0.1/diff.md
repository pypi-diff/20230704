# Comparing `tmp/Mesh Client-1.6.0.tar.gz` & `tmp/Mesh-Client-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mesh Client-1.6.0.tar", last modified: Tue Apr  4 14:56:05 2023, max compression
+gzip compressed data, was "Mesh-Client-2.0.1.tar", last modified: Tue Jul  4 19:33:03 2023, max compression
```

## Comparing `Mesh Client-1.6.0.tar` & `Mesh-Client-2.0.1.tar`

### file list

```diff
@@ -1,52 +1,75 @@
-drwxrwxr-x   0 zaphod    (1000) zaphod    (1000)        0 2023-04-04 14:56:05.015299 Mesh Client-1.6.0/
-drwxrwxr-x   0 zaphod    (1000) zaphod    (1000)        0 2023-04-04 14:56:05.011299 Mesh Client-1.6.0/.github/
-drwxrwxr-x   0 zaphod    (1000) zaphod    (1000)        0 2023-04-04 14:56:05.011299 Mesh Client-1.6.0/.github/workflows/
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)      484 2023-04-04 14:52:56.000000 Mesh Client-1.6.0/.github/workflows/python-package.yml
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)       93 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/.gitignore
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)       55 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/.tool-versions
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     1051 2022-07-03 16:06:29.000000 Mesh Client-1.6.0/LICENSE
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)      296 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/Makefile
-drwxrwxr-x   0 zaphod    (1000) zaphod    (1000)        0 2023-04-04 14:56:05.011299 Mesh Client-1.6.0/Mesh_Client.egg-info/
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2826 2023-04-04 14:56:04.000000 Mesh Client-1.6.0/Mesh_Client.egg-info/PKG-INFO
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     1213 2023-04-04 14:56:05.000000 Mesh Client-1.6.0/Mesh_Client.egg-info/SOURCES.txt
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)        1 2023-04-04 14:56:04.000000 Mesh Client-1.6.0/Mesh_Client.egg-info/dependency_links.txt
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)      105 2023-04-04 14:56:04.000000 Mesh Client-1.6.0/Mesh_Client.egg-info/entry_points.txt
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)       28 2023-04-04 14:56:04.000000 Mesh Client-1.6.0/Mesh_Client.egg-info/requires.txt
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)       12 2023-04-04 14:56:04.000000 Mesh Client-1.6.0/Mesh_Client.egg-info/top_level.txt
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2826 2023-04-04 14:56:05.015299 Mesh Client-1.6.0/PKG-INFO
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2024 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/README.md
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     1347 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/SECURITY.md
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)       63 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/dev-requirements.txt
-drwxrwxr-x   0 zaphod    (1000) zaphod    (1000)        0 2023-04-04 14:56:05.011299 Mesh Client-1.6.0/java-mesh-client-helper-files/
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     6650 2022-07-03 16:04:29.000000 Mesh Client-1.6.0/java-mesh-client-helper-files/keystore.jks
--rwxrwxr-x   0 zaphod    (1000) zaphod    (1000)      897 2022-07-03 16:04:29.000000 Mesh Client-1.6.0/java-mesh-client-helper-files/meshclient.cfg
-drwxrwxr-x   0 zaphod    (1000) zaphod    (1000)        0 2023-04-04 14:56:05.015299 Mesh Client-1.6.0/mesh_client/
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)    23438 2023-04-04 14:48:22.000000 Mesh Client-1.6.0/mesh_client/__init__.py
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     1923 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/ca.cert.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     3243 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/ca.key.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     1879 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/client.cert.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     3243 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/client.key.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)    10256 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/io_helpers.py
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)    11199 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/io_helpers_test.py
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)      338 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/mesh_client/key_helper.py
--rwxrwxr-x   0 zaphod    (1000) zaphod    (1000)      881 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/mesh_client/mesh_auth.py
--rwxrwxr-x   0 zaphod    (1000) zaphod    (1000)    17477 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/mesh_client/mock_server.py
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2562 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/nhs-dep-ca-bundle.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2615 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/nhs-dev-ca-bundle.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     4632 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/nhs-digicert-ca-bundle.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2985 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/nhs-digicert-root-ca.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2562 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/mesh_client/nhs-ig-int-ca-bundle.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2896 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/mesh_client/nhs-ig-live-ca-bundle.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2701 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/nhs-int-ca-bundle.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     1460 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/nhs-live-root-ca.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2558 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/nhs-opt-ca-bundle.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2562 2022-07-03 16:06:29.000000 Mesh Client-1.6.0/mesh_client/nhs-train-ca-bundle.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     2053 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/server.cert.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     3243 2022-07-03 16:06:28.000000 Mesh Client-1.6.0/mesh_client/server.key.pem
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)    15928 2023-04-04 14:48:22.000000 Mesh Client-1.6.0/mesh_client_test.py
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)      850 2022-10-04 10:12:40.000000 Mesh Client-1.6.0/mesh_endpoint_connectivity_test.py
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)      146 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/pyproject.toml
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)       67 2023-04-04 14:56:05.015299 Mesh Client-1.6.0/setup.cfg
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)     1431 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/setup.py
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)       17 2022-07-03 16:04:29.000000 Mesh Client-1.6.0/test_chunk_retry_file
--rw-rw-r--   0 zaphod    (1000) zaphod    (1000)      171 2022-12-04 04:40:37.000000 Mesh Client-1.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.864758 Mesh-Client-2.0.1/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2044 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.gitallowed
+-rw-rw-r--   0 runner    (1001) docker     (123)     1080 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.gitdisallowed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.856757 Mesh-Client-2.0.1/.github/
+-rw-rw-r--   0 runner    (1001) docker     (123)       48 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (123)      462 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/dependabot.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)      204 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.856757 Mesh-Client-2.0.1/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2683 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/workflows/merge-develop.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     4054 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/workflows/merge-release.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     7424 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/workflows/pull-request.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)      563 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (123)       56 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.tool-versions
+-rw-rw-r--   0 runner    (1001) docker     (123)     1696 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     1078 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (123)     3030 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.856757 Mesh-Client-2.0.1/Mesh_Client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-04 19:33:03.864758 Mesh-Client-2.0.1/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (123)     1447 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/README.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     1347 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (123)      734 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/docker-compose.yml
+-rwxrwxr-x   0 runner    (1001) docker     (123)    12983 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/git-secrets
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.860757 Mesh-Client-2.0.1/mesh_client/
+-rw-rw-r--   0 runner    (1001) docker     (123)    26312 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9982 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/io_helpers.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      260 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/key_helper.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)      831 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/mesh_auth.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-dep-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2615 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-dev-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     4632 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-digicert-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2985 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-digicert-root-ca.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-ig-int-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2896 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-ig-live-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-int-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     1460 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-live-root-ca.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2558 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-opt-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-train-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (123)     1499 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/types.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    97932 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/poetry.lock
+-rw-rw-r--   0 runner    (1001) docker     (123)       61 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/poetry.toml
+-rw-rw-r--   0 runner    (1001) docker     (123)     3815 2023-07-04 19:32:59.000000 Mesh-Client-2.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.860757 Mesh-Client-2.0.1/scripts/
+-rwxrwxr-x   0 runner    (1001) docker     (123)      532 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/scripts/check-secrets.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.860757 Mesh-Client-2.0.1/scripts/hooks/
+-rwxrwxr-x   0 runner    (1001) docker     (123)      390 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/scripts/hooks/commit-msg.sh
+-rwxrwxr-x   0 runner    (1001) docker     (123)      398 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/scripts/hooks/pre-commit.sh
+-rwxrwxr-x   0 runner    (1001) docker     (123)     6225 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/scripts/sonar_tests.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)      325 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/scripts/wait-for-container.sh
+-rw-rw-r--   0 runner    (1001) docker     (123)       67 2023-07-04 19:33:03.864758 Mesh-Client-2.0.1/setup.cfg
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1344 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/setup.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      425 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.864758 Mesh-Client-2.0.1/tests/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1923 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/ca.cert.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     3243 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/ca.key.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     1879 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/client.cert.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     3243 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/client.key.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     1414 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/helpers.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9449 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/io_helpers_tests.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      424 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mailboxes.jsonl
+-rw-rw-r--   0 runner    (1001) docker     (123)     3889 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mesh_chunk_retries_tests.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    10017 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mesh_client_tests.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1964 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mesh_endpoint_connectivity_tests.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9792 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mesh_sandbox_tests.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)    17388 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mock_server.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2053 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/server.cert.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     3243 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/server.key.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)      176 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/workflows.jsonl
```

### Comparing `Mesh Client-1.6.0/LICENSE` & `Mesh-Client-2.0.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,21 @@
-Copyright 2020 NHS Digital
+The MIT License (MIT)
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2023 NHS england
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `Mesh Client-1.6.0/Mesh_Client.egg-info/PKG-INFO` & `Mesh-Client-2.0.1/Mesh_Client.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 Metadata-Version: 2.1
 Name: Mesh-Client
-Version: 1.6.0
-Summary: Client for NHS Digital's MESH messaging system
+Version: 2.0.1
+Summary: Client for NHS England's MESH messaging system
 Home-page: https://github.com/NHSDigital/mesh-client
-Author: James Pickering
-Author-email: api.management@nhs.net
+Author: spinecore
 License: MIT
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 MESH Client
 ===========
 
 A Python client for [NHS Digital's MESH API](https://digital.nhs.uk/developer/api-catalogue/message-exchange-for-social-care-and-health-api).
 
 Installation
 ------------
 
 ```bash
-pip install mesh_client
+pip install mesh-client
 ```
 
 Example use
 -----------
 
 ```python
 from mesh_client import MeshClient, NHS_DEP_ENDPOINT
 with MeshClient(
           NHS_DEP_ENDPOINT,
           'MYMAILBOX',
-          'Password123!',
+          'Password',
           cert=('/etc/certs/cert.pem', '/etc/certs/key.pem')  # Mesh uses SSL, so you'll need some certs
         ) as client:
 
     client.handshake()  # It will work without this, but Spine will complain
     message_ids = client.list_messages()
     first_message = client.retrieve_message(message_ids[0])
     print('Subject', first_message.subject)
@@ -54,48 +49,19 @@
     for message in client.iterate_all_messages():
         with message: # With block will handle acknowledgement
             print('Message', message.read())
 
     client.send_message('RECIPIENT_MAILBOX', b'Hello World!', subject='Important message')
 ```
 
-Guidance for contributors
--------------------------
+Testing your application
+------------------------
 
-You should be doing all your development in a virtualenv / venv. You can install
-everything you need for development with
+We recommend using the [mesh sandbox](https://github.com/NHSDigital/mesh-sandbox) 
+have a look at this [docker-compose.yml](docker-compose.yml) for an example of how to run the sandbox
 
-```bash
-virtualenv .venv
-source .venv/bin/activate
-pip install -r dev-requirements.txt
-pip install -e .
 
-# if using asdf
-pip install tox-asdf
-
-```
-
-We use unittest for tests, and you can run the test suite locally with:
-
-```bash
-python -m unittest discover . '*_test.py'
-```
-
-We use tox for testing on multiple versions. To run the tox tests, just run:
-
-```bash
-tox
-```
+Guidance for contributors
+-------------------------
 
-For releases, we use twine. The rough release process would be:
+see [CONTRIBUTING](CONTRIBUTING.md)
 
-```bash
-tox  # Re-run tests, just to be sure
-git tag $CURRENT_VERSION
-rm dist/*  # Get rid of previous distribution files
-python -m build
-twine upload -r testpypi dist/*
-# Check artifacts are uploaded correctly, and that entry on PyPI looks correct
-twine upload dist/*
-git push --tags
-```
```

### Comparing `Mesh Client-1.6.0/PKG-INFO` & `Mesh-Client-2.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 Metadata-Version: 2.1
-Name: Mesh Client
-Version: 1.6.0
-Summary: Client for NHS Digital's MESH messaging system
+Name: Mesh-Client
+Version: 2.0.1
+Summary: Client for NHS England's MESH messaging system
 Home-page: https://github.com/NHSDigital/mesh-client
-Author: James Pickering
-Author-email: api.management@nhs.net
+Author: spinecore
 License: MIT
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 MESH Client
 ===========
 
 A Python client for [NHS Digital's MESH API](https://digital.nhs.uk/developer/api-catalogue/message-exchange-for-social-care-and-health-api).
 
 Installation
 ------------
 
 ```bash
-pip install mesh_client
+pip install mesh-client
 ```
 
 Example use
 -----------
 
 ```python
 from mesh_client import MeshClient, NHS_DEP_ENDPOINT
 with MeshClient(
           NHS_DEP_ENDPOINT,
           'MYMAILBOX',
-          'Password123!',
+          'Password',
           cert=('/etc/certs/cert.pem', '/etc/certs/key.pem')  # Mesh uses SSL, so you'll need some certs
         ) as client:
 
     client.handshake()  # It will work without this, but Spine will complain
     message_ids = client.list_messages()
     first_message = client.retrieve_message(message_ids[0])
     print('Subject', first_message.subject)
@@ -54,48 +49,19 @@
     for message in client.iterate_all_messages():
         with message: # With block will handle acknowledgement
             print('Message', message.read())
 
     client.send_message('RECIPIENT_MAILBOX', b'Hello World!', subject='Important message')
 ```
 
-Guidance for contributors
--------------------------
+Testing your application
+------------------------
 
-You should be doing all your development in a virtualenv / venv. You can install
-everything you need for development with
+We recommend using the [mesh sandbox](https://github.com/NHSDigital/mesh-sandbox) 
+have a look at this [docker-compose.yml](docker-compose.yml) for an example of how to run the sandbox
 
-```bash
-virtualenv .venv
-source .venv/bin/activate
-pip install -r dev-requirements.txt
-pip install -e .
 
-# if using asdf
-pip install tox-asdf
-
-```
-
-We use unittest for tests, and you can run the test suite locally with:
-
-```bash
-python -m unittest discover . '*_test.py'
-```
-
-We use tox for testing on multiple versions. To run the tox tests, just run:
-
-```bash
-tox
-```
+Guidance for contributors
+-------------------------
 
-For releases, we use twine. The rough release process would be:
+see [CONTRIBUTING](CONTRIBUTING.md)
 
-```bash
-tox  # Re-run tests, just to be sure
-git tag $CURRENT_VERSION
-rm dist/*  # Get rid of previous distribution files
-python -m build
-twine upload -r testpypi dist/*
-# Check artifacts are uploaded correctly, and that entry on PyPI looks correct
-twine upload dist/*
-git push --tags
-```
```

### Comparing `Mesh Client-1.6.0/README.md` & `Mesh-Client-2.0.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 A Python client for [NHS Digital's MESH API](https://digital.nhs.uk/developer/api-catalogue/message-exchange-for-social-care-and-health-api).
 
 Installation
 ------------
 
 ```bash
-pip install mesh_client
+pip install mesh-client
 ```
 
 Example use
 -----------
 
 ```python
 from mesh_client import MeshClient, NHS_DEP_ENDPOINT
 with MeshClient(
           NHS_DEP_ENDPOINT,
           'MYMAILBOX',
-          'Password123!',
+          'Password',
           cert=('/etc/certs/cert.pem', '/etc/certs/key.pem')  # Mesh uses SSL, so you'll need some certs
         ) as client:
 
     client.handshake()  # It will work without this, but Spine will complain
     message_ids = client.list_messages()
     first_message = client.retrieve_message(message_ids[0])
     print('Subject', first_message.subject)
@@ -33,48 +33,19 @@
     for message in client.iterate_all_messages():
         with message: # With block will handle acknowledgement
             print('Message', message.read())
 
     client.send_message('RECIPIENT_MAILBOX', b'Hello World!', subject='Important message')
 ```
 
-Guidance for contributors
--------------------------
+Testing your application
+------------------------
 
-You should be doing all your development in a virtualenv / venv. You can install
-everything you need for development with
+We recommend using the [mesh sandbox](https://github.com/NHSDigital/mesh-sandbox) 
+have a look at this [docker-compose.yml](docker-compose.yml) for an example of how to run the sandbox
 
-```bash
-virtualenv .venv
-source .venv/bin/activate
-pip install -r dev-requirements.txt
-pip install -e .
 
-# if using asdf
-pip install tox-asdf
-
-```
-
-We use unittest for tests, and you can run the test suite locally with:
-
-```bash
-python -m unittest discover . '*_test.py'
-```
-
-We use tox for testing on multiple versions. To run the tox tests, just run:
-
-```bash
-tox
-```
+Guidance for contributors
+-------------------------
 
-For releases, we use twine. The rough release process would be:
+see [CONTRIBUTING](CONTRIBUTING.md)
 
-```bash
-tox  # Re-run tests, just to be sure
-git tag $CURRENT_VERSION
-rm dist/*  # Get rid of previous distribution files
-python -m build
-twine upload -r testpypi dist/*
-# Check artifacts are uploaded correctly, and that entry on PyPI looks correct
-twine upload dist/*
-git push --tags
-```
```

### Comparing `Mesh Client-1.6.0/SECURITY.md` & `Mesh-Client-2.0.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/__init__.py` & `Mesh-Client-2.0.1/mesh_client/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,148 +1,213 @@
-from __future__ import absolute_import
 import collections
-import warnings
-import functools
 import datetime
+import functools
 import hmac
-import pkg_resources
+import os.path
 import platform
-import requests
-import six
+import ssl
+import sys
 import time
 import uuid
+import warnings
+from dataclasses import dataclass
 from hashlib import sha256
 from io import BytesIO
 from itertools import chain
-from six.moves.urllib.parse import quote as q
+from typing import Any, Dict, List, Optional, Tuple, TypeVar, Union, cast
+from urllib.parse import quote as q
 
+import requests
+from requests.adapters import HTTPAdapter
 
-from .io_helpers import \
-    CombineStreams, SplitStream, GzipCompressStream, GzipDecompressStream
+from .io_helpers import (
+    CombineStreams,
+    GzipCompressStream,
+    GzipDecompressStream,
+    SplitStream,
+)
 from .key_helper import get_shared_key_from_environ
-
-MOCK_CA_CERT = pkg_resources.resource_filename('mesh_client', "ca.cert.pem")
-MOCK_CERT = pkg_resources.resource_filename('mesh_client', "client.cert.pem")
-MOCK_KEY = pkg_resources.resource_filename('mesh_client', "client.key.pem")
-
-MOCK_SSL_OPTS = {
-    "verify": MOCK_CA_CERT,
-    "cert": (MOCK_CERT, MOCK_KEY)
-}
-"""
-Usable default values for verify and cert, providing certificates and keys
-which should work with mock_server. Note that these certs will not work with
-any NHS Digital test environments - such certs must be obtained from
-NHS Digital.
-"""
-default_ssl_opts = MOCK_SSL_OPTS
-
-INT_CA_CERT = pkg_resources.resource_filename('mesh_client', "nhs-int-ca-bundle.pem")
-DEV_CA_CERT = pkg_resources.resource_filename('mesh_client', "nhs-dev-ca-bundle.pem")
-DEP_CA_CERT = pkg_resources.resource_filename('mesh_client', "nhs-dep-ca-bundle.pem")
-TRAIN_CA_CERT = pkg_resources.resource_filename('mesh_client', "nhs-train-ca-bundle.pem")
-LIVE_CA_CERT = pkg_resources.resource_filename('mesh_client', "nhs-live-root-ca.pem")
-OPENTEST_CA_CERT = pkg_resources.resource_filename('mesh_client', "nhs-opt-ca-bundle.pem")
-DIGICERT_CA_CERT = pkg_resources.resource_filename('mesh_client', "nhs-digicert-ca-bundle.pem")
-IG_INT_CA_CERT = pkg_resources.resource_filename('mesh_client', "nhs-ig-int-ca-bundle.pem")
-IG_LIVE_CA_CERT = pkg_resources.resource_filename('mesh_client', "nhs-ig-live-ca-bundle.pem")
+from .types import (
+    EndpointLookupResponse_v1,
+    ListMessageResponse_v1,
+    SendMessageErrorResponse_v1,
+    SendMessageResponse_v1,
+    TrackingResponse_v1,
+)
+
+if sys.version_info[:2] >= (3, 8):
+    # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
+    from importlib.metadata import PackageNotFoundError, version
+else:
+    from importlib_metadata import PackageNotFoundError, version
+
+
+def _get_version(*names: str) -> str:
+    """ """
+    for name in names:
+        try:
+            pkg_version = version(name)
+            return pkg_version
+        except PackageNotFoundError:
+            continue
+    return "unknown"
+
+
+__version__ = _get_version("mesh-client")
+
+_PACKAGE_DIR = os.path.dirname(__file__)
+
+INT_CA_CERT = os.path.join(_PACKAGE_DIR, "nhs-int-ca-bundle.pem")
+DEV_CA_CERT = os.path.join(_PACKAGE_DIR, "nhs-dev-ca-bundle.pem")
+DEP_CA_CERT = os.path.join(_PACKAGE_DIR, "nhs-dep-ca-bundle.pem")
+TRAIN_CA_CERT = os.path.join(_PACKAGE_DIR, "nhs-train-ca-bundle.pem")
+LIVE_CA_CERT = os.path.join(_PACKAGE_DIR, "nhs-live-root-ca.pem")
+OPENTEST_CA_CERT = os.path.join(_PACKAGE_DIR, "nhs-opt-ca-bundle.pem")
+DIGICERT_CA_CERT = os.path.join(_PACKAGE_DIR, "nhs-digicert-ca-bundle.pem")
+IG_INT_CA_CERT = os.path.join(_PACKAGE_DIR, "nhs-ig-int-ca-bundle.pem")
+IG_LIVE_CA_CERT = os.path.join(_PACKAGE_DIR, "nhs-ig-live-ca-bundle.pem")
 
 
 _OPTIONAL_HEADERS = {
     "workflow_id": "Mex-WorkflowID",
     "filename": "Mex-FileName",
     "local_id": "Mex-LocalID",
     "message_type": "Mex-MessageType",
-    "process_id": "Mex-ProcessID",
     "subject": "Mex-Subject",
     "encrypted": "Mex-Content-Encrypted",
     "compressed": "Mex-Content-Compressed",
-    "checksum": "Mex-Content-Checksum"
+    "checksum": "Mex-Content-Checksum",
+    "content_type": "Content-Type",
 }
 
 _BOOLEAN_HEADERS = {"compressed", "encrypted"}
 
 _RECEIVE_HEADERS = {
     "sender": "Mex-From",
     "recipient": "Mex-To",
     "message_id": "Mex-MessageID",
     "version": "Mex-Version",
     "partner_id": "Mex-PartnerID",
-    "recipient_smtp": "Mex-ToSMTP",
-    "sender_smtp": "Mex-FromSMTP",
 }
 _RECEIVE_HEADERS.update(_OPTIONAL_HEADERS)
 
 
-VERSION = pkg_resources.get_distribution('mesh_client').version
-
+Endpoint = collections.namedtuple("Endpoint", ["url", "verify", "cert", "check_hostname"])
 
-Endpoint = collections.namedtuple('Endpoint', ['url', 'verify', 'cert'])
-LOCAL_MOCK_ENDPOINT = Endpoint('https://localhost:8000', MOCK_CA_CERT, (MOCK_CERT, MOCK_KEY))
-LOCAL_FAKE_ENDPOINT = Endpoint('https://localhost:8829', MOCK_CA_CERT, (MOCK_CERT, MOCK_KEY))
-NHS_INT_ENDPOINT = Endpoint('https://msg.int.spine2.ncrs.nhs.uk', INT_CA_CERT, None)
-NHS_DEV_ENDPOINT = Endpoint('https://msg.dev.spine2.ncrs.nhs.uk', DEV_CA_CERT, None)
-NHS_DEP_ENDPOINT = Endpoint('https://msg.dep.spine2.ncrs.nhs.uk', DEP_CA_CERT, None)
-NHS_TRAIN_ENDPOINT = Endpoint('https://msg.train.spine2.ncrs.nhs.uk', TRAIN_CA_CERT, None)
-NHS_LIVE_ENDPOINT = Endpoint('https://mesh-sync.national.ncrs.nhs.uk', LIVE_CA_CERT, None)
-NHS_OPENTEST_ENDPOINT = Endpoint('https://192.168.128.11', OPENTEST_CA_CERT, None)
-NHS_INTERNET_GATEWAY_ENDPOINT = Endpoint('https://mesh-sync.spineservices.nhs.uk', IG_LIVE_CA_CERT, None)
-NHS_INTERNET_GATEWAY_INT_ENDPOINT = Endpoint('https://msg.intspineservices.nhs.uk', IG_INT_CA_CERT, None)
+NHS_INT_ENDPOINT = Endpoint("https://msg.int.spine2.ncrs.nhs.uk", INT_CA_CERT, None, False)
+NHS_DEV_ENDPOINT = Endpoint("https://msg.dev.spine2.ncrs.nhs.uk", DEV_CA_CERT, None, False)
+NHS_DEP_ENDPOINT = Endpoint("https://msg.dep.spine2.ncrs.nhs.uk", DEP_CA_CERT, None, False)
+NHS_TRAIN_ENDPOINT = Endpoint("https://msg.train.spine2.ncrs.nhs.uk", TRAIN_CA_CERT, None, False)
+NHS_LIVE_ENDPOINT = Endpoint("https://mesh-sync.national.ncrs.nhs.uk", LIVE_CA_CERT, None, False)
+NHS_OPENTEST_ENDPOINT = Endpoint("https://192.168.128.11", OPENTEST_CA_CERT, None, False)
+NHS_INTERNET_GATEWAY_ENDPOINT = Endpoint("https://mesh-sync.spineservices.nhs.uk", IG_LIVE_CA_CERT, None, True)
+NHS_INTERNET_GATEWAY_INT_ENDPOINT = Endpoint("https://msg.intspineservices.nhs.uk", IG_INT_CA_CERT, None, True)
 
 
 def deprecated(reason=None):
     """This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
     when the function is used."""
 
     def decorator(func):
         @functools.wraps(func)
         def new_func(*args, **kwargs):
             msg_extra = (reason or "").strip()
             if msg_extra:
                 msg_extra = " " + msg_extra
-            message = "Call to deprecated function {}.".format(func.__name__, msg_extra)
+            message = f"Call to deprecated function {func.__name__} {msg_extra}."
             warnings.warn(message, category=DeprecationWarning, stacklevel=2)
             return func(*args, **kwargs)
+
         return new_func
+
     return decorator
 
 
 class MeshError(Exception):
     pass
 
 
+class SSLContextAdapter(HTTPAdapter):
+    def __init__(
+        self,
+        url: Union[str, Endpoint],
+        cert: Optional[Union[Tuple[str], Tuple[str, str], Tuple[str, str, str]]] = None,
+        verify: Optional[Union[str, bool]] = None,
+        check_hostname: Optional[bool] = None,
+    ):
+        self.url = url
+        self.cert = cert
+        self.verify = verify
+        self.check_hostname = check_hostname
+        if check_hostname is None and hasattr(url, "check_hostname"):
+            self.check_hostname = url.check_hostname
+
+        if cert is None and hasattr(url, "cert"):
+            self.cert = url.cert
+
+        if verify is None and hasattr(url, "verify"):
+            self.verify = url.verify
+
+        super().__init__()
+
+    def init_poolmanager(self, *args, **kwargs):
+        context = ssl.create_default_context()
+
+        if self.cert and isinstance(self.cert, (tuple, list)):
+            context.load_cert_chain(*self.cert)
+
+        if self.verify:
+            if isinstance(self.verify, (str, bytes)):
+                context.load_verify_locations(self.verify)
+
+            if context.check_hostname is not None:
+                context.check_hostname = cast(bool, self.check_hostname)
+
+            context.verify_mode = ssl.CERT_REQUIRED
+            if self.check_hostname is not False:
+                context.hostname_checks_common_name = True
+
+        if self.verify is False:
+            context.check_hostname = False
+            context.verify_mode = ssl.CERT_NONE
+
+        kwargs["ssl_context"] = context
+        return super(SSLContextAdapter, self).init_poolmanager(*args, **kwargs)
+
+
 class MeshClient(object):
     """
     A class representing a single MESH session, for a given user on a given
     endpoint. This class handles details such as chunking and compression
     transparently.
     """
 
-    def __init__(self,
-                 url,
-                 mailbox,
-                 password,
-                 shared_key=get_shared_key_from_environ(),
-                 cert=None,
-                 verify=None,
-                 max_chunk_size=75 * 1024 * 1024,
-                 proxies=None,
-                 transparent_compress=False,
-                 max_chunk_retries=0,
-                 timeout=10*60):
+    def __init__(
+        self,
+        url: Union[str, Endpoint],
+        mailbox: str,
+        password: str,
+        shared_key: Optional[bytes] = None,
+        cert: Optional[Union[Tuple[str], Tuple[str, str], Tuple[str, str, str]]] = None,
+        verify: Optional[Union[str, bool]] = None,
+        check_hostname: Optional[bool] = None,
+        max_chunk_size=75 * 1024 * 1024,
+        proxies: Optional[Dict[str, str]] = None,
+        transparent_compress: bool = False,
+        max_chunk_retries: int = 0,
+        timeout: Union[int, float] = 10 * 60,
+    ):
         """
         Create a new MeshClient.
 
         At a minimum, you must provide an endpoint url, a mailbox and a
         password. The endpoint URL can either be a string, or a preconfigured
         endpoint. Currently the following endpoints are preconfigured:
 
-        LOCAL_MOCK_ENDPOINT
-        LOCAL_FAKE_ENDPOINT
         NHS_INT_ENDPOINT
         NHS_LIVE_ENDPOINT
         NHS_OPENTEST_ENDPOINT
         NHS_INTERNET_GATEWAY_INT_ENDPOINT
         NHS_INTERNET_GATEWAY_ENDPOINT
 
         Since MESH uses mutual authentication, it is also highly
@@ -157,290 +222,310 @@
         are provided, so you will not need to configure that either.
 
         You can also optionally specify the maximum file size before chunking,
         and whether messages should be compressed, transparently, before
         sending.
         """
 
+        shared_key = shared_key or get_shared_key_from_environ()
+
         self._session = requests.Session()
+        adapter = SSLContextAdapter(url, cert, verify, check_hostname)
+        self._session.mount("https://", adapter)
+        self._session.mount("http://", adapter)
         self._session.headers = {
             "User-Agent": (
-                "mesh_client;{};N/A;{};{};{} {}".format(
-                    VERSION,
-                    platform.processor() or platform.machine(),
-                    platform.system(),
-                    platform.release(),
-                    platform.version()
-                )
+                f"mesh_client;{__version__};N/A;{platform.processor() or platform.machine()};"
+                f"{platform.system()};{platform.release()} {platform.version()}"
             ),
-            "Accept-Encoding": "gzip"
+            "Accept-Encoding": "gzip",
         }
         self._session.auth = AuthTokenGenerator(shared_key, mailbox, password)
-        if hasattr(url, 'url'):
+        if hasattr(url, "url"):
             self._url = url.url
         else:
             self._url = url
 
-        if hasattr(url, 'cert') and cert is None:
-            self._session.cert = url.cert
-        else:
-            self._session.cert = cert
-
-        if hasattr(url, 'verify') and verify is None:
-            self._session.verify = url.verify
-        else:
+        if verify is not None:
             self._session.verify = verify
+        elif hasattr(url, "verify"):
+            self._session.verify = url.verify
 
         self._session.proxies = proxies or {}
         self._mailbox = mailbox
         self._max_chunk_size = max_chunk_size
         self._transparent_compress = transparent_compress
         self._max_chunk_retries = max_chunk_retries
         self._timeout = timeout
         self._close_called = False
 
+    @property
+    def mailbox_url(self) -> str:
+        return f"{self._url}/messageexchange/{q(self._mailbox)}"
+
+    def ping(self) -> dict:
+        """
+        just connect to the _ping endpoint
+        """
+        response = self._session.get(f"{self._url}/messageexchange/_ping", timeout=self._timeout)
+
+        response.raise_for_status()
+
+        return cast(dict, response.json())
+
     def handshake(self):
         """
         List all messages in user's inbox. Returns a list of message_ids
         """
         headers = {
-            "mex-ClientVersion": "mesh_client=={}".format(VERSION),
+            "mex-ClientVersion": f"mesh_client=={__version__}",
             "mex-OSArchitecture": platform.processor() or platform.machine(),
             "mex-OSName": platform.system(),
-            "mex-OSVersion": "{} {}".format(platform.release(), platform.version()),
-            "mex-JavaVersion": "N/A"
+            "mex-OSVersion": f"{platform.release()} {platform.version()}",
+            "mex-JavaVersion": "N/A",
         }
-        response = self._session.post(
-            "{}/messageexchange/{}".format(self._url, q(self._mailbox)), headers=headers,
-            timeout=self._timeout
-        )
+        response = self._session.post(self.mailbox_url, headers=headers, timeout=self._timeout)
 
         response.raise_for_status()
 
-        return b'hello'
+        return b"hello"
 
     @deprecated("this api endpoint is marked as deprecated")
-    def count_messages(self):
+    def count_messages(self) -> int:
         """
         Count all messages in user's inbox. Returns an integer
         """
-        response = self._session.get(
-            "{}/messageexchange/{}/count".format(self._url, q(self._mailbox)),
-            timeout=self._timeout)
+        response = self._session.get(f"{self.mailbox_url}/count", timeout=self._timeout)
         response.raise_for_status()
-        return response.json()["count"]
+        return cast(int, response.json()["count"])
 
-    def track_by_message_id(self, message_id=None):
+    def track_by_message_id(self, message_id: str) -> TrackingResponse_v1:
         """
         Gets tracking information from MESH about a message, by its  message id.
         Returns a dictionary, in much the same format that MESH provides it.
         """
-        url = "{}/messageexchange/{}/outbox/tracking?messageID={}".format(self._url, q(self._mailbox), q(message_id))
+        url = f"{self.mailbox_url}/outbox/tracking?messageID={q(message_id)}"
 
         response = self._session.get(url, timeout=self._timeout)
         response.raise_for_status()
-        return response.json()
+        return cast(TrackingResponse_v1, response.json())
+
+    def _get_tracking_url(self, local_id: Optional[str] = None, message_id: Optional[str] = None) -> str:
+        if message_id:
+            return f"{self.mailbox_url}/outbox/tracking?messageID={q(message_id)}"
+
+        if local_id:
+            return f"{self.mailbox_url}/outbox/tracking/{q(local_id)}"
+
+        raise ValueError(
+            "Exactly one of local message id (called tracking_id, for historical reasons) "
+            "and message_id must be provided"
+        )
 
     @deprecated(reason="tracking by local_id is deprecated, please use 'track_by_message_id'")
-    def get_tracking_info(self, tracking_id=None, message_id=None):
+    def get_tracking_info(
+        self, local_id: Optional[str] = None, message_id: Optional[str] = None
+    ) -> TrackingResponse_v1:
         """
         Gets tracking information from MESH about a message, by its local message id.
         Returns a dictionary, in much the same format that MESH provides it.
         """
-        if (tracking_id is not None) + (message_id is not None) != 1:
-            raise ValueError("Exactly one of local message id (called tracking_id, for historical reasons) and message_id must be provided")
 
-        if tracking_id:
-            url = "{}/messageexchange/{}/outbox/tracking/{}".format(self._url, q(self._mailbox), q(tracking_id))
-        else:
-            url = "{}/messageexchange/{}/outbox/tracking?messageID={}".format(self._url, q(self._mailbox), q(message_id))
+        url = self._get_tracking_url(local_id, message_id)
 
         response = self._session.get(url, timeout=self._timeout)
         response.raise_for_status()
-        return response.json()
+        return cast(TrackingResponse_v1, response.json())
 
-    def lookup_endpoint(self, organisation_code, workflow_id):
+    def lookup_endpoint(self, ods_code: str, workflow_id: str) -> EndpointLookupResponse_v1:
         """
         Lookup a mailbox by organisation code and workflow id.
         Returns a dictionary, in much the same format that MESH provides it.
         """
         response = self._session.get(
-            "{}/endpointlookup/mesh/{}/{}".format(self._url, q(organisation_code), q(workflow_id)),
-            timeout=self._timeout)
+            f"{self._url}/messageexchange/endpointlookup/{q(ods_code)}/{q(workflow_id)}",
+            timeout=self._timeout,
+        )
         response.raise_for_status()
-        return response.json()
+        return cast(EndpointLookupResponse_v1, response.json())
 
-    def list_messages(self):
+    def list_messages(self) -> List[str]:
         """
         List all messages in user's inbox. Returns a list of message_ids
         """
-        response = self._session.get(
-            "{}/messageexchange/{}/inbox".format(self._url, q(self._mailbox)),
-            timeout=self._timeout)
+        response = self._session.get(f"{self.mailbox_url}/inbox", timeout=self._timeout)
         response.raise_for_status()
-        return response.json()["messages"]
+        return cast(ListMessageResponse_v1, response.json())["messages"]
 
-    def retrieve_message(self, message_id):
+    def retrieve_message(self, message_id: str):
         """
         Retrieve a message based on its message_id. This will return a Message
         object
         """
         message_id = getattr(message_id, "_msg_id", message_id)
         response = self._session.get(
-            "{}/messageexchange/{}/inbox/{}".format(self._url, q(self._mailbox), q(message_id)),
+            f"{self.mailbox_url}/inbox/{q(message_id)}",
             stream=True,
-            timeout=self._timeout)
+            timeout=self._timeout,
+        )
         response.raise_for_status()
         return Message(message_id, response, self)
 
-    def retrieve_message_chunk(self, message_id, chunk_num):
+    def retrieve_message_chunk(self, message_id: str, chunk_num: Union[int, str]):
         response = self._session.get(
-            "{}/messageexchange/{}/inbox/{}/{}".format(self._url, q(self._mailbox), q(message_id), chunk_num),
+            f"{self.mailbox_url}/inbox/{q(message_id)}/{chunk_num}",
             stream=True,
-            timeout=self._timeout)
+            timeout=self._timeout,
+        )
         response.raise_for_status()
         return response
 
     def send_message(
-         self,
-         recipient,
-         data,
-         max_chunk_size = None,
-         **kwargs
-    ):
+        self,
+        recipient: str,
+        data,
+        max_chunk_size: Optional[int] = None,
+        **kwargs,
+    ) -> str:
         """
         Send a message to recipient containing data.
 
         This method optionally allows the user to provide the following keyword
         arguments, which specify properties of the message, and map to
         the equivalent properties in MESH - either headers or control file
         entries, depending on the type of consumer:
 
         workflow_id
         filename
         local_id
         message_type
-        process_id
         subject
         encrypted
         compressed
         checksum
         sender
         recipient
         message_id
         version
         partner_id
-        recipient_smtp
-        sender_smtp
 
         Note that compressed refers to *non-transparent* compression - the
         client will not attempt to compress or decompress data. Transparent
         compression for sending is enabled as a constructor option.
         """
         transparent_compress = self._transparent_compress
-        maybe_compressed = (
-            lambda stream: GzipCompressStream(
-                stream) if transparent_compress else stream
-        )
+
+        def maybe_compressed(maybe_compress: bytes):
+            if not transparent_compress:
+                return maybe_compress
+            return GzipCompressStream(maybe_compress)
+
         headers = {
             "Mex-From": self._mailbox,
             "Mex-To": recipient,
-            "Mex-MessageType": 'DATA',
-            "Mex-Version": '1.0',
+            "Mex-MessageType": "DATA",
+            "Mex-Version": "1.0",
             "Content-Type": "application/octet-stream",
         }
 
         for key, value in kwargs.items():
             if key in _OPTIONAL_HEADERS:
                 if key in _BOOLEAN_HEADERS:
-                    value = 'Y' if value else 'N'
+                    value = "Y" if value else "N"
                 headers[_OPTIONAL_HEADERS[key]] = str(value)
             else:
-                raise TypeError("Unrecognised keyword argument {key}."
-                                " optional arguments are: {args}".format(
-                                    key=key,
-                                    args=", ".join([
-                                        "recipient", "data"
-                                    ] + list(_OPTIONAL_HEADERS.keys()))))
+                optional_args = ", ".join(["recipient", "data"] + list(_OPTIONAL_HEADERS.keys()))
+                raise TypeError(f"Unrecognised keyword argument '{key}'.  optional arguments are: {optional_args}")
 
         if transparent_compress:
             headers["Mex-Content-Compress"] = "Y"
             headers["Content-Encoding"] = "gzip"
 
         max_chunk_size = max_chunk_size or self._max_chunk_size
         chunks = SplitStream(data, max_chunk_size)
-        headers["Mex-Chunk-Range"] = "1:{}".format(len(chunks))
+        headers["Mex-Chunk-Range"] = f"1:{len(chunks)}"
         chunk_iterator = iter(chunks)
 
-        chunk1 = maybe_compressed(six.next(chunk_iterator))
+        chunk1 = maybe_compressed(next(chunk_iterator))
         response1 = self._session.post(
-            "{}/messageexchange/{}/outbox".format(self._url, q(self._mailbox)),
+            f"{self.mailbox_url}/outbox",
             data=chunk1,
             headers=headers,
-            timeout=self._timeout)
+            timeout=self._timeout,
+        )
         # MESH server dumps XML SOAP output on internal server error
         if response1.status_code >= 500:
             response1.raise_for_status()
-        json_resp = response1.json()
-        if response1.status_code == 417 or "errorDescription" in json_resp:
-            raise MeshError(json_resp["errorDescription"], json_resp)
-        message_id = json_resp["messageID"]
+
+        response_dict = response1.json()
+        if response1.status_code == 417 or "errorDescription" in response_dict:
+            error_response = cast(SendMessageErrorResponse_v1, response_dict)
+            raise MeshError(error_response["errorDescription"], error_response)
+
+        if response1.status_code not in (200, 202):
+            raise MeshError(response_dict)
+
+        success_response = cast(SendMessageResponse_v1, response_dict)
+
+        message_id = success_response["messageID"]
 
         for i, chunk in enumerate(chunk_iterator):
             data = maybe_compressed(chunk)
 
             if self._max_chunk_retries > 0:
-                if hasattr(data, 'read'):
+                if hasattr(data, "read"):
                     data = data.read()
                 buf = BytesIO(data)
             else:
                 buf = data
 
             chunk_num = i + 2
             headers = {
                 "Content-Type": "application/octet-stream",
-                "Mex-Chunk-Range": "{}:{}".format(chunk_num, len(chunks)),
+                "Mex-Chunk-Range": f"{chunk_num}:{len(chunks)}",
                 "Mex-From": self._mailbox,
             }
             if transparent_compress:
                 headers["Mex-Content-Compress"] = "Y"
                 headers["Content-Encoding"] = "gzip"
 
-            response = None
             for i in range(self._max_chunk_retries + 1):
                 if self._max_chunk_retries > 0:
                     buf.seek(0)
 
                 # non-linear delay in terms of squares
                 time.sleep(i**2)
 
                 response = self._session.post(
-                    "{}/messageexchange/{}/outbox/{}/{}".format(
-                        self._url, q(self._mailbox), q(message_id), chunk_num),
+                    f"{self.mailbox_url}/outbox/{q(message_id)}/{chunk_num}",
                     data=buf,
                     headers=headers,
-                    timeout=self._timeout)
+                    timeout=self._timeout,
+                )
 
                 # check other successful response codes
-                if response.status_code == 200 or response.status_code == 202:
+                if response.status_code in (200, 202):
                     break
-            else:
+
+                if i < self._max_chunk_retries:
+                    continue
+
                 response.raise_for_status()
 
         return message_id
 
-    def acknowledge_message(self, message_id):
+    def acknowledge_message(self, message_id: str):
         """
         Acknowledge a message_id, deleting it from MESH.
         """
         message_id = getattr(message_id, "_msg_id", message_id)
         response = self._session.put(
-            "{}/messageexchange/{}/inbox/{}/status/acknowledged".format(
-                self._url, q(self._mailbox), q(message_id)),
-            timeout=self._timeout)
+            f"{self.mailbox_url}/inbox/{q(message_id)}/status/acknowledged",
+            timeout=self._timeout,
+        )
         response.raise_for_status()
 
     def iterate_all_messages(self):
         """
         Iterate over a list of Message objects for all messages in the user's
         inbox. This is provided as a convenience function, but will be
         slower than list_messages if only the message_ids are needed, since it
@@ -468,130 +553,159 @@
     def __enter__(self):
         return self
 
     def __exit__(self, type_, value, tb):
         self.close()
 
 
-class Message(object):
+@dataclass
+class _MessageAttrs:
+    """
+    this is for type hinting on the commonly used message attrs below ( which are dynamically generated )
+    """
+
+    message_id: str
+    message_type: str
+    recipient: str
+    content_type: str
+    sender: Optional[str] = None
+
+    workflow_id: Optional[str] = None
+    filename: Optional[str] = None
+    local_id: Optional[str] = None
+    partner_id: Optional[str] = None
+    chunk_range: Optional[str] = None
+
+    subject: Optional[str] = None
+    encrypted: Optional[Union[str, bool]] = None
+    compressed: Optional[Union[str, bool]] = None
+
+
+TDefault = TypeVar("TDefault")
+
+
+class _BaseMessage:
     """
     An object representing a message received from MESH. This is a file-like
     object, and can be passed to anything that expects an object with a `read`
     method.
 
     Any properties set on the message (as headers in MESH API, or control file
     entries) are available as attributes of this object. The following are
     supported:
 
     workflow_id
     filename
     local_id
     message_type
-    process_id
     subject
     encrypted
     compressed
+    checksum
+    content_type
 
     Note that compressed refers to *non-transparent* compression - the
-    client will not attempt to compress or decompress data. Transparent
+    client will not attempt to compress or decompress data. Transparent (Content-Encoding)
     compression is handled automatically, with no intervention needed.
+    This is merely a header that is passed through to let the recipient know the decoded content is further compressed.
+
 
     Messages have a read method, and will handle chunking and transparent
     compression automatically. Once the data has been read, you must close the
     underlying stream using the close method. Data can only be read once. If
     you need to read it again, retrieve the message again.
 
     Messages can be used as context managers. When used in this way, streams
     will be closed automatically, and messages will be acknowledged if
     no exceptions are thrown whilst handling the message.
     """
 
-    def __init__(self, msg_id, response, client):
+    def __init__(self, msg_id: str, response, client):
         self._msg_id = msg_id
         self._client = client
-        self._mex_headers = {}
+        self._mex_headers: Dict[str, Any] = {}
 
         headers = response.headers
-        for key, value in six.iteritems(headers):
-            lkey = key.lower()
-            if lkey.startswith('mex-'):
-                self._mex_headers[lkey[4:]] = value
-
-        for key, value in _RECEIVE_HEADERS.items():
-            header_value = headers.get(value, None)
-            if key in _BOOLEAN_HEADERS:
+        for header, header_value in headers.items():
+            lkey = header.lower()
+            if lkey.startswith("mex-"):
+                self._mex_headers[lkey[4:]] = header_value
+
+        for attribute, header in _RECEIVE_HEADERS.items():
+            header_value = headers.get(header, None)
+            if attribute in _BOOLEAN_HEADERS:
                 header_value = header_value or "N"
                 header_value = header_value.upper() in ["Y", "TRUE"]
-            setattr(self, key, header_value)
+            setattr(self, attribute, header_value)
         chunk, chunk_count = map(int, headers.get("Mex-Chunk-Range", "1:1").split(":"))
         maybe_decompress = (
-            lambda resp:
-            GzipDecompressStream(resp.raw)
-            if resp.headers.get("Content-Encoding") == "gzip" else resp.raw
+            lambda resp: GzipDecompressStream(resp.raw) if resp.headers.get("Content-Encoding") == "gzip" else resp.raw
         )
         self._response = CombineStreams(
-            chain([maybe_decompress(response)], (maybe_decompress(
-                client.retrieve_message_chunk(msg_id, str(
-                    i + 2))) for i in range(chunk_count - 1))))
+            chain(
+                [maybe_decompress(response)],
+                (maybe_decompress(client.retrieve_message_chunk(msg_id, str(i + 2))) for i in range(chunk_count - 1)),
+            )
+        )
 
-    def id(self):
+    def id(self) -> str:
         """return the message id
 
         Returns:
             str: message id
         """
         return self._msg_id
 
-    def read(self, n=None):
+    def read(self, n=None) -> bytes:
         """
         Read up to n bytes from the message, or read the remainder of the
         message, if n is not provided.
         """
         return self._response.read(n)
 
-    def readline(self):
+    def readline(self) -> bytes:
         """
         Read a single line from the message
         """
         return self._response.readline()
 
-    def readlines(self):
+    def readlines(self) -> List[bytes]:
         """
         Read all lines from the message
         """
         return self._response.readlines()
 
     def close(self):
         """Close the stream underlying this message"""
         if hasattr(self._response, "close"):
             try:
                 self._response.close()
             finally:
-                self._response = None
+                self._response = None  # type: ignore[assignment]
 
     def acknowledge(self):
         """
         Acknowledge this message, and delete it from MESH
         """
         self._client.acknowledge_message(self._msg_id)
 
-    def mex_header(self, key, default=None):
-        """ get a mex header if present
+    def mex_header(self, key: str, default: Optional[TDefault] = None) -> Union[str, TDefault]:
+        """get a mex header if present
 
         Args:
             key (str): key
             default (any): default value
         Returns:
             str: the mex header value
         """
         return self._mex_headers.get(key, default)
 
     def mex_headers(self):
         """returns a generator iteritems for all the headers"""
-        return six.iteritems(self._mex_headers)
+        return self._mex_headers.items()
 
     def __enter__(self):
         return self
 
     def __exit__(self, typ, value, traceback):
         try:
             if not value:
@@ -602,44 +716,41 @@
     def __iter__(self):
         """
         Iterate through lines of the message
         """
         return iter(self._response)
 
 
-class AuthTokenGenerator(object):
+class Message(_BaseMessage, _MessageAttrs):
+    def __init__(self, msg_id: str, response, client):
+        super().__init__(msg_id, response, client)
+
 
-    def __init__(self, key, mailbox, password):
+class AuthTokenGenerator(object):
+    def __init__(self, key: bytes, mailbox: str, password: str):
         self._key = key
         self._mailbox = mailbox
         self._password = password
         self._nonce = uuid.uuid4()
         self._nonce_count = 0
 
     def __call__(self, r=None):
         token = self.generate_token()
         if r is not None:
             # This is being used as a Requests auth handler
-            r.headers['Authorization'] = token
+            r.headers["Authorization"] = token
             return r
         else:
             # This is being used in its legacy capacity
             return token
 
-    def generate_token(self):
+    def generate_token(self) -> str:
         now = datetime.datetime.utcnow().strftime("%Y%m%d%H%M")
-        public_auth_data = _combine(self._mailbox, self._nonce,
-                                    self._nonce_count, now)
-        private_auth_data = _combine(self._mailbox, self._nonce,
-                                     self._nonce_count, self._password, now)
-        myhash = hmac.HMAC(self._key, private_auth_data.encode("ASCII"),
-                           sha256).hexdigest()
+        public_auth_data = f"{self._mailbox}:{self._nonce}:{self._nonce_count}:{now}"
+        private_auth_data = f"{self._mailbox}:{self._nonce}:{self._nonce_count}:{self._password}:{now}"
+        myhash = hmac.HMAC(self._key, private_auth_data.encode("ASCII"), sha256).hexdigest()
         self._nonce_count += 1
-        return "NHSMESH {public_auth_data}:{myhash}".format(**locals())
+        return f"NHSMESH {public_auth_data}:{myhash}"
 
 
 # Preserve old name, even though it's part of the API now
 _AuthTokenGenerator = AuthTokenGenerator
-
-
-def _combine(*elements):
-    return ":".join(str(x) for x in elements)
```

### Comparing `Mesh Client-1.6.0/mesh_client/ca.cert.pem` & `Mesh-Client-2.0.1/tests/ca.cert.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/ca.key.pem` & `Mesh-Client-2.0.1/tests/ca.key.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/client.cert.pem` & `Mesh-Client-2.0.1/tests/client.cert.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/client.key.pem` & `Mesh-Client-2.0.1/tests/client.key.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/io_helpers.py` & `Mesh-Client-2.0.1/mesh_client/io_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,79 +1,78 @@
-from __future__ import division
 import io
 import os
-import six
 import warnings
 import zlib
+from typing import List, cast
 
 
 class IteratorMixin(object):
     """
     Produce a series of lines, from a readable that only exposes a `read` method
     """
+
     __block_size = 65536
     __line_iterator = None
 
     def __iter__(self):
         # We use a BytesIO as our buffer, so we can piggyback on its readlines method
         buff = io.BytesIO()
         while True:
-            block = self.read(self.__block_size)
+            block = self.read(self.__block_size)  # type: ignore[attr-defined]
             buff.write(block)
             last_block = len(block) == 0
             buff.seek(0)
             lines = buff.readlines()
             for line in lines[:-1]:
                 yield line
             if not last_block:
                 buff.seek(0)
                 buff.write(lines[-1])
                 buff.truncate()
             else:
                 yield lines[-1]
                 break
 
-    def readline(self):
+    def readline(self) -> bytes:
         if not self.__line_iterator:
             self.__line_iterator = iter(self)
         try:
-            return six.next(self.__line_iterator)
+            return cast(bytes, next(self.__line_iterator))
         except StopIteration:
-            return b''
+            return b""
 
-    def readlines(self):
+    def readlines(self) -> List[bytes]:
         return list(iter(self))
 
 
 class CloseUnderlyingMixin(object):
     def close(self):
         try:
-            if hasattr(self._underlying, "close"):
-                self._underlying.close()
+            if hasattr(self._underlying, "close"):  # type: ignore[has-type]
+                self._underlying.close()  # type: ignore[has-type]
         finally:
             self._underlying = None
             if hasattr(super(CloseUnderlyingMixin, self), "close"):
-                super(CloseUnderlyingMixin, self).close()
+                super(CloseUnderlyingMixin, self).close()  # type: ignore[misc]
 
     def __del__(self):
         self.close()
         if hasattr(super(CloseUnderlyingMixin, self), "__del__"):
-            super(CloseUnderlyingMixin, self).__del__()
+            super(CloseUnderlyingMixin, self).__del__()  # type: ignore[misc]
 
     def __enter__(self):
         if hasattr(super(CloseUnderlyingMixin, self), "__enter__"):
-            return super(CloseUnderlyingMixin, self).__enter__()
+            return super(CloseUnderlyingMixin, self).__enter__()  # type: ignore[misc]
         else:
             return self
 
     def __exit__(self, typ, value, traceback):
         self.close()
         if hasattr(super(CloseUnderlyingMixin, self), "__exit__"):
-            return super(CloseUnderlyingMixin, self).__exit__(typ, value,
-                                                              traceback)
+            return super(CloseUnderlyingMixin, self).__exit__(typ, value, traceback)  # type: ignore[misc]
 
 
 class AbstractGzipStream(IteratorMixin, CloseUnderlyingMixin):
     """
     Wrap an existing readable, in a readable that produces a gzipped
     version of the underlying stream.
     """
@@ -126,17 +125,15 @@
     Wrap an existing readable, in a readable that produces a gzipped
     version of the underlying stream.
     """
 
     def __init__(self, underlying, block_size=65536):
         AbstractGzipStream.__init__(self, underlying, block_size)
         self._compress_obj = zlib.compressobj(
-            9,  # level
-            zlib.DEFLATED,  # method
-            31  # wbits - gzip header, maximum window
+            9, zlib.DEFLATED, 31  # level  # method  # wbits - gzip header, maximum window
         )
 
     def _process_block(self, block):
         return self._compress_obj.compress(block)
 
     def _finish(self):
         return self._compress_obj.flush(zlib.Z_FINISH)
@@ -146,17 +143,15 @@
     """
     Wrap an existing readable, in a readable that decompresses
     the underlying stream.
     """
 
     def __init__(self, underlying, block_size=65536):
         AbstractGzipStream.__init__(self, underlying, block_size)
-        self._decompress_obj = zlib.decompressobj(
-            47  # wbits - detect header, maximum window
-        )
+        self._decompress_obj = zlib.decompressobj(47)  # wbits - detect header, maximum window
 
     def _process_block(self, block):
         return self._decompress_obj.decompress(block)
 
     def _finish(self):
         return self._decompress_obj.flush()
 
@@ -180,26 +175,25 @@
             self._length = data["ContentLength"]
         else:
             raise TypeError("data must be a bytes, file, or urllib response")
         self._chunk_size = chunk_size
         self._remaining = 0
 
     def __len__(self):
-        return max(1,
-                   (self._length + self._chunk_size - 1) // self._chunk_size)
+        return max(1, (self._length + self._chunk_size - 1) // self._chunk_size)
 
     def __iter__(self):
         for i in range(len(self)):
             if self._remaining > 0:
                 warnings.warn(
-                    "moving to next chunk, despite unread content in buffer "
-                    "- existing chunk will become invalid")
+                    "moving to next chunk, despite unread content in buffer " "- existing chunk will become invalid"
+                )
+                assert self._underlying
                 self._underlying.read(self._remaining)
-            self._remaining = min(self._chunk_size,
-                                  self._length - i * self._chunk_size)
+            self._remaining = min(self._chunk_size, self._length - i * self._chunk_size)
             yield _SplitChunk(self)
 
 
 class _SplitChunk(IteratorMixin):
     def __init__(self, owner):
         self._owner = owner
 
@@ -216,55 +210,56 @@
     def __len__(self):
         return self._owner._remaining
 
 
 class CombineStreams(IteratorMixin):
     def __init__(self, streams):
         self._streams = iter(streams)
-        self._current_stream = six.next(self._streams)
+        self._current_stream = next(self._streams)
 
-    def read(self, n=-1):
+    def read(self, n=-1) -> bytes:
         if n == -1:
             n = None
         result = io.BytesIO()
         try:
             while True:
                 data_read = self._current_stream.read(n)
                 result.write(data_read)
                 if n is None or len(data_read) < n:
                     self._close_current_stream()
-                    self._current_stream = six.next(self._streams)
+                    self._current_stream = next(self._streams)
                     if n is not None:
                         n -= len(data_read)
                 else:
                     return result.getvalue()
         except StopIteration:
             self._current_stream = io.BytesIO()  # Empty stream
             return result.getvalue()
 
     def close(self):
         self._close_current_stream()
 
     def _close_current_stream(self):
         try:
             self._current_stream.close()
-        except:
+        except:  # noqa: E722
             pass
 
 
 class FiniteLengthStream(IteratorMixin, CloseUnderlyingMixin):
     def __init__(self, stream, length):
         self._underlying = stream
         self._remaining = length
 
     def read(self, n=-1):
         if n == -1 or n is None:
             n = self._remaining
         n = min(n, self._remaining)
         try:
+            assert self._underlying
             return self._underlying.read(n)
         finally:
             self._remaining -= n
 
 
 class ChunkedStream(IteratorMixin, CloseUnderlyingMixin):
     def __init__(self, underlying):
@@ -298,18 +293,7 @@
                 if block_length > 0:
                     self._buffer.write(self._underlying.read(block_length))
                     assert self._underlying.read(2) == b"\r\n"
                 else:
                     self._buffer.seek(0)
                     self._underlying.close()
                     self._underlying = None
-
-
-def stream_from_wsgi_environ(environ):
-    if environ.get("CONTENT_LENGTH"):
-        return FiniteLengthStream(environ["wsgi.input"],
-                                  int(environ["CONTENT_LENGTH"]))
-    elif environ.get("HTTP_TRANSFER_ENCODING") == "chunked":
-        return ChunkedStream(environ["wsgi.input"])
-    else:
-        # terminated by close
-        return environ["wsgi.input"]
```

### Comparing `Mesh Client-1.6.0/mesh_client/mesh_auth.py` & `Mesh-Client-2.0.1/mesh_client/mesh_auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 #!/usr/bin/env python
-from __future__ import print_function
+
+from argparse import ArgumentParser
+
 from mesh_client import AuthTokenGenerator
 from mesh_client.key_helper import get_shared_key_from_environ
-from argparse import ArgumentParser
 
 
 def encode_bytes(key):
-    return key.encode('utf-8')
+    return key.encode("utf-8", "surrogateescape")
 
 
 def main():
     parser = ArgumentParser(description="Create MESH auth token for user")
-    parser.add_argument('user', help="The username")
-    parser.add_argument('password', help="The password for the user")
-    parser.add_argument('--shared-key',
-                        help="The shared key to use for MESH authentication",
-                        default=get_shared_key_from_environ(),
-                        type=encode_bytes)
+    parser.add_argument("user", help="The username")
+    parser.add_argument("password", help="The password for the user")
+    parser.add_argument(
+        "--shared-key",
+        help="The shared key to use for MESH authentication",
+        default=get_shared_key_from_environ(),
+        type=encode_bytes,
+    )
     args = parser.parse_args()
     generator = AuthTokenGenerator(args.shared_key, args.user, args.password)
     print(generator.generate_token())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `Mesh Client-1.6.0/mesh_client/mock_server.py` & `Mesh-Client-2.0.1/tests/mock_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,61 +10,70 @@
 
 This mock instance will use TLS mutual authentication, with hard-coded SSL
 certs that are included in the distribution. Matching client certs are
 also included, and the settings to use them are included in the mesh_client
 package as default_ssl_opts. Since these certs and keys are publicly available,
 they should only be used in test environments.
 """
-from __future__ import print_function, absolute_import
+
 import datetime
 import hmac
 import json
 import os.path
 import random
 import ssl
 import time
 import traceback
 import zlib
+from collections import OrderedDict
 from contextlib import closing
 from hashlib import sha256
-from collections import OrderedDict
 from threading import Thread
+from typing import List, cast
+from urllib.parse import parse_qs
+from wsgiref.simple_server import WSGIServer, make_server
 from wsgiref.util import shift_path_info
-from wsgiref.simple_server import make_server, WSGIServer
-from six.moves.urllib.parse import parse_qs
-from .io_helpers import stream_from_wsgi_environ
-from .key_helper import get_shared_key_from_environ
+
+from mesh_client.io_helpers import ChunkedStream, FiniteLengthStream
+from mesh_client.key_helper import get_shared_key_from_environ
 
 _OPTIONAL_HEADERS = {
     "HTTP_CONTENT_ENCODING": "Content-Encoding",
     "HTTP_MEX_WORKFLOWID": "Mex-WorkflowID",
     "HTTP_MEX_FILENAME": "Mex-FileName",
     "HTTP_MEX_LOCALID": "Mex-LocalID",
     "HTTP_MEX_MESSAGETYPE": "Mex-MessageType",
-    "HTTP_MEX_PROCESSID": "Mex-ProcessID",
-    "HTTP_MEX_PROCESSLID": "Mex-ProcesslID",
     "HTTP_MEX_SUBJECT": "Mex-Subject",
     "HTTP_MEX_CONTENT_ENCRYPTED": "Mex-Content-Encrypted",
     "HTTP_MEX_CONTENT_COMPRESS": "Mex-Content-Compress",
     "HTTP_MEX_CONTENT_CHECKSUM": "Mex-Content-Checksum",
     "HTTP_MEX_COMPRESSED": "Mex-Compressed",
     "HTTP_MEX_CONTENT_COMPRESSED": "Mex-Content-Compressed",
     "HTTP_MEX_CHUNK_RANGE": "Mex-Chunk-Range",
     "HTTP_MEX_FROM": "Mex-From",
-    "HTTP_MEX_TO": "Mex-To"
+    "HTTP_MEX_TO": "Mex-To",
 }
 
 
-TIMESTAMP_FORMAT = '%Y%m%d%H%M%S%f'
+TIMESTAMP_FORMAT = "%Y%m%d%H%M%S%f"
+
+
+def stream_from_wsgi_environ(environ):
+    if environ.get("CONTENT_LENGTH"):
+        return FiniteLengthStream(environ["wsgi.input"], int(environ["CONTENT_LENGTH"]))
+    elif environ.get("HTTP_TRANSFER_ENCODING") == "chunked":
+        return ChunkedStream(environ["wsgi.input"])
+    else:
+        # terminated by close
+        return environ["wsgi.input"]
 
 
 def _dumb_response_code(code, message):
     def handle(environ, start_response):
-        start_response("{} {}".format(code, message),
-                       [("Content-Type", "text/plain")])
+        start_response("{} {}".format(code, message), [("Content-Type", "text/plain")])
         return [message.encode("UTF-8")]
 
     return handle
 
 
 _not_found = _dumb_response_code(404, "Not Found")
 _not_authorized = _dumb_response_code(401, "Unauthorized")
@@ -82,20 +91,26 @@
 def _error(content_type, data, start_error_response):
     start_error_response("500 INTERNAL SERVER ERROR", [("Content-Type", content_type)])
     return data
 
 
 def _compose(**kwargs):
     def handle(environ, start_response):
-        path_component = shift_path_info(environ) or 'default'
-        if path_component in kwargs:
-            return kwargs[path_component](environ, start_response)
-        else:
+        path_component = shift_path_info(environ) or "none"
+        if path_component not in kwargs:
+            if "default" in kwargs:
+                remaining_path = environ["PATH_INFO"]
+                environ["PATH_INFO"] = "/".join(
+                    ["", path_component, remaining_path] if remaining_path else ["", path_component]
+                )
+                return kwargs["default"](environ, start_response)
             return _not_found(environ, start_response)
 
+        return kwargs[path_component](environ, start_response)
+
     return handle
 
 
 class MockMeshApplication:
     """
     A crude mock instance of MESH, suitable for use in tests.
 
@@ -118,277 +133,250 @@
     def __init__(self, shared_key=get_shared_key_from_environ()):
         self.messages = {}
         self._shared_key = shared_key
         self._msg_count = 0
 
     @property
     def __call__(self):
-        return _compose(
-            messageexchange=self.message_exchange,
-            endpointlookup=_compose(
-                mesh=self.endpoint_lookup
-            )
-        )
+        return _compose(messageexchange=self.message_exchange)
 
     def authenticated(self, handler):
         def handle(environ, start_response):
             requested_mailbox = shift_path_info(environ)
+
             authorization_header = environ.get("HTTP_AUTHORIZATION", "")
             if not authorization_header.startswith("NHSMESH "):
                 return _not_authorized(environ, start_response)
 
             auth_data = authorization_header[8:]
             mailbox, nonce, nonce_count, ts, hashed = auth_data.split(":")
             expected_password = "password"
-            hash_data = ":".join([
-                mailbox, nonce, nonce_count, expected_password, ts
-            ])
-            myhash = hmac.HMAC(self._shared_key, hash_data.encode("ASCII"),
-                               sha256).hexdigest()
+            hash_data = ":".join([mailbox, nonce, nonce_count, expected_password, ts])
+            myhash = hmac.HMAC(self._shared_key, hash_data.encode("ASCII"), sha256).hexdigest()
             if myhash == hashed and mailbox == requested_mailbox:
                 environ["mesh.mailbox"] = mailbox
                 return handler(environ, start_response)
             else:
                 return _forbidden(environ, start_response)
 
         return handle
 
     def handshake(self, environ, start_response):
         auth_headers = [
-            'HTTP_MEX_CLIENTVERSION',
-            'HTTP_MEX_JAVAVERSION',
-            'HTTP_MEX_OSARCHITECTURE',
-            'HTTP_MEX_OSNAME',
-            'HTTP_MEX_OSVERSION'
+            "HTTP_MEX_CLIENTVERSION",
+            "HTTP_MEX_JAVAVERSION",
+            "HTTP_MEX_OSARCHITECTURE",
+            "HTTP_MEX_OSNAME",
+            "HTTP_MEX_OSVERSION",
         ]
         for auth_header in auth_headers:
             if auth_header not in environ:
                 return _server_error(environ, start_response)
         mailbox_id = environ["mesh.mailbox"]
-        return _ok('application/json',
-                   [json.dumps({"mailboxId": mailbox_id}).encode("UTF-8")],
-                   start_response)
+        return _ok("application/json", [json.dumps({"mailboxId": mailbox_id}).encode("UTF-8")], start_response)
 
     @property
     def message_exchange(self):
-        return self.authenticated(
-            _compose(
-                inbox=self.inbox,
-                outbox=self.outbox,
-                count=self.count,
-                default=self.handshake
-            )
+        return _compose(
+            endpointlookup=self.endpoint_lookup,
+            default=self.authenticated(
+                _compose(inbox=self.inbox, outbox=self.outbox, count=self.count, none=self.handshake)
+            ),
         )
 
-
     def inbox(self, environ, start_response):
         request_method = environ["REQUEST_METHOD"]
         message_id = shift_path_info(environ)
         mailbox = environ["mesh.mailbox"]
 
-        if (request_method == "PUT" and
-                environ["PATH_INFO"] == "/status/acknowledged"):
+        if request_method == "PUT" and environ["PATH_INFO"] == "/status/acknowledged":
             del self.messages[mailbox][message_id]
             return _simple_ok(environ, start_response)
 
         if request_method == "GET":
             if message_id:
                 chunk_num = shift_path_info(environ)
                 if chunk_num:
-                    return self.download_chunk(
-                        message_id, chunk_num)(environ, start_response)
+                    return self.download_chunk(message_id, chunk_num)(environ, start_response)
                 message = self.messages[message_id]
-                if message['headers']['Mex-To'] != mailbox:
+                if message["headers"]["Mex-To"] != mailbox:
                     return _not_found(environ, start_response)
-                response_code = ("206 Partial Content"
-                                 if "chunks" in message else "200 OK")
+                response_code = "206 Partial Content" if "chunks" in message else "200 OK"
                 start_response(response_code, list(message["headers"].items()))
                 return [message["data"]]
             else:
-                messages = {"messages": list(
-                    self.messages.get(mailbox, {}).keys())}
-                return _ok("application/json",
-                           [json.dumps(messages).encode("UTF-8")],
-                           start_response)
+                messages = {"messages": list(self.messages.get(mailbox, {}).keys())}
+                return _ok("application/json", [json.dumps(messages).encode("UTF-8")], start_response)
         else:
             return _bad_request(environ, start_response)
 
     def count(self, environ, start_response):
         request_method = environ["REQUEST_METHOD"]
         mailbox = environ["mesh.mailbox"]
         if request_method == "GET":
             result = {
                 "count": len(self.messages.get(mailbox, {})),
                 "internalID": "12345",
                 "allResultsIncluded": True,
-
             }
-            return _ok("application/json",
-                       [json.dumps(result).encode("UTF-8")],
-                       start_response)
+            return _ok("application/json", [json.dumps(result).encode("UTF-8")], start_response)
         else:
             return _bad_request(environ, start_response)
 
     def outbox(self, environ, start_response):
         chunk_msg = shift_path_info(environ)
-        if chunk_msg == 'tracking':
+        if chunk_msg == "tracking":
             return self.tracking(environ, start_response)
         if chunk_msg:
             return self.upload_chunk(chunk_msg)(environ, start_response)
         try:
             recipient = environ["HTTP_MEX_TO"]
             sender = environ["HTTP_MEX_FROM"]
             mailbox_id = environ["mesh.mailbox"]
             assert mailbox_id == sender
         except Exception as e:
             traceback.print_exc()
-            start_response("417 Expectation Failed",
-                           [('Content-Type', 'application/json')])
-            return [json.dumps({
-                "errorCode": "02",
-                "errorDescription": str(e),
-                "errorEvent": "COLLECT",
-                "messageID": "99999"
-            })]
+            start_response("417 Expectation Failed", [("Content-Type", "application/json")])
+            return [
+                json.dumps(
+                    {"errorCode": "02", "errorDescription": str(e), "errorEvent": "COLLECT", "messageID": "99999"}
+                )
+            ]
 
         mailbox = self.messages.setdefault(recipient, OrderedDict())
         with closing(stream_from_wsgi_environ(environ)) as stream:
             data = stream.read()
         if not data:
-            start_response("417 Expectation Failed",
-                           [('Content-Type', 'application/json')])
-            return [json.dumps({
-                "errorCode": "02",
-                "errorDescription": "Data file is missing or inaccessible.",
-                "errorEvent": "COLLECT",
-                "messageID": "99999"
-            }).encode("utf-8")]
-        headers = {_OPTIONAL_HEADERS[key]: value
-                   for key, value in environ.items()
-                   if key in _OPTIONAL_HEADERS}
+            start_response("417 Expectation Failed", [("Content-Type", "application/json")])
+            return [
+                json.dumps(
+                    {
+                        "errorCode": "02",
+                        "errorDescription": "Data file is missing or inaccessible.",
+                        "errorEvent": "COLLECT",
+                        "messageID": "99999",
+                    }
+                ).encode("utf-8")
+            ]
+        headers = {"Content-Type": "application/octet-stream"}  # defaults
+        headers.update({_OPTIONAL_HEADERS[key]: value for key, value in environ.items() if key in _OPTIONAL_HEADERS})
         msg_id = self.make_message_id()
-        headers['Mex-MessageID'] = msg_id
+        headers["Mex-MessageID"] = msg_id
         mailbox[msg_id] = {"headers": headers, "data": data}
         self.messages[msg_id] = mailbox[msg_id]
-        return _ok("application/json",
-                   [json.dumps({"messageID": msg_id}).encode("UTF-8")],
-                   start_response)
+        return _ok("application/json", [json.dumps({"messageID": msg_id}).encode("UTF-8")], start_response)
 
     def upload_chunk(self, chunk_msg):
         def handle(environ, start_response):
             chunk_num = shift_path_info(environ)
             msg = self.messages[chunk_msg]
             chunks = msg.setdefault("chunks", {})
             with closing(stream_from_wsgi_environ(environ)) as stream:
                 data = stream.read()
-            chunks[chunk_num] = zlib.compress(data) if not environ.get('HTTP_CONTENT_ENCODING', None) else data
-            start_response('202 Accepted', [])
+            chunks[chunk_num] = zlib.compress(data) if not environ.get("HTTP_CONTENT_ENCODING", None) else data
+            start_response("202 Accepted", [])
             return []
 
         return handle
 
     def download_chunk(self, chunk_msg, chunk_num):
         def handle(environ, start_response):
             msg = self.messages[chunk_msg]
             chunks = msg["chunks"]
             chunk = chunks[chunk_num]
-            if environ['HTTP_ACCEPT_ENCODING'] != "gzip":
+            if environ["HTTP_ACCEPT_ENCODING"] != "gzip":
                 chunk = zlib.decompress(chunk)
 
             chunk_header = "{}:{}".format(chunk_num, len(chunks) + 1)
-            start_response('200 OK', [
-                ('Content-Type', 'application/octet-stream'),
-                ('Content-Encoding', 'gzip'),
-                ('Mex-Chunk-Range', chunk_header)
-            ])
+            start_response(
+                "200 OK",
+                [
+                    ("Content-Type", msg["headers"]["Content-Type"]),
+                    ("Content-Encoding", "gzip"),
+                    ("Mex-Chunk-Range", chunk_header),
+                ],
+            )
             return [chunk]
 
         return handle
 
     def tracking(self, environ, start_response):
         tracking_id = shift_path_info(environ)
-        msg_id = parse_qs(environ['QUERY_STRING']).get('messageID', [None])[0]
+        msg_id = parse_qs(environ["QUERY_STRING"]).get("messageID", cast(List[str], [None]))[0]
         if tracking_id:
             message = self._find_message_by_local_id(tracking_id)
         elif msg_id:
             message = self.messages.get(msg_id)
         else:
             return _bad_request(environ, start_response)
 
         if message:
-            headers = message['headers']
-            recipient = headers['Mex-To']
-            message_id = headers['Mex-MessageID']
+            headers = message["headers"]
+            recipient = headers["Mex-To"]
+            message_id = headers["Mex-MessageID"]
             acked = message_id not in self.messages[recipient]
             now = datetime.datetime.now().strftime(TIMESTAMP_FORMAT)
             response = {
                 "localId": tracking_id,
                 "dtsId": message_id,
                 "messageType": "DATA",
-                "chunkCount": len(message['chunks']),
-                "subject": headers.get('Mex-Subject'),
+                "chunkCount": len(message["chunks"]),
+                "subject": headers.get("Mex-Subject"),
                 "statusEvent": None,
                 "version": "1.0",
                 "downloadTimestamp": now,
                 "statusDescription": None,
                 "status": "Acknowledged" if acked else "Accepted",
-                "workflowId": headers.get('Mex-WorkflowID'),
-                "fileName": headers.get('Mex-FileName'),
+                "workflowId": headers.get("Mex-WorkflowID"),
+                "fileName": headers.get("Mex-FileName"),
                 "uploadTimestamp": now,
-                "recipient": headers['Mex-To'],
-                "sender": headers['Mex-From'],
+                "recipient": headers["Mex-To"],
+                "sender": headers["Mex-From"],
                 "messageId": message_id,
-                "fileSize": 0
+                "fileSize": 0,
             }
-            return _ok('application/json',
-                       [json.dumps(response).encode('UTF-8')],
-                       start_response)
+            return _ok("application/json", [json.dumps(response).encode("UTF-8")], start_response)
         else:
             return _not_found(environ, start_response)
 
     def _find_message_by_local_id(self, local_id):
         for message in self.messages.values():
-            if message.get('headers', {}).get('Mex-LocalID') == local_id:
+            if message.get("headers", {}).get("Mex-LocalID") == local_id:
                 return message
         else:
             return None
 
     def endpoint_lookup(self, environ, start_response):
         org_code = shift_path_info(environ)
         workflow_id = shift_path_info(environ)
         if not org_code or not workflow_id:
             return _not_found(environ, start_response)
         result = {
             "query_id": "{ts:%Y%m%d%H%M%S%f}_{rnd:06x}_{ts:%s}".format(
-                ts=datetime.datetime.now(),
-                rnd=random.randint(0, 0xffffff)),
+                ts=datetime.datetime.now(), rnd=random.randint(0, 0xFFFFFF)
+            ),
             "results": [
                 {
                     "address": "{}HC001".format(org_code),
                     "description": "{} {} endpoint".format(org_code, workflow_id),
-                    "endpoint_type": "MESH"
+                    "endpoint_type": "MESH",
                 }
-            ]
+            ],
         }
-        return _ok('application/json',
-                   [json.dumps(result).encode('UTF-8')],
-                   start_response)
+        return _ok("application/json", [json.dumps(result).encode("UTF-8")], start_response)
 
     def make_message_id(self):
         """
         Create a new message id. By default, this uses roughly the same format
         as MESH (although the format is undocumented), but it can be overridden
         in subclasses for different behaviour
         """
         n = self._msg_count
         self._msg_count += 1
-        return "{ts:%Y%m%d%H%M%S%f}_{num:06d}".format(
-            ts=datetime.datetime.now(),
-            num=n
-        )
+        return f"{datetime.datetime.now():%Y%m%d%H%M%S%f}_{n:06d}"
 
     def __enter__(self):
         self.start_server()
         return self
 
     def __exit__(self, ex_type, value, tb):
         self.stop_server()
@@ -398,17 +386,15 @@
         Start an embedded web server, running the mock MESH app. After running
         this method, the uri of the running MESH instance will be available
         as self.uri
         """
         self.server = make_server("", 0, self, server_class=SSLWSGIServer)
         port = self.server.server_address[1]
         self.uri = "https://localhost:{}".format(port)
-        thread = Thread(
-            target=self.server.serve_forever,
-            kwargs={"poll_interval": 0.01})
+        thread = Thread(target=self.server.serve_forever, kwargs={"poll_interval": 0.01})
         thread.daemon = True
         thread.start()
         return self
 
     def stop_server(self):
         """
         Stop a server that was started by start_server(). This has no effect
@@ -423,52 +409,42 @@
         self.allowed_retries = {}
         super(MockMeshChunkRetryApplication, self).__init__()
 
     def set_chunk_retry_options(self, options):
         self.retry_options = options
 
     def outbox(self, environ, start_response):
-        current_chunk = int(environ['HTTP_MEX_CHUNK_RANGE'].split(':')[0])
+        current_chunk = int(environ["HTTP_MEX_CHUNK_RANGE"].split(":")[0])
         if current_chunk == 1:
             self.allowed_retries = {p[0]: p[1] for p in self.retry_options}
 
         if current_chunk in self.allowed_retries:
             if self.allowed_retries[current_chunk] >= 0:
                 self.allowed_retries[current_chunk] -= 1
-                return _error("application/json", '', start_response)
+                return _error("application/json", "", start_response)
 
         return super(MockMeshChunkRetryApplication, self).outbox(environ, start_response)
 
 
 class SlowMockMeshApplication(MockMeshApplication):
     def __call__(self, environ, start_response):
         time.sleep(2.0)
         return super(SlowMockMeshApplication, self).__call__(environ, start_response)
 
 
 _data_dir = os.path.dirname(__file__)
 default_server_context = ssl.create_default_context(
-    ssl.Purpose.CLIENT_AUTH, cafile=os.path.join(_data_dir, "ca.cert.pem"))
+    ssl.Purpose.CLIENT_AUTH, cafile=os.path.join(_data_dir, "ca.cert.pem")
+)
 default_server_context.load_cert_chain(
-    os.path.join(_data_dir, 'server.cert.pem'),
-    os.path.join(_data_dir, 'server.key.pem'))
+    os.path.join(_data_dir, "server.cert.pem"), os.path.join(_data_dir, "server.key.pem")
+)
 default_server_context.check_hostname = False
 default_server_context.verify_mode = ssl.CERT_REQUIRED
 
 
 class SSLWSGIServer(WSGIServer, object):
     __context = default_server_context
 
     def get_request(self):
         (socket, addr) = super(SSLWSGIServer, self).get_request()
         return self.__context.wrap_socket(socket, server_side=True), addr
-
-
-def main():
-    print("Serving on port 8000")
-    server = make_server(
-        "", 8000, MockMeshApplication(), server_class=SSLWSGIServer)
-    server.serve_forever(0.01)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `Mesh Client-1.6.0/mesh_client/nhs-dep-ca-bundle.pem` & `Mesh-Client-2.0.1/mesh_client/nhs-dep-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/nhs-dev-ca-bundle.pem` & `Mesh-Client-2.0.1/mesh_client/nhs-dev-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/nhs-digicert-ca-bundle.pem` & `Mesh-Client-2.0.1/mesh_client/nhs-digicert-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/nhs-digicert-root-ca.pem` & `Mesh-Client-2.0.1/mesh_client/nhs-digicert-root-ca.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/nhs-ig-int-ca-bundle.pem` & `Mesh-Client-2.0.1/mesh_client/nhs-ig-int-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/nhs-ig-live-ca-bundle.pem` & `Mesh-Client-2.0.1/mesh_client/nhs-ig-live-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/nhs-live-root-ca.pem` & `Mesh-Client-2.0.1/mesh_client/nhs-live-root-ca.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/nhs-opt-ca-bundle.pem` & `Mesh-Client-2.0.1/mesh_client/nhs-opt-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/nhs-train-ca-bundle.pem` & `Mesh-Client-2.0.1/mesh_client/nhs-train-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/server.cert.pem` & `Mesh-Client-2.0.1/tests/server.cert.pem`

 * *Files identical despite different names*

### Comparing `Mesh Client-1.6.0/mesh_client/server.key.pem` & `Mesh-Client-2.0.1/tests/server.key.pem`

 * *Files identical despite different names*

