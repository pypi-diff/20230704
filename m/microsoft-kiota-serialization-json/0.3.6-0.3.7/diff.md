# Comparing `tmp/microsoft_kiota_serialization_json-0.3.6.tar.gz` & `tmp/microsoft_kiota_serialization_json-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_serialization_json-0.3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_serialization_json-0.3.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_serialization_json-0.3.6.tar` & `microsoft_kiota_serialization_json-0.3.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       82 2023-06-27 09:36:19.290674 microsoft_kiota_serialization_json-0.3.6/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1874 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.gitignore
--rw-r--r--   0        0        0    15976 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.pylintrc
--rw-r--r--   0        0        0     1250 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/LICENSE
--rw-r--r--   0        0        0     1146 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/Pipfile
--rw-r--r--   0        0        0    71082 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/Pipfile.lock
--rw-r--r--   0        0        0     2545 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/README.md
--rw-r--r--   0        0        0     2757 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/__init__.py
--rw-r--r--   0        0        0       23 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/_version.py
--rw-r--r--   0        0        0    11570 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_parse_node.py
--rw-r--r--   0        0        0     1433 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_parse_node_factory.py
--rw-r--r--   0        0        0    16605 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_serialization_writer.py
--rw-r--r--   0        0        0     1297 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_serialization_writer_factory.py
--rw-r--r--   0        0        0     1344 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      909 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0      119 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1569 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/entity.py
--rw-r--r--   0        0        0     2692 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/intersection_type.py
--rw-r--r--   0        0        0       94 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/office_location.py
--rw-r--r--   0        0        0     3077 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/union_type.py
--rw-r--r--   0        0        0     3133 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/user.py
--rw-r--r--   0        0        0     2151 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/user2.py
--rw-r--r--   0        0        0        0 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/__init__.py
--rw-r--r--   0        0        0     1554 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/conftest.py
--rw-r--r--   0        0        0     5236 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_intersection_wrapper.py
--rw-r--r--   0        0        0     4123 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_parse_node.py
--rw-r--r--   0        0        0     1679 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_parse_node_factory.py
--rw-r--r--   0        0        0     7188 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_serialization_writer.py
--rw-r--r--   0        0        0     1018 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_serialization_writer_factory.py
--rw-r--r--   0        0        0     5873 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_union_wrapper.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1874 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.gitignore
+-rw-r--r--   0        0        0    15976 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/.pylintrc
+-rw-r--r--   0        0        0     1362 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1146 2023-07-04 14:29:42.020263 microsoft_kiota_serialization_json-0.3.7/Pipfile
+-rw-r--r--   0        0        0    71082 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/Pipfile.lock
+-rw-r--r--   0        0        0     2545 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/README.md
+-rw-r--r--   0        0        0     2757 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/_version.py
+-rw-r--r--   0        0        0    11570 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_parse_node.py
+-rw-r--r--   0        0        0     1433 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_parse_node_factory.py
+-rw-r--r--   0        0        0    16603 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_serialization_writer.py
+-rw-r--r--   0        0        0     1297 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     1344 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      909 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0      119 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1569 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/entity.py
+-rw-r--r--   0        0        0     2692 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/intersection_type.py
+-rw-r--r--   0        0        0       94 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/office_location.py
+-rw-r--r--   0        0        0     3077 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/union_type.py
+-rw-r--r--   0        0        0     3133 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/user.py
+-rw-r--r--   0        0        0     2151 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/helpers/user2.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1554 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/conftest.py
+-rw-r--r--   0        0        0     5236 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_intersection_wrapper.py
+-rw-r--r--   0        0        0     4123 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_parse_node.py
+-rw-r--r--   0        0        0     1679 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_parse_node_factory.py
+-rw-r--r--   0        0        0     7188 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_serialization_writer.py
+-rw-r--r--   0        0        0     1018 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     5873 2023-07-04 14:29:42.024263 microsoft_kiota_serialization_json-0.3.7/tests/unit/test_union_wrapper.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-0.3.7/PKG-INFO
```

### Comparing `microsoft_kiota_serialization_json-0.3.6/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_serialization_json-0.3.7/.github/workflows/auto-merge-dependabot.yml`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.5.1
+        uses: dependabot/fetch-metadata@v1.6.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft_kiota_serialization_json-0.3.6/.github/workflows/build_publish.yml` & `microsoft_kiota_serialization_json-0.3.7/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_serialization_json-0.3.7/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_serialization_json-0.3.7/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/.gitignore` & `microsoft_kiota_serialization_json-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/.pylintrc` & `microsoft_kiota_serialization_json-0.3.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/CHANGELOG.md` & `microsoft_kiota_serialization_json-0.3.7/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.7] - 2023-07-04
+
+### Added
+
+### Changed
+- Fixes the key assignment to the writer in write_bytes_value.
+
 ## [0.3.6] - 2023-06-27
 
 ### Added
 
 ### Changed
 - Fixed a bug with loading json response in method to get root parse node.
```

