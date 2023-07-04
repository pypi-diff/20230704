# Comparing `tmp/dexie_rewards-1.8.2b1.tar.gz` & `tmp/dexie_rewards-1.8.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexie_rewards-1.8.2b1.tar", max compression
+gzip compressed data, was "dexie_rewards-1.8.2b2.tar", max compression
```

## Comparing `dexie_rewards-1.8.2b1.tar` & `dexie_rewards-1.8.2b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-1.8.2b1/LICENSE
--rw-r--r--   0        0        0     5721 2023-06-11 09:31:39.287155 dexie_rewards-1.8.2b1/README.md
--rw-r--r--   0        0        0      805 2023-06-30 09:11:11.103550 dexie_rewards-1.8.2b1/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-1.8.2b1/src/dexie_rewards/__init__.py
--rw-r--r--   0        0        0     1125 2023-06-30 04:40:39.340510 dexie_rewards-1.8.2b1/src/dexie_rewards/config.py
--rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-1.8.2b1/src/dexie_rewards/decorators/with_db_connection.py
--rw-r--r--   0        0        0     1169 2023-06-10 08:56:40.443038 dexie_rewards-1.8.2b1/src/dexie_rewards/decorators/with_wallet_rpc_client.py
--rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-1.8.2b1/src/dexie_rewards/main.py
--rw-r--r--   0        0        0     5013 2023-06-30 09:40:10.161232 dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/claim.py
--rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/list.py
--rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/main.py
--rw-r--r--   0        0        0     5159 2023-06-30 09:37:14.115364 dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/utils.py
--rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.341294 dexie_rewards-1.8.2b1/src/dexie_rewards/services/dexie_api.py
--rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-1.8.2b1/src/dexie_rewards/services/dexie_db.py
--rw-r--r--   0        0        0     1792 2023-06-11 05:27:12.034750 dexie_rewards-1.8.2b1/src/dexie_rewards/services/wallet_rpc_client.py
--rw-r--r--   0        0        0     1124 2023-06-30 04:32:23.576365 dexie_rewards-1.8.2b1/src/dexie_rewards/types/offer_reward.py
--rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-1.8.2b1/src/dexie_rewards/types/utils.py
--rw-r--r--   0        0        0     1863 2023-06-10 08:56:40.444913 dexie_rewards-1.8.2b1/src/dexie_rewards/utils.py
--rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 dexie_rewards-1.8.2b1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-1.8.2b2/LICENSE
+-rw-r--r--   0        0        0     5817 2023-06-30 14:39:04.284007 dexie_rewards-1.8.2b2/README.md
+-rw-r--r--   0        0        0      863 2023-07-04 02:16:18.442773 dexie_rewards-1.8.2b2/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-1.8.2b2/src/dexie_rewards/__init__.py
+-rw-r--r--   0        0        0     1125 2023-06-30 04:40:39.340510 dexie_rewards-1.8.2b2/src/dexie_rewards/config.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-1.8.2b2/src/dexie_rewards/decorators/with_db_connection.py
+-rw-r--r--   0        0        0     1169 2023-06-10 08:56:40.443038 dexie_rewards-1.8.2b2/src/dexie_rewards/decorators/with_wallet_rpc_client.py
+-rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-1.8.2b2/src/dexie_rewards/main.py
+-rw-r--r--   0        0        0     5013 2023-06-30 09:40:10.161232 dexie_rewards-1.8.2b2/src/dexie_rewards/rewards/claim.py
+-rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-1.8.2b2/src/dexie_rewards/rewards/list.py
+-rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-1.8.2b2/src/dexie_rewards/rewards/main.py
+-rw-r--r--   0        0        0     5159 2023-06-30 09:37:14.115364 dexie_rewards-1.8.2b2/src/dexie_rewards/rewards/utils.py
+-rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.341294 dexie_rewards-1.8.2b2/src/dexie_rewards/services/dexie_api.py
+-rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-1.8.2b2/src/dexie_rewards/services/dexie_db.py
+-rw-r--r--   0        0        0     1792 2023-06-11 05:27:12.034750 dexie_rewards-1.8.2b2/src/dexie_rewards/services/wallet_rpc_client.py
+-rw-r--r--   0        0        0     1124 2023-06-30 04:32:23.576365 dexie_rewards-1.8.2b2/src/dexie_rewards/types/offer_reward.py
+-rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-1.8.2b2/src/dexie_rewards/types/utils.py
+-rw-r--r--   0        0        0     1863 2023-06-10 08:56:40.444913 dexie_rewards-1.8.2b2/src/dexie_rewards/utils.py
+-rw-r--r--   0        0        0     6661 1970-01-01 00:00:00.000000 dexie_rewards-1.8.2b2/PKG-INFO
```

### Comparing `dexie_rewards-1.8.2b1/LICENSE` & `dexie_rewards-1.8.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/README.md` & `dexie_rewards-1.8.2b2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -87,27 +87,28 @@
 ```
 
 ### Claim all outstanding (claimable) rewards
 
 ```
 ❯ dexie rewards claim
 