### Comparing `microsoft_kiota_serialization_json-0.3.6/LICENSE` & `microsoft_kiota_serialization_json-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/Pipfile` & `microsoft_kiota_serialization_json-0.3.7/Pipfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [[source]]
 url = "https://pypi.org/simple"
 verify_ssl = true
 name = "pypi"
 
 [packages]
-microsoft-kiota-abstractions = "==0.5.4"
+microsoft-kiota-abstractions = "==0.6.0"
 python-dateutil = "==2.8.2"
 astroid = "==2.15.5"
 certifi = "==2023.5.7"
 charset-normalizer = "==3.1.0"
 colorama = "==0.4.6"
 coverage = {version = "==7.2.7", extras = ["toml"]}
 dill = "==0.3.6"
 docutils = "==0.20.1"
-exceptiongroup = "==1.1.1"
+exceptiongroup = "==1.1.2"
 flit = "==3.9.0"
 flit-core = "==3.9.0"
 idna = "==3.4"
 iniconfig = "==2.0.0"
 isort = "==5.12.0"
 lazy-object-proxy = "==1.9.0"
 mccabe = "==0.7.0"
@@ -31,15 +31,15 @@
 pytest-cov = "==4.1.0"
 requests = "==2.31.0"
 toml = "==0.10.2"
 tomli = "==2.0.1"
 tomli-w = "==1.0.0"
 tomlkit = "==0.11.8"
 types-python-dateutil = "==2.8.19.13"
-typing-extensions = "==4.6.3"
+typing-extensions = "==4.7.1"
 urllib3 = "==2.0.3"
 wrapt = "==1.15.0"
 yapf = "==0.40.1"
 six = "==1.16.0"
 uritemplate = "==4.1.1"
 
 [dev-packages]
```

### Comparing `microsoft_kiota_serialization_json-0.3.6/Pipfile.lock` & `microsoft_kiota_serialization_json-0.3.7/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9866048303548304%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'b144c90232a6fe4dc73700fa35a8a3c4ed0bdc58cab58f6af5559a8aa99fcd01'}}",*

 * * "'default'": "{'exceptiongroup': {'hashes': "*

 * *              "['sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5', "*

 * *              "'sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f'], "*

 * *              "'version': '==1.1.2'}, 'microsoft-kiota-abstractions': {'hashes': "*

 * *              "['sha256:838ebd421e9eea5c1b4655b7722968b4e8c4540da004382c0cd5b […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "7da2b2b5b7679b9c55cc180ba16d69712289937c2ad5426a767c095584712661"
+            "sha256": "b144c90232a6fe4dc73700fa35a8a3c4ed0bdc58cab58f6af5559a8aa99fcd01"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -202,19 +202,19 @@
                 "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "index": "pypi",
             "version": "==0.20.1"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
-                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
+                "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5",
+                "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"
             ],
             "index": "pypi",
-            "version": "==1.1.1"
+            "version": "==1.1.2"
         },
         "flit": {
             "hashes": [
                 "sha256:076c3aaba5ac24cf0ad3251f910900d95a08218e6bcb26f21fef1036cc4679ca",
                 "sha256:d75edf5eb324da20d53570a6a6f87f51e606eee8384925cd66a90611140844c7"
             ],
             "index": "pypi",
@@ -308,19 +308,19 @@
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "index": "pypi",
             "version": "==0.7.0"
         },
         "microsoft-kiota-abstractions": {
             "hashes": [
-                "sha256:27152023d0a4c3ad2dba52240f5fd3c7276942c7f85f4bab34f16dac4bb71dc4",
-                "sha256:590e3f3f2c8e1d7c525c107bece4afa48faedcf02409f2fc828456cb35fa19fe"
+                "sha256:838ebd421e9eea5c1b4655b7722968b4e8c4540da004382c0cd5b5203db1b1d5",
+                "sha256:bfb047b14c554f1c1bd29e587b0e91bd80e433a4e82d4ceb5828c049edf89a47"
             ],
             "index": "pypi",
-            "version": "==0.5.4"
+            "version": "==0.6.0"
         },
         "mypy": {
             "hashes": [
                 "sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042",
                 "sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd",
                 "sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2",
                 "sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01",
@@ -468,19 +468,19 @@
                 "sha256:0b0e7c68e7043b0354b26a1e0225cb1baea7abb1b324d02b50e2d08f1221043f"
             ],
             "index": "pypi",
             "version": "==2.8.19.13"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
-                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+                "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
+                "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
             "index": "pypi",
-            "version": "==4.6.3"
+            "version": "==4.7.1"
         },
         "uritemplate": {
             "hashes": [
                 "sha256:4346edfc5c3b79f694bccd6d6099a322bbeb628dbf2cd86eea55a456ce5124f0",
                 "sha256:830c08b8d99bdd312ea4ead05994a38e8936266f84b9a7878232db50b044e02e"
             ],
             "index": "pypi",
@@ -1007,19 +1007,19 @@
                 "sha256:0b0e7c68e7043b0354b26a1e0225cb1baea7abb1b324d02b50e2d08f1221043f"
             ],
             "index": "pypi",
             "version": "==2.8.19.13"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
-                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+                "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
+                "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
             "index": "pypi",
-            "version": "==4.6.3"
+            "version": "==4.7.1"
         },
         "urllib3": {
             "hashes": [
                 "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
                 "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "index": "pypi",
```

### Comparing `microsoft_kiota_serialization_json-0.3.6/README.md` & `microsoft_kiota_serialization_json-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/SECURITY.md` & `microsoft_kiota_serialization_json-0.3.7/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/SUPPORT.md` & `microsoft_kiota_serialization_json-0.3.7/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_parse_node.py` & `microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_parse_node_factory.py` & `microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_serialization_writer.py` & `microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_serialization_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
             key (Optional[str]): The key to be used for the written value. May be null.
             value (bytes): The byte array to be written.
         """
         if isinstance(value, bytes):
             base64_bytes = base64.b64encode(value)
             base64_string = base64_bytes.decode('utf-8')
             if key:
-                self.writer['key'] = base64_string
+                self.writer[key] = base64_string
             else:
                 self.value = base64_string
 
     def write_object_value(
         self, key: Optional[str], value: Optional[U], *additional_values_to_merge: U
     ) -> None:
         """Writes the specified model object to the stream with an optional given key.
```

### Comparing `microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-0.3.7/kiota_serialization_json/json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/pyproject.toml` & `microsoft_kiota_serialization_json-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/requirements-dev.txt` & `microsoft_kiota_serialization_json-0.3.7/requirements-dev.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 astroid==2.15.5
 certifi==2023.5.7
 charset-normalizer==3.1.0
 colorama==0.4.6
 coverage[toml]==7.2.7
 dill==0.3.6
 docutils==0.20.1
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
 flit-core==3.9.0
 flit==3.9.0
 idna==3.4
 importlib-metadata==6.7.0; python_version >= '3.7'
 iniconfig==2.0.0
 isort==5.12.0
 lazy-object-proxy==1.9.0
 mccabe==0.7.0
-microsoft-kiota-abstractions==0.5.4
+microsoft-kiota-abstractions==0.6.0
 mypy-extensions==1.0.0
 mypy==1.4.1
 packaging==23.1
 platformdirs==3.8.0
 pluggy==1.2.0
 pylint==2.17.4
 pytest-cov==4.1.0
@@ -35,13 +35,13 @@
 requests==2.31.0
 six==1.16.0
 toml==0.10.2
 tomli-w==1.0.0
 tomli==2.0.1
 tomlkit==0.11.8
 types-python-dateutil==2.8.19.13
-typing-extensions==4.6.3
+typing-extensions==4.7.1
 uritemplate==4.1.1
 urllib3==2.0.3
 wrapt==1.15.0
 yapf==0.40.1
 zipp==3.15.0; python_version >= '3.7'
```

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/helpers/entity.py` & `microsoft_kiota_serialization_json-0.3.7/tests/helpers/entity.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/helpers/intersection_type.py` & `microsoft_kiota_serialization_json-0.3.7/tests/helpers/intersection_type.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/helpers/union_type.py` & `microsoft_kiota_serialization_json-0.3.7/tests/helpers/union_type.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/helpers/user.py` & `microsoft_kiota_serialization_json-0.3.7/tests/helpers/user.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/helpers/user2.py` & `microsoft_kiota_serialization_json-0.3.7/tests/helpers/user2.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/unit/conftest.py` & `microsoft_kiota_serialization_json-0.3.7/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_intersection_wrapper.py` & `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_intersection_wrapper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_parse_node.py` & `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_parse_node_factory.py` & `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_serialization_writer.py` & `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_union_wrapper.py` & `microsoft_kiota_serialization_json-0.3.7/tests/unit/test_union_wrapper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.6/PKG-INFO` & `microsoft_kiota_serialization_json-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-serialization-json
-Version: 0.3.6
+Version: 0.3.7
 Summary: Implementation of Kiota Serialization interfaces for JSON
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