-  --fingerprint  -f         Set the fingerprint to specify which wallet to use
-  --verify-only  -vo        Only verify the claim, don't actually claim
-  --yes          -y         Skip claim confirmation
-  --verbose      -v         Display verbose output
-  --target       -t         Specify a target address to claim rewards to
-  --help                    Show help and exit
+  --fingerprint     -f        Set the fingerprint to specify which wallet to use
+  --verify-only     -vo       Only verify the claim, don't actually claim
+  --yes             -y        Skip claim confirmation
+  --verbose         -v        Display verbose output
+--target            -t        Specify a target address to claim rewards to
+  --completed-only  -co       Only claim rewards for completed and cancelled offers
+  --help                      Show help and exit
 ```
 
 ## Troubleshooting
 
 If you encounter any issues, follow these steps to help identify and resolve them:
 
-1. **Check your Python version**: Ensure you are using Python 3.11 or later, as older versions are not supported.
+1. **Check your Python version**: Ensure you are using Python 3.10 or later, as older versions are not supported.
 
 2. **Update packages**: Update both dexie-rewards and its dependencies by running `pip install --upgrade dexie-rewards`.
 
 3. **Verify configuration**: Double-check the environment variables (if set) to ensure they are correct.
 
 4. **Enable verbose output**: Use the `-v` or `--verbose` option with the relevant command to get more detailed output, which can help pinpoint the issue.
```

### Comparing `dexie_rewards-1.8.2b1/pyproject.toml` & `dexie_rewards-1.8.2b2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "dexie-rewards"
-version = "1.8.2-b1"
+version = "1.8.2-b2"
 description = "dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "dexie_rewards", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 rich-click = "^1.6.1"
 aiomisc = "^17.0.9"
 aiohttp = "^3.8.4"
 based58 = "^0.1.1"
-chia-blockchain = "1.8.*"
+chia-blockchain = { version = ">=1.8.0,!=1.8.2,<1.9.0", allow-prereleases = false }
 aiosqlite = "^0.19.0"
 
 [tool.poetry.scripts]
 dexie = "dexie_rewards.main:dexie_cmd"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
```

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/config.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/config.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/decorators/with_db_connection.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/decorators/with_db_connection.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/decorators/with_wallet_rpc_client.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/decorators/with_wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/claim.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/rewards/claim.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/list.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/rewards/list.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/utils.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/services/dexie_api.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/services/dexie_api.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/services/dexie_db.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/services/dexie_db.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/services/wallet_rpc_client.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/services/wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/types/offer_reward.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/types/offer_reward.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/src/dexie_rewards/utils.py` & `dexie_rewards-1.8.2b2/src/dexie_rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b1/PKG-INFO` & `dexie_rewards-1.8.2b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dexie-rewards
-Version: 1.8.2b1
+Version: 1.8.2b2
 Summary: dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet.
 License: Apache-2.0
 Author: Dexie Contributors
 Author-email: pypi@dexie.space
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aiomisc (>=17.0.9,<18.0.0)
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
 Requires-Dist: based58 (>=0.1.1,<0.2.0)
-Requires-Dist: chia-blockchain (==1.8.*)
+Requires-Dist: chia-blockchain (>=1.8.0,!=1.8.2,<1.9.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Auto-Claim dexie rewards
 
 [![PyPI version](https://badge.fury.io/py/dexie-rewards.svg)](https://badge.fury.io/py/dexie-rewards)
 [![Python version](https://img.shields.io/pypi/pyversions/dexie-rewards.svg)](https://pypi.python.org/pypi/dexie-rewards)
@@ -107,27 +107,28 @@
 ```
 
 ### Claim all outstanding (claimable) rewards
 
 ```
 ❯ dexie rewards claim
 
-  --fingerprint  -f         Set the fingerprint to specify which wallet to use
-  --verify-only  -vo        Only verify the claim, don't actually claim
-  --yes          -y         Skip claim confirmation
-  --verbose      -v         Display verbose output
-  --target       -t         Specify a target address to claim rewards to
-  --help                    Show help and exit
+  --fingerprint     -f        Set the fingerprint to specify which wallet to use
+  --verify-only     -vo       Only verify the claim, don't actually claim
+  --yes             -y        Skip claim confirmation
+  --verbose         -v        Display verbose output
+--target            -t        Specify a target address to claim rewards to
+  --completed-only  -co       Only claim rewards for completed and cancelled offers
+  --help                      Show help and exit
 ```
 
 ## Troubleshooting
 
 If you encounter any issues, follow these steps to help identify and resolve them:
 
-1. **Check your Python version**: Ensure you are using Python 3.11 or later, as older versions are not supported.
+1. **Check your Python version**: Ensure you are using Python 3.10 or later, as older versions are not supported.
 
 2. **Update packages**: Update both dexie-rewards and its dependencies by running `pip install --upgrade dexie-rewards`.
 
 3. **Verify configuration**: Double-check the environment variables (if set) to ensure they are correct.
 
 4. **Enable verbose output**: Use the `-v` or `--verbose` option with the relevant command to get more detailed output, which can help pinpoint the issue.
```

